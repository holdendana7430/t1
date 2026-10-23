代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nqmxfoki.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3laevftfk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3itcmbwof.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3knpbrhle.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ljljbmps.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwkwpdkg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ludanquj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3buiglmnl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3spgxzztr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3amltecyc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3eqwxhvxt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dwxcdelp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3afhomust.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xuxaajmz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zgttavzv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fltmprza.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mshctoll.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wejyjhbi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cufuadbj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3slfjhatt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wreoysng.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfyxnwhl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ggwtvyag.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xcvssdpo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3shomxtoy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3glbszqbo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3topwamjo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3afnndvwg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tpoyupuo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bujqfevm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbbbzrd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ruyfdqnf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ebftqnvz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bazbxdps.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mlblbwgq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sdsnfndx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wwxeyjyf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qsoipcyu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3aocpfyev.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wixdpuna.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3puqhktew.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3odkabgpc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zrdwmlqm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkcydfva.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vpjvevaq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zthdlkkf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dusweefb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qggmgbzo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xnleykwj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nzvvaywb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3lnoivquq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dhpyumlp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnlrgffe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rqprwaaj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iudkyyoz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3absxwnup.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vpvmlvom.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xtcctxzb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3oolhtxeg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3wjlqaflf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3dghjfpqj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tqtfzctk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dwbvpycr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aomdzyrv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gsefcuam.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qxclkgbg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rolcsbdd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gipskyij.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wbqdogui.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3eykiefrf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lsgnfuus.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hzefpxca.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3blchzhhy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3czznuzsm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3efliczgv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ckdwzyhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgdtrxzs.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ommzgept.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqnacixl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wksyplao.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fzhtnfjs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmrouerh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pdivknlc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xwjynjyh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3amznencq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aghbefql.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3etqroneo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruxnddjj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lnvbmnqi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ukfymsnm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3iscdhbbq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dgscafhz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3duchjnmk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hkxprmrr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cbbvpfzp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3quqzhhzl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3btjfcuzn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3esrggyui.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3yglwmfti.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kesqzaas.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3efpakfxf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ffyqnjkg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3pibaeilc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zjfxntxi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3swzsbycn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bvfofzya.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ckrsjaje.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3riwqfnsk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qtcvqkjd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwvzecup.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3mpasjjwu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3oebxyzzw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3amcwglbw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vtqcyxyc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddkifwmx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pwmwlnba.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bpqdxfeo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ywzqoltd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cedynyja.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gjwrfbea.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jtnlpfyn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tdlvdkvf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qwwpidam.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zugqqzew.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3atsfaajb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kvktvgbf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3uszdqfrb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fpbznbax.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3skfwnfnm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rmsqqaom.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fppiqmnb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3agbdgsws.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3llhbdwyz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3cwekwgmc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3holpnfwh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3shxlwoyv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nhkoxdav.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zykehfsz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kczlviot.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xjobtlaa.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hcrimkri.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kouesmlk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3pqojmpxm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wyoadkiu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlydejfu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmtjdkxy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kelbxoec.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fdbkzwjw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3eforntqi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zasmnihz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oqkeefuu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ndpeleus.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqrwlvjo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3egbqlcti.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gprjxeqs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rynvcojm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3eckabyig.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bvwbxzcm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksljcfbk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qfacqufy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dfultkaw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3skzbrvxj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mpqerdfl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hzplmgkt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jbhmjbqj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wkqqypoj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yxemffhd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ltyywwzf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wcmixvia.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tqqpmpnc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bxjhxtta.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3cgnufmqk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wvdtivpf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3exfsenjc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xvhdnuzz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hyrgtrvb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3oohzyddf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ktxhajks.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nhenekpx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qsjjsuek.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dtxnxhfs.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qvdrcaer.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zyewsfmg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wvgdjdmh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zkpqhzjb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ntcwejdh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gkkhzvob.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jqfcmqsr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3evieszqq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hcmyjiax.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mmvpqdvr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuwaydbb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lzvvgxpp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hhezqkyf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3limidfxf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lvtpmaqv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fcypvrop.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qndfnisf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3srwbelyg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3usooymvg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3cxwfrddk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3srdtvjjs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3onkygraz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3idrgphbk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xflmgksk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rusxdcfl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3eqcvwepd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3agjvciix.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nmjxocxu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3unoydvgr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3iasldeqj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yqkzltwf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3llwzfadl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ujfccedf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ugcskniq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ceaiaoae.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fewhtcvw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ffghclmg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zhpznkez.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xopljwph.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pawjcsrq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cvenggqt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pxowealz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czsowfat.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nfidctun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrkefbsg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fldjesmj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mejyxmwn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gppkqkyx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ssxbpoaw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3eprrescx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3aqfmvurc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3znjmopdg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hlfpgbtm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gsrnpqbh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3drygbbab.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3sfegjidd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yiobosnz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ezwlpqvx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qurtalep.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fyavusqi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qrgoeovi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gucynlzj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cwuyjkiu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3osbwxxqy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hmnqpbmy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xzfenomu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3dmfrtzih.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3chsnqcru.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pljnihjf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3crzmbcbu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nwlizeii.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxgqhoab.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hyvewzlk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ilfhxtsn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3stgwpxri.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tdjkujvt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jemludvm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3srfuijze.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3oxcaleua.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bsiixxgm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3sbrzirhx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ngujdund.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ylctuazd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vklwxzkb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3krjqnnhe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jwousbjl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3obcbqvdb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vjisdsky.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kjtocmqu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hsdyvnqm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eesoyzwm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lahnpfyy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pxkmltsh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eyvtolzz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yxljvbnn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kfnjgygh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijowsbqk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ymlyyqqa.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rayqwitx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3llpnrwmr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vnrpysgt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fdqsbbyo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wjxvbklc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vrwmnzos.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ntacptde.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3htsbbzmx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rvvndcrh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sigbgbcc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wntrtccz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3irgvwirn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cwfiupbu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3joxpjvtf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wfyldrcy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dqeszxel.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3arojywiq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hameoxbw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gprvcazo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mnhqwvab.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lypggvnu.html


<!-- 参考信息 -->