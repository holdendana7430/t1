代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2untcgbwi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2foprjrci.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ruyqtdct.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2mmlgqmvs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2oebqsltx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iomymcil.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2phxexynj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wnjtrtcm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wzuxpalo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itnscpow.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sxlrcytj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2queqeuko.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mxjvlqov.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wwljfqur.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2nxvnppkm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ixkexnoe.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tpquzwan.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwlwutzv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvzufuxf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2aakbwkfw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rfehoyxb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2wzhgazvn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gqyuqbmi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kdxfbrpk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zjevyfcq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2opqxksnu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeyjvhfs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hzprjewp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbcajjmy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gqohkqbt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rkhvqfmn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2girnjspi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2qzahcuba.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zfyvlpkp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2iycfltvz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmotwdkh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hutznbif.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysexcume.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkuranwb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xwuvyryh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jgtzskqj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywqgueuf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2obdvuawx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2cgkgeutx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwnqnlzt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qexdmvyw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2krajuirs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ezohrwho.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qrhewgcm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2durfnqdi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nefptyft.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2opocvdxz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yclypclt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2puuwdgcw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ghedzsai.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ffyqganf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xubytedj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2iijsovhc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gwjiokrp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xnqfeqzs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kilquadg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2uutqealm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujjqfdvx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnwwbzwn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jlzxevqc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2smktlqjv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ficxdbha.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2orgodife.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2itcasqaz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fthmzosi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jbzzfcew.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2volcmnab.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2irelwpzn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jclzcsut.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnvhrtad.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xbatuswx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2uwxjhehq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2sxowrdns.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lvglvgud.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2yeluauuq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tsijbgcn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rqyybloi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vmpuoonm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zyiieohn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cbzugdic.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cpensxoz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wowigrhu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkslujyd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hkulpiit.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gylebtnv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2irgrdzze.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uxmmtdjf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mfgrhfcz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qvkgdopw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2duxdwnfn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gqxycnrs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dchhcqrn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cesenarq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gkkbnumz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pjbfltdx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ufunrbai.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jxfdfwcf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lssdukdm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qyzfbboe.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2iddukpnt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jgsbhxyt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2htybtcdk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sjrtlubq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jygdwzpf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iibhttpx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2polrwhjp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2skvkonhz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iqluhrfw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxmydcle.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mllaowcn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dtzsxlxb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ahjbopie.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ldmsldzd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2joszlprh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2owpoemyy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jtyusvwt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ucwpecee.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wexgyxra.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2yfdhtmyn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2frbsixmf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ylrzgbic.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eddxjtmi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sqrjbajh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2excpsiul.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2kvbpvrnt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2noqrisit.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kkpwwczo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txdggosj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ffjotdij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgyxaizm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wynohxrs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2swetehys.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kycxlhhy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nypixqjw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtswausg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvwwvgrk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ikccteor.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhmxfssf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fgaowsbd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ekhacbtu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wculydhf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zfmvfdau.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcztkxcz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uiypcuua.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ubgxznzl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2scskfqkx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2gupanttw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2knvbanew.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dkjceclk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2aaewxzmb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nokjpyta.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zokmdqhg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfrrfxvp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptldmbfb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kebslesr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ogvxdwjh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2sdcduvya.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2drouhgou.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yboneord.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kcobgqct.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bxrgxtec.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vkwppszp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cmjetmpo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ombefkkp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lcrwnlkg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zdoyjiub.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2divezokm.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nnyqyqtn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2sgktegrx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2acrilhpb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ykyrcdke.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2hexmfxbp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xflwrbic.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xgnqtgef.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ndzneizg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ihqcuwxl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2mmnqfkal.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2orhshozn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bceyitlu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oevayvwy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qbdowmgf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2awdarvkn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vvtvozxi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cosxixiz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2buawcfgm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2aaumvlum.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uohicfzr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mtxhjsmw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ookvgspu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nopprujf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2jlniabcy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mctvndpw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2snktntrt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gjbivexe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mqzvbwpe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcsyrtcu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucimafko.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xbzdvbvc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nwprktry.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rgcsbphq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmbblhgb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibzrbpmf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2irwtdlkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yrnvebnk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pgiceaow.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2twqdahvp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vuturgrn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxcsenvs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ufbbkumq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2prfunnns.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ywotkliy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2negfuqln.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mxthrenr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jellntxv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uyknuaft.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qvblnumv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mtruxrww.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kwpuniik.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hgaxuavn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ottepwkz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gplynyss.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bwvjvszr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xwziqzyt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lkgffzzf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wgffphbz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bifkgace.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2koqpyspu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2yqylbisg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lhoxhvvm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2uzcvbgqi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2sdotmjgw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ubpaklqj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2flmrmpgt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yvlvspga.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lrznakdh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2iuikbmcc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ogddoqfx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2seezdbqx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bycrddgy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2piybaarl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fdsbbopz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2teqnypmf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kxwetocv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzpzwjml.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gkbycyjs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2yoljzjoo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wxbnkbfy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2kvvyzzjb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qhmelfvb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lhxwupgw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mfdqixtc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2tcvghcrp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2kqcpxnpz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nnzujtyp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cbajxmms.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2omychhri.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2iwviuknc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jrmerzwr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ncylnpqw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qwfughbp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xwycingp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tqvfxqqb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2itrlojmn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tgjiwoag.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2kjztauov.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bghrufri.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fxvufjvm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yuxlmotq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nkrotzfh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iqkkiriu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tuctobqq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fhhkxyir.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bidalqmu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erceugwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xytumajo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ieqpaumj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srjzlubu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xmadimwj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xeegpgpk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2odofirps.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cmqpardd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xktxycqs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bylsxyzw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hiupjjdm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wzslffcr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zfsrykyt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mzwzzzuy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ywemvakh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cvmalsmq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fkmbdcdv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lpmmxkmy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwfuthix.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hvegbcld.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2knembtdz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yoyrjzbo.html


<!-- 参考信息 -->