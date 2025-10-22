# math-rag-chatbot
# AI Math Problem Chatbot (RAG - Gemini API)

## Projenin Amacı
Bu proje, matematik problemleri veri seti kullanarak Retrieval-Augmented Generation (RAG) tabanlı bir yapay zekâ sohbet sistemi geliştirmeyi amaçlar. Kullanıcı, belirli bir matematik problemi hakkında soru sorduğunda, sistem ilgili veri parçalarını bulur ve Gemini modeliyle açıklayıcı bir cevap üretir.

## Veri Seti
- Kaynak: [Kaggle - Math Problems (IMO)](https://www.kaggle.com/datasets/chengjinzhang/math-problems-imo)  
- Format: `parquet`  
- İçerik: Problem ifadeleri ve çözümleri  

## Kullanılan Teknolojiler
| Katman | Teknoloji |
|--------|------------|
| Embedding | Gemini Embedding API veya Mock |
| Vektör Veritabanı | FAISS |
| RAG Pipeline | Python + Numpy + Pandas |
| UI | Gradio |
| Model | Gemini 1.5 Pro |

## Çalışma Kılavuzu (Kurulum ve Çalıştırma)

Bu proje, bir Python sanal ortamı (`virtualenv`) içinde çalıştırılmak üzere tasarlanmıştır. Projeyi lokalinizde veya bulut ortamında ayağa kaldırmak için aşağıdaki adımları izleyin.

#### Adım 1: Sanal Ortam (Virtual Environment) Kurulumu

Proje bağımlılık çakışmalarını önlemek için bir sanal ortam oluşturulması şiddetle tavsiye edilir.

```bash
# Sanal ortam oluşturma
python3 -m venv venv

# Sanal ortamı etkinleştirme (Linux/macOS)
source venv/bin/activate

# Sanal ortamı etkinleştirme (Windows - PowerShell)
.\venv\Scripts\activate
