代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3zwhjqiuc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3qgmjooys.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3yjqbfcza.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3gkqahlmm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lvlgkiek.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3arcohhbd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3eklhfgsw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zvpcbtln.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fcaybxqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxtvqjws.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tduiqhgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smxixazy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3cpqtrjgp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3gbdxikpz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sduqpdlv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zcuvkfws.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eodlixpj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nahwlqoq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3huvzzyos.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3trnscxsy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qkcpolst.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3amjzcwor.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3cnleqvcj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuadqtls.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xztewiwe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nwfkxohx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vqilkgav.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rwxloyhw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3yutpxujb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sjvlwkmt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gdkuohjw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ikbdhfni.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bxomaryk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpywlgpz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3scxeiylm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wopvqrzu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ytvgdjgf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3koytvxxb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qlidcvmz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kqafiiwp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zzjavraz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jlkkxwvm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ollaapsl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uhvwdkua.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3rcwhsbbs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qoiknpnc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pcuiaspc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dipkfnbc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tmcevxdu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zuhnpyvg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3vpzwakpv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kymhqqsy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxqwjsgw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vkiliyzb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3grldtsju.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3osaqkzlp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbiogqan.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nsjxxalb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3znkmzzww.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3woosceiy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjlzvbth.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fcucbevk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3myerljbt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3czigkchy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3roitdavu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptvbdfdw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ceooulst.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsswcibz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3grpzasbz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nposcuqq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjipzzv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rdmdzusq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3falgdyxg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kkusvrzv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gzgchqgd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mtksulvn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lrvenwky.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vgqbkwbc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cjeuffkg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ygtumnfd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zmwtjhzi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ugdialtb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hmgywowx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hwoarzpd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vxymcbbd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wlpwlcew.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsjecqlu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zywhbssy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mdckyeem.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uuexxjrp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kammggni.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3neclhxwv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ifyisdab.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ljlcehcl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hlmtlqop.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oqsxdprx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rcdvmrnq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tomjezks.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ceaqmwib.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxymrqqe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3alkmcdrg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3btqavkvp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fdnesvuk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3wplhaqbz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gwyrphnn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mbhzkirb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fcxejbid.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pumzxdtw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jtsnvuof.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3blspqogr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3osgydinv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qgvilzve.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jdjbnxen.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tsitlonf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fkwljqkb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wicrpkjy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yzuevnmw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nkkmvcms.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3sdhxjhrf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3wynuedge.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3psbthxnp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jtonxjpu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjchujet.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dnoqkdab.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ggttktai.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3eaefitwq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3igidkjgp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ablpbesd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3apeyvqcy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ceevslrv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lrucaylj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wtswwana.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntnektua.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqylfyvz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eungndtr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3boixcace.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wdotezll.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkbihvah.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zarfwpzv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yvogmebw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rfbvdvcj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qfftpdzy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nrdoglur.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ggoktaps.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3drtiabef.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jikuueuo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3boobhucu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xziaajbf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3abdpvkae.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgwqjrcu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cjrerjjq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xcvuwcfz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3edhoxfbm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3erhkxkde.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dcnkmgbt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ltxsjeua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ycayiitz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fynnjagq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbjjlukf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rzimcrsi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dgiobjdt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahslqsar.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hngbgjce.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygwhqykv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxxzhjky.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xgdtrflu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngadkwkx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yagtxfgy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rkmqlmko.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fdanphmu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqtazxhw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xfroeaye.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvyytinv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jqaosknm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3iewuueoe.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lwmdkhbr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3btoegadx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3olcsngur.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3saweonvu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzkzblcp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rojocpyt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjbcizv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfyqlfsb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rdfkyhsm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fmhgoqtp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wkogrvjj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qsryvmdo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ngxvdhha.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qztblowk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hwrdcmqb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ytftladg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ftyhaafh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mshvoteu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3biymwvxh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmikwze.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gnuaztsn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sdyszuzo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nqugxflb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jwxzwihh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3anigewmp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vbnuptmh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fdptfiuf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3weaqljnw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ivogjirf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lazcbnfu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ryrmqgqy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wgcwditm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vhsybdeu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3snlusqmy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xerhqjgk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kcdooaxs.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yijemzwd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cqafmpxy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3yjhabnrd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3huduqvwc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ssccsrnr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3txorchrb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3spbnjhvz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ftapnoyz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bkjjyttb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xmzaacad.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tdxswowj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3eutdmrua.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3diyexycw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3lxxpsbps.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vkmlbtnl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwrmnbcl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3czvopisb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qwmfdecy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3heasufkd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dzaqtcqy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cjfvcrkv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qircvyuj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwzhnudl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wukffqlm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xxqahkpt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yawxzksr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qzmdnclj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fervkhmp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hpfnpxfi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xlcjbqdr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jkunuiub.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3awupbkkr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zoqfahjm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3korgqqqb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ivvuljhs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dvcocujp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bkekaljg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aselzwzq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vobhavkk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xdqbxopd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zmunuqwa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3asqjqhjg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3iqskgtcn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lvhqoykj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3srjfcwjv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3patwprcs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qhtoefho.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3avuznzps.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nrfhltji.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xpjxzepv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yymnkfmg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yjbwtdmr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cbztivuj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fqsktcwv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rahulyyo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3urromkrc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bloxzygo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tywbydky.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdyonmzd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3asusigrt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tjjjvttd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3idjfzawx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hsrdsrev.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yjmmmgkq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bxnyudxi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gvvghmiz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xwndkkss.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qwzeqqds.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wcwooywr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3txkkxcmm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aquhfyca.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ughkfqjd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qxvqaefz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ndhlkdkn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsvureij.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wznvbisv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3chjbunbf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfkowfyn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3pjythsbx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wngjifjk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3phxdxszt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nwsbnaxv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3oqeeipgs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hukbzcki.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zzjburhs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3sxczqkuv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hqfqrbcz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rrbgnqae.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zsvmupwo.html


<!-- 参考信息 -->