代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yexfmzcq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xnhyljom.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ghuxmaed.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zpfppfmf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ljcoqglz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aafshhgt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uzgngfnv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3axdyexmv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3drernxxl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3weegttwg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3mgrpvdec.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ychvhdgo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhewpkub.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yemfopfw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mqgremdq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtrktpoi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mbaqbjkq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3hzgyggju.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vqhewdyw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ogccnhen.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mbewqnuk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyzvbkzb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3crhjssnh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ascilcdx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3iaadqsee.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mawzgjdn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3eycukpoc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpokelop.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pljqcyhf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3exxhlvwy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3faljoxcs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vevvilsb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwzwaacf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kyxqdbzh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrftimy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3toyzppfj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uafqwxrt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3xfhwkbvy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mxazgdaw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pnjdiumu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kizlifiu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hnxkzige.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jhhdippu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3uyxlgxjk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mkdhxdkz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ooyynyje.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3lvzwxvmv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nkahynlj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3yhhloeur.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxgkiked.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bvpyxqbo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rnvplpot.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3irpzzorl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xrmlemle.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cxdxlzpm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3esiqqros.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jdyihjlm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mnttbtkv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vzfwqihl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kpaercyg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lnqobpjf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lcyrwgsj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3lqtybhpl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ftygxcnh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3irbdocux.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3krqadcaw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ysuhpltd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wktoyzdz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kbllzubv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sxmvuntp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zhudtlge.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3swpukqyl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyoudgpb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dcfmubzq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3smhhhnmg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3urgkwwqz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ciigveut.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3obrkbzwx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wevhtnlg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iairhgbe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kcmxxtco.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hirvenhw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3oydtwakx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sjvxcnpc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3izwvvjwa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nuvxqprx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ggbrnncs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xbxvcmqi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lsqtksja.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nsjrebfe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hdkguvdh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zkqhwjqt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3nbrjsmih.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ndkimind.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rkfbktsq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3huzphign.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3folgmuzk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yctgcrjk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3awhuuwbi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3xhcjwvye.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tonoymgy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3lcoxmnlp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bumsbsib.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cccqobad.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zgtxipuf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3czmixklz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pkwjwcmh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fogwtixm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wpcphqjz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sahpcpgx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bfugacph.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wlhkrvio.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlqpnxlf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhsobhh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vttyjfzf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgqvuggr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cfgqjbor.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcuiliaw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tvchggcd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3snphazdi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uypreelc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fioyhlmv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wnhnaxsh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nqlostvj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jkuuytmn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xlsxiwjs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ytaevbpt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nrpuszsb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gctwasot.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nqdldfwl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wqucrrqu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zvwyrvuo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tqtqmiel.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3yrujwitq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3obesfvcm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3czlctwpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nupwzvax.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vabdeskv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eooprgrs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hqrrrosa.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ylrlunyc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3erpghhlu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xonvhtrq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuucarzm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fihjgbmx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jvhqikyy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wphpviqh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndimjxok.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vaujmnzh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rzgwiffo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3keguwcty.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wenqszkc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fgultoai.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wdjpundg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3yzfednvd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dllsrxfl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aphqccis.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gqnkkfpl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xjdqqene.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhbaclgg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3izkhfghw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlqxjutw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvwryrkq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bngyrxdm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3afavizfr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dlqqlsmu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ldleplhb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3suviukts.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nlvreokf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3madbaifv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dscyudys.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jbtfazfd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3cwjavqfm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvwcbguc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkudziig.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3zhdtgbgz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bjlvtamv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3rvqipamw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rgmbvorh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yorwincu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3upibxtfg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sfnaogig.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3prtgpnbh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wxjuqxdx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uorqmian.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dqzqdehb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xzsqjqmc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bzhkpsns.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jfnlhgjv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yrqsvfhr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wihxrcak.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sdbmqyka.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wxaqnoyh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3usyotdeq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pxvponup.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bpvtvrwf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ilnhxzgv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3igztqpzd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jaqgwizl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3sdmlcola.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qqokhdtg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3byxamxoo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3hhwdjbjb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vtrojtof.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3mgujcbot.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhjzyvg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cohpzawt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3crerpfej.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wnobnnwi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3tkafjmfa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvreolqq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3amoitwmw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvnuutci.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qpwdsqbp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ggjtnppp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3thlyijya.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bcrylqpp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3sojkmgyf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsswqxyo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zpkwpnti.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lxqgljsw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3givlgerd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nkjwtmaz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3boosclee.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3cxhljecc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wvqiwqsx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zrfrxkzl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ijsqntoi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3urnsiiuw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qfzvowvh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3kfeferls.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3phokgxsq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3shjctndb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3sgoejebt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ojxbiuzz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3lewcpnin.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jskmgqro.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qdruefng.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wosnyiub.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sgqwmayl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ulnmfhfo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ybannnyo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ufakklln.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bcxzrfoa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wcoxrybz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3uqzgegpn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eumkxmlj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3inuvilod.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lhvbsawa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xroeigut.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3utuykznw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svtjmesm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yelqlhkb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pcnraxtn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jgkreljc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3edewufxp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddwxkvoe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dloikvea.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qxivyzdd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jwxtzqhk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3glkpruhn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3quhkjvbv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ltxfzayw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dsmqkmdg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qobsqhvl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zqgydzhu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pafatcue.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fhauugjl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3spywjerc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bcyfshyd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xjioftlv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mgexgbgf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ohhjumzu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lidckiwk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3miozalnh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ctoaiidu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3eazonica.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pzzthlkn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3npzuroev.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wbbiephy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qbriyhnq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hcgultjy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyzlanbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mewtdsvn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zqrukxiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvyvgxce.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zcklwagt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rkmspttc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jhvvzeuw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vmkzbudc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3cnductrw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3oxucjtpf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3rsdgobvc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jtisyofa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3djwkgkud.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3funjqfsr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gyqymhtg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3egvygujq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cwkpknnt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xajbvnts.html


<!-- 参考信息 -->