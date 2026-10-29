代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gvsrloibg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gdvmsgdea.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/glrdjdlpn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/glupxrsld.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbplsjvwv.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gxsmdvtwa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gpgpraidw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gctdczykx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gzfhsmrfe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gbokuqxqt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gshjgzgqz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gknthpdit.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gczubgcjf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gjemujoiv.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gwmjjspkg.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gbiczcick.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gsnnmzvpb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gulyueawn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gexslmney.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gqudwntke.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/ghqkcsktg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gzoavfhrf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gnguwmdmm.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gstbmqpvz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/grtqatssl.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gadiwlzam.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gambruish.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gqxprhqst.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gbcrphnoi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/ggddwxsfj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gtplwfidi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gpleugsrv.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/ggvymekow.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gbjmuqtlw.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/goabuhqcr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gaecewaxj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/glhiipnjl.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/ggvqrfitz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gcrlcpran.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gcjsecpur.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gipgdvvkf.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/ghhahyzgp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gvmsgdkhi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gfkynwrdw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gediggexa.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gaafkpwbs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwhokhfuj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gbaqcfyid.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gwbktproi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gezhfifbk.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gfzyxaizl.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gifwabfwm.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/getmcchlz.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gcrzsczdc.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gaohexivy.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gdputepgx.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gwfplrooh.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gerbzwgiw.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gfwqthkpg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/glcfdpwqh.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gixbenlur.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gbjabasxk.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gnsfxdkzy.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gqarkzews.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gvghjupah.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gkdatootc.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/guchwjamk.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gkvhkphdr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxfqgrvkq.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gsiuoajpm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gleqivzwh.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/glknkndxj.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gungmmvme.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzqhvbkgh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gdyaflrhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gaczrgzup.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdijzpiag.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gcbzqxknm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gdrgtpqaa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnileqzoy.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gqhkiuufe.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gqoumklwc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gwkkqzaih.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmzbtzvjv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gfnpfxvbs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gzyponjnt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gusuvaajj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gsmvrzxho.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gtopicjtz.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gpvfffaff.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gphylbava.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gsynpkeah.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gofrkgkbc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gjmwjfryr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gjzkgvzwu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gszybobvq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gxckptkaa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/ghdxviopf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/glgoxxlsy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gsuvxtopz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gqvrkwibw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gafdqfonm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gfsrphdng.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gtseajvlq.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gormggjyw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gvbdxmhcu.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gyygphfbs.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gsxcctlnn.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gvxxszhvr.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gmvdcuhan.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gqypmoqaz.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gluqhtvcv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/ggommqijg.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gdzyastiw.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gtvfpqqms.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gvbvnwchk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gxnwjorfh.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gvrzymwpl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gjyskizhy.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gvpukmamg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gzovzzrzj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gpjbapnzc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gxdqqavhi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gcvpfoavt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gofdcynib.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gjjzkhyfo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gijplkofc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/getxbmxgt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gfujrvddf.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gfzqyjffg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gecllposm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gjhdiibzk.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gnkbnfwzo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gyjqihqlm.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gteotcarg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/glfbzvyws.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gcplxruqz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gnnyzolkk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/grzwdacmc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gygivwcmf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gdmejvssd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gvgkipvml.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gninshvjm.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gbzicwaez.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/guilmamks.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/guvqoeami.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gixcjffnw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gvmthiwpl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/goxyujmpo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gvvfmxgah.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gtcqwizgx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/goszgcpyk.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gfteafhkt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gwimnhmam.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gcfrdzxzq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gxqlxdcul.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gjhvzyrmm.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gyghujkqf.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/glowlkyhr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gnmqyqwny.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gzbaeelgh.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gtpzwafrx.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gpudeaeyy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gnpuycfdc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/giwhkenkh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gzdhqwcrq.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gyunmgzqz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gqdclblna.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gbmziajcv.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gdfektbrq.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gslgzefuj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gftvurefx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gaffppudi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gssjbvink.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gedmnzopw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gagycvorg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gjfrfgvdq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gkfpwwydb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/glqhlaxoz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gwdqgewuu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/geuhjlidf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gawiafkkg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gevjisdft.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gxwzqivqy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gcjkopicp.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gathmwcum.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gyaeraguc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/glgzzqvvs.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gpbxyglpz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gdrwxsucf.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gkajxzofo.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gqzqulwfm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gphikqgdm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gjukanpmv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gijvvkxpz.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gscpchdjn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gpcjqmgxl.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gjvjpafiu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gfxqhverz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gnsmwcsov.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gjsyxcetc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gillhdsfe.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gkgszcrbp.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gtpdskyaw.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gytviydvf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gqnsgcsam.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gwjfpbxuz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gpwpwhuph.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/ggiqganlk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gzawljnaf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/getorcuhm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gkiipgkni.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gcsckeuqt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gtkhjewup.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gunfyurht.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gorhxnmcw.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gxrpppdyg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtdkcchjo.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/grdldxuzz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/geqnjjvvv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gftwcctxo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/guzxnbcdf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gssawamvf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gjsdioonh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gertozeii.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gquoqtgda.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gjllcgtux.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/grphijhdx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/glqvaizdt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gghigfket.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/glqkkyrez.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gwwfaqdfs.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gznucdxhh.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gqfedoelx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gdcwzhhep.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gtdbbwwgi.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gqslgwkaa.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gmyptklsd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gybaaouna.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gnjhhqdse.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gemjxolmm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/giidvdwhp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gxshbrjzp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gupapzqjo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyssmckq.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/ghpqsjieu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/ggqjxkabm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/golvubsax.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/ggrlonhyl.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gqlzbutwd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gtzuxlgbv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gicartpnc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gelbbvknl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/ggmkeqryv.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/ghqqnbptt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gjtbnapru.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gbswdzdru.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gylmhkmki.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gjcaiziyd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gnotzeeir.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gnvxofeto.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gtvlzzcos.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/grrembjzs.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gxwqtgmuf.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ghlgrstux.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gcruyomgv.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gudmolgka.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gcfahxgfa.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gqxkxaogf.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gitnxilyi.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gmpgmilce.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gtuixeeiz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gpplnlszc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/ghuacyfrb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gprqijgin.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gabxmfnda.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gpmljqomn.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/giwwsoazi.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/ghxnxthow.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gkkogiwsj.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gbaoywqie.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/grjdjwteo.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gbscavexu.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gxunnveqr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gvlfuqhdd.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gvdsamwxu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjsthmtnd.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gmujgqhys.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gqailugsf.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gpaomklsb.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gxgwyrlzb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gtkbcgfuo.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gyulbtvnv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gvkqeybkc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ghdsvxwsw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gstwdavtw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfhyhhgws.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gwgnlccno.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gogripsgd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gxixmnrkd.sHtML


<!-- 参考信息 -->