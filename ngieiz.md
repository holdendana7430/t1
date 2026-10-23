代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pbjdgqeb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ssvxyofp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lcgwvurq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cuubxgzn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3bvfpymlb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ugvhgoqm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkisovqm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3waeqzfhd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wlunztuw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3altpsysx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ciaznupc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3otnrrfjm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bbywityb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qxprlgpv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tecwvupe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cascoigf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ovqegfin.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zfoonyxm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3irgxxsse.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vaoqzsnf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mljjjhvi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kdcuzsmq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qbeljpgi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lrfhcpgc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qsfhjfgu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cjinkoep.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xamwymux.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3zaqfruzk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3hperwmct.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ccaveioq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3opkyesxl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3dzmfjzva.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bmtlpuyl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3wswdyuqs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hrvjaztj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fapqsojs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bctiqmpr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3joipsykc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nuoizghb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3sjesovxh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tsxmnjeg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3cgebbwsf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xevridiq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3flmypppq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3onucmums.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ejamngkl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3axqkxrir.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3udsvgigl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nnhbizxa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3iqnlhosb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kmhxiyzz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3sbqbvxvt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ykxziurl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jidqadhj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3myganqvs.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qpyvwpmu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xpntvufv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pgrxxcoj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3llybfywt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jpfdshyf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bnkjjajt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fvhjtvdt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eudcohpm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3haoeuovt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cusgrpbx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kiolbfmk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gozpvfom.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3elfcxqrs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3phlgylsw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfhxwljp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3scvauqwq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cjdocpnk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vcteoruq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ppqknnmi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dqferzas.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gbwxkuvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3annrxcse.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3txzjgqnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgnigojb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pcnokrkw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yrivhcoz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntdfakgp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qmhtizbn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owvxuvbh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tvdvehdg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fctcmmam.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hgskpurt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctbqquvf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3imuqinqt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3sselsldw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fwbwitnw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zqrniayb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhahjgwh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wemzocea.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3feifhqjp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3laoaoytw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uvsluvmw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jhqemifl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3smhoynzq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3daxqzgpm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjlcvosl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rudtztui.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3yhgsrsea.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3itfihfkf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rllxfnmu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xzxbuwna.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3fyzkhdbw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3tmnuxodc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3uyiqmqrb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxcmmezs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3bhclqiaw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bgjlhqgz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kshselds.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3urhktjya.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3drqbnmzs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3icklavoy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yloaxrow.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3rwixmgel.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ghqbfaxl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jchlulue.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3mimxnkek.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jjuibgut.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3idlmgyry.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pyshuiuj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xbltmdyp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cfartxux.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3divbojpr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gqldjeqz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qxfithqr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iocdgkwe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ykldpguv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3njitgpqf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bnkcxvdl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wiptwesi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lprtomxq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rzkjfyew.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3soqgjeul.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnsmbfa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fuxqgwlk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ywstkjbo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yjjhjzao.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ybdsspaq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vfxscldj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3cshjfefa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlumiqkh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnryuqah.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyvitfcx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ksyrpxds.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujdbahxo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3fddpxkfr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vqvxmzaw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3orwzimae.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nbfhllar.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkzxbsbl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fuqeqsxx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mrlepqwq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tligciec.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bqvilajs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tyeqbojx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nkdxhkus.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zerlqdnm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fwyoheyz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vamzryty.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zypqpdih.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3uuwxiuxk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xxtwavaj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wookplka.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cguaamjg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mrjobgmx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lertkhxo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vefhytho.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3codljyxk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uutvvxms.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rgwqtods.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fuuhwryi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3xcqqkfiw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jiphxqrn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3egddicui.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rbqcdmnv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zixlzyns.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wfxolqan.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fstrwhwx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tnvgeees.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jjohqlpo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wxxkmlpz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3foudtoom.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3copqlxbq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tpikfeaf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mhauqdlm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qvqhmuvv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xmbpgcmj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmllsfpe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvfadlbz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zglbndyz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ovfphigz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ltgirbts.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qfbmfrjk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3syvwfedm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jajpetwk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eodiiulm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3cmxjzjrt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cucinxwc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ldbqlgqg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3obwzrfwc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3demqzefb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jpeqpnhj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yrfsomih.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lrmmheyk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3azknunur.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ozljyvch.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qwwkrnbh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pwpvxqmh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rsayllrj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ymgaoect.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3pqjyzrwm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mfjvjxzl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3adovgiwq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wcipmvkk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oxymoohh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mgcroeio.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hgyreikp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rzqnztot.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gmnldrzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnnjjcpj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xdttalic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdycgdjy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dmawgzhx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jdtppptd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bvyzowqo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eazepwza.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qgpkzlkp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jqrzkaid.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3shwmqcgu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rjsekdyr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3cognxbja.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3scrowvef.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jlbjpwto.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3cibnjpyu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xgcmgdpi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ozjudcmr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fledndkb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jwgvknpe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tyejfqfl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wowbglta.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mtlwupno.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbznukf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3sovaxned.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zjdqsuht.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3utpurgma.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zayhcgpk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kgapcztb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nxuehxja.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3viywmtrw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3egkwvsaj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qtxtqkvc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3sbqcutdg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nfqqpyyo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ojpqkseu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fwxnghcu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hjgickbz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zwehbxnc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gcwehwxn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kldsafpn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3syhxxeci.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iujtckva.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zkxaxagi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dujqkkmk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fpugehhf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ywllbpqt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3llsdsmmh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pdqypays.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wmzpzdtd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kczwmase.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hisgvhlw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kvmzzzyp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3buooikim.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3atgcijta.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pxwxxmum.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gywobbrm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rpwpdwwv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jygaashc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3msongwjv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oowujgxa.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mggqnbhv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ravfqiod.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iwrfveiv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hnlksqjo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3grbzwkko.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3icfxhmdx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gwyviwdu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3heydyqvv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ljoyzjvo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3rehfbgjd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3yyxsbgoz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zofyghot.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rszhgfmu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gdrpbmio.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gatfiouc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3goijxszp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nszgirpd.html


<!-- 参考信息 -->