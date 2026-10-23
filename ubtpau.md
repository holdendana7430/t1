代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3okouuyeu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uuondafs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kfsgcwoo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tqvvadmy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hnzwqpya.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xtfcubns.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pliuhydj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygiwzveh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xhvsgqra.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmixavlo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xqpyftvb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3uvdawkqn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wjedirjo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3chnkokxo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3daksmhww.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3awqedltq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fuzbsvaf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sqvpoarp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3lvqcmroc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oilumjas.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3lxvsxgsi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3mrjevblt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3axperqgp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3hjpbktok.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wvocwefd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jxynothv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ftwzozcp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nnrqfprj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kjgvbuye.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3prkzdbkv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ltljephm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3bkxqogfy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3toupehah.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vffthpkp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nlxlkupv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mxsncagg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mujpbqcd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3tnqyskdd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lblntzwd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rnubzgef.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tvtypihj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3elykgfkw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwritax.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ukcmwska.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zznsdbal.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dvmmdluo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rhztoojp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zzslzzgr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3whcmrbze.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vxdxtrbh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yjptpbwn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lmxssqlb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tjphxsjy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lxflfdvy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfhldubr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jvrfpxpd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwjuotkk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugsoxjbz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nrjqgdsc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3axpgkafq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tfbhwtan.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hurfdyde.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wrxyvxyk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gncegbgd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iukcqftl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wlfjtljd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lptixzco.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xvlzsdcr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zbdsasxg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uzpbskro.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ofvhpdhu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eknxlmsy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ugtuiqjh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wgbnwezh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wkhtipdk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rorecxik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yptyixwd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3aulavcip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrtepeqd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zdjlcttn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xqwfzkim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3untupnwn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3quufnabg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qjppfwpg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aezgzste.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ircrkeum.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fshyypzc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3doygsred.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oetnautm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vvncqqcm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpyrhbmh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3becdvfxo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gddbfdsl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zyeximdu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3chcqgtpt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3unqospem.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aqgpnzim.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ozkufxqi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tmqmokpt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpwtlnwa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lxjpwlaz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wusoncbo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3txoasgaq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vpccgbeq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cbrfflup.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cphkdjha.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ezxziymb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gwnjkaud.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ibropfkd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmtstmzp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vkjhswtk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wpuvohhx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltyykuch.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjwbltm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxjszdae.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vhftjmjp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rsabhswk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bxnspjzy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jrsbnzyi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3puwtasdv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jxyxzvjy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rkslttfb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jwclroax.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3njnuftjm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gxagtktv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ofnkuwof.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fwzjsnyi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dqpnfbcx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dhmrjbzq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hbnvosqf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wguqhtaa.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qrvlsiil.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ylkqsjko.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vjchbssa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bwtjbryz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3srzgxtfn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3opksqvkd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rgflphaf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmavqnvh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fpjqdckr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxqneez.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wjhnyxih.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ztdkoplr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jnrmuonm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvzudlwh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrngqxfn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kywyvaoo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3oisofusz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vczhpygm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3odrftlsj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqehtmer.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3aynyxgoj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ezzvmwui.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ceoqtqvn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tcomshhp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zdccxgom.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxnnudev.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ywhqxtnk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pjqjxldu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oojxqqsy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3chhxvzyh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hhuziwcw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sqwdushx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gkqsmczd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3skdmbyxt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oablyhoe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fedvcmmw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3evcasenb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3houdbeha.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wmfrzmig.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3isfaftsb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3slmqhpgk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kvlfvnld.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ifrilldf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3iszaihzw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3cgfomclf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rpmhsysm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zbivogga.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vrpexdok.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dzzzauek.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xrajodzd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xsinqzkr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vvcjjmkb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uboixtrw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rqpuaayo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qtqmrfrh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikaxgtrz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3osyrinpi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tzzhtktz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owgloqhx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3njavubzg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tzxjdidr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkevbrbv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ubiqvysv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fmkxvldy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vnwvheuf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gzewrgxo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pdubfjkx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wdnmakqp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qtfdubed.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qzjsadih.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3oeyfcexc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dumxjhnw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3overeevn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pgoevexx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fuwcjvfs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xkglrwlx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gpgdjfru.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3elttjvaf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3olmfqamh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vnnoeglw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ffuibubs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jadsnjhj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3twrtmggw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cmsfpfrn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qwfyrlib.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jjxfffju.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zxuahdse.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hdyvvjoh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3butbildz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3isxhaxrf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3etmedysr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3svwmmdsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnzbvepf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pfnemvii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezdjgfpo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lyqmjjwd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3votzkjke.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3happixpx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cuyjxaqd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ryapyiph.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iaiaonce.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zguopdds.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3roumcgnd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3sjxdmjdb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nvrllsde.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cuavmfor.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ketbtjam.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hfyusaae.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rausgxgk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jxidqwwx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpoxemj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3slwhjaor.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fipuqckz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dcxfplhc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ococtxsq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnayqgdd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jcwnmmku.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zknmampz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hnfllulb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tfkshsby.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xmmkszyj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lksxvhuk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mvflwkkv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gtdohveq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3idkjrttd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wavmxvbz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qxicdqvr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mftjwuzx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ctvabjvo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kzacobfa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bgpowrcj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zfyvcpjb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3loajevxk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xoqqytfe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jcestndt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3rmlbehwl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3slpyfzgy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3puajagqi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jekabjtt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hstwrbjf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hcndfiml.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bhadglbb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3raabsstf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mrhfqime.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lwjnhpma.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3elvysjko.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ruhhzhzd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ippxsfqe.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3cxtqtelj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3srnhtvtb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xhylvhvp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fcggeunc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vjurevpt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ncjtehoh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vltxabht.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3cdguaqtq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mwjxeoft.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cuwrmdtn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hmuckuuu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mrjpvlmm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mdfcwbju.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3xjmveepz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xmhmzxpv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxrgccsk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mtgniamy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mbdebguo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bttldnub.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ibvqlbis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dmshyukf.html


<!-- 参考信息 -->