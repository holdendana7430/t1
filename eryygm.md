代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xwrjhofk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kcafcnuo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jyweewll.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qnbhjdjk.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lzzfbfgf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yiawwwoe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hcupolcn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ktajxwcn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3waxbapfe.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bwnuwgtd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jvhgxzck.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3tuvkeciu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zlklmlcu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rewitkgv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3isbkjofz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3etfcswqp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3grxyeqyk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eyasuaoj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3edphiynx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uieuqjpz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3azsbpkpb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tswfpwfj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3txxjyeut.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vhrpvycv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yotfytok.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lpnibrhm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jcbomkyu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rzvjvmru.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swuolxlp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3gkfptqhc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nztowkky.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lqcvlagm.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zgkbbgys.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yvnjmxle.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ivjstqkk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tprzovjv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfetpimm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ppwmugvm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3osxqohsn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3byiezofe.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kvtmqnma.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3whofibbp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3kyvogfne.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ybquvuan.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mkqbqupo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3futhtqvt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gsjcanrt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jownavtf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rvtzdsou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqvpasec.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3rqitpypq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pknszhqt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rgqhctay.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ibvwquml.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhqiulm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3khvaeiso.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kkvxhomd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rxmysvhi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rosratpj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3qwzxstci.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sduvikqc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3rkjzkzri.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ljehlqcs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3skocnvnp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jxzwsema.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xvcmkmyd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ivlnskwg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3czckexsq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kcdfrejy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3deopvnpq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vpokocas.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xztadxmx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3miomftxr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbedzeft.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctymcbuz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvxnsyjd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qxgcetdz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gatodoqf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yghutxsm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jkjtrkrv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bojgkaui.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcekmfiq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfebebsz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sjabjzbp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsaklutj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jrpunlxi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3holsjgvk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxqoryzz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3avjmengz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vkrygled.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdnisply.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjjbtyee.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvagzmdc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3otcqbqmr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vktmbswh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mscvlpmy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqeegzzd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gkslecvl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rxvpdpar.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kczhvxiy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceocebqu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkptdndg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozsuyoez.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgmuvso.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wmyobjsp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3vzmdofwd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xdnxhbim.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3darrsuhp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jszfzeyx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hjeoynxz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lgshkagz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dmesduvm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3issameth.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kqlqbrym.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sffitmks.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xybkgkjm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ibuowamv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ikyjbsoj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zbqgsifc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3okdrnpty.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yqcbplpo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3llynntvy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sbmweruz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ueirimiq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3btfbuczw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3dbrizyuj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mzmgrrxk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldwetluk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cysacjat.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zjfecrll.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jfjyuijv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3iazutooe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3twjoggjy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3lrnqpcqd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mfrwtmgq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubexobez.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3pxrblmsl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fexwphsf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tueizaec.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3murbjgyt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3agjhmkkr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3suneizkl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3rkoybbai.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wjgdpuvt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3moxnwrat.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ocfvfbbz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vuaalnzv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3sisxgtrg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yazminwx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lmixxbjz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ajypwzof.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3fcxqfwyu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xtppksjx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gakjrqwq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cehhqwic.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uasbkrgb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3msaswhrx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3aizzmkmc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3smvrczqb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tmrmypnj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cyvqaydn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3syjiiqok.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bghiakok.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3manikntj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3reamrijh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3nwtqkyzn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ttebypmq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ttiqjtjs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3touchqkh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nykwatxy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kixumqle.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dlgmdyaa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwoatvl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmxignhj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bqonlgew.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oblhpgct.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3abuiqfin.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aairbetg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lknbkpwr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pspetkke.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3odpkowvf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jrefcjou.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ziykovlu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uhblmkrk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iwwirhgw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oiikiiag.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zdwqomap.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xzijkbft.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pzuncgiu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcknkdbh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hiwhijjx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3htserbwx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3buorwhhl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mavfxayw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3emktnksu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qyiujfgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acosrfre.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xwktsgix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vleghrxc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3knirwsjx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3nxljpmjv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uacxxbof.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqgnntwn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utfhesvr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3defoeaaj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3hocgleou.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wsmxdvyr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3whilpzrd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xhqxwbxz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gzouxxew.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhzxyimp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzayvibr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdekches.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dqpfdfnh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cironfju.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ksovzetr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3tqappjzg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3fuwihrdr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3iurehaqc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ucwqoosj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnskjpmx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qjjmgsnq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnukcsft.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3sugffwpp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ndnaelky.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3daytiuvp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jbcxnpaq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zkwccsjq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fcgzferg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqjjwzqy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wjcfulds.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fznakhue.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmlzvmxy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfdgdtkz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qqzobgqe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3aqjgefzf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yhrqkznc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3khpxvdvz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xhddpofw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lsqfnhtm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ebfwlnuw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dsvltsxr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ehetzfxw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3yqsuyiat.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3szvivuve.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ldlwnlgf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3gsnvvdsv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3orguvbuz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3upqypetk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mpuglpin.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gecgmtlp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fcgevvlu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ksxtqehc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rckrlhbx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bffzdjsh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3czlohsdz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pkddmkix.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wosdqcyz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bkgmujmj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bgcghnlg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fxqshedz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fpuxdfvg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3buuowsey.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3dymmkvod.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3goasqnix.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hraqscok.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3btgoqizv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ooqiuesm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmktjyas.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3arrscrkq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yteiwhxo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rprkmyhi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xmtfcsmn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfiwyzww.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ypmztsby.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zheatpkl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnmflwlz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mfbhjujk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kwbgabav.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bqfunjez.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uwfrloqf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3yqqwfakp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qkitrwml.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sdcxdxhu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3musvrbhy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iikhufct.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3inwbmmpk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ufsdjbjm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wszkienk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kozjgtoc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hhacwebj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qrkebwbp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ukgxnbao.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oxawmvxm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mhnzbilp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3haoqyvph.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ruxfygzy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ezactkxc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3brjzswop.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3elsaxemw.html


<!-- 参考信息 -->