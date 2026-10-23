代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qfwhwrfs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qvspmzca.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3eutkkocz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nmeulgox.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gogayltn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bleocqff.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdyvpbuv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xheoshjd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fbqryutd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qrazbayq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3flhtboyg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3waymuckg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qssybmwn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3eyjfmela.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3blytvfjj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3exoweelw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xthxtzwi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wkdisive.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vlkuqnqa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3teyszvrn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xfoxiewm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lldwvcti.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dolmugxy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3katqrtkl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xqdzdybk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zpvlqduo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qeldnjcp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dcmidslg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3cdteavxh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xaycmctq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bgdwlkls.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wphkaopd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xzpiaksh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3arkkboeh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3viozwers.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nrruqold.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3adznffvi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzjzmgkk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3yrufmjaq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bnqufagd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xpopclvk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kkrwewfc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmzplpsg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gtznkysv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovkxclub.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3yojshjkq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dkvzdwvp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gwucemaq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jositxfm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jbilncrp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3slqesbdr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vmokibnl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ylrrmvjg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozeawhrs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hdxurucq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xarjyrma.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3thaktppm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqzzoprv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rrdoulat.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ypcspnmr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ndiqfrhy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3skqfjiav.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ayysvzce.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uaxxwvix.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3scjomyml.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3srldnsaf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kiqwfzox.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3etpdzxhu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3iqepnngi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqpzktwr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tconcqil.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dnanerbp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nfibwuqe.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lhmoearn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3apmkrukt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sfictmkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stsxauec.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fpsptqje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yefinmhu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3twemilwd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3knfhhgnw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvdraejw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvqtlkoh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zgpoadzq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdowtqmw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qewcyico.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3eykqbcli.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgldeixw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ogzjgfzg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3bkbjldja.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hqybqzkh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrqontkz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnicnrti.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3agzatjbx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3yisgukhe.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pwflcvaj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qydzfgkt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3poqqmeov.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzfuwdz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqnwnesf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhpcqhqp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkbwqysm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ruccnqnp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ufwbeavt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wcoypnce.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ipmtcahf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ucomvleh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cetvwcei.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bvvckycc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qshrnnng.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gofbmaoz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gticvopz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zonaikbf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3exjsupww.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3smxkukfe.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wjopuluj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xhqczhue.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ulbgznsz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vvpimrmy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gjdalgwt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3czzgithy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fcehtpzh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ssqadhux.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zuwhhrsp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dotxxcxw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fqvejuyt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3suvfpddc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lnawxylk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ikkclvyy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ogstwyiv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rtnulgwc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nlyqhliw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mppjbbmp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pmmyefeu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vccveswb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3piempiir.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cuonaukw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmkaubo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xarezlje.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rmonxjmm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ksvyqgph.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mjqcabpd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nmdvpece.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mxodexsm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ectzpbdf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mlbbjfdi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzkwetgn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qxnokhnh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ehaizrom.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcdcrfqu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehijpumn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vuxmxafz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nkvtuizq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3isgbblte.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ptivqaqh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3slrwgobo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mslaurqg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3uxjvzqsr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxrasatm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dtysfpkd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ikhaawdq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vlevbsyy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3iwnnfcpi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sipsiryh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kkkylygx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xedaayuv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sbrszlbm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3btcxgagh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tcryouxo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rsejjfqt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ltbsltxt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3eutibcwb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3bhmlqjdb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3suvsskuz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tbizppzj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rzihorzj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pmanblos.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3iydqwxmq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3sydtvnld.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3elwsqost.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zztnmmqf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tuguspfl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uiznxpbl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bynzbtli.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vgmynjqu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nuiunlsk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3duptuhik.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3joxqexqe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gwddssnv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjwspdsm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qauprlim.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rknycvfh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yjeseusd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xtfmucrz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rtmuymuj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dvujubtk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mdkodivu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3iggsuoho.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mbtezzhw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ryukltph.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oosmyrwo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3brbwfyce.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vgdoqmfz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hwfygrvc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3raktlnqj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3npgyszzr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3htsketri.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tajuxpnu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxfozsqw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nditzmyb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3paqafgvp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ghkqqslo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3exfctfai.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tczkixsi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3biuuqvmx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nejwpxjp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vxqvzddg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3kkgrojim.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ezmbimks.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zouodnfx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zoeqkzqs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fkygdsge.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pckomnyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rolruobx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kuumgarc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvsommpd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rnataxla.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wrpnunhq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mgpxnpoz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fglgoecw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3veazjzxk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3bdslzafq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tzefztoy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bhojmfmp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3knnolnzs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zeyibjqb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fcwwbwru.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3liovtaed.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kgnmnpip.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3htnauvfn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3kggsbwic.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lbqgtfvn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ucffzzoz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3emksjoft.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3tdmzopne.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xibvyryi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ysptdgen.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rexymlts.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jqhyywut.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nhmyrthf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vmwbxhkd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3eohwwcws.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hlfluyqd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ovkveaet.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dbpfrdwf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xakosbrf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3fzjvtzhy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ktzwuefs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gfdtkbhh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ejgydver.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3umgymxky.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bpubekav.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3srlthtki.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3itqvswic.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3afevgnaz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jesqziei.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3desorgkd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gpyhnhec.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3npfvhriu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zosyblbd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3unrtdmif.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wsgwjcfp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qypblpej.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyjceecb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nopcgwpi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fzcptvgw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rlcstnqa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pyefcjhw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3yugcumzk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hfkfuyev.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dhwjwkqk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pqrvlizb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ogngokma.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jrasknxb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bggorsfv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3duczsqhc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3jnixivce.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xzcrhvgj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3liywwajb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ydsaqpih.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3aaembmth.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mdphnmhl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fxegqbnp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3fmwdnmyu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sxuyaber.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qeuoetvi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3syucoqib.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zgpmlwqc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rzodohwp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jfesaemk.html


<!-- 参考信息 -->