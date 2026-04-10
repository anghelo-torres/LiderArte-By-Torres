name=script.js
// ================================
// FUNCIONES DE SCROLL Y NAVEGACIÓN
// ================================

function scrollToSection(sectionId) {
    const element = document.getElementById(sectionId);
    if (element) {
        element.scrollIntoView({ behavior: 'smooth' });
    }
}

// Cerrar menú móvil cuando se hace click en un enlace
document.querySelectorAll('.nav-menu a').forEach(link => {
    link.addEventListener('click', (e) => {
        const href = link.getAttribute('href');
        if (href.startsWith('#')) {
            e.preventDefault();
            const sectionId = href.substring(1);
            scrollToSection(sectionId);
        }
    });
});

// ================================
// ANIMACIONES AL SCROLL
// ================================

const observerOptions = {
    threshold: 0.1,
    rootMargin: '0px 0px -100px 0px'
};

const observer = new IntersectionObserver(function(entries) {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add('visible');
            observer.unobserve(entry.target);
        }
    });
}, observerOptions);

// Observar elementos para animación
document.querySelectorAll('.problem-card, .pillar, .modulo, .servicio-card, .beneficio').forEach(el => {
    observer.observe(el);
});

// ================================
// CONTADOR DE STATS (OPCIONAL)
// ================================

function animateCounter(element, finalValue, duration = 2000) {
    let currentValue = 0;
    const increment = finalValue / (duration / 16);
    
    const timer = setInterval(() => {
        currentValue += increment;
        if (currentValue >= finalValue) {
            element.textContent = finalValue;
            clearInterval(timer);
        } else {
            element.textContent = Math.floor(currentValue);
        }
    }, 16);
}

// ================================
// FORMULARIOS Y CTAs
// ================================

document.querySelectorAll('.btn-primary, .btn-secondary').forEach(button => {
    button.addEventListener('click', function(e) {
        // Aquí puedes agregar lógica para:
        // - Abrir formularios modales
        // - Redirigir a página de checkout
        // - Capturar leads
        console.log('CTA clicked:', this.textContent);
    });
});

// ================================
// MONITOREO DE SCROLL PARA NAVBAR
// ================================

let lastScrollTop = 0;
const navbar = document.querySelector('.navbar');

window.addEventListener('scroll', () => {
    let scrollTop = window.pageYOffset || document.documentElement.scrollTop;
    
    if (scrollTop > 50) {
        navbar.style.boxShadow = '0 4px 15px rgba(0, 0, 0, 0.1)';
    } else {
        navbar.style.boxShadow = '0 2px 10px rgba(0, 0, 0, 0.05)';
    }
    
    lastScrollTop = scrollTop;
});

// ================================
// TRACKING Y ANALYTICS (OPCIONAL)
// ================================

function trackEvent(eventName, eventData) {
    console.log(`Event tracked: ${eventName}`, eventData);
    // Aquí conectarías con Google Analytics, Mixpanel, etc.
}

// Track cuando usuarios ven cada sección
document.querySelectorAll('section').forEach(section => {
    const sectionObserver = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                trackEvent('section_viewed', {
                    section: entry.target.id || entry.target.className
                });
                sectionObserver.unobserve(entry.target);
            }
        });
    });
    sectionObserver.observe(section);
});

// ================================
// MODAL PARA FORMULARIOS
// ================================

function openModal(modalId) {
    const modal = document.getElementById(modalId);
    if (modal) {
        modal.style.display = 'flex';
        document.body.style.overflow = 'hidden';
    }
}

function closeModal(modalId) {
    const modal = document.getElementById(modalId);
    if (modal) {
        modal.style.display = 'none';
        document.body.style.overflow = 'auto';
    }
}

// Cerrar modal al hacer click fuera
document.addEventListener('click', (e) => {
    if (e.target.classList.contains('modal-overlay')) {
        closeModal(e.target.id);
    }
});

// ================================
// VALIDACIÓN DE FORMULARIOS
// ================================

function validateForm(formElement) {
    const inputs = formElement.querySelectorAll('input, textarea');
    let isValid = true;

    inputs.forEach(input => {
        if (!input.value.trim()) {
            input.classList.add('error');
            isValid = false;
        } else {
            input.classList.remove('error');
        }
    });

    return isValid;
}

// ================================
// SMOOTH SCROLL IMPROVEMENT
// ================================

document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const href = this.getAttribute('href');
        if (href !== '#') {
            scrollToSection(href.substring(1));
        }
    });
});

console.log('LiderArte Landing Page - Scripts loaded successfully');