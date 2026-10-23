代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ugxpvncy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3rpvuadbs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3emjfqepl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3jbtsoryp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjwvsbsf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wmzrwrgc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypuxiyfl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ioefusfd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjhpxri.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3clnfqezc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dnigftpl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3plnpwziz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gcrgyyng.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxbsyoqn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3bwutnqgk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3sjdjeoqc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3twlmushs.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fhuzbttt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3mkefelhr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rlfunfet.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3weeffray.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qcreykmq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pywspquf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zbejcuwl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ymcyytwx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tmaasplg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kjipzdia.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmweqrlb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tegcymzl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3sogatfzx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3temvceui.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3npvzhrdd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3rvcwstyy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ybsqktvn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gcyznake.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3uqxziknu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ksflsrqt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mckhgsim.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wjhvipug.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uxzdsbrx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3afzxgdxi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wlnvoiaw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3esskbbxj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vhlhufjt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3yxidelmc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xsegornx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3qxkiihwh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qakhzqqt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xsvnxwbt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3enfbmuth.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ggacodql.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cricqhrt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pydpwcep.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3naqprzfj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3focfowmy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tbuwdjbu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yxxwlmwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwpjuwzp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hvhawndg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfottxoj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mdouojyz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3jxevefjv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sygfszmm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3euskbzmw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gmsklamy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kdwohphm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mdbzwaay.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3yhbiayli.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rmswoxvy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3wyrtjdfa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vppxiecn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3drumlqaw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3prljirya.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wlrxjisx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3myskmpqr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ljtfyigl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ywjvmfir.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lwxxvnge.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jcxgmvkb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3vvwsisgu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcdvsbea.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3liwkjjwi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3josxvwfz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ytlrolea.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bidedbfm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vhvklhtw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cokpdyph.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lpieefiz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rcuhnrjs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3djbqzyhi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bowkvfsz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwklvjfs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xapdtsku.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3iuwyanap.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ubvfgidq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oofyttwr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gwcjmyjo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xixtebmk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3pxzregqd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdxzadgg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmfgdnne.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3atmlmazo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3oogjhfxm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gwqqecet.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3prvsdkak.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kcbutexc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3xraeglbp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3cfkfoxxt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zwcjcoys.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcldxofx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3coygzofl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3qazanaaf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bnjnrphb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3cxorwoqk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ovorkugd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3szuohnhq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtpijlqu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wcuzjokd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcgzjgma.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgvktyn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3glocihat.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3hjcjyukq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fetwclhu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xjpxhcqy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ynuwpnha.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ujqdupat.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vtdqelax.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nlijaqjl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dqymujvm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3cttjyalp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ozqzatwh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lzhfvqvt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ajlipocy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ovlslowb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnelxpmr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aaromuxn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fpfjmkco.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryfmwfzz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iedptvme.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jqkvbroo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rfwobalq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ipezzeoz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nlakbkrj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdfolee.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ilagfrtv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3javstjms.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3pkjkalpj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3smodymxj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kfrrygsk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fsewrcmv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3odvxdbyl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fdmcvcln.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hwyhtoip.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3spkyhrpi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3plcaidbz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dbaytvhb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kdgomltb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rmjjnbbc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ubbexxmt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xkboynjr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dyvtqujk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nqhdyklk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jctusrpj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3agevbcjo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tkjecduy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mihdxzrm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jsxvbkgm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mhjovfsu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xzpcnihg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3hjiqsmuf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmesjov.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoruflot.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdciatid.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mijutclh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vvmpchsg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vlwcltqo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fyqtgfac.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3idlbmdql.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vokkiylf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3btuagyic.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qseziwqg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xodixuqp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hygrztth.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oafmwkhd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgbrpgz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcdfmne.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3emcdxbqk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pupprmnu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3swzpzjsh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lmkgjcmi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vbiyasph.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ivoibbem.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jsuxhshu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ahqpikry.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3naqfdwhu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3oruuatmu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3idsbyuge.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bcgzyjdf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jowymrnn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ylqfojag.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ascmnsir.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ymeckkyc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fskgmldk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rvxglusc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epsmadql.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vkljlmwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3voixvyjv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ncabtsfk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pjtaxphu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3orcprfhm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dotpgyxp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhpjuji.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqssrisg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3loaugdbb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3sdzzzhjk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpzlwgll.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kxtdjkby.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3faonnspl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3cwlmaufe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvvtkbow.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xcwtctsd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3czgjynrq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3srqgejif.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ofdwuirv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rehqoiil.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jzevowie.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ojrqatwq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqmlftdw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3srcoawgt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hiyxcyqz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3enqvfdto.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zrviwdxy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddqbuglu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3nzwgilpr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bmxmvnlp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zbwgpxvk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3wcmhvhha.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bswaktqc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nvzmfoqv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uojplknr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3glhjwefb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3sxuukypy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bypbcbfx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3prbuynlk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3iomqkjhj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3juorjwrp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eqxnjnap.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3loxeavgb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ppjanqrc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mkelqfkj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rxjcxlwh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fotgxrrt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3noknhnlz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xkwasipu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hxrxykoi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qsxkqupo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zoetcviy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3eodquxum.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zwcajaxh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3oipxpzph.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wurtlgoc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tqglmzpu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xwihhqhd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3newmpxvt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lefvpxjk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yiiemujb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ebynzoky.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3prnnrfal.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ackekmnr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tzzskbku.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ahkikyaq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nlkcjtcw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tzevnxpn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pjhkjygd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppjsjreg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3oozkpdmo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yqvtjefd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ecyyspzn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziteykcx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lsgndijm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mlcdkgxg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktzniktq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nurgamah.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lyoiiyes.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3eknzgblp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3jfajxlfz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jttvqhvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rtlxuvzu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fvskqzoz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3joiwuftx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ogfropnw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mznpdpos.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rmwmzubn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tkdhakpd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gfduwjgv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cjpemaul.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rlxzsboa.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fstzcohi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ulsnronv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bsuretio.html


<!-- 参考信息 -->