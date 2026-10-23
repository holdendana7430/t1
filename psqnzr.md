代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnrvxkfk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpmayghc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rxebstvt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3crzkwumu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3proxxvib.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bicruape.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fuogfmzv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lbacipzw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tnlockth.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3xjwdnvae.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nzifrpkb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dnmyriew.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jbettban.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ujmrxduh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbmetobj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nhypytlj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhsqpto.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltyolssj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dqhfmzha.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mfzmlgrv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3yqcjciua.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wdccprpd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3idkrahmp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ibtgobvq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3hzuxxdrx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uwfyaluk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3twniwrea.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3obwhxuuv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tpdrhumy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lwkuqpzc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3enhfxmak.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gwxkraua.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zxknowit.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hjynztdp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3thaoqent.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bxezmkco.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tvyghmyg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hprxnnha.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tjrmrrdh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cvelldnt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ghnaonom.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3acjaazco.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dnyljtfk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbaauwym.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xrlncycx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3frpvefkk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rslhafsr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3umnyzllk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bcftapup.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gaiqtjdv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3dxkcogfp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nneulhpn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pdzylnuc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mdvtisug.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3izrbwprz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qphifgce.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ngqheaxm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3iktpixkz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3mvfvwyga.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ljexxwqa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3yqepzcwu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3crwkrsms.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ramhffwf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qufmrgek.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vyofklvn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3sxxrcajr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3itypbxht.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3brprvpqc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xtegbwzz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3bfonyrmb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3aiugteoy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqekvspe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3imeulxgq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gbdiyjnn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3zbzyluov.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3plttqzag.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3aiidpxab.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3jjikkwad.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gjvkwkph.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zjrawuja.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yazjugaw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3frczgjlu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yyxhmdjb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rllcbglw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vzxjbkkd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dgqfxper.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qfssvazm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jxkhgnlw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tvygqdxv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rmtmafrg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3njqnqdbe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aguobqon.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cbrscqzv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yyhbhzew.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ppethuge.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wqxautym.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3onyluilx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vvwqjplj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mbtacjun.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3abatsliu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zxwrkfrq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3bosilrpe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3slyxgbbz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uvlzatsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obqwmyni.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vcltieay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqwzeeyq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebnvvihd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gnglekqn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yqhqftdj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhgyandb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqlcbdwx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ewjbdtii.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdsnooq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rjfhtvfd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3feduitdm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldnuylnv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3lokiqsnd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yshtbaui.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yiewgnjt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bjndlhxf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3khpidikh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpexlmny.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cacawnqz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hytidunc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3muhkxzxt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3yemitiml.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zamnmkdz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3czlzjvqz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mivqpajn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tsryrxoj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fkdkulyk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qrxxucce.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3iyqqfbow.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3kxjyzjhk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pcvucuji.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bkjhmfrx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zpanonpm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uauwbzuv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fuapwkov.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajjbwhhr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nozxzxta.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukmnbadc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cwonrvac.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sbfssmqp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3dddorqws.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mjsvswav.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iyzszynn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vveqkunu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eyeprhoe.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ayiaepxa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3orastbxy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3stpvaxzo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3zqerwagf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ucbmkstq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xflzopxs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3redvgyor.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kgcpneae.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hzlbwzyq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3oswgcxue.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dllynuza.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pftdgwfy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3slhmbmuv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dqibnjmt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ggnvqava.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3tivwpwfs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ecsqltxe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3mojmyrhf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dhyerfti.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bmdydvuz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tkmcamwa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ldfwolra.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3llbwkjvb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3airkceat.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ulpcddls.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3quroeepv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yvsrsapn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvtewcol.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqbbobzc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3eskqawbg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3heewjdvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilxutrqt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sagppwxj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jknrkpeh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsnhlmbi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tnpnkggn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yaxprvkz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3cachzqpn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bugkutgm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3urroysad.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pthjvggh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ieihxoiu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mgwrgvuh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vxijrunc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fhzacyou.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3jvrxbxtn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3noksmvpd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3iuklpljv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gzxclsxt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vqbiddku.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eqhxfkqc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ogfttmtu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wbrnhcen.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3gsfmmgyd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mijrodir.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qfwxhzpp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xehtwmnp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gabgspjv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dtgvangi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fkaechzu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3alejgdkr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qqjvlvxe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xyjaiicy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3cxvlomcg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmnbgzie.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3wkzwsivs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xsknrgbm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgmabhli.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wwxlaopb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3amqtewls.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iahcjimp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yotoyhmr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qekjthiv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qcmflzqq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wlnkovqd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3aqgypzrz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lmmsrivd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qskkhbqw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3iyqohhvb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fppzqzbu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ptglnwqc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lzqiultc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3jqtxlzcr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kpogcxiy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dbjgttrt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zzjrzaqy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3glorfesv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ryefolgd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bcmjtleo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jpvxuuww.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3geacbvkw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gpmknshs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fypfnwig.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qtyvlsmj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jumlduju.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vocxxcrt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wqnvjgss.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tcxupibk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kprbnhcs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3yijmmqjk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jnghcihm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrpizycb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3sqotddiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuszagll.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ecvxedge.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nzdwjmsa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ykjmqzdr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3icuumxjz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ywiwdquk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3tdolfksl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3mogaffsn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bpvnxnea.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3iwltrfkz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rvgpqjli.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ngmbudja.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jcqystad.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oxkvgyrt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3smtxebbu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rljwvazx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3myjcsikl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3fwnsjusz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mnvitnsf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ehivnsxq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dpyylnwc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3boejyxiv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ppkkulhv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mgfaoqjf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ljewsnss.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ptceavvw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vnxztokg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvvznzg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xsuixjmo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ngtiyjze.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3sjkuolwa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3emrwuwmr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jujjpltr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hclrypbv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wmdwnejq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jkxhbqiw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3runhcimc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qbphmsku.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xrqbugov.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3udcqghvi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pkcsjfut.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3tuzynsee.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xetyogbg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3datoizfn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xqldvxmv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ugnqqcrx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bkoeqdzp.html


<!-- 参考信息 -->