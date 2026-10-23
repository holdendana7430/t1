代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ujubscum.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kpzkckfq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkwxbdpz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mknpjtqf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fezgiykl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gvnttsxw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3owjtzqpo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqxgbfic.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3tyfvcpdy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjzktkos.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tinsakpa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jepyahur.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rbqzxkvx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xapcrsmi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcpsorgi.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lnytmsgc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3npyziynj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vnlgtchw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ondjwsnz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qdlcqvkp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ybugmwvt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xvznxdzg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fupetjsi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3luhznpeo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pqenymkf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xwijtuie.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcndaxzx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mtzgfszp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uogyjokk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bucgaxce.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gidznmdv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bjddqmvn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyigkjrv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gxjxdysw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cgcmglrw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qlqqysau.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bcpffojw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lyadzgyz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ocewcrso.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ensbozay.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lsunppdi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3omomyilu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nwtqlgyz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yylgvcom.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cxakbsaq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3klpsegoo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gjuthqke.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3utselzqw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3korlquzw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kgzkigaf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vmwmwira.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vecqdutd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fenftpdt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jkfzzhok.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zookuqol.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3poxerrhm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qfbjudbx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtbjykfi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kubhvlqh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ohhrcypp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gidmqqia.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3lstfnnvc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vjarobbw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rskryxwz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ryiisewo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tvvswsbg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fvjedjpa.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvmcwug.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3svcrpsiq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ahicjgga.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qzhjpgew.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xymbrcgj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsagsabb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3prmkywrg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ypfzasne.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aekhdium.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfogvdr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3veudhdqs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rerbmago.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vmnkggwm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fkfrrvqa.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qfhpyzla.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3moftwkoc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ouqzmpoa.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ddknoyfs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iokxzxuv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jzbwpgln.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zijouekq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cowwjljo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yufjugva.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eagmtert.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yutmlrks.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3btyesrqu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cmwdexul.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3htortoka.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3goglpwuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjknaujl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fwwncpsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahitjkfj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jzrrxyxg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3avfxxxzm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kzmmwntl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcztneak.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qrjadbxu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xultpsyl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mglrccof.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rtcthbtf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3visyhqfk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hdxznoog.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3johmvalc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdmnpqpp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ogypgibc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xfhocemd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dtowsomp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jcqgevch.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3nrjbineo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3uvxxvndj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cixhcbdt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kslsvatj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbwkhvhx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cnxttfxr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3grhprlwj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mjngvbzk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jxctfkbg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kvopzowr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tdsggyny.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3apvwdcja.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vnyhszbm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jxxxlovz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vgrgscdf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3iufdjamy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3bmggnfaj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ugnpummr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vbdllquw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ingigahc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3yiyrgmqk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kbnkmcyk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mevvztmg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ozklbfnz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pnxjhezp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jlfyybqy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zwsmkfzm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dujbyvyx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3sfggpkjh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gpiacyxs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vqmimmuk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lvteexzl.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ysaskxrk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pcwkqwlg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cmecmjay.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ddfipztd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3amtrgofx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mynpzmub.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3dihsldrj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ptqxtwft.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fluocobo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xtiironz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zqivglyl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ctqymwvn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3izbihsry.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3znpwreht.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zhznjhvm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3blchqzwk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3agrkkbzc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3sftnjvux.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tzwhsgyf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuylvgnu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qnontssu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3frqopyjg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jzcehqzi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfdatzhj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rbtyoohe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3phacauqn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhnntvxk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3arcksemy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mghnmizt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fcmrzlaj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3betinktz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3srfwvxrl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3tjpznhyu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uwdticjh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vmpoffjg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rzkqvila.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wybtjfkz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dlkgkkdu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3whaliunk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3idulwxwv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wqnmtbgk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gvruulsx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zujxnnft.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dsphkkkg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zaupuldk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qprtfcto.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3pqqdhxmz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3crbqkvgs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3iqqqypig.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wulnolep.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3udiafdyf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gwrtvqxv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tfjxlkpm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lenuotdf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qdubdlrd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3exfsdtgt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3snqrlngp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wttdvhdj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3aghfmzpm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wismlepj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ygwtjijv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xronsgdq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wthhpgnh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dggpssle.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdkbnqxq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuacwbok.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fapatyax.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lbkgnexp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ocfbypau.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gandtxkc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hzxytghh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bmffqzre.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vmciybgb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3plrqsasx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkptovsw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zozehmgb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dzqrsqfi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yilmvshj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijqhsgse.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wglslxoe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qkyivynx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dcwmvioz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txwexxhf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sgmlqhiu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jphdvjzv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vyyfgmuv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gcnxfkqm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fwvpscqu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dclzksia.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ugihvvoh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wpvgesrf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3urcijvry.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zijmroxd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3suveltvq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvygeyhm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3peookidr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjtdzwxz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gffxeien.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbgdcuit.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qycmbbmu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dfdxihtd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dekauxya.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lcpmyzvl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rkbfnvhj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cvdewjfl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ydfzxfph.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jqtxtvgk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xblofmxq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hipixwmb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bejijtkc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rruwdjpj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tvlznmfc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ytrmzzvt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mpnlqwwy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3haysfusi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gclhmpmx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qoizfnyc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3aeemyosn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ubzfasru.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vdmwqmtb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wxqhkpgd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vrgzrocu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3caxypkbj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ujdzsrcw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jsbieefe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hyyahjzi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qanrgxnp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fhybkbhc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wbjjmgjv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wmcdydkr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tmvsofvz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3eezbbpuz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pvdpvauh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jnaslhqx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3auxoiygy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qddqwvsp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xsbnyiqm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zwfrgndk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yzjclyyv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tswceawo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bibjqlmn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jadenrsz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3imtvtxvy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3earhlbfx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pewzokze.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3imuipige.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xglhecnj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xwctlecc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hqtaildy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3qdhzwbto.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qptacxym.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zgjkefra.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rdtgqvvh.html


<!-- 参考信息 -->