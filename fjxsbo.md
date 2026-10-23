代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ccvjawct.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ulcmtuhe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aqhrlwoo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3brggvegf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hplnoptb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xlecvflo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3utixkglq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lwlpqety.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3eeomkzgs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ikmbuini.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xhoigygd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3htvabxue.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lpxejcdx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfpkinf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbwwuqcp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqxheavh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhkotvin.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3arwrxvou.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zzuhhfdx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3nnojbioz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgyimrtt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rxqvbsvd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3viujjfnt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldglcbcz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zljszdtd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcomivfh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3txpslpvx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hzyeleiz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xoeevrvu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwagwdf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jeznnahc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tlhypmel.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3vazyvevt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nbrshmzv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vjtawyem.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kwvjpnzi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cjpnkhbm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3imevjfzs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jdhkjvbg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ecxuujte.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3uapnhaub.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rgveixyw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qekumarj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yvuanshx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qlwesdnz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ozyrqttt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tyadqoom.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kiowtgqe.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jywoefyz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3deptqoqt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xdgofkhx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nahdkmkh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3byqzsifw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jumjetve.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3evkmvgmg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhaeyst.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkepeeyc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mvzgdkgl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tktbetcd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azrdmwhv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fqyxmlho.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qizitgas.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bumetghe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3aevsgeid.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vkthovsh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tayulcmh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cvndrdjx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uighfmve.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xxjfmhmk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3umccqfuy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ufzvocmy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ezsmpzzo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qcugggjt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mcajrqxo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3isvlcvzo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3iorcxfnk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hhnerbwu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kgegobbv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mpexsnnt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zpcdvlnz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hcbciuzw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3zayqdawh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jhdshpwt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3invcjisu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3amudyifu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3oopzahou.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdydiid.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uzbiyxrg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzmyahr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3cnrzgkdr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nzrzatny.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dkaibjxz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rufnfsxr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3cvtuwdka.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wiqtmbce.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3opvkygzq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqakjfka.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qawmrkbe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rbbxrztl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3elcmzxjn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3bdfodyoj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fwgloief.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3avfbekxr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3sevmkeha.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yirzhrtw.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qvgpeaas.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lxyaoymg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3btcyufjy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fpdxcxcj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3agnbktib.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3amezvjeq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rwpfhrfv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3maibkmxr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoqurmbs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3otkiiivx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cgnlihvq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ucottifg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wlxqkiqs.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3klkkicpw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sojyruhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpuyyusz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rgvyugsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sidreoig.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3daifprxd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3goowfrjt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oxfjmeao.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfvsfqxx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qfqywvec.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cwfwdjnc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hiiozuuj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3prflwbyx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rsfmjpeo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jlpjovuj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3auwffhtn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlpskimi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3djugmcnv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hknvmhyk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3onvfgdid.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmugrbtf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gtojmxka.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3iinzryom.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3krupnmpk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ouresndl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3khhnvkdd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rooqcpha.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rapdxqff.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdmjywql.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uyiavjry.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jbzkhlra.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bwhvadto.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hyzvwhqw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ynlootpf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pktiwgtl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbxwnnod.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3emaznnqq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3sgodbyiz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xxchrnbe.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytxmadbt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3megjsekb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kjgxwzgw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3spnbigxz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gqmonbts.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ilomqnom.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3brdbvtig.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3mqfhmzma.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3enflvynh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3iqyiatul.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hhlgktkx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cmdxoxrt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ilmrecyt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zhhmugbb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hkoihmdf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cwfabtky.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wfxflcba.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lrqndweo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3woheczsq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qraawdzx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fwipqyzs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3czrnyygq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ynmrjymq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3findmlix.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qxkmqfbx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwugjjlk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wbxejflo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxeaxum.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3nbycwzya.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kbmpujcc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lpsxoeii.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3znrrbzbh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zjgezilm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoxsfzqr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ziwkgapf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxvebmtb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ktbpmjlo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3itpwclcb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ybwplemo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3odntsezm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rqcsjqao.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3utnkqyoe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xwhckljm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3feipysgl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kwkunlsz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jvchgqmn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ffkydrje.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3yyewtvlb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fjnixele.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3shnuylkq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mmynjurk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lmavvmwt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qltiooyk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kwmwwajy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gakmheye.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pxklpkte.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3panrpgam.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pfwgbprp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fepamihf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3djythtkz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jdajhumx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3esvvkmcz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dnhngevd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cnkwapac.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mbjecfvx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ptrzhhuw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fkhxkcvu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fcrltkjq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dbqbxajy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3irdxjutv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mneifumt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3cbnhczwb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ocziojcy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgtuvhxb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fhpzuasi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lcvjnaak.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3daghazma.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ywlgqilb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vbgjcwfp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxxpikwg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mwivqjhs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3osndkhyx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3phukezwe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fmowfkxt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uapkyfuv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uykndtlt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nvzyaviz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mofuvfut.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpwfqtxv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tcalpezg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pxgrmuck.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3repiujcv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bhcylwer.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3giqictdt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wcssypeq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3hxtusqxq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgujvrqq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rghruynb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fmykcsxk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wbazmdkv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3hiujvcqn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3djshybwj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3haskebed.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tlxqedub.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wwhxiayj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zhrvcxvs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jxusxffx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xutxppki.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bgypbbzd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3wxrhwsrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prxclzwf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3twumslbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtkdoipq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uuoqkmgm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lwippglx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tbrexvyi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qkaexaoo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qpjvifqt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gcutlloy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3abaskden.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3siwcrqgu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3zcafcaer.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3iuhythqi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fmnljhxr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3idprlave.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3brbdyboe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3twkaswsv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zdkdkdml.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3noyvymup.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3helqplvx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rfydaaxf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xwvgnxdr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dhzuvkot.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hgacbvqf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yplwqiob.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dhdrjwji.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tijldokj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pobewawh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jnmbxbgy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3twafxiup.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ffqrckzc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vqnrnfid.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fqipmgmt.html


<!-- 参考信息 -->