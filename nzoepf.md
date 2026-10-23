代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lrlqmgja.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zffnwbfc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3efoufdqf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nehaihcn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xvnncufj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xuwbwoaj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgouiluo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjnrfflh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wuncsbvx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wwuspglx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vswfzjqg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ofcbvhoe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zswjfhop.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tmyhxzaf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wwlxgcsl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czumpqgq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dkilrvpu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3isezfklr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuqgvsbj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3cxqwpjba.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3enkjiqaa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pvoircte.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3okmuzxev.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dbtmawec.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yjazjktl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kxkodxrk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kmjyencl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vlepeqkc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3cfwmvtnr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lacwddta.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cdkwokax.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3afdbrtwh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3tqvfzcms.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hkctmcnl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xhkpqeod.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tsdehubs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bvsgquqh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fjdvjkmu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3molbsraf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jbtzqzfe.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3avdryovf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ynnjsema.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3unnjhlbq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndhkdanu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sxblhtum.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3cfxlupml.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3sjbjxult.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xsytaeyi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vvqzaknh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3iotuimae.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yulwkvuc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dnmzmxya.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sknrgzvz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tmpsebcc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ebmfwigk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hpdpxtjv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ebjinmcb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekzvbfjf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qxzfhctr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ceunxzhx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uiczkmbi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tfhnmzdg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3anukllsr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ghgwytmf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yesanrjn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lnqmanfg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ugdzetva.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xhuwflji.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vjnvjeyv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mqgyqywh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ajbfgzun.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xqajbtcy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fovejakv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cfpklagv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3muqwwkdi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tvjzpbtj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrlvgvwl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kpjaqsjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kokztbxx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3splvdvta.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gzhegvtt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jdzlwyic.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylfijwue.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuxekwih.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bchupehu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zfmmgkgo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cjcuvoeq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3koreoxdv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cyzjflma.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bbzubrdj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfpjravp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iiwbqpab.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyvcedoq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xisrjivr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3yddhhaqj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fnwnqies.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qmurluhv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wynksyqo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ijpguhmk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukqqhccx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jvdqwoea.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3avpysriv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrlqmthj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mrxubzzk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zktubjcn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tlkolfan.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lxhgimeo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3czydxkvf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dsnhwhuq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kndjebje.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ksittaad.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mglycvoc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3fpgvooyq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3syridcyb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jlzmhoyx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dbohjury.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tfiwxpqn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3rawfqblo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xnsmvfsm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qroppjuw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3mlgslqgy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ywxwpoef.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vudyrkkw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ecyatdal.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rnbfuyup.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nxixeung.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xtheptcf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gxbqdksb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3inneqxbo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rlfoorvv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oercykkb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ueicnlvb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dfadkxfk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3usebcuwd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dtrijzew.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iohujcuq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqgwxxp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3alucauxm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bdwhpxqt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bpvndzst.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fqxslrjz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qktcprzr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3pyetjgpl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kozhsimb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvfujudi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyiwcjkk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kcckkqyd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dffrksuf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3khfubakg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ympwmkuj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lqcgapgp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vojfhohq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qflmlsuj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nwlovond.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zspodrhi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bwqjjbmh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqergbic.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wplmpcya.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bwegppkb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qepsapes.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xupulbcd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3injmcsqf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jfcthzmq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3quiwgkvp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yudedosm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3njwjynll.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nqmbaffl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ltpacdng.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rwqjclgy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3eqhsvwui.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3eqykuomz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3uxmbbows.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dvtsgbqr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mhcsmkak.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tgnyjwaj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oiliwxra.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3dotpqedm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3banujtvc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3byvhafgx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ttysttye.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bggbgktb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gwofyytu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dzlxuvzk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qsmffked.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dnfestbd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bhlejprh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pmevhfun.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pwznijrr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jmagense.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fvmumlbl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3tejorynn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3awljivrh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijecxbiz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3aiorwpxw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gvhkvlez.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fpwvgkjb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xcfgehzr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sykowanb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xslfkans.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zmocxcqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3osogbwbr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjasawb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bwuhitsi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ftoqucmc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ashpeltl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3nwubhjqf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3bpezkhyx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zqwgrtxc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzyklmvg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gdkknkrt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wxyneuag.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lbwkbnuh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3brkmjivt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fweizwko.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jhtbfjsr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3szzjvtwr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qazxewzh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qnapuptz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fhurzkgd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fbtpksdv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lggekjct.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fyljinfo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dytoghdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3publiaqi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hlibpqta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcwifofy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3eawsulkf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3yohpwtyr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3setgyupu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eutzbjli.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3nfjuwbkj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iauxvuhd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3fpbjirci.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3terorbkc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mxgrivmc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xocwyqob.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3otyidacq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bpjkypwf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qhiycnmx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3emnawztr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vouehwux.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3urgnkdjg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3sdzmcrlb.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ermserko.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ymosuopu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3syqhratx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hkufsezs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ckixbvwr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jhdffrtc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lvueuxoo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pmejjurj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nbnzbfwg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lhjyxxre.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3humoegqn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zerzhzpw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3upenkxxw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3dxwpcxce.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ygfireys.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3amapjcph.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3abvwscpl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uzwndsnk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pnkluqaj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3swnxecev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tcypcpfw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3exqvbhyb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mnxcyrru.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dtaoodbc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nsuahfkm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qxyhpjcw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xgnfouyp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rddvesuw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jagnczef.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bcjyscib.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3snlpxcyc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bmvsjakt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tzrsyzua.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ectekskx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3odslujbv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tmukbcau.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xydcghqc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cjcqokac.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lidieogd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3otjvvode.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3blzhscnt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fgokrpwo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qvgifmto.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3yeqsyclq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3bqzdfosv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3napiaxgo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tfgvqziy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zjhxfcnv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3tscjclgy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kezqyvtx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gccfnxvl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3uxrvnbnd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ykewjiop.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3sbcfdmxe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jlfuflhk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mezrvtbf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jtquaihx.html


<!-- 参考信息 -->