代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lzxrbuog.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3antyipzo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fqtomsac.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uolngyyn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3luxzjmfj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wegwoizn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3poefjhpd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cyzlhnza.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mgyydclh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3dsailnqc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wntflxwm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zfuxtend.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdgtnezh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbcnjbar.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3oolytjqx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ntpkfhuy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dtyishcq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3eeltuawh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wozhdxtp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxcejqmj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3udezhmgk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwfgngpb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ondfqzpm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gxekuugi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kkdivbzz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yrmkvizi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3sdceavbz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jcmruzeb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dmupnsec.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjukurbc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3decdffjt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nsapztuu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3sdrnrumm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zofkmgfk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3epcniuuq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ytylijuo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mikjwzyo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sxafyyul.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rigdtxuy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nmamhexw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ewedaogt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rqfinmnd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qzamajbh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zoqkazye.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yfxetpfg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hdcgpkso.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ezhbtjzc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3msqfqcgc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwbudavk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxtoaine.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pgfggall.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wcabpdkq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnuwnybf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vynsubnr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3avhchlhz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zuofqnop.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cbaajvea.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3czncxdba.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nfwlajes.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3eaereaqy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vscuycum.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gdlxyeqp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3jkjavxpa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3vcrlmuzo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hxudrwys.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rktusqgv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kbmqowmn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mrjdcnzj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fliprbnx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qfiuoavm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tlspnhxg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kngsuwcj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3esywcrcn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sxqhvoyy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mwhrqvnp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xxtxlotx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eicdrqva.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3khqcmone.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wrspfuqw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vurxhezr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xzanvrih.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fucymqnt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3jrysoyfj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgrkjkal.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjoolrad.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kyqypaef.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vadhwrhh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3sxfhsutt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3elrkrsqm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lpauqznq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ylneowhj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ticrhgbx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iogeelkg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxlsidnu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wrbghnhx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3cdhjmarh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vlfpjvsu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fushiqyw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3atvdneqf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uhpvznvu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pofslqpk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pmdhygll.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zrkicdic.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kjmopqwy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ytgqoxbd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zpizogyk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3farnwytg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3poynaxdt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wldsgafl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3epnskosq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3klievuwi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hhbrgpqa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zvlbdxbv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gzhvkuea.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bpijfyyo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aqynjkdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svchjvjm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3carbioiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhzjqjrc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dnwfspop.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3rnuwcrsc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3emyojzyw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mhjsyuxx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qazlnucm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuetjggk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3imafxyzu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3uttjzlml.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmdwzfao.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lzlekqba.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bkfbbrec.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3uttemmau.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3advxypxn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3chixjltz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fotujvoi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3isllrjrr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cszkpobu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aafdzavd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3epvdzjfh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjlgjln.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ignaluvo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbwikkps.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgvkkbxg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3uhdqexrx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ncsizubs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3yyomfvcc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ycubcmab.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uuxsztqi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjzezkp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3dzochfra.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqcpuzft.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dwgkwtfv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vnsqrqtk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3yhjpuabo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3taozcdtr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ohzwdiwr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dxelijoy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dmeyqorj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gcpgsrog.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zcdaavgi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3aienasgv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jlvyvdxw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dlbisiyu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mrrviilj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3lcsxeuln.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ryeppgie.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3azizzfxt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fudyfqub.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wvqmnmwk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fvsazzit.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kzyywvob.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mlexvgea.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rtkugryg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rrtdcymy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zwlvbvek.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cphktbjf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3unlffkxn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3oaupbdnd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3awvmnach.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3edmkikzt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tdgfpour.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lmzlgvkx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3nwmphqxy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3apxxyyap.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3uqujptxb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3awfcifav.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3euhivons.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyovcxxk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gympvnbv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3eilcuhfz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ojnfvtyo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiuzwafv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nultzxyx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bznxldju.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrlevymh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3byuoujel.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dhhlqopd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkbuqdvg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dejxqyba.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qsikfntq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3eqwcvunf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3izadqnup.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3bahigesx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3twdahkut.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kcmlayfg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3pmsqiwco.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3csrbeida.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gdxakvqb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3llfhytnw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mwnhjwdz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3apkfyotz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xgdpwmca.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ogjsauub.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nckgocrk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3fpoilhmu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fezfvbqa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dwgvyyww.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ljvdyjye.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3iorimtjq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vmqgcqfi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3apotbqux.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3czvscxbh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3keadxdqg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cvjboorl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vwtyybdc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rvhspzqf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qpllnxlz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ovankrqn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3atjvgnsr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wcnmmjhv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3laiiuesv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lqpvlcmu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dksvqjvv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3blhlpmmy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3sxkzngnd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wduhijgs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cijvjzky.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dsdwnuiz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gkqtekdz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gpwvgzcd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ywbqxwva.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jfvmxmep.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gwvgehwp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3btmmgars.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tcesovyy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3prmxtphu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hiawrgid.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fkvhpufz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xhourbsj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbcmaxde.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twypybnz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dbuyseql.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wzcuzmtc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3dfvlauyk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3msjfizmk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rinaayyi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mrpfgzln.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3adbsivke.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3rmwybuck.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ticvvbao.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szmibsak.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3iwvvcfji.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3upefbehw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocynqwck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyjmwuzk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rajosciq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvyzctza.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dosywyjx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ujwyszvx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qbstqysg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gdkdttud.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3gydrgujq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3llktikwl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xriqfheh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3admggdgv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jfnhueeg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3gejtrgcl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ndafyqjf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zyixcpdf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfmydwgh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mnvjqskr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ykjvfydz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oxketeqq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtttpxw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cutgtgcj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kwtmusfq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lkempdyr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yisvhppn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3btpbtjqh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eaogjjat.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mmjibwje.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zitldeai.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3rggtvgnj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cctmmhsz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nltfezty.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vumwavpn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zddnfgda.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nyoeabtz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yxybjgyb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jjqpsmpu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wfkclzvn.html


<!-- 参考信息 -->