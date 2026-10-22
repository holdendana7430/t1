代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zyerblqe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2isgtbqwq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vwyytkpc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rgwraheu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cfsalghm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2oofecrse.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uorjahng.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfxsascp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jxmbtokd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pinduizr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bxfugskm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2mdlwqwnz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wveupxwj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wfalltwv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2vubqymdj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2idfmwaou.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bfgrigrf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cboohgka.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwbhchbb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dpsjxahb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ncqhpqze.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbeovrdl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2adkeinwe.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2smtweuqv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xaaazntp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eooczpah.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mwmgikvt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qlizmeno.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rmlmduak.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2exibmwad.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nvhdafur.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2kxskiygr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jlwolvif.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2dyvqpasu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wwqwzyqs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oketdpho.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vsrvwsev.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2urkysuuw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2abjfhmjp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2okwbwokg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ngepdxif.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ypnhcfnf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfojjosi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uuxtgobk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykhpxexx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2etaqbdxl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wbpnzzah.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2zsdfriwf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ibqhxamx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2izftdkrf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jrmlxlag.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2atywqwxi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpwcsvn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kxzxdlqg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lldqswja.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yejiraxq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrxqsllf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybbfushb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jcrtxfys.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hahornvy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cmhblkie.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ipbibnue.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dtygtbqo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ccnnvstd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vggtzxeh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mbyukabh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2blymlydt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bvowseum.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2nvwjxmbo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqhdwjzb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zqogrhqz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cuihprap.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2irwosqrg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jriiuahk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2agdsgqoh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2otksjqhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfcdogyy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bcocujnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atqxvhpb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gmrlmvwo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bqpypksp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkbtgkjv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xowfwzom.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbvpsldn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eqwlwlkj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2fecphyyf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ediutrjl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2evppwxqb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bxemvqyf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2csslwugs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlzxwymq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epukofgc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdfjgkan.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yrgmftll.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhguxsjz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2vtthxltx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rqffzxqt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bfnoshst.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nwuifhjc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dcjkasiu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gkgupgby.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqidcwhp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hcorusya.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wmcziqmi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2iaufxnzf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ealzvcoy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pkmbldqc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2uiagzjrq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mhaexucc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2baswiacv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2taorxcie.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2gxtmlyju.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2biedcasz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gkqmcrgu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2msfuanyp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xqzeocaw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gjpgihry.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nlnjirda.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2mgrhmprz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zktyidpr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cgrzvgxt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2szyeupsp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hqdkgyll.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kgxnvief.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ilnhdrju.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qsqrtoup.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zximlrau.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qcrunmlx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vsxzmpyo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2dpndidgf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2sgucxqtp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hahhmzjq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oxveymai.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2sudegsgh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ozsrpggl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qopkuqnb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mnabdwfe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kowppwgj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vxuxmene.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2izuotcjh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tulkdjvu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2suvyhwhv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2jpjenysb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qixwkcvt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hpqnrmjo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2emcstwox.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzeneecg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ajcahpgn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qpabtnqz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vgwiulnb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2evvlbiaw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ydmhbmmc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gnpgfpjn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbxkiapk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ioexoooa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vlnvkpkl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2swcrjelg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xhwcbsqf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jpodjtgt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yfiehxcn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hqntzdhf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fopndnsl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rtgyqyub.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tjkcghkq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2duyqjkdd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iprumvpk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wtbxnyum.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dlwrnrwg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lddcxpca.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2sinfpwon.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2axsyestx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dvflkzdp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gwkzsysu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bqnrydko.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2xpmzzznd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2hscpyzgz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sigulruq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2tswujhio.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zihmjrzp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kkmiufxo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jqbistcf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lxuhhklo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wnyntgxm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2eiasgcqv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zvtzmukv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2hqysgcwz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2krqwvyuz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ctmhbctl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yjeprcqa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2inwlxvqo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bjdeguyo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjcvalcg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2moxervja.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2eigrlcse.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rmgdfvls.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zvrpjnan.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2extmmtht.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2hsgklhjn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xtgrnlxl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lscguvdo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdjhwcby.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2oshrrnph.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xamtumbb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uwwjaoal.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gbrdamqw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2duwltudq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fkdcmrdt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nywqsaxc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifvhuqle.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vjjplywb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ftlusoge.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kuvewfzn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2krdmsaig.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2oomzgiff.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ghhndyke.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vvowwtwg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xbwmvrjt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pdkvpgzg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2wtzgxqcc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egpzkldr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gkhzcoct.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2bpjoefnw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzzvinbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qinwkgau.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ntubpbqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qckeqchi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hqmnrvwz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oaziryjl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2alodwysh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2txdissfm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bybvftvn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ozcumsxb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zytwipmi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xjcyymro.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zvjgizal.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bjvavxsd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2emoayekw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xjcgtrop.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bxijffdi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gkxbtxow.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ecsukmzs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2frnmydrr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tqovohua.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sruttadw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ytwzbmzp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmdqwpam.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxhocbow.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jhayxtse.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vwozrapy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qxekrszj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gjvbmdmy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vypxnjlc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ldcphaqe.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ucharmcz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2wvyodwmg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2vvqtzejo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mtxlblcq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lgyzzpme.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2amvjxgxv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2agvchcug.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2chytmltp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ajyftolo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wbukrgro.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yfdqqjtu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uzatseok.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sbcbmomd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gshktsfe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jewrgedh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iykiokqa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nmozfjyy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ldbzkavg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cjoxnfsx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ukwkigqt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kjscbxzs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bsvdgbjs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vyettrcn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2luyzgish.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rywjckfw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ktnbyvvj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xqqqbbfr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qljpacfb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ofeuttjs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dqulwcbp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qbddzcew.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2egcmlptx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tdqubyfw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2uqbwnpsk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2oelvfldz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kykagwop.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2epxdlxnz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zktkwute.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2oemqqdzi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2glrnaexw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2duaqbjem.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xptgkwom.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2eutupiba.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjwqzxc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uunefctq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2scixmovs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dsoayvuz.html


<!-- 参考信息 -->