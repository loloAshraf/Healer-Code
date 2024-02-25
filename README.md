# Healer-Code
def diagnose_kidney_failure(symptoms):
    # تحليل الأعراض وطباعة التشخيص
    print('الأعراض:')
    for symptom, value in symptoms.items():
        print(f'{symptom}: {value}')

    # تحديد ما إذا كان هناك احتمال للفشل الكلوي بناءً على الأعراض
    if symptoms.get('هرش في الشمس', False) and symptoms.get('ألم في المعدة', False) \
            and symptoms.get('لا يستجيب للعلاج', False) and symptoms.get('ترجيع حصاوي على الكلي'):
        print('تحذير: هناك احتمال للفشل الكلوي. يُنصح بزيارة الطبيب فورًا للتقييم.')
    else:
        print('الأعراض غير مرتبطة بالفشل الكلوي.')

# استخدام الدالة مع أعراض عشوائية (لأغراض توضيحية)
symptoms = {'هرش في الشمس': False, 'ألم في المعدة': False, 'لا يستجيب للعلاج': False, 'ترجيع حصاوي على الكلي': False}
diagnose_kidney_failure(symptoms)
