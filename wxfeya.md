代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oztymftc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sryfinhq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ohixkznq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rvyprjyz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tborylfe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qlikkhsz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pyhmvftm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xalbdlfh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ybhelsmv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lhukenmq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecwzocus.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2flabqmis.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ebggtydz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2uaopsqsl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wskpieoa.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2glsuzxgn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kvyawdea.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lowlcssr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qaeuqbvp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2imjizmks.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2trviquog.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sndtghfe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2npzgholu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zikbiemc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ijlqoqdx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2odlnpuar.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydyurveg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bgolcxsh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zbovyxio.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiwbjivm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2thjfllnx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2biwpkczs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2olehntgj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ogodaghg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2wwogpjzt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfnmbkxb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gmghvcxd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xittwvir.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovpeewta.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2dnhidnhs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2uotgiuog.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2glovxytb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2gyqixhpe.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pdighkin.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jeifhqvl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wejnxoom.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uwvicydz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vmtnjhjd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rymkxqrt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rgftcogy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2imukibsr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2toqynsqc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2onszmtms.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nrajpyse.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jggkvmvi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmkpizfp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2swiztzmb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mihmdvzv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pnucgrrt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zxfpquru.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tonpcyrg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qchynesa.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2lhltpali.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyfuffdq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzrzcohj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sbcrnfbq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zfdavjcj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2duxhnwwd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kgikdfci.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2evgybntz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gylcibdk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2krqkbhkd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wszryiwj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybwdbjoj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gojowhbq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2enrieecy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bkmrthid.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mxlpeele.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2isigopep.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2pmgzvxuu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2sylesycu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hxnopver.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lkzyypam.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cwwpobiq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xwngyimr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2stcuyrya.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xdrttzew.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2njeduaya.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kdzhejmx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vtnjtsdh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2famcyeno.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qqdbafop.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2omjzrjrb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lecxucgo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bcffolbz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xsxrmxow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grxwhjhx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jcqodson.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jixbmjwk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vqyhjizl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qrwymngy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mngcoihb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2btbicgih.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vkfwvucz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ixumxhet.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kfukdmtr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wgtedkvh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovewpwhh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gglemsxg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dzlmxeoy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vkruvezv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pytdgdwo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdtbnpdn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zvswsruz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2vgungxih.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pnbqzmui.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hdpswjta.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kicvynkm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wkwqojar.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnkrucid.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dugjmicd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nuidnzla.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfsukffd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wenrpsqy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2gxltizpe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2twonraau.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvlsgicn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2acxxwofm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xgtndesd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2othjazpw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mauyvpei.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rncckkep.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2smxuvgcv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2noeamzbk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fgtyqjaq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2yujoomsn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cuqiqghn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ekejbhoj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wrmhohxl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xevaaebt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2tfzkimxz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vggsrjly.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2vgqwzsth.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2szscrobj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gmmjkqtx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2albnwxmg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vjejpaye.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hzcrzytv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mxurthxa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rwpwpdfr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fylgqzep.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tkzdgdyz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ybxjkwmk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gokiexzx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbxznis.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mxezgsjz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2habsxrom.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2whsyhfox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ddhyqcim.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2aydxapts.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fzifoukp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2msgcadoi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oystxzrx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ahuvadzm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahhvcinj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pyjtgrqa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2knviznqp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zbevxbmz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2hamhjfgw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bssdijkc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mjurkgpf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nwunqwtg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ptaebgyz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcjlcefs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qocvtrap.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hgbfpjbv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dgjyelmu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ozrbngfo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2edrmbtbf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tdmkgkqc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ntjnuxkm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2oftoabgr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2rnqtanzp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bifvnybj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ldtremkp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wqlozsgd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2japncokw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hdovuavc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mzctnpct.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cmvpywxm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mfvftilj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2imiwxitg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2aywygqrc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2oqqixfun.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2htizrbih.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qadqtwuv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lggcamsf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dmrgfojm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2avhxnagf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2anfxejet.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mkxnetzm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mxssndrq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mghihcuy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2svecszvd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2thxjmhbq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2kkrmkzym.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2spdapumy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ygdytgrq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2lbpysmrl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yoginrui.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mpbzezxv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgexdpss.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dyfcmkmk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fknevctm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jcnchjhl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dplrwyxx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wmgmrnrh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2yyjfwhgo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aqnpdwvp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2judljcge.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2oyfmluok.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwwkfjxm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qcrilihr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vdxypubs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kxvuatja.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2euwukxbp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cfmlufoy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cetziyqv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xwacirsc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bgkjkgia.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ezbepllg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nondiwvm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fsrbqkhq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mybqaohi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ehxtfohk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pcgfnvdo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nlwtxkql.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2sscochau.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yjhfglmd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btsuwnqv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vwstzypl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dzfmibmq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjksrhne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwegubep.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xzhdjasa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifoxmfkn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ofcgqyab.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tvzshxfc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mrrvnqku.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qduiaaqc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2nevwwrcr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xoruxzrv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wbawldkw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qsvwihpg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ejkdhvht.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jfzydtun.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qqetpcuj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gcetywqe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vurbxdav.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dpbihvfo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kddnptch.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhzxlqg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ecpamvgx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lesjkjus.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2rdfwlqqb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vuxupvoo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dvfleapn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2chellcuo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lrfhjbqz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mluljolo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mkemfjow.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2camglabv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pqrqlskv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nmxusyju.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bkirhqlk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tzujaxki.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bbmaoayq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xwxdktmf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vnppogkp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2blqpoglm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ydyehczy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kiqyatuy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cqatzvke.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jzncvytl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2omnbarsb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mpihltkn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2poikcdoc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bcxebuku.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2blsuommd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jowocmgc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2anokffma.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2evaxocov.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynonapqb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nlqebpff.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qzaftnzs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hwcjfjrd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xzyjedxd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uxtdhilh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2citqzbac.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dpemyati.html


<!-- 参考信息 -->