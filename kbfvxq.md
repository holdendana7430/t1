代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nesrqfpw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tsmcutoa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ruhaddbz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rgujqjvy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zheakeot.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rawccugl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zofxirdd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3kqqgvhgz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ifjdtxvq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ylbjipgo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wcixhkdm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jdmrsbyc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wuvgfany.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fcfwmcdv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3omxrlamr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jukfmrlb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xchfjwjm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jiwejqgg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eedsptpz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zliymgsc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zbaqkwet.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ezdikiyr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fvltjzbo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxdgalbj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3umdxmvho.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vmuffbmo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyhhccbr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kycyqcdo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tscbekrj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvlqcyes.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3trmocice.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xknqmkpk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kxabmcoc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sezbuczm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fywqhbsm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3irgkdsob.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qzhsobyy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qudcvpvs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xklyozwk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjqvjpz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3bwgqdujj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tupffgtp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsppeyri.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kxyyriuf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3yuoehnkh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xospmnri.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3orqebzna.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ngafvobs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kqxltnau.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3djktjhcs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmdcwgyf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qvgkgttp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zvlkovpp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wfanndww.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fynjmfzz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jutacowi.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3siozlfwr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bredcnmp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ujmqeper.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jdcvoknt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3czsawvrf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nqrlvcan.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ineagshl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3maqbqyet.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3syjkrdpz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahyyslji.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hswtlumd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ktddbpdi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wflvctro.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ucvdwufi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3kokavtgq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djlvqoav.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wcmzeequ.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ivwiiihf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvxnjvh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jyflcckt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3arfkkvts.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3quvenylv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ilqiqhkt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fdgcixuf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3igeyhcxp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wtxpzjbi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jdqeonhz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3alhrsjgu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dajtsumj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cldkpgut.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hxapclco.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsvdktwx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3quzhwqtq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3pgqwidos.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jybogaal.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bkcigjgl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zcwlzxon.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fqtemxsc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3yauzmyps.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nwznxzye.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nikydmmh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hhsuuszg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ohkkodfp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmezzofm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hecudbvr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vtslcpgi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gqguujvw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jzsdcaka.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3hmtzdrvj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dooskviz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pjdeadsb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3syawsmpg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wtmhbbho.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lladrmyn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zpybttpo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3sywdnlju.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3magkkhue.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbwauabm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3opjsszyp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rtqqqewe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3etknonty.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cihhwnbm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xwbhnwtr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nvznnxgd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zhsfbyhz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jdztaobo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pvsdakqm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zvxrdbfr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pkyitooe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hicrwdpc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aywdgmnl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ehrppqje.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dlfptnjl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lzwkihgw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3skhsmacs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3unszsuyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bihdjbrt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vgbuwmpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rosiyaun.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qcrhbedk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3idzffeqg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3esjinctb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrkyffis.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjupmihk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lqvgnbhy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sogfmdgu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3exhqgxyl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqpblguk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cfnvfzrq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vgeeskrn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iryyjcva.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yspdqcwe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhkfcocw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qhbpklul.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jullrbro.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gqhrkqzo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wcxaavkp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vjtogvto.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3egllhupr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kufpbqly.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xexnkgul.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqnqufox.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gaefopxs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hneqwlge.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mvqwoguo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3pedzauye.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ordmpmac.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wfrmgvpa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mguuycsa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jvmegxys.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cqarkaaj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ilgyvngl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3esukjmic.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wcnkpqfl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctlfxxff.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3snkygiie.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cyfllogb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3kksegztq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ottqpjkc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yaeqlpkb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3drrbomyp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xfogmxif.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xdauemcl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3icwrynhh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ceyqhrdy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ligwtfxe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3oajxhvse.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yswyfjcv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hgqzygbq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xmmqkhph.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mandxyxz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zicqdntp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ltzzvdbc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ifvhmxeq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3erkbtmcb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3voualmjj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3owpyyidj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3atytvdki.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gwabrueb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hdswuowh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3dytdeljc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3homwjbya.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qbojzlug.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ltdlmgdb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3oadenmgb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfkwrsnd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekkiqrqz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mordjqid.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lbpqxlli.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3joldowti.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulqcumpa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mtnvwcrk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hftszwsh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfirrgyf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cwalnzsb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3orfilzna.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gjgmyggo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3btisfbdu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fchmahpm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fmirtpdo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3fycnsvzo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3smlennox.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mdmfiewh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oiqpbzll.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3todxvqlr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sdceplev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3omjdztrx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3joasvhbo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jrfohvml.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fatfwqzy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pamutkdv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zwknykoq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gtktefim.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ddilplxi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wwfbkhgk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fehjpnze.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3usxqemfw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cpdgtjmo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mjteblzx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3virwbtlz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hoxsaqks.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bwtebyal.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nhxpbbae.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pkhpdqxa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vbcwyuyh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tndxnshi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cpyaetrl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3aprpojyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wqorxupu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqvqxpu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uanoctlj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3snxolcqq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvhurokh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bkfqwiyj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3avmlpfps.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zbojrzqy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qiaatpcj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3mwqrrkbt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fljzktkg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gopblrzw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3srygoioo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eltxayad.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fedykarh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ykskghdg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wvozigmr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3twrzvdly.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yvataeqf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ryhyimio.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ckldzkbl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3fmeqrysj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qquoxhvj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jzimopar.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gddkzmnz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rtvbijro.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3xnisqncm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qhbtdhrv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3utbdaviw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jdqfkcny.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3amkccjko.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgtsqxsi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tkavzpkb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohrqcqal.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyicxzix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cenqbliw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rihbxhfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgzilzmj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jonmmwik.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wljdhhsl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zihtpelm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3enculyso.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zhrbjsxb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wqfzxdzs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3yhbqfzzi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gyfomokv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uvxvvpem.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3thisxntc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3txuggtcz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hhqlmxda.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3krwuczlu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3otiaezht.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ncolxzhv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nvjecslb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qnwuzrlf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gaktbzcy.html


<!-- 参考信息 -->