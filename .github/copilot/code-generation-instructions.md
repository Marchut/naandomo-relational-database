- Adhere to SOLID, DRY, and KISS principles.
- Create small, reusable, single-purpose functions in English.
- Split complex functions into private functions and use a coordinator function for orchestration.
- Implement Hexagonal architecture.
- Use this folder structure:
    - `/adapters`
    - `/blueprints`
    - `/domain/dtos`
    - `/domain/interfaces`
    - `/services`
    - `/settings`
- Write concise, documented functions without `:params` or `:return`.
- Use typed variables and descriptive booleans.
- Avoid inline comments.
- Prefix private functions with `_`.

### DTO Guidelines  
- `/domain/dtos/common_dto.py`: Typed structures referencing other folders.
- `/domain/dtos/core_dto.py`: Bridges Hexagonal layers.
- `/domain/dtos/input_dto.py`: Structures external input.
- `/domain/dtos/output_dto.py`: Structures consumer responses.
- `/domain/dtos/request_dto.py`: Structures outgoing requests.
- `/domain/dtos/response_dto.py`: Structures incoming responses.
- Public functions must accept and return DTOs.