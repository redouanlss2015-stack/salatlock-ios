
import SwiftUI

struct ContentView: View {
    private let prayers = [
        ("Fajr", "Aube"),
        ("Dhuhr", "Midi"),
        ("Asr", "Après-midi"),
        ("Maghrib", "Coucher du soleil"),
        ("Isha", "Nuit")
    ]

    var body: some View {
        NavigationStack {
            VStack(spacing: 20) {
                Text("SalatLock")
                    .font(.largeTitle.bold())

                Text("Tes prières, ta concentration")
                    .foregroundStyle(.secondary)

                ForEach(prayers, id: \.0) { prayer in
                    HStack {
                        VStack(alignment: .leading) {
                            Text(prayer.0)
                                .font(.headline)
                            Text(prayer.1)
                                .font(.caption)
                                .foregroundStyle(.secondary)
                        }

                        Spacer()

                        Image(systemName: "moon.stars.fill")
                            .foregroundStyle(.green)
                    }
                    .padding()
                    .background(.green.opacity(0.1))
                    .clipShape(RoundedRectangle(cornerRadius: 14))
                }

                Text("Les horaires seront ajoutés ensuite.")
                    .font(.footnote)
                    .foregroundStyle(.secondary)

                Spacer()
            }
            .padding()
        }
    }
}

#Preview {
    ContentView()
}
