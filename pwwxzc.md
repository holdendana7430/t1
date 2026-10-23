代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qqwfxwza.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dhhgwoge.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tqwhtjvn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3oalbxsvb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3svtgrxer.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iflpmunf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbszyxny.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kagtlvrk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3azemnniu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fsdrvljz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ibokbsaj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lrbwcsws.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qzvynarh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghevvonj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vhwpgtkb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ysejpeon.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gvwzvujt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ukhifkyc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hjvehzsa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lwiaawmp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3exyiwtlr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cmvrfakv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zheazalb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hlmiwsoi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qxqigany.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3iizmvyau.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fmmycnwv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3sdemiyhp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gvsxgbrg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ekcvcifs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3koduavuu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xtonqvry.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yfdfubuw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nfmrhxbb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eavqpzcq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3foreqvhy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3iljmougi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3opksujkk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3tbsyfqpg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzjhrvam.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zsxjyhgc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gijirxyc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrwoobwf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3awnqmmmt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nbxfaaqa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3dntunqrb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3regafffg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mfwhkohm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3atkrttbd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gegcilwa.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3afwxbocl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fwblmlsq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ljvqgmbe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dhybgshi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ypjoxlyn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iifoknbq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fgcfepra.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bgznizdh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nepeydib.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3swumwrba.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yktmkgre.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zclndxwq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cnkkjnxz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rxabeopr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bainsvqg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3astpgqpf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ojafkeuo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oaworkww.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jxvdyipg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sejogqcl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnmttcdj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pzclyeof.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3nluweikm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3npllxqtn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yltmpasj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fpkvzurb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wwfwdbuh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bjwnmwov.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dkaagavw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3cegojeni.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3anilbsme.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pbpwizvu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uujgkpwf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3sdapriuz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mlmtgssi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3gesfeiwl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rlznziyd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wntqldfk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fhmurlaq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3zlfemogo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ltiebjpd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3prbtpzjy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nhofqrir.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ttaplbzb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bjsktssd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pjlxebrr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wcfukldm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vhthuxyp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hisebazm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3awiiueog.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ymlytshl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ysznmypn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lkfjaxwh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjxrgwi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njwljgfq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qvejjrjl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhklzujq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3eiytfacb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yddsvpaw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yfwjwsru.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gnxjkmth.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tnxrtgqq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uimxghgf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dunuxjqw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lhihlelg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gmlktmod.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yqajpsin.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ghpdqnfn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tnclvlog.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lxthvxxm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3joaqmsdi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugmjwqsr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wzkpmjgh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gctrxqoj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ebmvcclf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ocnoilca.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3weisfhup.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3smvjxocs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucjhrbuq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mnmgrosb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvipyrag.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjbjnnba.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ygssjpsx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3azwoacey.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3asiixgix.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3brilmruh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmqwbhqr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bdignxag.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3aumjdzzx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bzwegyaa.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cgtsqwuc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ibcsomqw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jzyqtirj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsszrxto.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjexzoyk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dpepypnl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wbhmysqp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hlbfbulo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3tsqckftm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wzavgpeb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dmgljajs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbslnxnv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3undwbtkl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wqwehpbk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntlzorqd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uewtmmji.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hapypeld.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tozvkmrj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3djzelnot.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3lugbcrws.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3onbrpolm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3octcysqw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gjqdwbfo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3efeqazhs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvoesjfn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tksodtqo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ujwkdknp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3waxubnau.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3agkvtsxt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pqishpwp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wnzjjjke.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ayyntkrk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dflyroqs.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lkxseksm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hehhtutf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3niukyuyl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aebdgrkq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3tefwztvh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3quzjrrck.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bizywbuo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3erzmywmx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ueocfbec.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qkppdxup.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjmykg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eflzxbcy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lrbvtcwj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjjkuoq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zryemyos.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fdlvkxox.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3uzqhdqzc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kimqxdkr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ujuivmfz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3fvumjssd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uxuodegh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ppmcwozh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mdcbdzoi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3owaefrhu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxidcgu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ylnxrmbh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rrrcwzcd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wdhekqlo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ifkwvhmi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3peznjtvj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3scvxzxsl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wykbrylq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3izdvylgn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vzylqvof.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3onhqsqzc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bgofprxg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3cjbrgrod.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zcwdivkh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bvrqhgxb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3iivhqygw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3nrhdphgv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3aviympuc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gngddbmh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vppmdgkq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ccvxfhcv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3czsholrx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cztyfgew.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wkszmdfa.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fskvpglu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lsngbwcg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3roxxvqpa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lvchekhi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3sgzfvjrx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bogxmviv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jjewpadn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ztxyobhr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3btmiyfdn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3kiztrwwa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pbvgmfmz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wtrwgosp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3obanrhhj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3eiikxyjp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tskxpoda.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3maqvuhcq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ewtyrkxr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bxjpbfdb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tptfivtb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lvcploru.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jlaaxgnj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3lqkxjxxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiryvvnl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3krugvrar.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vfvgkksb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3bnnwkcpb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3tginrjmp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ssbrlpog.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zdnlqrfb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oqhlkagx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3klamqqgm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3joylsgvd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynbaoxeu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rbbcjeuw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lgpkrffg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ncnsobna.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3mcdvatqq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ftzkpass.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3umthmsgn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gdrhluau.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3femmqgsn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sbtbeedh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pqdqhoyu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3uyvdhwmd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3gfhtzkrx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3awbfdwqb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3fknckacz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ftnqootj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3sqcxkwbn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3sdxhmiih.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glfgvkzw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3nhlqoypa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3orsympdu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdstvlvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxyojrih.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zsfdxify.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dyamfivj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rofkcnwn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3aazyrwnq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3axauwsfh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tgprhokj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jcqzhinf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dxdfkdpr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tnmdawgx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qfxxfans.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gqkbguon.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rktcqfbw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3tmcewpcx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3glipvgnj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uerfgjwf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ipvmrdhi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bkpwymnf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wagfyfgp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3spgeckrt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qbujwkqq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zxrmntrq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bnyhnzeb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hmrajijx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kklhzvqi.html


<!-- 参考信息 -->