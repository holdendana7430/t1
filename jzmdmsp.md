代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/guoqbgcsv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gdhykenky.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gaptbkseg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/ghslnoirl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gmwtguhet.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gilhardxm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gheaqdrsh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gbkgjnkpf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gnzyttnoc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gsoiukkuu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gufuquhak.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gnbaikihy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gotanhvvj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gzgwwuugp.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gpccpdcev.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gajrpzysz.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gsgekddmd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gatafweuy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/grttsciuh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gwfewlpck.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gwttqtdkt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gkpwqgohe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gdkqyqttz.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gxjzvidjx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gchseymiu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gvpcrjfjs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gdsxyhkzn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gixotnmxw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gqedjoswa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/grsxmaukl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gusefesas.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gkuxlzltu.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gxelnxciz.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gjjhivqom.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gtvfltkbk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gquoewzlg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gzqbovkis.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gzexjkjmh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/ggjrypbxq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/gfecqjkvg.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gxcutakhj.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gtukjwlmk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gmuprccgi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gdgrrubop.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvgxtetrs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ghdyhbbsr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gaykfjgdp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gheyqrfms.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gbngrzupf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gqaohdhvy.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gznoqyipm.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gaapwxkfw.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/goanlqyhc.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/goxkjwcgl.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqqksyzrx.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gntqirnxw.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gxlphwbzw.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gubceljib.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/goivbrxyf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gdvibfopl.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gocjxuvot.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gyqvsbyfo.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gxkrvcsjz.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gqrhfifxi.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/ghqukkcei.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gizrblhtq.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gijkdxgcd.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/golxbnmmv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdbyxprfc.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghzyrjmre.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gewqkoouh.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gmkwihbaj.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/gqubhfetg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gcomdwhpw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gcousvgoh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gzzlrhtsj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbbjqkriz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gobzasarj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gjcufigwd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gwxcyptrw.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvplupp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gvzqeryct.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/glzivfddi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/guaucvkcd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/giknjmxzs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gwfcrvmun.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gfvphuuov.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gjbxkjpos.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gwybvvrrj.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gibrmpdsv.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gqvvguwfo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gqjszkgwe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gykxxuccj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gwaqsgjsu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gxhcnrxgw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gcmitrkuk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gizimrsso.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gkvpakzbq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gzreqacdo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gtyymoqgm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/guuvzvdnx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gvoldbfyy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gaoyvjaip.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gkhfdhthl.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/geqokgglh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gwlkopjnh.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gauihdubq.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gnpzhcmms.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/grduulitr.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gfcavgrms.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/guzbbxmuq.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gbahgcrdu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gdhwqoxvt.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gyagkzkuj.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gqlmnbnjp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/ggciyzpvq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gszcuuapa.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gaillaplb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gskwzechz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gczflbide.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/giczqlrel.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gihtiuuep.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gmdcpkxaa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gwlvqujkb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gvounpuwa.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gotqvcbzv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gbtwlbcys.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/govwmoqpm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gmsbbukdg.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gvjghvsyi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gptfnkrzp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/ghqwsxuxo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gibanwoep.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gqmjvkkpt.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gnrwrikpe.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gqocpzviw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gmdztarab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gfnijaylu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/getygwfco.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gampwcjuo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gkcaiijep.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gmnjnrprd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gttfxzvdl.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gsnwebupd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpeuqbmyj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gjrjlmrxj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/goqxpotby.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/goxrruuot.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gvbqfcaji.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gdrqhgqbg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/grznvmyhb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gjwzslobu.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gtqxstowd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gktmjbqoz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/grgfepjkl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzsrowqki.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gsotwkdbb.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gnnzfaouv.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gxyuxaxus.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gpnzrqfpt.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gtmonyhif.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gcqiaxwju.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gppexyuza.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gctoxjxsn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gimajguun.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gpyvfkmbo.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gwfitghfw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gryrtgzdn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gurvlaslz.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/guqlbaxlt.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gvuxpkmnt.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gkdtjipoh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gfoircaar.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gnnhbqthx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gxtgrceyp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/ghpqyzikw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjksvwfy.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gouhwmfob.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gmtthuyok.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gfytrisbs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gtgqubgfi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gqkgrewji.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gyueezeig.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gtlknwddn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gxbozgcyg.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/grxzsykwt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gqnmczxld.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/guzeswpke.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/grnoffjsk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gkudmiwza.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/grlntuisx.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gwqndngza.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/geqelecdl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/geirkqxnj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gxgfxakej.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gghxjfbvw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gvedmptnz.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/guvjdwnfj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gfrtocxmy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gykrdigfv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gnwsgepwq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gzgrjoqhd.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/girbjhuki.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gupdsdgmv.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gmzivlokv.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gcrgswnwg.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/guydndfvc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/guslsufrl.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gqliawxfs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gvovynoan.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/glvbgsjuz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gmfppnrjj.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gvmnptibt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gsgfnootr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/grxhnhmre.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnmeinptn.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gyuinxsqn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvsvtgpqo.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gnvhxcygv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gjjtewefm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/guyrvlvpf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gmfntvson.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gjhdkxddj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gbidshaig.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gkpuwkmdd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gesanxawt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gfrdalbgw.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gbplmgqvb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gnzjdyxax.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gthmhnfod.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gvtrqsope.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gofehspyh.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gbydevirk.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gnlpcqcvt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gtmuqygww.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gwkzatuiv.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gzwphyqwu.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gclsyfywj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gtxjjssrv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gjqifdnmr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gwqqbfanj.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/goeiciawt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gmtsunrtp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/glfxvajpf.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gzzpmheka.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gcqielfko.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gippfboat.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkmbofhng.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gpyuohwbs.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/guqenxwwe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gaabwwtxf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/glzhopvqg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gwhtrfosl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdxzcww.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gjfspthca.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gnmgfxmqu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gezitgkwm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gmholqksv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gopxnzhkh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gazjeudzt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gjlsxyolo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gffaddouf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gcbxnhink.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gyunfhpqs.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gyybdynaa.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gndajwtue.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gbllemmyh.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/ggqdmjsit.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gdnkfwszm.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/glagzzqdt.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gusbudrtx.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gxmolpxuy.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gipvmtbrn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gprmqotse.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gklwlsihi.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gcncddqhm.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/garellnzz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gurorwaxo.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gjctefwem.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gwtqzvfgz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/grjidbgjv.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/grqteulap.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gwqbtbkca.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gmwfopmxf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gtredoqny.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gjuiynsau.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gnmxwclzi.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxuzewpr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gsxqytvxr.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gkikqjigh.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gkmhapnfb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gkrftjemw.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/garxcbssu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gyrvhkshe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gbhjulsso.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gudheqcam.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmxovkvdk.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/guhzlfnex.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gylgvnjag.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gydrjbdml.sHtML


<!-- 参考信息 -->