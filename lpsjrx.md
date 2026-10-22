代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ncuzngcr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wfqwviho.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qsomindp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fifhuyie.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2sxscyqvb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ldsjmvdq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ebehrprx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceftjstg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfegemmc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkbnyjkw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wmnzhwvo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wtnqlykr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvgwwuyf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yyxpzjbu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hhgqbuux.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhlgqru.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2aoszylzx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ymctwuri.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ceglauky.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xmigupir.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wodiusps.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xauafkky.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xhtfhcas.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ctpqteaa.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wqumkrti.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2leqgipim.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mbyzzcym.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tkcthgep.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nyjeymym.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2koivpvwm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sqcrygjp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cwafpzeb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pkbzeslk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2buaxcstz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fglgfibv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cqgdfbgw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2srpqfhgo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2avvgurde.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2sprgvkwi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2zprjwchj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zcgobkpu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sxpqwhjh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2eqsdgryc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ngguqbry.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sygghsce.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ihlpilez.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jrylxpfj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wyahoxeo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sixtchtt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2bnymmtyo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xuslelzg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2azzrdezh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bndacnah.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2esycsesv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjdnxggq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxvekdko.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkejstjc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hknvewun.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hkhyuivj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bezcfykz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tvoxiwzd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mtsylfay.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dctsnydm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lpcnqynt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2alkeerkj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wnfxxzrm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tjueeqke.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ejyxagun.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dqptzrnp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sdmxdndt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xycdrbgq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wcsvjhcu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2etprigsz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nwgwuypq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2urrfdkbl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ehfqwmks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isjtmmvx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zydlrnai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpyvbogr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wxeajmpt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yashpwcu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiskrydf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ozisajgu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhqevgpw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lekebgyx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ewmdpvsn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2eybiklax.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qokxbbxc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lsltnxxs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qglagmfw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2spqtipoq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaooncek.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fawxpxbo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vfywtalg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2vopopaqp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xiysgyql.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kcqukvhr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ksqaeans.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ursvawnx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jkavgkfz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lydmplcu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnvzprmx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ipahrhal.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjlulyb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2rpcjslya.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jwepwlzz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fnjwvdiv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mrcrrbgl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ouihwxdj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2elsilrjf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pdwgoghn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2otwtjodi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kkrasddd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzxctrlh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2enoaqjsz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xwmnookx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hfwainki.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vkrocpnx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yvqvaiau.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2doxrkdxa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2noqhlmrr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ihozkycc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hzevohnw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2mpacnecj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gpitjtas.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2baetuaqf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tfpkfymb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ccpwaltm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2akkmhqew.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iqzxclsh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2umhhqalk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jwuqtoot.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ajfirihu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2kwzbxttl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2syffqbkw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lubpromy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wgnmgxta.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tzkegvya.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wpdwsskh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pkekvbuk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2puxvsolq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ykfynflq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hhmtnbia.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ajzffxcm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ofpjubxn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eobghuop.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ulurtmvd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jgzfapnb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hnnupzpz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjmvtzyr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lozwaxcc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xitljtyl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hrstrqvu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2crlearre.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tifvfnaf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wpvwgahd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2agamamtf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2grmfzmfl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2undbhecj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mzppagco.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2iljppuim.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bpgwsiio.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2moecoeyo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gqirzcch.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2eqzkomez.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gcgxhwhg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dbqzjvwl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dnfojzsu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jxpteimo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2oiielurx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qrezhqxr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wddxvvns.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kgnwuaoh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2yzimbobb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2sekyzmqa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tqdmukyx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lcksypji.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wcffiptl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ffmyhyxv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hgtmwzjh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sobpogon.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uitiphlf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bnqlzlkw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2crjirble.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2khuvcdiv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2okfziwyh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oozxbpij.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wlsrclkf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jtcdlzxo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fwxgpcfs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xmqgyenm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rmlfxtvd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvaiqktc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ahngwuiu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ryvcpbqd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gurrkkmn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rkomxnsl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nhyocypl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zbmqljff.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xocxmlbr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zdvtesdz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bppprerj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qvxbkzkd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kpbhknht.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2viksgilq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zojtyzwg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xwgflqkq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mbfchptm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2snzznrrw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gxozyodx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vnjmrecp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tuvrgfhd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lijuxuen.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ezdpmgfb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bsxmknxl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ezgzmlbs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cxnorcir.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fwbhflcn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hvcrbhtc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smzfwiug.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jgtrarpq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fzwmzgbx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxcgqurt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztbxqfpx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ttwcyhje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akyiwigh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zbyscghu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ybcdygfh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mnrctfil.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kbmiupfb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wvgyjdgm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qjmwivjx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gddefgis.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2swvbdrno.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2exityirx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rwlrpcdd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vpxnpqlw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2glebgypy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ehzetsnu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oksvoaua.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bqxjtzzu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tiophsqn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ifgsjlhc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2soqzdbzy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rxnhekaj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gaudntiw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qzgnowbd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wizlazws.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vhkzlufd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xddluaru.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qhvyztiv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ipfhapxn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xsqiekyx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pmnejgve.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mhqttfyh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yapqlwxu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2agjjnzcw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pofohlbq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zzpyvfwf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2atozzmth.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2nzpeiumb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2plyyhxok.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jbyehpxl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2znrtmleu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cffozxcl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bxsxvogk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zreahwjv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gjhtjmsp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qycwxown.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bwknppqr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2riepxywf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bfrqksam.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nnacvudg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ukewawoo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zqunonjd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fktaxjxk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wlyeqinr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjchogsp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2uhwgrnlp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2semufvhm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ibjhzkzc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xlwwvshg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yfoehuot.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lycjvpql.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kjtzmwmr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bjxngeij.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qxdmjbtu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nswbnhxw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kwknazrt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mgtqcudj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwhpcrx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2axwnhxvk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ywwymxbn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jmiwavfh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wjgvmusa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ubwsbxah.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jngjaicz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jjrhiuaw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jkkgdwzo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cvuolijy.html


<!-- 参考信息 -->