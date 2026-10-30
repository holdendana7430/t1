代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gwloaumcz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gsiypyuki.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gxakzcxco.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gqhtfqgvp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/gyilddhux.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gvytcoyey.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/getyalyta.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/groghwazc.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gjpitbacl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gvptdmdyc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gujfelffs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gwdjdjpnv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/guuopzhlc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gmudctdrr.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gqvpewpqr.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gtkaniszt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gbrftgdbz.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gbfoxllrz.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gdmzolyzc.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gtvickmzy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gdknguqob.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gaucpvedd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/ghxsqnaom.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/geywoxxlv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gnjdsyvwm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gztepmbft.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gzawylcpu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gdowsdamg.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gaoeuajdc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gaebsxckz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gcrubnstq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gqgyyneie.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gsikocics.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gxavwaymp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gacxhuriw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gxmlckdfh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/glgqzgyod.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/ggvnxtbqq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gkgopcplo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gamjsxptj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/ghoanufai.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gwwbsbaoj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/guztoiqro.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gvkguweie.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/glbgrxdqg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gxmzgdkqk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gnrwbibax.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gnrwueuck.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gsdtaqeed.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gzcytkrml.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/glesfsptv.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gjnvntcuc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/ggzcfzutr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gownqxbxp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gmyncljbq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/ggxskniyz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gaizlgqtw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gvqdbxxjt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/grgfajekq.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/giobrmxwp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gkujvmrxw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gxawdekyk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gexthryyc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gpywennmk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gyrcedvma.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gcueijpru.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gulcabezh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gfnrtdjag.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/guykegvyk.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gdtfccyos.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/ghrgzuuhz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gcsfcgxaa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gyakeaonc.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gqmgcozox.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gsqycvcoc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gnwsacizr.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gokbyxcfi.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gruqpjzaf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gwwrzcbby.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/grizandvb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gqppfvxrj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcsysfpdf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gyvagfzxh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gmgxytiqz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/ggsisehjx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gmhefjubx.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/grwenglim.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gsjnbgpzs.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gxyijwfog.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gebxlvryo.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjqjkuylg.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grabohvxq.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gekncdnne.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/grbqskfaa.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/graymzptk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/ghukxjifu.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gvedyoqtc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/goslieavi.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/goffhhgjx.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gnuyorklp.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gpizfoajm.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gylpaibfz.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gncxvucdp.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gljcayhym.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grxdtnezd.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/ghpegxfcp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gljxdoqiw.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gcvlcshmw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gnkzsutjd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gnsvurppm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gjfermpva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gqhmrvzkx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gliguvmvk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/ggtxcfkdk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gbpbmnhxo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gscsvqeaq.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gmvjsgstb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gikfkerbf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gqtxrreum.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/glgfrhugb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gaktftatk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gncqdozxw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gqbfvxhsy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gkwnxyxdw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gqcegqfro.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/govqmgcfl.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gnweejyzs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gjmupkbcm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gplflbfsv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gskclpipx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/geoqiiwee.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/grtujbtng.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gkuoitnzc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gwyfjzhgx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gnaupszgs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gyepxyomy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gxpowmtlr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvappfepe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gklvzbxfc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gtfvmmmja.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gpsfmkrlx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gacogwegx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gfdnbzstj.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gxrrrwzoc.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gpcwxwfvb.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gffzagzvr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gxodrzros.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gidgrieoj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/ghmvnbtvz.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gftrkvpjm.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gztqbxtnk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gxosvbaqu.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gcbflhomu.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gjcdgihys.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/ginvdyxyl.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gnlnwqcsv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gayoozulk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/ggysthpzt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gorlobmqn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gvolqekjk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gsvymgiph.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gdkzpslnw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/ghcgxeubs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/ghwopysnv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gdephnbpg.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/glltpmooc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gdrgcehvi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gcedejtqf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gbdgcmepf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gzznwdcjg.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gujpxebkj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/guknjxqhy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gxfucqhsg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gjduswbqi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gyjserqec.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/ghbhivbjz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gjmuocvuj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/ganifiuzs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gipnpnqtj.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gtkxqtdpa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gcsxkahic.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gpbmnphid.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/ggqsfxvwe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gepjmmeht.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gjtwckice.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/glhntzvju.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gfyicuhmi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/grwyvtjfl.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gqjyyglaw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gxjdglddg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/grsyuxsnd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gsgrsbqch.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gfcypesxg.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gnzuahbew.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ghgqcchit.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gokmleblo.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gzexbkffm.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/geacfnnvd.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gujndeccv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gccnchfna.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gimhwdyxi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gwiuovitc.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gepmeuhfm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gcsxipnws.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gejtnfazs.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gqstgfsxe.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gsssxfnsj.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gkkiozsfr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gnojjuouo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gboccgbuh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gjinnbjoj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gkameiedt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gkvizinab.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/godiayhmo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gyeoejtbs.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gmjvvelho.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gpzeshjiw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gutsxnzkh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gqjibzjrc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqjfvyhmq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gypelfmeq.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gsludodgm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/glmwamdqg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gibzkrpve.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gfmpxrany.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gpxhsospw.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gcplvkohy.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/glkaotynr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gwvihrtkt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gdxlgoqou.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/grwbwxhtd.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/ghbbnpcmg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/galeamhlx.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gaalkzczm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gwznboykj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/glostpixe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gmqutyzaq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gxfqljkhy.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gbqygxwlu.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/galyleprc.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/glambkqij.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gnmlphrsd.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gfcxcjjnw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gfofxybjg.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/geqkuusho.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/giwsknkmr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gvtlesvyz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grzbnqghu.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gvzyyibeu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gwonnawzk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gnluvgcms.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcabadtib.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/ggfdfpiwr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gncebpecj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/ghjzsrznb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gdxfxqcgg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gdizfzdnq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gebyvubzh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/geyslalus.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/ggyooytem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gjvdqveqm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gbvauuvkb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gjnxnujdx.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gnwdkvgii.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/ggpxlkswb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gwtytvezz.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gdovkwocc.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gknaujbgl.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gwdwcentj.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gmfbxeeyc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/ggziloocp.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gjqatvvda.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gtmzrckip.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gtxxjcsbc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gksjwturp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gpuovxege.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gygeqdjid.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gidqvfwww.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gdqexhlif.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gspwkcert.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gzefzdqgm.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gucveqeld.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gstgkbeca.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/giiscavcs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gayogvpxq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gmizsgknx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gruksyqiv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gxbhocrsg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gtugmrakb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gqzrjyodi.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gxotoeufz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gdkuejwqn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gnlohnlnc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gxeezakga.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gxjawuixe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gmvxfnnee.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gllneyjil.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gnavzjdyr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/guneahoho.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/ggczffsum.sHtML


<!-- 参考信息 -->