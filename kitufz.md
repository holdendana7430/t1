代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eatkymfz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zicttozm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nwalyyux.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2obkcaghj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kwqrefdv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2aqxphnkd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iowbzmdl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2phnjmdgd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mvtrospp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhjgktha.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ccnqggyy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2awuwesmp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejulsuxy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2sklnylao.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lrffegsx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zkjjjvwj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hpryyrmp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mzayykca.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntykydqa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lpccsgst.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfburyx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2uxhmssbo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2sdjypmeh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2sypjzjjl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eehgairm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pkywjhkf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vovzzrci.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mvscczto.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2lxwjixvd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wqgifvzu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2fmkbkotv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ehcvlkev.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jvxuxjtt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gveqqaoi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2crjosbxt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rxddebmf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gjisoucr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozqkwuje.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qpwwktnk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fsaprdlr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2aboxcziu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wfpfkxey.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ajgyaxrh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hogtkegi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqhizgva.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2xwvexrna.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rvmwbrdi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ifbtytdp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lwnntbpm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2giuahkbs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mluyquzz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ofufdoxz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sphvnpqa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vthxqzke.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyprmvof.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2azwedrzu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xenoftfl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mfobkewa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tpbsnrit.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2eumyzsxj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cbrkvrmr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pvezhepm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oyttxrru.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ohdagauf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hpmxxmzp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cytlrbwy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tdytbqcs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fxjlvajx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2acbmpydd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrvzhkdm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mqddlmjn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tofefvyd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vvrnkucr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qpmiblec.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mrmsijsc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2stpcomrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxzazcnh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2unhxsmjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rtsakluf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gmrqeijm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2afhphupw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hwccafzf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pmunbmjj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fiomoewm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pelwaadg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2aesqukvg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2hbhpjuuj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oobwgifk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uvnfhhoi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2avkfgwqp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzkyvteh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2klbfdtyx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2brxkofye.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nvthmvjz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2njpnpgkg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ejofnjoe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gwpixmtm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jpgejqbd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvgnyyn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2uhxnlhac.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qiqaxxrc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nghyyvvm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ztflcfsx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2glmqrljl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rntikupo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kldxpgas.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2sijaohht.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdpzisy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mwaydgoj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dqlvtzsc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qubkkfrg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2nrszlxbu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2oewbbdug.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgnqipno.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hejxrvhf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zhkntpfl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jjfggzdx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xoygmygn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jsvpmgkr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qpnlkdtk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ilqgzlms.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2idwiskdi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fuvjlkxh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cmsrrotr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dzthxuxj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ylmxyzle.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vvjaefnc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vlhypkyw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vciwyzqs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qcrqyhvb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dkhagdtb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2idysabkm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fionakbs.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2inbrmzpe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2tfrgmxsd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2klodpgqo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vkfdrzbd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bobnewqn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lowknpen.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qhshgeya.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2eylugaor.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qxmouegf.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ncutfjeu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hpmiyrim.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2pscyskcw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qlhikzlf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oxhtindh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kbubwbxt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2uzavdvgp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gnzitdbt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uokvhevt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2msigrjlz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvytbtei.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrmebkbg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tvikhwcb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mgaydnkj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhkwztpm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ouoxauyc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yymkhzdt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2spvoygeg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2umpvegie.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cxoghgpo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2imkfbqrh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2enfitiec.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rfduomqm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2omfbtcim.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ctdwjjec.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2omougdmd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ocphkcbq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2okdqsiwp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dzsszpnf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2pyyftyap.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2irxodjss.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2owildjgg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mawyujky.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zcuiuiiy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jqqlszla.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qfussibb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xmgnkdfv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kpbqghrx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qbgfxjli.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lbnxnewm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wupulfwx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pmyamtlc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fetwtnpv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xhjsjhop.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qxpkoafz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nefyicce.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2acqhdknk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpxbmifa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wqbyejzo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ryokguki.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdzovwjw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2aggqvxbj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lxbdlbab.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yqpvosmc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vkbcbxux.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kqifcpjw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rwnwbyla.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tpmnsvvd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vszbduzq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eijjngft.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vqznucur.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iqyndgwq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tfrfmxok.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xlngqasu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qcyykxxg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vhjcjolf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mpnazpxf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsbsduvt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mqhrwpjt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mnhhxcus.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bwatrfmi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gegvgogl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2msxvjvzq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2anuzcrak.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vowmrbsf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wokiolep.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jhsmznyu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zedizxou.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mavrebsh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ozejxktk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpyyfkie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emnwtkjt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wxnguhft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glpbmwxx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uaurbvkw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xccijtya.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uumxbfsm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xyvxethx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tqjdivrd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2cdaydgdb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qnznsnyb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pkyzymzl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qpnujxsh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2vyxukunh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wngmxcma.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ldsgizgd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mpfiduyo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mfunuqix.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2zzenigsl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qalcgtox.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jalauggs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2txvmrtti.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ryvllaeu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uqewmagz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mmbxjddr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kgvrfuhe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uskatpus.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sbbmwajz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qbifcyry.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vkzhoaqn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2chezyghe.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2oejnhkul.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqjvcwi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ebfbcrcl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vvwncjbe.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2buzsqagl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xmbuyvrx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dnuuipod.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ksihdjja.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wpblvyik.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vgfjcgll.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2akahuuzs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tpfpweyt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yohqzpei.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vnzrlvlx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2utqzllqy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cfxcaymn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ufsmptmk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rwwaweyg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lagwzysa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hltnyyyf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cncglfve.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iwympptn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2teubcvmp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lrxdpixo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2asysegoo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uuaoitpf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2awlflemh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2sgnedjuj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jnjbdzug.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ftoakyww.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gscttdwo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pushlxql.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvoccmoy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ejizltkf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tirwfovj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qzcpjilb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ceyubzxb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zxinqxxy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pfccsiln.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yulenfaw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2htmhxqyz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wjzpwpnm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2itinconm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2yiqctsgv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aaemrjtm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2naijevvx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dbdyavjh.html


<!-- 参考信息 -->