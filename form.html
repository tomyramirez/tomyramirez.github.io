<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Confirmación de Expreso</title>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-sRIl4kxILFvY47J16cr9ZwB07vP4J8+LH7qKQnuqkuIAvNWLzeN8tE5YBujZqJLB" crossorigin="anonymous">

    <style>
        :root {
            /* Colores suaves, inspirados en tonos naturales y house */
            --color-primary: #528a5d; /* Verde natural */
            --color-secondary: #f0f7ee; /* Fondo muy claro */
            --color-success: #6c9a72; /* Verde éxito */
            --color-warning: #cc3300; /* Rojo advertencia */
            --color-soft-bg: #e9f0e8; /* Contenedor de formulario */
            --color-text-dark: #333;
            --color-close-btn: #232323; /* Boton de cierre del formulario */
        }

        body {
            /* Se eliminó overflow: hidden; de aquí */
            overflow-y: auto; /* <--- CLAVE: Permitir scroll vertical */
            font-family: Arial, sans-serif;
            color: var(--color-text-dark);
            /* Quitamos min-height: 100vh; para que la altura la determine el contenido */
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            padding: 20px;
            position: relative;
            /* Revertimos overflow a 'auto' si el contenido desborda, para que el scroll funcione */
        }

        /* Pseudoelemento para la imagen de fondo con blur */
        body::before {
            content: '';
            position: fixed; /* <--- CLAVE: Usar 'fixed' para el fondo para que no se mueva al hacer scroll */
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('https://lh3.googleusercontent.com/p/AF1QipPrgZmqcHZmUueNO4STMud9t6NfXZib4LXlk90n=s680-w680-h510-rw'); 
            background-size: cover;
            background-position: center;
            /* Ya no necesitamos background-attachment: fixed; si la posición es fixed */
            filter: blur(5px); 
            z-index: -1; 
            -webkit-filter: blur(5px); 
        }

        .form-container {
            /* ... el resto de estilos se mantiene igual ... */
            max-width: 500px;
            width: 100%;
            padding: 30px;
            background-color: rgba(255, 255, 255, 0.9); 
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2); 
            border: 1px solid var(--color-soft-bg);
            z-index: 1; 
        }
        /* Resto de estilos CSS */
        .alert-danger-custom {
            background-color: #ffe0e0;
            color: var(--color-warning);
            border-color: #fdd;
            font-weight: bold;
        }

        /* Estilo del botón Guardar */
        #btnGuardarExpreso {
            background-color: var(--color-primary);
            border-color: var(--color-primary);
            transition: all 0.5s ease-in-out;
            font-weight: bold;
            width: 100%;
        }

        /* Estilo del botón cerrar */
        #btnCerrar {
            background-color: var(--color-close-btn);
            border-color: var(--color-close-btn);
            font-weight: bold;
            width: 100%;
        }

        /* Transformación del botón a tilde */
        #btnGuardarExpreso.success-state {
            background-color: var(--color-success);
            border-color: var(--color-success);
            width: 50px; 
            height: 50px;
            border-radius: 50%; 
            padding: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            transform: scale(1.1);
        }
        
        /* Estilo para el modal pequeño de éxito */
        .modal-success-center {
            pointer-events: none; 
            background-color: rgba(255, 255, 255, 0); 
        }
        .modal-success-center .modal-content {
            background-color: var(--color-success);
            color: white;
            border: none;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: auto;
            min-width: 250px;
        }
        .modal-success-center .modal-header,
        .modal-success-center .modal-footer {
            border: none;
        }
    </style>
</head>
<body>

    <div class="form-container">
        <h2 class="mb-4 text-center" style="color: var(--color-primary);">DATOS PARA EL DESPACHO</h2>

        <div class="alert alert-danger-custom mb-4 text-center">
            <b>ATENCIÓN:</b> El costo de envío y despacho a Expreso <i><b>CORRE POR CUENTA DEL CLIENTE</b></i>
        </div>

        <form id="formExpreso">
            <div id="errorExpreso" class="alert alert-danger d-none"></div>

            <div class="form-group mb-3">
                <label for="expreso_preferencia" class="form-label"><b><i>Expreso de preferencia *</i></b></label>
                <input type="text" class="form-control" id="expreso_preferencia" required placeholder="Ej: Vía Cargo, Correo Argentino">
            </div>

            <div class="form-group mb-3">
                <label for="expreso_email" class="form-label"><b><i>Email de contacto *</i></b></label>
                <input type="email" class="form-control" id="expreso_email" required placeholder="ejemplo@correo.com">
            </div>

            <div class="form-group mb-4">
                <label for="expreso_telefono" class="form-label"><b><i>Teléfono de contacto *</i></b></label>
                <input type="tel" class="form-control" id="expreso_telefono" required placeholder="Ej: 11 5555 5555">
            </div>

            <div class="form-group mb-4 d-flex justify-content-center">
                <button type="button" class="btn btn-primary" id="btnGuardarExpreso">
                    Guardar y Continuar
                </button>
            </div>
            <div class="form-group mb-4 d-flex justify-content-center">
                <button type="button" class="btn btn-primary" id="btnCerrar">
                    Cerrar
                </button>
            </div>
        </form>
    </div>

    <div id="redirection-area" class="mt-4 text-center d-none">
    </div>


    <div class="modal fade modal-success-center" id="successModal" tabindex="-1" aria-labelledby="successModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-sm">
            <div class="modal-content">
                <div class="modal-body text-center py-4">
                    <h5 class="mb-0">✅ ¡Datos cargados con éxito!</h5>
                </div>
            </div>
        </div>
    </div>
    
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js" integrity="sha384-FKyoEForCGlyvwx9Hj09JcYn3nv7wiPVlz7YYwJrWVcXK/BmnVDxM+D2scQbITxI" crossorigin="anonymous"></script>
    
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js" integrity="sha384-FKyoEForCGlyvwx9Hj09JcYn3nv7wiPVlz7YYwJrWVcXK/BmnVDxM+D2scQbITxI" crossorigin="anonymous"></script>

<script>
    document.addEventListener('DOMContentLoaded', () => {
        // --- CONFIGURACIÓN ---
        const REDIRECTION_URL = "https://natural-house.odoo.com/shop/checkout?try_skip_step=true";
        const CART_URL = "https://natural-house.odoo.com/shop/cart";
        const ADMIN_URL = "https://natural-house.odoo.com/web"; // URL de redirección para ADMIN
        const REDIRECTION_DELAY = 5; 

        // --- HELPERS ---
        const getEl = id => document.getElementById(id);

        // --- LÓGICA PRINCIPAL ---
        
        function iniciarRedireccion(finalUrl) {
            const redirectArea = getEl('redirection-area');
            redirectArea.classList.remove('d-none');
            let count = REDIRECTION_DELAY;

            // 1. Inyectar HTML inicial
            redirectArea.innerHTML = `
                <p class="h6" style="color: white; text-shadow: 1px 1px 2px rgba(0,0,0,0.5);">Redirigiendo en <span id="countdown">${count}</span> segundos...</p>
                <a href="${finalUrl}" class="btn btn-primary text-decoration-none">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-left-circle-fill me-2" viewBox="0 0 16 16">
                      <path d="M8 0a8 8 0 1 0 0 16A8 8 0 0 0 8 0m3.5 7.5a.5.5 0 0 1 0 1H5.707l2.147 2.146a.5.5 0 0 1-.708.708l-3-3a.5.5 0 0 1 0-.708l3-3a.5.5 0 1 1 .708.708L5.707 7.5z"/>
                    </svg>
                    Volver al sitio
                </a>
            `;

            const countdownEl = getEl('countdown');

            // 2. Iniciar contador
            const interval = setInterval(() => {
                count--;
                if (countdownEl) countdownEl.textContent = count;

                if (count <= 0) {
                    clearInterval(interval);
                    window.location.href = finalUrl;
                }
            }, 1000);
        }

        function guardarExpreso() {
            const pref = (getEl('expreso_preferencia') || {}).value || '';
            const email = (getEl('expreso_email') || {}).value || '';
            const tel = (getEl('expreso_telefono') || {}).value || '';
            const errorDiv = getEl('errorExpreso');
            const btnGuardar = getEl("btnGuardarExpreso");
            
            if (errorDiv) { errorDiv.classList.add('d-none'); errorDiv.textContent = ''; }
            if (!btnGuardar) return;

            // **********************************************
            // CLAVE: COMPROBACIÓN ESTRICTA DE "ADMIN"
            // **********************************************
            if (pref.trim() === "ADMINNH") { 
                window.location.href = ADMIN_URL;
                return; // Detiene toda la ejecución normal del formulario
            }
            // **********************************************
            // FIN DE COMPROBACIÓN ADMIN
            // **********************************************

            // 1. Validación (NORMAL)
            if (!pref.trim() || !email.trim() || !tel.trim()) {
                if (errorDiv) {
                    errorDiv.classList.remove('d-none');
                    errorDiv.textContent = 'Debe completar el Expreso, el Email y el Teléfono.';
                }
                return;
            }

            // Deshabilitar y mostrar animación de carga
            btnGuardar.disabled = true;
            btnGuardar.innerHTML = `<span class="spinner-border spinner-border-sm" role="status" aria-hidden="true"></span> Guardando...`;

            // 2. Simulación de Almacenamiento (3 segundos)
            setTimeout(() => {
                const datosExpreso = {
                    expreso_preferencia: pref.trim(),
                    expreso_email: email.trim(),
                    expreso_telefono: tel.trim(),
                    timestamp_guardado: new Date().toISOString()
                };

                // Almacenar en localStorage (como haríamos en Odoo)
                if (typeof localStorage !== 'undefined') {
                    localStorage.setItem('expreso_info_confirmed', JSON.stringify(datosExpreso));
                }
                
                // 3. Animación de éxito (transformación del botón)
                btnGuardar.innerHTML = '✓'; // Símbolo de tilde (✓)
                btnGuardar.classList.add('success-state');

                // Mostrar modal de éxito
                const successModal = new bootstrap.Modal(getEl('successModal'));
                successModal.show();
                
                // Ocultar modal de éxito después de 2 segundos
                setTimeout(() => {
                    successModal.hide();
                }, 2000);
                
                // 4. Iniciar redirección después de la animación
                setTimeout(() => {
                    // Revertir el botón (opcional, ya que se redirige)
                    btnGuardar.classList.remove('success-state');
                    btnGuardar.innerHTML = 'Guardado';
                    
                    // Iniciar la cuenta regresiva
                    iniciarRedireccion(REDIRECTION_URL); // Usamos REDIRECTION_URL estándar

                }, 500); // Pequeña pausa para ver el tilde
                
            }, 3000); 
        }
        
        // --- LÓGICA PARA EL BOTÓN 'CERRAR' ---
        const btnCerrar = getEl('btnCerrar');

        if (btnCerrar) {
            btnCerrar.addEventListener('click', () => {
                window.location.href = CART_URL; // Redirige al carrito
            });
        }

        // --- INICIALIZACIÓN ---
        getEl("btnGuardarExpreso") && getEl("btnGuardarExpreso").addEventListener('click', guardarExpreso);
    });
</script>
</body>
</html>
