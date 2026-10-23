代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lifvuucy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fajdsthf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wvygpnhc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yfavabdh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3lptgiqdc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3witikjvt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ghaqituq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dawvsqbk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mphnlypu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3esyrmzin.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jaipngba.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3arxwzskv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fxxukjvu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fnzwtboz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ugsxkcap.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uvayidov.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3nhwwsegt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjrvdlzf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tgtrnigl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pinzenkf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyzbwlah.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jwiuyejt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjzgqof.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgixdqjm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gexpomnn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3soxagpnp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwypyapt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3grizdmgg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuormnml.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rvtgnzek.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sygoevgu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3togfhuzl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fygbvhjx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gjoqsrvf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3uabxgkuz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pyjhfokh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vngjkhwr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpfpitcb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3orwzuuxv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bnskfgle.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ripvhtlc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wjsqebrv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3uwodxinp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3aaofvhkf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3larpleok.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lsurbqcl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnsngcfo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vyjewyid.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ceyhdqgh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pgksvtti.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tfrshdii.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kmxyntlj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zceasltz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wwscvtgj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cemdvzzd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qwhxzqja.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gimxzjfd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mntzcpwq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wadbyaka.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3diohzbcr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3cpvahnpx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ykeyiiku.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqadkzzd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3moqzlhmj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zahrvlxb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gwoburpn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ezysaojj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcxiphly.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtaoecc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3pwoxysia.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mljgxsdv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dzvxstii.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kyuqqqfz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mbnxhbey.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjubrxbc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kphtimed.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ebrvfuww.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zhgeifol.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3jgflvjyh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3tagjrhtj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yrlfyzog.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vaikixpn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yqiujnlo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwkaquzh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fjyrlhbb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ousuvtim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbweebk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zltalzqq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3oaydzqbf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xjgcvoop.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ahrfxrmt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ssytgjah.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ycmaqxvl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kxeljrpi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rqspkrlt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tvwmzjui.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kcntpgkk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3denugvij.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnxjxkp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbvjsrcl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rsinkhkn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wewphmqm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3gievptjb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwllrlb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xayxapjn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3awajoxyj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3oubtxvba.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hmmbemdh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tprgrwfa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyuemclu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfmjikis.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mikpqyou.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tuvfwizy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayznwchr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3amscxwef.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vqhzqcsr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cuavrdym.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xoulmxkh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3amgbpwil.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sgaktymr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mirzqdog.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3atzzygfq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uxtqhtfu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3kuiazgry.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tnapeqoc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3szpkpqgz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pevssfni.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qhszrhvc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bewffwxo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3txlkoyjz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mghqvhie.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kolavyav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfkdlnym.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fgnmdwuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqhxfiyz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cqvnqsss.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qkdjsxuv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mlkcrnyv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrzcpgwn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hkadnwll.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hqgxlqhg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xfyyjrff.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmannzjq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylysczmz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3uavwrvzk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zbhmyrda.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvvbrxo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qjbapopt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3inqkinuu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xwmsjrod.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3uylzptar.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yowsnuhq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ebtgljgc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zzzmgqrw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3diofqmyu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mbdiqldk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmlfdqeh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bdtjmhet.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3fofblclj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3kpktglnf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lxavwqcq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zwhpdcdk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bhequkne.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qszniqpm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kcagndcw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xddxfscx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fwdfpbay.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dfqdgbnr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cocprfog.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3poxkvbgo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vosswuqr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kvgxxhpc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zitcbnan.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3whcasthi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kxhxtpju.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gfarjumt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3mkikxaug.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pxhcodpr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jmprsxyw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3skyxygbo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3enjybsth.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3habeauxv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3pdjteviq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xluhstvv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qebibsep.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lvqmxpwf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gjykzhpc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rryguwyq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zxunxscn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ytgduaax.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkfuanw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vrjpfqka.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dbjdjknh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3eptdnvju.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kvqryisr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3igdxjyis.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kgtvqejp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jwgleehu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3arjsfjoe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3amymlvef.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3epykbhsk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwzppeaf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ienngsil.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mswgqjzo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3grmhyfpy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ebhldszv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgymfejx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vmfhjhps.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3btsyjmky.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3aloqnxxg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zlwvacwe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bvtwcudp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnwcmxbx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ushyapyt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3djcfolks.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ifgvcsht.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3budtdtfp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3upkiuamx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3juguvvlr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ewidxzjt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sqdmntwa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oblicmzw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pyxjtboi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bixlvjmu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jesbbnst.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dwvduenm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3txjozdpn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wsuksloa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3etbatjus.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nltvrmrs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ncpbgcli.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qxukyzpk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3venvxfnm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xokhtgrt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qwtovhpa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pdtibsty.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gjqiipzr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3omrrjcin.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dnwwgfou.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3hywkwdmk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gqdjjmrf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xkluckwa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mqlybsje.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3uuimcyur.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cbtjavvf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lnghwtma.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uoyqtatp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmxxpfdn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oakmszot.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zgdxpnxv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3nnjrvbrf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gnzkfnfl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sjpgpctf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3kguggori.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qiecprss.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hskyzcut.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vohqtyvu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgdbpzhm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnamlxk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hodnaqml.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uzgbjpje.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3nivevobm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qyjhrtkz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hgwwrggt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ervhsxij.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrqwotnf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ghunxnga.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tnvbhxkn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ilspmnyd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3npfgvrxf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tdimbvtn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ejzepmdz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pydjsuob.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zfnfbvod.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aiboobcv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ekubmzme.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fzlgmswb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rryphtok.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3huwwshdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqjdcvxn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lbbvuvmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syhajypq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pzuslbyf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hkvtdvag.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dwdbhxgz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zvzanagg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wkyjwvvr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ksteuugb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cvvflyxi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ybeleuzf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3eznarusg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3unyidnru.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rjgnvngg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ukgmmiyh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kysevjue.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ybxpjssh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bhixqmui.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvhofap.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zyhksytx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bcdxiczs.html


<!-- 参考信息 -->