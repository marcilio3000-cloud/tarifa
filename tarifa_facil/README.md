# Tarifa Fácil

App Flutter para cálculo de corrida por km com tarifa dinâmica, mapa, rota, configurações e histórico.

## Como rodar
1. Instale Flutter.
2. Na pasta do projeto: `flutter pub get`
3. Android: `flutter run` ou `flutter build apk --release`

## Como funciona
- Toque no mapa para definir origem e destino.
- A rota é calculada pelo OSRM e a distância entra automaticamente no cálculo.
- Fórmula: `max(tarifa_mínima, (tarifa_base + km × preço_por_km) × multiplicador_dinâmico)`.
- Configurações e histórico ficam salvos localmente.

## Produção
O app usa tiles do OpenStreetMap e o endpoint público de demonstração do OSRM. Para publicar comercialmente, recomenda-se contratar/usar um provedor de mapas/roteamento com limites e chave próprios.
