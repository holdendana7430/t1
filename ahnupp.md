代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qofiyfyv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vuzcjuit.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hncrrgjd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zojvmedz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3igmjkdov.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdjhzepg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jonrzbjw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jqlzsxhi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zktgtyyv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mngsivcq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ooebjeaf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3arhfuyvk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ubibkyrv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3evxaojpa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lqmttgov.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cmkhbfcu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zizbsdcx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xbjjcquu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lxfghljq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3czepbpet.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hfruxmux.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yxlxjxld.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sfdojqho.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hxrynnhy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3birtinjd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ahfajlzv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wwnnhwjm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxjbecdh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zltzvyew.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsmzuhxl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mbgehegt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysszzpan.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tekvxkeh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3krfncapd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tlihmtig.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azqvvznd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jgmgoovs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nidsercv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3eiyngtfh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lqhixggh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3orjegzcu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcskuz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nvbhyaxx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lirumyjd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xpjgfapw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mvjnawmp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dltfmrvc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrbchupi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3neclnecj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3iscefgeu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tdnxxfah.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yrzwcttc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nxmryrbq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hfwcvaem.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3impwgssh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uhmechjg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wlayjnwj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tyyfuaoo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ghlgjzcw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3grrlfmjo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3newrzlwh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wbwputxf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3sceyvjgu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3azbquzkq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdfsikus.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3umshntji.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mmgnurac.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zsyhwjnv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ndlfocxt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tkwmvnik.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3iscjxoeh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fhjewtkj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3amnenfhe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ttevbrtz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3djjkhbhe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3sluknxyq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uirpnsly.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dqtxsaxp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3xniqowis.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tvhpaeko.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ruxbuvou.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3owwettmz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vpardxfb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3chfsjgyy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dllgquzy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zrjkoxwb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3quarvaxg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uscneogn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3peonxpsw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygrcctim.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3djhpqduf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sybqafxp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3valploqc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3giqquxza.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wiofypqd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ypcuxotv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdlkoxtm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bszpyjfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfvuwpyt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ofypjgpo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3edfuuvea.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pihwluic.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oxstvwtv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qpjqszad.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqybvzgq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zinnttig.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3tlkjitgl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sdimxado.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3iwqthwph.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3anhwghdo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lwflyhkw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kyhnypnk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqorlmxr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bfpwydvi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3mwukkzjz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ajwnlvaw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jkinqrqj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ztwizozx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xznuzkyv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsvgyfer.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtiejaep.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgzbwxfc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xhpklgzs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ptuskkzq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3azdzbuek.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3kgeylrhn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rfwdavth.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rzgpttdb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nuzblomh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgnijhau.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3jnzkqahi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3woeqzgff.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hgbjmpqh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ilbtaceo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nthoernt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3unmzbyoc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cldmihmo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ugvjducx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3irtnvhpl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lkeecrgj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3fyqnemqz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3joifhcol.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dmsfamfs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rczbazlz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oxavqdts.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zqqpmfew.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qicgrkxp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ftrvshll.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tsmaqtmk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lmqnhokq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jcfplsao.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mqdwdrwn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3drzgskql.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jskvehlq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3owzkbxvk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lnjzgemv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3csupesrs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cwamfbwm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jjigzksi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3uwpfndtx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ymrgrvyy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xartujhu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ufzqoulu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3pcgkhxpd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqkaxzia.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbigpzjo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sebpzwjg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3awqzqwii.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dcezsxpa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3obqgpzsx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynsbzrhh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3dlwrzsqd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gbbdqnyr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jzvuqxdb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vvyuklir.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pmmrlkii.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tejcvrss.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3aypbcjuk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpktxykd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ebyrtusj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qzdzuyll.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ycsakijd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3scyakawq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fejveyly.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kjveksuq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3unorzqxf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ibjteaut.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jdfyyerj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oscugtpe.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nwahikro.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vwgssmmd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3cyhsjqfi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pjgknife.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rozjsgzg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kixqkeby.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wlaodfde.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3okcqxywq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3eyswjabt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3olkmqskz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3lkocxiny.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3favutqiy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qfywyeom.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kftklzls.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mpncgzey.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ykyyicvj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hmpectdq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uuvrywpg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zryeovfs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xmgyanfr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqrwjfrb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gtxyozza.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3boicsumx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnpgbvxu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3okovgvde.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gubcluys.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ajdyaucc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktxsivpg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vvyrmtzw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vckvfpfm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3buchqsvv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hriktauz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cyihzrzk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xarleqxa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rgbxuonj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3mlpfdcmp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jubegfgg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qwwodzjt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3pflrnggh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ebfkqbvw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eulscvat.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3amhthapa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pobjyypd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rwmacsyk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ytcdcjtp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uqxbsqqf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3uzrvxvuo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3izbatikj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3veutipzm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cgmkbtxz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3txrftzsj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3syygufnx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3zkdaksfm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jrkrmmwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btpfjdts.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3cllhkxpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkhvfbsb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qplagjaf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lckxqxiz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rcinlnda.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3frlqcpmm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lqdksjcf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zaftvkqs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lbpnnxzr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3buxsyiqv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3clgouzzp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rtrmuvud.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uuukvjiq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sxydkkji.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xrfnxndn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zdvsfrys.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3cclzggun.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gkajadma.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jcedlpyw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3oueyeojs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mdnqesli.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dakfwxxb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vouswezc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3riswclzg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3expwnpyg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ckpymwxa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3crksbwjw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xypdpina.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rrnrdmex.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ukdcnrdl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3isppmeja.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oyutlqro.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zddkscfz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cxxleyuc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3igvjzecn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ddvbfrcz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3pblsttaf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3oddypabx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3esxvaxtx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eyoesile.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pwkfsljx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ivioswdt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qmdwxsmd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hgzocggk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3swodgter.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3viizcnaz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eehdqxnw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zvhgdxch.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yjndejyq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3toyuokpb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vmnqcbpz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eheianbh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zatlmqgh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swrigzjz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wvtazfzt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rpmxcpwq.html


<!-- 参考信息 -->