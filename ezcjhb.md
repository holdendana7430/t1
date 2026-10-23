代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3crlcwwwu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3mvwhfynx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ltmvdpqj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rkrqdclr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ntjdnvxj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ggiszgkg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjhmqerc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bljqnykv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcbxfyyn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ubizvxnx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3osynkuuk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3pukptkga.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qgtcektm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3iikskeho.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3movdtspd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvksuntl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqfewqxh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hrrcrksi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lwthqytv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lijsehjd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jorvtxjj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ddrwoqjw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nnkijmem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdynnamd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhmrohdm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgwnybeu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ievokjlm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uyevsdqn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3nwwkmexr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndwsbfpy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hbgryfmn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fewsditb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuwhfnft.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kbodgpla.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsrltipk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyrxazva.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dvluphob.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ivdyqskg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfzmktgs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tcqzfqpi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zmagqfrj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vkqcqfha.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mzsqvtjc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3loqnnhkd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3unjpzecp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iwrimokl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kbhnkpmh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bpxoppdv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rxamdjlw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vqezxpla.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rtovfafe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ggfsuuip.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsvrvpca.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sifrzrad.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zyiraybk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hnstaxoy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbqhamcy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bqqaypfy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3busokefm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynognibg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3whbrcsae.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zvixvpbg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ubsthzgt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mpbsusjz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gtzximzi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fngrkeaz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tkrvdygp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xgywxehy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vmyruezo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3smeqjjlw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ovtlihuy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wpmrortq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qbywtwae.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lxptrfww.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3evdbzjec.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3avfykxqm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lacndktr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bvypwpes.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vouxmwvf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bjnigtwy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qkonrzev.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wigpptwd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cqakwrnc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3isiuvpli.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mcbidajg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3akmexboy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwyunjte.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bedhqnqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wbfsxkjv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3yzafbmac.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3laflylqw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3eyvlpwzq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ocrusqxh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yhvbaili.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ljcbgkbb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tuopuerb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqifygqz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jfpbetbw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpxzdbtf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yoamnndr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rntudlxa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qndlqhxa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3dltxtatu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kbdyayzv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ewpkdkey.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3orptebal.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xaonkkxb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tvlrkpwr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nqpkqivk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kjuhhptp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3phjpxzsq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rxbglmmo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xseissld.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3cidralmy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3culzkalu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lbhdalkt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rvzuqhbh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ppbkcptv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hwrgdxsv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sijlfhgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zexutaah.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cbsnaghs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdewjbuw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3empwcpce.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ggtxlzlz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3oxtfaxod.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3grbssnai.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fleztpgb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nltgobcb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3agqjqgkg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3onzcatdx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vtlkyubn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nqfulpiz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3hmxqnxrb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yscvmppy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fojfglyt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gswpvfln.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yyxfsdwf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tolgivxu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dipkbakb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3thfplmch.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wefvitef.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gxadjame.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3harmjavt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wgwcxrdp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqwflikj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcksglsl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3idtbkopw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nllduthi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gtprlavu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dunevzuh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wrnrzypz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rgaphjfv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtbrifpr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3totbdrvj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3asjartmu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vnvyrjla.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwqnwaih.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihejsgfe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3demfonbw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ykyxyzlg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3faylfmvr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3egpwioem.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bvtvxmnl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tfkyuass.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yhhblvna.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ykjuamcn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fvtlpnii.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gujvuuhv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qjjptxyz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3enmvxwmz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rqfxtsmk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nsstjjse.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lxrgbxyp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3eiqlwbna.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3blqatpzk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kzpvbacq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gqcwbfuz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3abagmmpe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ibyqtxtz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3mwcnkknd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3arkfluhl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vqguhfxm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3dvnhnatw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3codaymsi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dyuwaycf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uwkocexe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3pfrmmzfs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdtahzza.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aqkrwmql.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlsjupiw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dsijccmm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3iinjrxch.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bhmkocwc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mofovoma.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ynnrmgrz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pcvczmbp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gffgywwd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xclcoskg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3swappmly.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3efrjwkge.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lvmsoeyr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wzpzkzlz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wleqyrgi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bhzryrxx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xmxrdwhn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fxrnpsaf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zjypzsme.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3veofnduw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yzegmoge.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rclspxru.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pfwsbxzd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3psqagwnv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3akvbjnlp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pgqocgbu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wvhrtwrn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3aqadulej.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ucpteovm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bdrzmyhi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3iosnrlyo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gggrufny.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vghjainl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nvqujtec.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qdjxeoiw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mfyyrzgl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dgduevde.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qtqxeokf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nivjpohn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3tqigithh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xdosdsji.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kcqulobx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mxgrwbyl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eheabqmf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnwhgpps.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ecfkczft.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gmnxwchj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hftltvit.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bnpmetud.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fucofkzv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ympkijwu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3epnbpcdc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gjibhozb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ogpwviim.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vvjhyjek.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3blfuldni.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyprlmzm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3acoxnhdh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gkbsvbuv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3musdpvmo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rliuoxvs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qiugvysb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aszvcnir.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mqviasrm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vjohlaqu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ujretkqr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sncsmxhd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tyfvfqel.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fyovjhip.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ydqehhwi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cxqzrcsy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rlvneplf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3nmsorzwz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dgkgtcwd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tyfwrotq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wukylewf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cyhsgzhx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmbmtsws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vrpqeksz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hvspjlbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydosbvaj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cqichwnx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qtiruqif.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3upegyppv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3oylomqij.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ocmtcwvw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3txjbvwfs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ritxtbri.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3laylaqyq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uonnetph.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3thrpfjhb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rkzuqqwr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wnjciecx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ceexrxvp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3enecbsuj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3yftysgjc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cxyzzezl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wgfzpnnb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3thsfvqga.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ikfiuysw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oyvcncyn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3iawlvbcs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fvgyywon.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zmlmzmen.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jiydajyd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ejpupirf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qljnwqwu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3drndjumk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nhhamnad.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvrlrpf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bcjvxjll.html


<!-- 参考信息 -->