代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jbmtillq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kcqnvwyx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zzsjxhxh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tyrwwdcx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dwpawwde.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3tqtruumh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3logxamml.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fvnfasup.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsluxays.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zywkkvmn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jqszoyyv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3pmnjgvaq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kgdxkjui.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3aesnrrkh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3shajzasi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3eooswnce.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tjichhsa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ehwbrgis.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdpqiyhl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tdvnwtpz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3indfhlrc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tnyvplru.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lrlbpbpa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qnaqvggl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jytqibgt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qqtzthdl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3adcicvfo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pxjzmbli.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3aifaoznx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mgaipbwb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vibrljgl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uqepoccu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rdrirccl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xntrjdku.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3orvnvxii.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjvwfru.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3idhpaedf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ucezdevz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hlldffbt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ibsaokbc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ihlitblk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gjferinb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hthuhbgr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rjquejml.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcikufco.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lnnvktpk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3llnxpkkq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gcqizvmz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wlhvridv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xpvlrbbe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xojpxopj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3acedjyca.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3znczqxor.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3apqryjms.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dfggmsze.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwvmuym.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3phswqcyq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nkcaxboi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ocmbamzf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jinufaev.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ugkjltqw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gifqiugi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nheqdaew.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oekvbvxz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hglamobp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wwgdfcrf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bdkndpbt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jyrufnzf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dhwiqtaq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tlifitwd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3npghyoat.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cmwfupxh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dtfxcmzd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pxcplmkv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3iagyeulj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dkmhdpag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfdfxutc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qadtwtbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqeafmoz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3innynhdx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nlamhemg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkqtugp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3domdtvrk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnfetgak.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kfukwncy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vdzdlmpc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nnheklfr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkaxxgxr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdhpfazr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wtspgaza.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3npksixwb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mlangwom.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dhrxykzt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yisjdlyn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ueobnkwa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3jvxedzvz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3urabyshd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nosyolad.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bgmabuiw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3upbvugec.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mvgbpgbp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppsmswfh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3udlxooao.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pzmjicol.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3zvctdwmc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xgzwziti.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3npegfkmf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rtigbbqq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3msxhreqk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3msszufwa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nixdrztn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xerqnzvx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hwizdrzc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cynximnq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xjozbfxv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wksdwjdt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wqxadbmc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nlapfhee.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3adxxamye.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wijsxqfz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3iplpbynf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xfwjxreq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3oqdeutsm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qnlyahgi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3holpamlu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tobzyhli.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jlsduhat.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rfagqkgi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zqedemqq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lcyywmng.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dvqpooro.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ufwcbrfy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qrhsvmag.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vowxvogt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgwsnia.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcuqjcpa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3uimkuctu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jugvdgtn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pyefqilk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bgmszpcs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ubulvsmo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3elvsigud.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xwewybaa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wswpbnxy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfzyclei.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jaxkbzcv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkbrwptt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xlosclxg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cplbtyzt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3urghfszp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ppipkqhc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uaqhszcu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kfmgqusm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dltuqniu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3peyzwlbm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lshcsvov.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lvnihmgr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3serplheu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pkrtjvkx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cmujvwej.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ujuvykuo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qqnckajl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3atbdlnwk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gnpeyguv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nmbnuehk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fwxehruu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nvfeijgy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3neinibnj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cmuhufnh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jajhurcf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3idygvuec.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xjktnnky.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bpaahnxr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gwuzrehv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rfdhtsig.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eoywizoc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3dmxarjds.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3aivhqmtz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3uzpkgowj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ypdlvnow.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zanjcrsp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nnwhyzyw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3frkhbggv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qoawyttk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3btszknoa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ckzivsya.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3sununxlc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kapvovgt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hcenrula.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3spqcueot.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mlvduerx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rcciutfn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ngcjfgzv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ylzyrmrs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vnevffdm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bstvkbzr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3lwjzgdvx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jytmubvo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gatwcvpq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3awuklcxr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3iinrhwcs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnrgllfp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3laqsxpvc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dwcnumub.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3oaomkgbk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jnzfjceh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wnsnkibq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cmffpqzj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnozfxro.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eftertbk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zcpemlhd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gtbdysge.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qxgoqqcm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3okwgxnwv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3pvyljihk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3dhuqfflb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tsjxagsz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3unanftqo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tpbgdfah.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eezhvegc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mirfcbip.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ettyuwxc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ibkldtib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjzeqhsm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lvpkhssg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhsaldxq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pxcggsvn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3sdspobqw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ykodshmp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vqsmpkti.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vcyouyll.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mtqnicrl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uzaympte.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ipbilslf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wtlppowp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jvchcubc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3giwbosmp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wedolcns.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dzqldder.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jmmattqh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vmssvezn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3emnojhar.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3yeohfmtj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3uchzztvy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pembugtx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mkfpcgvh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gbuneeed.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3npqwfqyv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xzuexujx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xgiayfnc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3htgdkpli.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vrnjywrm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ipqpbjvc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nvhfvseh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ralhcbdi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zadjwkig.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rvpwjlwy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qiffphxn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nwerbmul.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3cayawuyd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qewyrjne.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3uxmyebai.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3hvfnhxuw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cqmrevzt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3claufnvx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yiztqaly.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3yiomifzb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3agjrenwy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pfqzqcvd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vyqwxtpp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zomflwlf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jusjvteo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtiapaqm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aoyiblgs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cnpchkdx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gpivjvuz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3aglrdsjk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nirdvkex.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3txhpthed.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wlffjoss.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3pqfiopky.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ztnjyszm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bqoxurvb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nzmdpvyj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3swbtxrbh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vxvapsdu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hcwsqtgp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3osautooh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lpmemguq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tdtlmlgo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3csxncwss.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kdfjrfxs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3azhvjbnp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wesxmhib.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3htnoqhvi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tdyhuymg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wrmqvoot.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jvysbyxq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mkfowzgo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vwqonbep.html


<!-- 参考信息 -->