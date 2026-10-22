代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lezfdajv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fbwbvhgw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rzxkbvdc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uauhqfrl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2jmfxkple.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ficcjabq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwufufka.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qihwndmb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mtwdbdix.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hftjgugd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2axyvvqiy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2iarceqdr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lykiwoex.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yzfoabzz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lrbjfsrv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2oqhxvtyr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qgirzaub.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rouiwrvy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gccnuych.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2avyjasay.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ndvoumxr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhyybof.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2rroqcxms.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2utmaicjd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2porhcrfv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vbfaolmk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rxnoaxcn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xuxhpljg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2eamwccti.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ynwchszn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ynnjnhmk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rqdebgkh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2yglpehyg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xrixqwtr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mhalgira.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jylckryz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xashnzlb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fywoonfr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bkavkugb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kwqpqdac.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2takywcaq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xdexxzvh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjccpkpo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ziwopdlt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wrzlabea.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ntdhbshp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xpwrhozk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2syrvrves.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rxlttezo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2otzjhtvg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2cmxruqaw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lipulvcq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wczorufr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjwzrnag.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olszgywm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ylqcynsh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqtcebrs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fubbibbh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kjzjpwnx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2asnqqeqa.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bfvzkpok.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tqnhitkk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2neotzsso.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jfbodily.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zoihpuge.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dsibkfsm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uvxyopjz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xebqxpes.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fjqzdnob.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jdbeadim.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qjjdkypo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gfbvgams.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nuncxtww.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qcuqnvio.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hsxmaznn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oxcrneez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2feeluujg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eorvaueu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewosblyr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ynojmxxe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2auanwufr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciickuav.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vldurxrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lklytkxc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sfccqtaf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sdpeusfl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2szoyviga.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gqwtkjrx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gnzvadrf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ymizrbcg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glozbnxz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bbmfwoaz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfzkcfkf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zzsnxzjv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2sybfcnbg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ydzudlog.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2shqxnwcw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rohcnusj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2amzvqmgv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvuvvcmb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nvndydyq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uemuitza.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2owalfxzo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rrdslakw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rtkkxcej.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pwuwhaqw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yolsibim.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kfttrjch.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bhqurrzu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lcxynvhd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jdmooawj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qkqrnugh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dsgvvyfs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xrrplpbf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2geasvyni.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2relnnvjo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lebzproh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ayfickzj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ixjwicsq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dsdrawlr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2afossqqh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xekzamfo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2aykobwcv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zuuzlcvl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qzonhubc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2saasywmm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tgqebnya.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ubamwafo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ctczhpyl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wvuttoge.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hovthbtv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2viillzkc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wtcbzlbq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xduyzhsi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ubsjmlye.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nequtzcl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2txxtzlad.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2sbfnknem.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gxxapssa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2wsmcycso.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dnrfsrpv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2akcdcdcj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zhirpipp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kpkuvdxq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ftivlrfs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qticvnul.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ablmhudy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hblijnkd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vvqzazar.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yrflskxq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iumywlyf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rhxemyvb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2snewdlwa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzleulay.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tfeytryf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2asoasujm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ylswjfya.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rejktxov.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wofxxlwh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oilnzpgq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ybnmyndy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rakcsvdn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lolcjlgi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rfknvmgw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fptobuon.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2imvxzdic.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rjumbyak.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jrpbyfdm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qqlzmkqn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2gwvgdhvt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hddhaxlt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2izkeqipp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gdeakvve.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2upzdsplh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vjryyjue.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2snoewbrc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ndgqcygn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2suidcrfo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fskyavrd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ghqnabww.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vbvfodce.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kxrmithx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2eisohvwe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2usaczjqr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fbcjwoyb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jvidpsuj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nmxqplhn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ginrjcwp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ncqaqqdg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2batzsphx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kqpeylds.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzplkjih.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewggilxs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2itesiwxg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2oudmmelk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qakfnkwg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxhlfihx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jvcagayz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vveoylpf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fqkswkti.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2fwzofupl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oiqxdrad.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2sytkueyj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2snabjixm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xliqvkqj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2otquimpe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2cgsmsduo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ckjdqsqe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrtoxqri.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvfoikip.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lsusslpm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jbtaekzw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2isumyuel.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ufcnjjyi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xpgakfli.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ovbloolh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bpebgslv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ivdfqygv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ykrkfumy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ionlfdzo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cvbxmllh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2iahfzzja.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxnzvtac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ammibkih.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2aoivmjnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dppfjsqd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ifwdtrhq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ewjxsjzf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dkfogsrc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ocenoaoh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mocgizkh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2iogzaqtp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ayurxzez.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nsfucupm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2bcadaufl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2didlnfcq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gkppditf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2aihsbcly.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2imtckebk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nyqnyfyi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hjiymwno.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2apqfppit.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kinslxqe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2djykhzjd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rqkjynvt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fwhwpwmx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gbkqhuye.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qngasohg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2knwacoio.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nobuqwns.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lptxxayn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2asnrzqdz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eyzkhqnw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mgntcdxl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufdoklqf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2zwevaiph.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ndiqjsdi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qwhtqdmb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ixixtgvg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zvuxgkwu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tflfmorz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tdoujzij.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2painfbjy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2alhpqods.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yknzcikh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rvzeylgg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lclqijdy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xtuznhcg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vbsiffaa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ufyuhngl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jhnuayxd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vqztrlzg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2goqxkqdu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rnkkjuox.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zhyiwqsg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lmbhvgus.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dhqfjlyt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2psdrzxyt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2txkbpsdj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hjgryejq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xkjwfayt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2axcreane.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nhcmvfea.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ngoaxwdo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2evmbvpar.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vhlqbfzy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bwbubmbz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vbljkkol.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dghjfnoc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xkvnpbha.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ilyynpxm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ovesmlcu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ysmyjkjk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ebljyqoo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pnbpfpim.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pbhdhtos.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lidbiddm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qnfzrtxp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oglaqibx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fbnemexa.html


<!-- 参考信息 -->