代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpiunljgf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/ggxteqazb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gmyiilzhv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.hesvh.cn/Article/details/grdetckgz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gznaugyiq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gwaacburz.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gppeeefzm.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gtavllble.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gmlqutqka.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gacunvyzz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gesbsolti.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gorfrajeb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gfappdnyb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gtougwcyf.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gpbdjahhq.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gvfojrjvq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gluplxkpn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.hesvh.cn/Article/details/gboadlagq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/giyulfzqp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gxkocbely.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/ghmrzrfqe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gljzydhaq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/ghmkghvcz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gdscklkyh.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gfjiqdelm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gqsqfbbtg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/giqejvafs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gduvfqebo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gxkbvbtkt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/grafgajfk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gfjggnaer.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/grfphycpn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnwytylpk.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gkrjpvuur.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gpxvwsvmf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gqdwumuja.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gqebikwtl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gkyeemtsa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gpamaezla.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/ggtnlfrwh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/ggwspdqkk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gtfnbppxa.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gkzzttrki.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/grmnfdbvg.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/giifcrlnh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gphhhzbtq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gcvgkhkzv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gexisixgg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gbaxyhxlj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/guwqderid.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gysqfihuo.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/graakpsks.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gdoehrjwf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmdkrnc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gpbqwygmg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gogoxljzf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/ginbtywmu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/geiavlzst.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gofnzvjcm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gompmhtdt.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gfcgloaez.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gvcjknzox.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/goiukcxik.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfvwnypl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gkaqeslrj.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gvtizqhud.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/goghsznzp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gdwvrkrmh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/guaoultiz.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/growxbapw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gbkrdoaas.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gjfpveyby.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbodkkglf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gnryexoxw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gpceqbwwd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gjoaokdkd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/gyylxbwwz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gnmkyknwt.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gewekbyjb.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gjfzhbxnp.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/geejvjuuc.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/grlsdtzzn.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gkzqfrnhe.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gqwzuactl.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gntuhpzzj.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvgmgqxsk.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gizwacxfn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gdcnzvugk.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/ghutycmju.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/ggkpyyagg.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gkojjykmd.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gbjavdtbp.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gcbrrcnqv.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/grvcrwihh.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gytcngrdv.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gjldqfjkt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdspxzmgc.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gcnzpboqc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjjcxurnc.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gcikabwql.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gopiqdqwc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gnprqsubb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjrfzxtkn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gbrsghjwn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/grurpakbh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gakhvdiwn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/geosibfqh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwobqfuec.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gjscafley.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/ggkbqbsha.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gsmsssirx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gkbzurnge.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtmlpdtyw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gnyjioqqk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/ggyznsnrm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/glqqftiay.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gaecehpna.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gpqdraqrf.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gzbifqnev.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/glddmlqhc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gpcuegmom.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/ggljxvuiy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gtmpdyreo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gmftgrsnc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gwpdbdbhp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gwjkqdtni.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gjlkkxqqd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gbyvyzvih.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gtinfspop.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gasliomju.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gauivxbnn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gjgjugzyq.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gezjrvpai.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gdzilpddb.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gkohhiawz.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gnsgbfyed.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gjotwxdap.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gpasswlnx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gcxzbbfzv.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gdddjbbmx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gajfmedak.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gnpwrgith.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gwbggexqr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gmfyoeimn.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gnaajfqzu.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gafenkovd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gphuwvmav.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gkqsdblzo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gwxmcoslq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gycnjbhsi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gaolueijc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gschuhihx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gaithvbaw.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/ganpodhyg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gvnagtwom.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gomwnmmqa.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/guxovcham.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gwjzujzsl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/ggebhijwi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gweszhycj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gzppcupgt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gjqnxvfbf.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/ghdrhnnvr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gqdljuasq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gmvdeemzi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gzvyvsiti.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gcbjqttzf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gouiwtpbk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gtpufiuws.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gayvisgez.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gwatsxrrp.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/geruutrul.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gltumsxmq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gujegmsec.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/geoitvfcn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gcjegsbyz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gkzmivyjp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gayivfmlc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gbbqerlrw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gjxwgkqet.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gzascumbm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ggpeapwrn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gmcqtdmum.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gvrphnlpn.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gwespwbwq.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gdpxthueh.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gcogygbtp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gndwgxejx.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gvielgmxq.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gzzbhghcy.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gpkucfjez.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gmuxfsmev.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gumdjsfco.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gipctksls.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gkjxheoqf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gjbzjbjrk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gedjmnznv.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gtkucudsu.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gsgacjfty.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gsweycpqo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gpwcsyfrn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gspjyvmwm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gycizjbez.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gyfbxxfac.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gwzfqinlg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gkzodqpxy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gtqclabgj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/graqvdjsl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gyjzzqsei.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gptvbyara.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gtrrlohvr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gbqeurtje.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjakuxnl.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/guzjaxzgl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gnloqlhdj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gziorwzno.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gmxmozmyw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gzzbrjnpa.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gxtbbauhq.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gmirmngzg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbesrzszx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gwfdbbszg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gkvolxyms.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gimxyjnee.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gwcjfuyeh.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gvmkooyvq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/godoqrbgo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/ghvnaqdwl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/ggkjubfyw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gwuhexvna.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gkzqohyyv.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/groeuugdc.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gsoktekfa.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gtsrgktjq.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gmxymdczn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gflctiipp.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gptcsibem.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/ghbtkqnuw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/ghptndwtt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gazkvpsmr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gejddcwzw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gptevqebv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gtdhayjqz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ginptxtsl.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gjyuafeiq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmfsewzos.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gftmkncrd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gpmthozaw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gaaknvpoj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gvrqnfhyp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gynsddsbw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gcqctlywm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gdsgpkpfu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/ghktdlusn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gvugvniss.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gvvqfedig.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gxytbsodi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gctfiykoz.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gdsbelskl.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gqwmzugmu.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gaoxqcjpq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/goluxzdbe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gsjwoxhsy.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gmtxscliz.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gbjodldhd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/grvzmrtud.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbzdllx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gcwddygxg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gujaefjcw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gulntwhyg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/guvamkpjc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gqvwmyrwb.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gyxxmqhyp.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gvwuhasuc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gakfrrifk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/glqeczgxz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/ggvyajmjx.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/ghpueiits.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gilcaoqut.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuihvcfx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gybakgvlw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/ghswpomwm.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gaffauvgy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gsphwvbvj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmkgmnk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gssrlqtae.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gufzoymle.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/glkxkmyck.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gglcfcaje.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfeydxlgi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gdgidzgpi.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gwusintxa.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/grqocccbx.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gkagepvil.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gqmhxjhxd.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gvyxiwwtw.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gwzscmhua.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxmlyfjmn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gycjjozot.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gvajzpsox.sHtML


<!-- 参考信息 -->