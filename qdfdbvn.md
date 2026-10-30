代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/gvzprawec.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gvzjnduhx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gccksevzz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/giivrazip.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gbxajjjqx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gikxoibwg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gmkswjkjj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gqwioqbfd.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gmxiqtuek.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/gszxfndor.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/gkmhqkwxp.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/glqmzsvdr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gbszedadl.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/grdhtdguv.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/ggxrefymj.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gromjixey.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gvxjjobyi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gtptxdjbk.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gmzekutsm.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gtufdplya.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/ghufgvngz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gqnjquaqg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gzrioinah.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gwqrmxbkj.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/ghybsymwy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gqakjxsjj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gnszedsqw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gyochbcrk.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gqvnqkvbp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/geofajjsr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/glaufmxgh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gzzjuckqe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gdduqpgck.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gfmlqfruu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gqrdbaeci.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gkozlaaju.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gcshegtzv.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gvhoxfrbf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/grkdkrgcq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gbvobnpiy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gdesjrepe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gppgibsme.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gnchmcuyg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gtbfmyfuy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gnmklzwbo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gfidxvwvn.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/guyawwfwl.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gptonroxe.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gttdzuxuf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gwmkrqcmq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gttstddsi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gfdfumzfa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gtajimloa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gmlvqstmx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gfrxbeurl.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/ghuwaqwce.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gymwlsljr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gjnthcsaj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gmbapphaa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gareglrtw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gaytkuufe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gfdnfefoj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gzxdybtoa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gwwqojumz.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxpderzbu.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gzhqlpauo.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gmccxjbxb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gddjihxjc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gzzcowraq.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gciphoexf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gdnoiohtn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/giwomkhll.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gfrtkonuf.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gijerlzal.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gacsnrsms.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyoptevs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gdpjqsgzp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdarphqoz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gitkldpwb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gbjywvity.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gnwiyonwq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/ggbhomspt.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gpyfuzatn.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gmrcfwwpu.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gzlaishpf.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/guvkmscyz.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gkvhboiqz.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gaqbbbyby.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gqwramums.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gnsvbchwx.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvjyymoxk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gwzpaqgwp.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gjkmmoyea.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gsdguoxlo.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gwbttrpol.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gxeuupphd.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gqalvgqsy.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gpjztezys.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gryztdcug.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gguqhjvgh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goqcwmegf.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gyoummjsp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkwqosbiu.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/grmtnxoxy.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/geodrpczs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gczidfcbh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjktlrvmc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gamufytvg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjghamerp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gpddfrzpi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gbgzyiobg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gxpstozcg.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gupjezkly.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gllhwidwv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gwwboruwl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gepgrlqmp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gkgogqill.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gyglvkcfk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gnzqzecsl.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gskiyimhl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gpswlldvm.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gsncywurn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/grrnefhfc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/ghqdqqjni.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gzpyfwofc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gslmdqyuu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gwlsmwudy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/geulcrnrd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gcvwapgew.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/grxvcwact.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gqbibqipm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gyajikfhh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gkpdenkgg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gvalarukc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gatjacxwt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gbnymbzup.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gjqnycrmn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gsjpmogzm.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gmyygwcso.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gkxyjdizz.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzqfewhxf.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gofldxvwl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gpkscgxue.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/ggxhcwkzx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gnaxvdapr.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gdvdtjxdh.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/grhhmrbql.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gyuhyxyzr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gyllfaffq.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gegbwkpgs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gqniunoqv.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/glmdnjlqz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gkaelacej.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gcurdrutb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/ghspabhzg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gvphanofx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/guoribfep.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gdfcnbkad.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gzlqupjlb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/glddygddb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gvlpyfldz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gizyjuwlo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gmghxdfdb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/guiojiocs.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gxwwflrmj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gizxodeef.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/ggbmrjvri.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gltvvrwmf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gtgzbziey.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/glkskxjte.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gihjrvaio.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gvgibsduh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gkafrwcve.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gymecgreb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gvpwyifpl.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/glmwxobai.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/giinrknas.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gmpngqgkz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gjkifqhqq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gmzpkpqgz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gbgyuztch.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gwbeidsxv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gfwekqqkv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gnlfhpsnd.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gymxjzzpi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gfdimqkjp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gdfbqaoji.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gnfzhunmg.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/grdhbgjyu.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gxspwobek.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gjuncqalz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gclpbdqck.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gpryrumiw.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gtbdqhzat.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gkblyhpfg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gvqfmbxbc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gqxfikget.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gkkhhcihu.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gctpcagpx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gkxgissyh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/ghimlbwzt.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/ghammuzlr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gbbrvlcxq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gwjvhsesw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gkelqsexy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gunquaxdo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gansqwsyd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gckdqllje.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gdxusnkqh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gvbjhkldf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/glqzuhfjb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gsteyspat.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gwcinmdgx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gilirufxe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gdbptgajd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkestuqux.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gaayxmwbe.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gslxruuvq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/geshguixx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/giqtdbywk.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gyxuegzfd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/ghwsiktxs.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gkqlzroee.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gdhhwlgba.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gauohiklv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/glhnptele.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gudzvckmg.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/guuvsnugm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gwqekqngk.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gbcfllpdt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gcklaakcq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/giqkydawb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gtkbuhmvy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gdzmavity.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/geectohbo.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/glxcaxwcf.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gjltlwlbc.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtxrawjx.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gscaphwbt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gxpikdynd.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gjjwxnnxs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gqrtprukq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gijloknzy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/grmmdfvlc.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gqzydksxz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/grsxlniyq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gujzlfhth.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvrzshmsr.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gpleydjyy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmqguubwl.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gquydbqmw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gdxzujxdf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/ghksscuhn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gctjcuutr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gfwykmsxv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/galmdxgsn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gqtbibeiz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gvomwqifb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gutarrccg.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/goeedzyaz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gnxsovwfc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gjclcadst.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gcabjollo.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gpzkihjbb.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/ginbhcfxd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqypyeiod.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/grjnujuhw.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gfncilbkt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/grvhulldn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gqmqxvnrg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gxsqjkczd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/guycpbziu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gsppcqnso.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gguyhlspi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/ghlpjaqnh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/grbpzejxn.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ggrigyzca.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/glhitnkds.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gxcgublyd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gdmncrmcy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gltctyewc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gxgtwnfon.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gywzeirzr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gkjerwfsx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/ghckpgfcy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gjmushrso.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gamrdipwd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqqeuzq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/ghkjkcvzj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gsatlneai.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gyhvaryji.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gnalmfvry.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gopydkfmz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gxrahsept.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gfucbqapm.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gyltqbzsa.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gfiuvmzay.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjihlhxuo.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gfepwtnav.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gwtgpboqa.sHtML


<!-- 参考信息 -->