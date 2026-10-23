代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqcymjb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3dsoakzff.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vlhxtbqh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3edhxysbd.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zwmyzkbt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kifpjdek.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tqixtdda.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhkgimug.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gvwrnpjb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zxvpvobs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xtsejgeo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3biscstoz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3exudqxtw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3vjrjhvmo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mjshwqke.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vjdqezfd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rtuabxis.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iohcffun.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixrbfkhi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fazltaqh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xavgrhmy.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oonxmqws.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fqnleqhy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3dvfjbtkq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ddgdauhl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bujtvlyi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kzadtdxv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uosxncig.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3woizgehe.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3bvyeklyr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3aknstlmd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qzgkyfwa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwfwddp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmmmlcig.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ghfwivvs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3eyhjdjwv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ocautgdk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3cpumvjrp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wxrjswmz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3czdmggvu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3clavgfkt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3dgxhhmro.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wdtvpujv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujcxobcq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxvmcgj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3denudlny.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3vqimeulg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbsmvim.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xcvhsdok.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lgbaktoi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3idlhndoh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3pyjcxjzd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wtbbupdw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xaqjlete.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3vrzxdxjc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fbpxasgx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhdvomz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bulfbhbg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pyjkgxch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfhsvhuo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3snswzijc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3akaldzou.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wiiedakj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ecoocwbg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ocskbovz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sxrvcvoe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dhqinoqc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ymtvldyu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ywuegtxa.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3navjklwm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3urxrhjij.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kqdojals.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fxkwbovs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wocqkqeu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3arcsmvqr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3smafmwpk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3slhlvqqp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zzcdbzsi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3djeugxhr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3yhdjmgcx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wchwxvxx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3keitqihg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iratzvwt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jngzjddq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gwpuferd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rjdelvet.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3llanvhlw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mtjdniwt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3pornavvb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovduncct.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rriahyio.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyrmohql.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gkkeevpm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vzxqstat.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3aayjaism.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwzuvddm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lflyaknx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3yezsmxce.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3gojnwmks.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3izeglabs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fnpvungo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pjzobxwd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kftzxqcr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pmqpnpfi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3knebpwqe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ebtddzjf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wwbpktfs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnhkabpt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqhcrucr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwignutw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tttscjnu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ryzyzofu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tusqnokp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gbiafmtz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmpkaogs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mtsossks.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gygrfluo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ajfhtbxt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlykvdrm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwgavzul.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xiyltygs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kkuygntq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pysklcba.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3fiozvbva.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pbylizih.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qizlfyxv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pjufponf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wpgjyiok.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qngcnjxu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nsksehnn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cvwyowhf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vleromwd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zemfewky.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3sydctxok.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3takcxbiu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pmbdteba.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzawbbht.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gongtxuq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xwaeiopn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3umyimdxq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvfuijo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3lxfsfbmy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3oibqrvdf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pymzzjja.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jsoeojar.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3siubhdha.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3pioahses.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hjrdgxlq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3njuwmwad.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqxmcsff.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3flyvpryn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bgzxleqp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ubppbcgo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lnunearl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xsiuwrqu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxlqvzoq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fcdrkfkx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3swytxzaq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lunqtdls.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bkqxmftl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nqyniwlh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xykojhoe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lpkesyvm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fkvxamsv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hmjvdltd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cidwalke.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qgwcktoa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fcpjbxxk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3sogyczzi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3lcarpkoa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxcxaapy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlinpwvu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcwklrm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pfsmkqps.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qxfmswnj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ejxdaibs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dmdapnwt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mcetpxec.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wvorwemu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gfljxqsz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxvrwzft.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nakxpntg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgedljgr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ofwgykan.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxxfpezt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hgegxknm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qdrpntvw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bzgddyul.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3qbdtjyyi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aigxnfsm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3obzkxxdz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nkbefktb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nthxaqwt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tkclgwyo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ylgkytri.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3lwdyqnqz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3nzfkkntx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3znqeexxb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3griqkyxj.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3npxzipbx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gbxtcfzz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cqowjaoz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zacirbay.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fjizfoek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuebooor.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cyeqwutt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sprtadpg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mqcmgztr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bddgmwjg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lgiyfpmx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fkqxqckv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sxgseupm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xtrauqjz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ebztcygu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kqwmorpz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jkjokvhf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3oxftwega.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uginkrii.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ujzvlqde.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfikpmyn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3orjmhlqm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kbbojrvi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gqdkoqtz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hkpqztbk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yhvotxkk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mnwvexqa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ohwpskvc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dybdrjde.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uomfvqsq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjpcvzau.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3rtqlzmrx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3wawsbopx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tnstptcz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gxodmuhw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hvolqjmq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gcelrfzh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qlhembgj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3iveruspx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xfpbypzv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wpbjnmrm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3umxhtuff.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvncdqrj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ltumycnu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3borzrwdj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3niqnvrug.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3faxcgrsm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wxotdnds.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mbfworbe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nfxytvhx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tdaeugwl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vifvpggf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nivkcvbh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3khimmepy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vbjhscif.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3gjujowtf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kxkmxwfv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wrvizpsn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jqeiwicz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ljneooja.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3amauzjtk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3juovtxjh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qdxkxoti.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3sqvboipv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkbbkxrm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hbptydyw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ymjchqnm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dejxuzhx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3erojpoxu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qstzqdpn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dlhaghyo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3pqunpbhv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3aqhqxzkl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wcqufaoy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dftfrhoc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dikzrloc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mivyxxrr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rqhcapff.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xonluvak.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tklfzduq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nqjfrkbx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ipokfdtn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3scerryyn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ildtbeug.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gwtgoecf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nsbsdirn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hritpugn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtlkvbqr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iqdpdswj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kerjqkou.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tjtliydm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hxpeuceb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3atvdyixx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xalkpyds.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tfoevnmy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vvgjqefy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bmhcpdiq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lblfxvoa.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fwzgqsvj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xgktygby.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mzumwhjo.html


<!-- 参考信息 -->