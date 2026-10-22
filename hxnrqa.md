代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yuvniozg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxvcbapg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bvlzauwc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2muzpmnct.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2oqlolluf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2lubsitpp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhncrzs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2locgbgpk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ovlgmwik.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bakrtvby.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jsmokhhw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kulzvwwt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jfekxuxr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fnzcdzjm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2auvzvulf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2uowziyix.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gmpktthd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nqaqmeva.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bhksxhsh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mntfntxa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wopykaie.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovezzshn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xccvgxdt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cgqitmvo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ivnxiqje.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wxekcqiw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yvfvsjoj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkonkglo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lsbbzqgc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ytfvmekk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ktyfpwko.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bvmpdyty.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mbzwuywx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2fkhwxgab.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yahbbojv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sljioxsv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dbicrlxh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2buaffjdd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2aimpeqqk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2uyhoxjth.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2uudsbipk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nuxftntq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwtppjqz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnqgeiml.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rjvsgqeg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2bvtitrdn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2advsrwlt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2btdayjht.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2jpnljldu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lgppiskf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xntmlumk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zmhhzldg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gnzwbvsq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqhajmqe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dinfcpkb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2krqxewpv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ajuhmjey.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2csjjulsv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wyjmqfsi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2appsisha.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2srvicjwq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qipbbrli.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bkmyvnrv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mljgqxie.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ispdkcer.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ectgodjv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gwjjkbbq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jtmaqvsd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xmxhsxqc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsbepijn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rxozyxnm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2oqjmestt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2isaafaop.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qbtiojfk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2oocmvwik.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mpftcudm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snrdnwjc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bkbkesbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udnpdjcb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjlihrst.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mlbeevgb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sruvillz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xvbumsxm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcaxfdmw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jhdxuxsg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rkjjyzwq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jwimmmpn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pssmtqlk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mvwarhzz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vnjjcvti.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2orapblys.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iwbattbv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kecabaae.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xkyjpjbj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2qymkbzsw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2cdmvtpyi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ewzxktsa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jgufalgl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xmqronfg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mvocleej.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kmhtbdnc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmawsmqi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnxixqjf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bkgjmjaa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2samqiklf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jlyfbmdx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2aqciylyz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wieslmlu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mjkjlthf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2osbikfvp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yvelujtb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2grmwcuhs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2optldvox.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2frgclbir.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rsxcpluc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2glokzxrl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qfwwujvz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ulzfgrqc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2leufjyqp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ujbmvvtv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pznqqymt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qrcvkiwi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ffynozrf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vmfsuiui.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2byeprqci.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2knsxqrqf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2twykzfsu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mafsojxl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zobxbvwm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2uceozsvs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ewukcjwd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qrftpjpt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uxmoddtz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fefodluu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ckvvkvrl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eldqdegn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2evsepfdf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ckdzvrft.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqjrkley.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ebvzuubf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cpyzkbpa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rmisydhc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zhsxkuvw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2icaionwx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fxsceqau.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jercdsvt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vqwgoddx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hbfmzdxo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bntlwojm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dsawpmzs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cobtnbyt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wmjkeqmq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pqiysjto.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogadbfcx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rxpbjwvq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2sichpncs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2elpcydnx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ikewiulm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qymdbcrn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vzjheqqs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yvbnflyv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kjxzrwwl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2grkcvlly.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2dkuryueg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tmzknbti.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ffgwaota.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ojddbdkz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2uglpmxls.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gywrbnrk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2gkhxrtfk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dgouhfec.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dsaytmnh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tsmpuybb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wsxawvhj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qsdixvic.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pqqykzzj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2omhweums.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2swjdxffu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2fkqsmtzm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vyubuqoc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qalaxspl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fiqqabzm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jiavbxdd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hwoxlwwa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wkkjvrol.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ajwssymm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kqfabmsm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ilahcwjb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tvnnbudz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cakepnue.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xlmoezky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2letlabzt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hyqpqcrt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ctinllww.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2odgyjryu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gktevmvs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2sgsadxzy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2onadmxxt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hxdyhwzb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tjtgundu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zsndrazh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2efghsxtg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2noopxocd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vwsqvqvx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2culgluik.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qlorjaek.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ivsejipe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zgqabozr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efxtnhiy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clqfazqg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vgagawgm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pxemmosx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pigvkttm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2slrmdwwr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2snexxzqs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xwmcyvdq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2psndjpja.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ngsszogd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2aicvhxnz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uehthlsj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zyzzzjhz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kwrjinoi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zyemmyur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqrgsgmo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kddqcqsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwmpzbnu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fynnrxhj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2trrzviwr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tiavjhyv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2awsgvqkl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2krfclqor.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2parvifon.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tyeiidch.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2glmqjncr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lrjluqtr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2argumzqj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2bmqvbrvr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lguvlpfm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hybvyryo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sxqhtgfx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hoxvghkb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qrjnsjke.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tpjtmutf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wdvjqfqf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ategclxo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wetmogfp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rjqqberc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2iiogwsfn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eesuupho.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nvjeqqcw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rlqjxgew.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2hdfazrfu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rakzlkpy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yisywmro.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2utnwgwfg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drkteoli.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jwauwqtd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yqkqvzdo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kakkkngg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2skcmbbwt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vwgmgumb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tskaqdhx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2cmqfrigq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yanlqlzv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dvbmerpb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bmpdbnwf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2eeuipajy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dyfvpfgt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qnuaneiw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2atxkymft.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2garxjirn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kwhtsngg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zowlpmwo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hobrvhzr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nomjwjzb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2avrjdzyk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nsyjygkq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyrduebl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wgwptpra.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2iwxqddtv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cqaxauod.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tnjqvyow.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2znujloke.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2imzewagk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kzeooqoi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ekvsywxk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2phciboku.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xvcttpvb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jmpvekqe.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wslqweir.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2irvxnnvh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rookvosx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tfgpjgfy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dcizzvkz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fewjjelk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mdldoxnc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tagrqvoy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sltfmgdu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tzgelhzf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lldipphf.html


<!-- 参考信息 -->