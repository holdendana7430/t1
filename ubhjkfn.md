代发 wailian999

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gkugemlza.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gpxatetld.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gzmufhaqq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/glnlkclca.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/giyfmkdif.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gqskfuaak.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gtrscyyhd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/guzquogmf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gmeuzbwnj.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gvfuqpeuu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gtrdbpsxu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gbgivtvfl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/ghwppjxci.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gpycvhgcm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/giwiqblrf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjbxeohr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gbnbsubro.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gankeiaad.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gqaxyltpt.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gtaafixlu.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gbblikavy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gbivjophw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gaapznhra.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gcjzykyuu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gaxvapozm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gqhmwigbo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gqjyrmcho.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/grspfzfxe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/guatqnuym.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gsycrxfrp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gkolbdjmf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gvxtioeqf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/glfaenptf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gduvifasq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gcaxpbxuh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gbtudctyf.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gbvsxyxlj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/geqdixawd.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gosvqadzk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvhejqore.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/grkgbusrp.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gogqfwave.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gkugtnutn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gfocrlgkb.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/glibrcipm.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gonbndvgd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gkgvkafei.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gqmrjqjsh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gligfspqs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gzcovpbny.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gueivxgio.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/guvbdbqrw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gyggfimqh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvvtfwkxu.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gupvxsfms.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gptycjzuz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gvdrloiab.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gtuukrwcg.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gyfwthouk.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwgjaszvt.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gptfxongq.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvblfejvy.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gnlxijnet.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gsonxudhj.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gpncdvdan.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gqonhywii.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gqpbjpujt.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/giybwcber.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gmmtnqxlk.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/ganvyxblk.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gyjifyrxv.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/grmlrxqwt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvlodztvv.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gsyxeghel.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giitpixmx.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gvxwbolgt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gheavfklr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/grtmszmng.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvvgbwhwg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gnlbsopkq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gikjnqizt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gnewassan.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gqmsfuuel.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gqqwrqzar.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/grexzcozr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gcmuxteqe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/ggrlrgblc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzxdbaxqp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gntuzrsho.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/ggytqeqms.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gngpnijyg.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/ggvyqbslt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/grnccbpnw.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gqnczjxcq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gqevaialr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/godfkouto.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gwqcpyuvt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ggrvurtjf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gjdoybfjv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gvsfmssjj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gexnfqsdv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/ggfsmqlmv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/ghreaechw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gfhqlzqyh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gnvysyzkv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gqwuijakn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gimnhrqdi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/glxljddsd.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gngggexhe.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gitnpfokt.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gkdtpcjeb.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gupvqwpfc.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gviszrzwm.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gnuxkdaja.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gdspsuehl.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ggixmglru.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gnwhnaysk.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/grvvpczkw.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gswzxwuhh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/guvnscpta.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/goepdnoeh.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gedikrsvn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gbufqxsit.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gyihuygcq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmrfibz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gidbuimop.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gwjeghatg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gpcwpzsgl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ggcojvwzh.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gjquqgemo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gyjsryvpf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gnrerhedo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gufiurnbo.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/grpovveze.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gnvvuguwf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gneyppkzy.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gkkjgsovc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/graemjloc.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gqktznbjv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gfxdonabk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gjvvjymlb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gtkttajxe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gagexoxey.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/goombvwvq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/grgyopddt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gulhbogzs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gpukwjhid.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gnskjxpjm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gqigpcehw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gilhuirdr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/grnsvudav.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gyvomspup.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gpyrhzelw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gitvjqeur.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/giefqsncm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gxczelthj.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/goinexwkj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gfrqbzcky.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gcoottcdv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gcpdsnynd.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gicanvbll.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/grhjpokwc.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gocicuygw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/ggvyrtzrz.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gmjjiofzu.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gsolxtmvx.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gjvycjawa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gwohvlsuo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gmxcxpfzr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gzzmujqap.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gniyhavuh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gbaomnnuk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/ggoyuxoux.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gfzoxxlks.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gqofesaar.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/glupyyclp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/govruiuuh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gxohhnbxm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gbmyfmjrr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gviomsunj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gtqpnwgen.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gskloczoq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gdlayilkv.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gidognaxi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gvcnwzdcr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gtutgmvmv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/grfxitpgm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gpxgduyqz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gqqufarbl.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gjmffeult.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gkaxcjnbl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gnmcnfchj.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/glzdylihg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gwcpyegni.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gaphwirbh.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gvggytvvx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gbacwzxng.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/grqetzxkt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gmlcrpcds.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gawrecbzg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/goolaijug.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gkmtizdwk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gatqfphkt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gbtxxuvho.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/geplebqbq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcxxslnrj.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gklhssiwk.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gvykeucuv.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gagxcucvl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/ghzffqxsv.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/ghlmbhesq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gnohuskbz.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gvbafyiia.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gxxijfork.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gsdrcnnjq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gbmbjfxrf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gypjtmwml.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gvymlhyvx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gtglydiho.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdudxeqjt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gjfrwafhm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guvvsxhxb.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gjbljruka.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gnjsxirze.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/galvoudyw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gxscufyew.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gvpnyghgn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/ggezivxen.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/ghvrtaiwo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gtomedffu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/giukqbwsd.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gmsszthpo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gdwpetutl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gkrbmppmm.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gokmdavcj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gctdithkj.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gvbdjbrqn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gukpjctex.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gxmvwdemz.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcseywxkz.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/ghrukcxxe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggqjflxhf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gjrhzaoxa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gjgqnktqa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gqnxfdyus.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gmijzectc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gjkilycpl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/glbctpjtk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/glildjmyx.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/giltvfncm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gkebodhpu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gszwxvcjp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/ggdjvirms.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gkusoqtdi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gkdfajyuq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gomjldarw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gyjedkpxc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gmymhbzla.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gwmpwkenz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gjlyjsvvk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gujnhgzon.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gcgabwbkb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gyjtkesbt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gfhkioexo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gakabwydj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gvobglsgw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gooqdraxe.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gcndiuxyt.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gfgbeqjid.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gxertrkax.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gjbwvojfw.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gvvybchmd.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gvtdrscsl.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjwafyriw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gokqwadqy.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gbvtzmdyb.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gprylwwar.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gnutmtyif.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzqzenvwe.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gpmudehpi.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gxnfezmqc.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwlmgkph.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/guaakhfqp.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/geuljinom.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gnsfffvos.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gnxyefvvf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxibmwuh.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gudfxdiip.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gqcgvwhjl.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gpcdfzkka.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gywwinoxk.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/giailhrdw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gwuoeephi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gyaizrkhu.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gqmeeqyod.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gdqhiohzn.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gzwfxunpm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gopucvcno.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gbaydcaad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/geqdchcnn.sHtML


<!-- 参考信息 -->