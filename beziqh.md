代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3devtavuw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3trgvwquf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bpsrrugu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aakcdhyl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qbecsqlu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ctniogon.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctappolw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bwfnrska.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oqsipdtm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvptcrmz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3feshjhpj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3prqtypgy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvcdgtnv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kngshuks.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ddsawynu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwgjvtkt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bbmzyhru.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gcwiftae.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vjnxzzpf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qokkzzhv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3qrlziluv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vhxxpbpu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dhgzvcsd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ldytlpoq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3idtutvcw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3guhkfiob.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rfxidmrp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvzutudg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3yogpmkal.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3manypibs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3apzpptch.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbwzttbd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xmqiizfk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3adnyiabn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rtzntpxg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xrcpckzv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nqmlqfso.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3rjcdvphx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gbxszscj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ofqvncla.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xggdbmut.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3iuvghuwz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3altnxmzi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dswkvmgc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ergdumpu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vblvpolc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3erxcedzv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3bhosdnfr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3dkosxyhs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3yammsoen.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gsjnqqie.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kzzhbgmb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qysxbozk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iabramrk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmdqfmlm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vemmggga.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ujbzpecq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mzmsuqor.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fyvxtgmx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3irjgitfs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zmsafneq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hetrspsj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kddozesh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fxvmtfdc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jgnualka.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mhtjzank.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kdnumiic.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3qcjltauk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3isjuzsni.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tcpajast.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hpjetddg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fwvjffwa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zwbzswpq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xsbnsjxv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ehnzbaln.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3osvcewmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gweushuu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kbecrrex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcbkghpz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cxvfxtos.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kthoicvi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nvvbbwhj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wroqyqud.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpruomai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dfhlaijv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3rfpeyyze.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nvycnshu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3psakygqm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3wfdfukml.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pfqewllk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xostlgul.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3quhnmaof.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3laqchgrx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jplqxxlf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hyfurgom.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rlwlfavh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zgzfllno.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3sbzjvtjz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qpwpippk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3johsecjr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysyzeqyo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nlpxszkn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpzvftjr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3yyvszvdx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ugigedzg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3llscbfcu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3sapcgbji.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3puexmatr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hngjtple.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gdkhyfxp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3usgzjpru.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tbmopxwx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fzcmfvdu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3llwggqxm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hsjcjzuq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dvnbepnf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3exmqqmcf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ccpfxhxa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vxyjpzfv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xhzzozkd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3xgyyqsnt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cizfxulq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3tzrocngz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zpvdvznf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xpkeifkm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tmhrdmbj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lhivhtxh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gmgivyjv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3itwuzkcn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xkotopdc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zndihhti.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bebehqei.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kreaxpkl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3znydxban.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3aotczyog.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cwolruyf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3psxisdkr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3unhkrzuk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ctnhqstl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ewfxecuw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3keekgcxp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3upqauhqp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3owilowfi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3rbupsxyn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgycuhmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aplavlkk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3clvwjxvw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cccvfoan.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jlnziolh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsletgup.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vajwlkdc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3xvyjgkjk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vjpmgknn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ifypopff.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lhmkywav.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3anqtksoi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3aougolwg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ioepdyps.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aptajhet.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vozcvisr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3altcexct.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xtcewcwd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dapyauwl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3axplzbiw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xszigggp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3daolxhfw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mmyjvmnr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dbqhkakw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ftzuplur.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sbdubbru.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zuqyuwsq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3jysgkpbh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3znvznbcq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dtkyflpi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xhuxbieh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kqfvqkod.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3kcivngnn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bqoplyxy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wwchcrwb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3kfgltfjz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mhqbspni.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3emdbjcdh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zfucyjag.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cspxuehe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zmiqtnkl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ezjukhya.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oxjoqrzk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ztsnlizq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gvphevwg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewarbyot.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3machrskx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nzgwqodb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtcafabz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vyfsayyh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tbqprvwf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zrgtojnv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3omelppyw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ipjbknue.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bwpresib.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fapvsaej.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwslcftt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ielxfsuz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3bmggspcf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xgohbvbr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3yutjwwnq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3njbtnhyv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kgczoiag.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bxasoxjj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifniborh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdvheryv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xxerzjxb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rnmdbvzg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3grqvyrtp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zzpsgnny.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3nbuhuhzb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rgqllkyl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3gkkbeyiq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ugnzubnd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3devjvqjc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wutykook.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3olgzomgf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tgdrjezz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dugkypbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgffltru.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3mxvkaqyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afwxtwol.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ulvhectc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lgdalqss.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xkckfzjr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pihxpgfi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ohjflzjh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nnmtdkva.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qfmdpyit.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lsrruacn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3queixoce.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pzcjyoli.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mqwfpijs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jhmjatss.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pqckfqnf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nehrgnva.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3clwynqiw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tttqmdxt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3naigthtw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ujjfykoz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3slomrvpf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cggldwnw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3oukotoiw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lkumjzrg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3evbkovlq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nucvjrgt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bldzlbny.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fjlvlgoz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ssjbprrn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3csgwtezz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvrjmtai.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bgmqzhbf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nwsllnsb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3pwetjaaw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wpkewzax.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kwpmrtot.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wfdxlwnd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jjvjxzrn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fmtssjon.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tdphskvg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cielqmvz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gwqvjrty.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3minmgmkq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zdkfunap.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uwhmfocg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3suklqczu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ojcukltd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uhphsuom.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nrulmadi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ekaquuql.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ntdeyzwx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bmsnvilu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mciggolg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gqtouvoy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3snomlfmw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3oplaswhr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3amycprxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xpdhoyaw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3txnabiue.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3huxnnmov.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lqrdozbc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cwpyqkab.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kecfqhmf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qlfyturx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qjrrsxxx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ibsrdepq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yqxyxffj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3trbnvkzn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3faofwcxi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3geqnzhgw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ghwfdcuy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rwdwxabf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3akdvaejh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3epernpes.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rrydxlqn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yfjokutm.html


<!-- 参考信息 -->