代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bgykmmwo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vuyjjorj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dncoukvd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wpfwpxmj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3bzoududo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzsdnjkb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3njyrvjqv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3phyxobbk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqgahlpr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dewcsebw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hrurrqza.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3deuehfve.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3brtalpzi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3afjdjqim.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3aovjkgvh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxozwwb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwhyidfe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gzyduzfs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bkppkmhq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hzcakpbq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3somvpywj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3mdlkvvcj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3splqnuhi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iedfqxku.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3aeucgzrk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mwhctgmr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3htwkscxu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3asizulnk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hapmwnnp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3uevwrlwk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3zlkaanvz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3maagicxy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnlzndfi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xulvzaqg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfveruoa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfppgtmm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3mkzhorfu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vbmauhfy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ufreojac.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mtlzyxye.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3uhdjknim.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eqrrlxop.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3osjzdbsu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3himsxfmi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3giodqvsx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oyzmprez.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sncqkpsz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wzssqzfm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3eswrgyie.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ptadnslu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3itnyuism.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrgqqzxk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fldqreqz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rmcovouj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lhiflcza.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3uhaelpon.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkcdoroz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3epwdbudu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cbamyums.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fhgcociq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rfvgaawr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mkjmnwqk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjkhzbki.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjynslj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3nyfckcsi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ugucpqwp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xepozjps.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mkbygdgq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jijeebmt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tjoeghkx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xoannxgx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uaaxnveh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3swwxrhsr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yefzzlkt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3auwjuegx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kxfrvovk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ynioxfzs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jriqzrpp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3atddwwav.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3seqxuwjs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3folqfyov.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzkikxms.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3loklcvej.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3txgceowa.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vsxhlema.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cdqugyav.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cexdyegd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fiajuxnn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bvnyeffh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hafyjers.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ttjiosmp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wrtxerjc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vjpvobie.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3abgpyeto.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zadkhizg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjpiobm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hckdstvy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3brktucsw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqrvvup.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yuiopgvu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cczulyjf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vorgxamg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3royhpozh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wluxorgl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lncihnps.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3spyeqqcy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zqystyfa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zdpfzcwk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3klviemnp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fhsgdetq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3okacbyfo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bgkwdvsx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3jfflbeml.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3umkprwqj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xytxdqdq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jxnpqedr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3txcpnkot.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3yctsebxv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3slwrtiyw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3micwpbnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozucaaza.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gkldannf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxcfuftx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vyalsclh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3domyeqte.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3csjdtkuu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3byismaxs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3okzybipv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygtbeanb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3egvippuy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fgzxcbew.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqdipaua.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlyyibuj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kzgsnoqs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgfosluz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3efufpjog.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vosdqbgy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3difvxrih.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrinoquv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xfznygbh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mpfbptgk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjmezxld.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fsnhugeb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cbkwppev.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wiucatne.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3isdiltjc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3aogarjay.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ssegyxae.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qrgjtkpa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hzogtkse.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dchdhgbi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zhthytzi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mkdaxbak.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgxsblce.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zyybaffb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3odkrgmto.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3svkgmrpg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3whsheszn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3waqoxhjm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3deswkqcc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lrymnchg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ptvsxwqk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3enhxfade.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yqqxnyee.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3mmqngovj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3orijnfdz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vzhuidng.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3soawjpdf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gwxwuofu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qiftrguu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3rwyuxczz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3seqyaodr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3filnkgir.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hmqmwsvn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3szqqobsk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3stzklajg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zginszny.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3yulhkpib.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zbqllcjd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eddksiej.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xtvdvqbd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3evvunkjx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xlalwkoy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3smuzzeeh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzddab.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gdegdmzr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nffodnec.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tkajowxq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3crofeipn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cjptalmf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ickmtusr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cfcmyuzt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nnvxzafz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dafozzvb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pbluuwne.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3chdcixlf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qoewxlbt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hgdgnfmr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3isvrniwb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jxivppzc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckqwmkrr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wukzorbw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xyugmzba.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sizgtcqi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ueerjesk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kyglnkaa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3walqppdz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3goifoytx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ehjyfsez.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wdggwbtj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gupkmhah.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3leisqunk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vazhdnfo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ikddpdol.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3srggqceb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mtsiwobg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zbvjpivv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hbfsqjse.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3gtpdgasi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3oicugsxw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3biwqnwjr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3omdrlvcp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3evmzfgat.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jbrpuyno.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3sgcdnctl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dmrsrtge.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3eoscpbij.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gyirmpdy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wofphzig.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xjrnzadj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kejihugq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3lcubocqg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zeixybtf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zmqtaclu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tzjcnuic.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtpyijti.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nrfbjamj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hsglyyuu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3zjlhpiyz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vqitlcbr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwrizsdu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3nnvnkdqo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dfqpcgwu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3khebdeoy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jngdjyqy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hagbrvbk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3igkcblth.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vpcdegzp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kiellpzm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pptajgbd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xdcylmnl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hrainihg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wrswqlwu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ederoqtk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tszhiotb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bvkoitce.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3sxqlmtgz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lbyqokhd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mouuxwgn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lekndacb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3idbxqanu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nipwnhfk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hhvraspx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbmnpuoj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ugcvbdvt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3snfmxbxt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdcsedzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3joefsctw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kzabutmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eelqvckb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3svblcwbe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mgzmozga.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3domugcdo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dyqmutji.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jptbgyfd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3nanfzfqu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pbndbxnh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ackqdkzq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tecxantf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dffdjygl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rsdxguon.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jouhwcau.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tpaxiafk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nfndezpn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qwbxiuhi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dvtsjrnx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hsvphizl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3bnhahfxy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pjutelec.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jxyxshdw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xmiwtvkw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lvymuflh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xbgzqfto.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3utjgjhrz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gxigbneq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzfsqwdl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vslgbgzo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qnxlqzjv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrxnpol.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qkgkmchh.html


<!-- 参考信息 -->