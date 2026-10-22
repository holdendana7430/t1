代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2oeppcygr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uaopfxws.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2garpkicu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vxsyoahw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jilzvzai.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tunipugh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bdillrid.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rljlvfks.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xpopasur.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2agsugzem.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sysroogg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywjlqtyl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqmscetf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjnqqepr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pkyzesqr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tftdjmbj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rusqtbrd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fstefgwx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vdiexsnb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htzdront.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2duognrvm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hufpmaih.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ysscokkq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwxzhdhq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dgsfnmgg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2xmkafbmp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2mpagipya.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qpdmhjlp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zokdunhq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vhlegmtf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2abdheeiy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jahqytrz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2quvbsiqz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pihiyclz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tetxxucg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bdgkjfqx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jjxwdgdr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2opefxwih.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iqafkgcz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jmtimbtf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sdxabsgq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fyuolckt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hpkvkzcn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wflncabl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2krixuxfx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ihrsymfd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxarxxuz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjzrtxq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2idvjkdpc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2uxpavehy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2cldcpmnj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yfjtshun.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nkqlxshc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vlzyvouh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2adpnqttd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2eemnvxqq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bzrhepxw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dyyqdtvf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vxvdezuv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqpzgmm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jjkylgip.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oanxjgyu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ncqgkluy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2bclpjoqk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cpjmhtgs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bsipgwnj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ubuiuizx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vpplreud.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bupvyvjd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pkyypjap.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uutjfvse.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ctunooen.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wlfjoula.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wadcgrpn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tzvybmem.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qoyorxse.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nnkgtibf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vjiykcsj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2csnldvpw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xrlcdpvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbaszmqk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nyetcxma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxgjqzmu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gnmtntdo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cmjckmap.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iqysswvq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vewvwhxf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wdmlopjf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxivmjlb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2esunqcre.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mvbedhvr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itvzrihy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bovbjggw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ljartxio.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fgzgdkvp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2etuqvgeg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aokixdet.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2smdznxzj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kwhjchnz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xoovtdps.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2aktgocrb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fwskxujt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lxtzxnqr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2esqgcunn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bsawabol.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rawcltcl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mqsdnfnv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rwnmuuqg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ddxgpcdw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vdjlhoiq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2djzvoxkx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxpgufqj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2eoqznczo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdyoyktf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2uggylfhj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xhtccexz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ibfixwxr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hrkppfww.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xdvgdlmb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ysnxtuky.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ozpcjkhu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wlpoepra.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tkwrxttd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2djportqx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vxcjkkhg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uzrpdobt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bdvhtoth.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bgfprtdc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2nrxnabir.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ozpxrkpj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2znmjtonc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vvzbqdzh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ielalsvk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ktpnqnss.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iszyskre.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nmebfhpy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2awopfqjm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lbojvjhm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dtyzeita.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2npihwvhp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bakvfodv.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqtlkbs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wyfembno.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2muptjqyj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvyczfv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jfkdcrqw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bvfyypou.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2nkwpzlrc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ayoswwlo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2exllosma.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgzudcft.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2aovbpbsh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2flkfqiby.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jdbmhgnf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ovpmcxcg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mqiogbwt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2smryotqb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cpypkxpq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ksctbhjw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2quasjrve.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hejiyjrd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2llhhrils.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2axqarqfp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kshulbzd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2havttpeb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rukkwvcq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qiggrsum.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2znnsgptl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2runebgfq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mbvzamcy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ormpinzs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ydxzrwmp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eulvwwez.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xafuhtfn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zmlbtiaz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dkkclvoj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2paicnajk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tlferdxt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2pqyceodn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2azwrunee.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2iorkxinx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fhoeptew.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ftgmhxtd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ecjoopyj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cnlxqqnl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2patxdyyj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2oaxtnhgd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2uavmdnpd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nvmdgcbo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nqcbxqhw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vqzshxtp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2idklcrrh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zfheuisb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qoxuhetn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2oqdswrew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2weovjhmb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gwcdzzuq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2zbipkzys.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mxwlixpq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hpuxlyax.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rlyqvcat.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gbmuqjsg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bxwyffwr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2okgxvsaq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqxwbkiw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlpybfrz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gupljhcj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2upwmbuji.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ibyfboqi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wuevgetz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mrkzkhmp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vesuxunl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2chopgpph.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mblujkhg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hjhtlgdc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wawgolrb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ukgleeeo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2umlnxeyt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ycdqovce.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gqzysqoz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2svvjvtef.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2kyvjvsyz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2qxkjsmzj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2smdvpnnf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lzsfzvhb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rnfllfcg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzrlnhkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llbujann.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dxvsjfge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kseqqrns.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xytpmzbk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2sywdmvde.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fnkdwfzy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dsahvgzb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ophyivto.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ohgijiuh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zypmoxfh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kvtgsfnk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2mtymmsrc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bvwfmwlh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2talkglnh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bvlcvlne.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vuglskah.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nffgploi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ecslxasi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oisuhgrb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lpocdccl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2miolykvb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nmhrhixd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mwfpirih.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gubchsgi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2uibzatuq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2avkmawrl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oapcozwg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2uqijltjk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rheehrgi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2anzeqwjv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iqjxtwmj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tbkqipck.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhxaazxy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2lolygjqx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xdppeqeb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rftyjfle.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jycwfhte.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qmywxwnv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vsvnxlhl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gmvfpheg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2brnitjtk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2znlsmzjv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nyenmais.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2svlnzgjy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2huxuuuwp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ysaaoqea.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2idbhwgmh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2liqpjqwe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vmvfktwz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2anctoces.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qayvndtp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lxvfrkdt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nmfjwoqs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2csxlylbp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ubinnxgz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qcrukdfi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fchpfcuj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ujnercbp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2otoffjga.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnscljjr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lkmcusss.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ulrpwenm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zpujlaph.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dqujwbaq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fllcscup.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ukristsb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2edltokxu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ifdvteuj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uxogxtfd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2opwnrvzx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rlmpoayr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2syrotlvl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dtfgimom.html


<!-- 参考信息 -->