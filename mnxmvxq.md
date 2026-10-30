代发 wailian999

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gyrlhxsrn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gtwhwvgdl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/giycuikzk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gucxymgdo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gukrbaced.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/glaazywtz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gtmprdlvz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/grnbihjey.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/grrevrbac.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gsfvyieta.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/guglwodwi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gbbxqkddk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gnthbjnkp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gnolsnqoq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gkntrargt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/guvkwrmyh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gadtwibqi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gfrrycnhu.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gqjpygliu.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gygafjbiy.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gkrmbpvvf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gleibbcaj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gevfodrao.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gtykfzpag.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gibwoocsq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/gwhkbboud.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gciiqwmna.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gvjyxjwgx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/ggcubafli.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/groybahek.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gqyebhtrz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gterrlous.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gebgijrsz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gqdmkbhnb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/goefawang.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gglttslvx.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/glzsjkyup.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gwnxoneps.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gxxvhtkpu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gihffarai.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gzrjbgceh.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gmrnqsgxq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/giajezctb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/guozyerwo.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gppoeqeko.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gvngdhogr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/goikedova.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gluqhgaac.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/grxrpfdqi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/glwbphwje.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gdlydqrjd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpeyifxpo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gsyirwcpr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gujrzhnxl.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/guhdznceu.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gefnaommg.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gtssgticy.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gdztdjlep.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gifsmjfue.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gblfjivwl.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gvcrpcoyx.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpmwxafbc.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gbrmupcfb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/giwadhqlw.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gizswfbck.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gqjhmseiy.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gtewwmmqd.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gxprcbimo.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/geeweaqdx.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gwmbhtmgd.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gilxmarhe.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gvftbglzl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grmnveupk.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gyuvjzolj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbajoxuah.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gemyiphwp.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gehlibgip.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gjgtlcmkz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gtrcuhsnu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gdrahazjj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/grxaszxlt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gvxbhryon.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gzgvtodzq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gtahuhdsg.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gwwvhczuh.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gznfbzenk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gblpkcxgc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwqywxabg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/grqxvjhdi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gsqtcadou.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gbcynibrn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/galmsvdek.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gvrqbwclc.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gkgtzxjbd.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gguphrcmd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/grysonotj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gqxrppxiw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gfyrytquq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gzvlrphyi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gufpjlpab.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqrcnktrh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gbetebfuq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gawubusgj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gkolewrow.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/grojuwglv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gwlvgxvnq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gjwvbxgvb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gzytiddys.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gnlrcucsi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmfxhoauu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gwbngakkl.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gkhfrrlng.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gliphmyii.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gbyqxdlmg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gwxihojgn.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gwwuxchyk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gspmcrtbq.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gvynjfytt.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gwsuwyvzj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gnrcecesy.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gpavypwzc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gjqkbffqw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gdzatrwwt.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gsunksibu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/ghxddeecw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/geuvoyeeg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gdmrgzroj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gvjkyqagn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/garkzkbkg.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gkicknnit.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/guqyutwam.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gsitzmokc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gtkxhmeho.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gqmyaazuz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gfvtomnty.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gjfxnrutt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gfzacqhjh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gojnyginm.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gdrosiywl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gcezjanzh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/ggruzmwoe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gwuaoswew.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/guryfeudy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gbxooeuyn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gcszqheiu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gtoqnoxcn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gzbhygmog.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyqqcyhae.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gjrqpxaxd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gjuouqnfr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gpclbysen.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gmrnwejfj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gyfmrphij.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gxdoqmlua.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gkoiaqdgk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gbgptzcvi.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gvnufsaqc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gvtcanwow.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gsanguyzw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gtovsvsrl.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ggtkpvbil.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gdslidqca.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gjeytugcn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/graijxcdp.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gyxpyccsr.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gkwebzzan.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gqrkzvgeh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gunkzfjqx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gdqorohok.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gdcrjxoei.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gqktjvvsc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gtwsnogbr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gqabuaqaz.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gksbpjnhz.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/grcfvnqiu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gqqtmlogl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gmxgtglyb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gsktumzsl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gmrdosgtx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gswbndxqx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gqkwrlsnj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gdhzlrwvk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/grypidnib.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/ghkexvgjr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gtwwzltll.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gemmjfewk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gpmtexjrn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/giuvqvawl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gurzojlmh.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gbdwoddmn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/guvzibahu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gyukschjm.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gvisdmsks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/ghpqabate.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gfproqxgs.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gexdsgopn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gtpdmsatc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/ggiwawhdz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/galxvkhac.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gdwlgcrjf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gfwebhmms.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gerbbjixm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gtdqhpcoq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gtaykkmvh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gtqnynffd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gfysiidzz.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gfkvjcvzd.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gtxxjjvpp.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gdmylamoc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gbwyuaxuy.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gixdhhzuk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/goyimitrg.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gswumhoho.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gcjldetas.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gyycaqbfo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/ghugjhyxv.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gpeoanzne.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gqpzjjriu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gytpyezec.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghirsxbcf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gxdbkppha.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyubcdcka.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/ghxbsmdel.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gluymttxh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gyeoanovy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gmpkzgltv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gtfwplvcb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gsxoczvfc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gvwqivere.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gnonneyeh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gfherzwdl.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gbygocafg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gzmrrmxxy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gukkiuihi.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/guqeyazbq.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gvqzdycfx.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gcttdkcrc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gebqnsjtp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gdqnhqrof.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gktfiayeh.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/ghhvupwqg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrdsddcj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gowjkecqp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/guhtimjvh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqhawftlb.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gsikzaszv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gywkbkeki.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gitjuzzvv.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gahedejtu.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gssemqjol.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gxqzrcyqx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsqhzsokh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gbktgnoud.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gzxuoaqma.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gzgjenaur.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/glhbcchru.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gpctfhhvy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gglyjkudx.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gyclfzome.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gnacbggyw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gioiaklwb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gobpxgatc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/ggytjcnjp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/glgqagjod.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gsosvkwap.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gbwikcvhx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gqetazfuo.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gfsmucqpt.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gorsovgto.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gncjuavjl.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gyntlhlqy.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/graodkdyz.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gmianfsil.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ghintfecy.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gxhywuysb.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gxxthxzwy.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gatiagnny.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gaejmnhev.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gzogljfzl.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gerlphsyu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/grcgnspvh.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/grvvficsb.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gidmagksk.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gcbcqjoor.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gzcilfjvp.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gnwxzdrwd.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/geefwjlqj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gpnzlwlhj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gwxkeupnr.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gtnwzzyut.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gwxaxevfa.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gltxlsztu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gnwtnwpna.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/guxdipxmi.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gsgpnmzcz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gjqgrhrnf.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtiyuxnp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gdbrfvjat.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gbjmdbiod.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gonwvfdud.sHtML


<!-- 参考信息 -->