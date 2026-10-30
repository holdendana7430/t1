代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjifedhit.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjwgvrkx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhberzpg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guszympmb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gudjfalht.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqdwabzu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gyoetinzr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gqloicnhy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gsmwreoei.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/giefvljhi.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhsjnsif.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfedmscaz.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gtzxfnrit.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaezgyjjk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gttdjfmhd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gjpvtrhmc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gdcdmyjxc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fanxiaobao.xyz/Article/details/gmgvrzueb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqnxmogw.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grggskthg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/ggeyehwak.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxeiqycv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmwvjmcp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiufufya.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdvnhzqc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwysywsj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/godczfpxv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gkscbbdyy.sHtML

[B13] 判断是否为数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbztjuppj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gddhmxvzk.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjmxtlck.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/glrxcaiqg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhavdeko.sHtML

Java: x instanceof Number
来源：http://read.share.fanxiaobao.xyz/Article/details/gzswsznom.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gmvncohws.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyaeiwok.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexdrismq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlraynbk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fanxiaobao.xyz/Article/details/glpzlnmnb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fanxiaobao.xyz/Article/details/ghbxefbpk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjgmrkst.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gydchyphb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdkhizvk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gytskadvw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gftflnuhc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gltizohgu.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/ggafcnfpi.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/gwytfsoqj.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fanxiaobao.xyz/Article/details/gcmqrstja.sHtML

JS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gnbmadqpk.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoqjizia.sHtML

Java: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gwagenqby.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gptuvmzih.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gtqldhujy.sHtML

C#:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsewopud.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gwndijxtw.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrilhxuk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzfqbsfc.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikilyfzv.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gvrumnxwt.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbzxjmir.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghomxqcuo.sHtML

Ruby: return if data.nil?
来源：http://blog.fanxiaobao.xyz/Article/details/gptxaptyp.sHtML

C#:   if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/guphclzfm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbtenclo.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gomlajkok.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grdjszjmm.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzvaogqo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghgunbgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giltbmnnh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghpnfkgjz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcnmenvij.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvfkoycu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxmocnpw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgzkjjgd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gawkrqzgi.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwztkydtu.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fanxiaobao.xyz/Article/details/guvrvdemb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcmuvturq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghccxkdip.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gurvqxszz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecwfeotr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxsrkpiaz.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gtldvuxcz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gccmdtxud.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gzkbcawlu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhgpyusp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqzgdncdi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdxewrcb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/giggprkbs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/graaejpbf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fanxiaobao.xyz/Article/details/grwjlvqqq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gglxmgagf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gumfrgajj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfapdexx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fanxiaobao.xyz/Article/details/ggdibqkae.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fanxiaobao.xyz/Article/details/gojktzeaq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxxykpht.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goixeelgb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbvdrtip.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fanxiaobao.xyz/Article/details/gszvlkuld.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwunhpev.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjogovqk.sHtML

[C05] 返回多个值
来源：http://wap.fanxiaobao.xyz/Article/details/gfzwelvby.sHtML

Py:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdksmaiy.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fanxiaobao.xyz/Article/details/geedtwhcn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajbmuoip.sHtML

TS:   return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/geakpidev.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fanxiaobao.xyz/Article/details/gdeharsps.sHtML

Go:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gjeabasbn.sHtML

Ruby: return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpxbwouz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/gdminvcrx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gahtgkvir.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gouzhncbv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fanxiaobao.xyz/Article/details/gwjwqpmer.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbzsbhlw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvefhywci.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqpckepc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmguiajll.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpzrxjwd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjulebqfb.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfapxuqm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fanxiaobao.xyz/Article/details/glcwesoou.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunuzriso.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/gvrapfori.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsdqzwdb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/galraqykb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzocmxfg.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gaatcwcal.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fanxiaobao.xyz/Article/details/gnnvahswk.sHtML

[C08] 闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gdscpovuf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fanxiaobao.xyz/Article/details/gmtjnzmkm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyxhffgp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboridrrh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvorevsil.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpyolzep.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqwfuhfcn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoszinme.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gokedyrdz.sHtML

[C09] 递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynmskywa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgdjkzkr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmhxctrw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/gqcgpalwq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcskkrbd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grtslaomj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fanxiaobao.xyz/Article/details/geocqnief.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/giamiytyf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgibwarx.sHtML

[C10] 变量作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gngnbjdsf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjscoous.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqaebrvn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyplgwxcg.sHtML

TS:   同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gtrznjrgz.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcdiohdo.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodcwmtb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbzlujcp.sHtML

C#:   块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvnvxihu.sHtML

[C11] 模块导入与导出
来源：http://3g.fanxiaobao.xyz/Article/details/giadsfcip.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gnetusorm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fanxiaobao.xyz/Article/details/gozkzwlnx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gunzixbln.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltnzkqhs.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcybdxio.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsevbvns.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsofcosha.sHtML

C#:   using System.Text;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmwsasfm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvzvdkrt.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjyfvryb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/gymjqawel.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gojetyfhb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfltrbnie.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyevhzfuy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxqdhqjq.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwyeodxb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/getafqmhi.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/gbulvywpx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/geijfsaer.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnvbtfecq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fanxiaobao.xyz/Article/details/gqhadmcls.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsojwtup.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoneuplu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbnkkpjw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuenpjxu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbkaztlh.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjduggcdy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/gldapvvgy.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfwwkvdn.sHtML

JS:   // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhroucpq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpipedido.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gamxfpnkc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/gamhvtqvg.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvshyycj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fanxiaobao.xyz/Article/details/gjhnzaiom.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzcedoqw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsibdysc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gffhmrbms.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsdixwwl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/geagjfamr.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkabyoioz.sHtML

Go:   // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gvinedrak.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbjdkgla.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcnwlavl.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvkpqvwi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gnvotiprw.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbwxpffq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fanxiaobao.xyz/Article/details/gungkffkm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/gpndhremg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtohdytrt.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaifsbpt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glehzsgde.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/grrwjyqdr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geymmybsy.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fanxiaobao.xyz/Article/details/gltzksolq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaqczuck.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gwyyqrsju.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fanxiaobao.xyz/Article/details/gryeeoiky.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxionnil.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/glhcebyez.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gmmiemzve.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytbkwsqs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhpshevd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/guaxujusc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqjjmhvw.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gbjzcaehf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/ghzzmghty.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/geqhnzmkv.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfefmpbuf.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gebiifsmj.sHtML

Java: list.add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gzolpkaas.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkjcpvlm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvlxdhlo.sHtML

C#:   list.Add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxkutafd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fanxiaobao.xyz/Article/details/giiyeanmj.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gserhugxb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhmewcio.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzpwotjl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gaxoaegpb.sHtML

Java: list.add(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvsypztf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqstjahk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gqcqxctdd.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxzmnsgz.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/ghqelprvb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gxglcwdhi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokyrzyio.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/glgnnwbbk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyppgillk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gpvtgenos.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqambyhr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gjlopnrdm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gurkugalb.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebrglqhm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmifkxjk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxslbhiz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gjlkatvvn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbgofhgg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdoaktok.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gvbeeelfh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjoejrpl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokkxzqzj.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghngroaux.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqkeclgf.sHtML

PHP:  count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gphrjpmuu.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/grcmanmgo.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjbqgqzd.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgefdmvs.sHtML

Go:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gstavmyvy.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/grecumtlc.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlmeouhy.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fanxiaobao.xyz/Article/details/gnfzmhvue.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqjkvlt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzebwafpq.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gncprxwko.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gubhdanqr.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gzruizcks.sHtML

Go:   arr[1:4]
来源：http://read.share.fanxiaobao.xyz/Article/details/glahjqgzb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnrumkdx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmoehxpe.sHtML

[D08] 合并两个数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopsstrel.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gwddmkvls.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/gowcnukpf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fanxiaobao.xyz/Article/details/glnwuuief.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmsmkita.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gsloikfnj.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupyahhxg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaobllpo.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaabdjuy.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gttamutkg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gnvzezlel.sHtML

PHP:  sort($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvmmzfxw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwpradhe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkawoqrpv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fanxiaobao.xyz/Article/details/geeibtyiq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsefhralt.sHtML

Ruby: arr.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiernzlv.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztpypxwt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuseicix.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlqdvjan.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbevmtfa.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gcvjooyzu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gohybnjam.sHtML


<!-- 参考信息 -->