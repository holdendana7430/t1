代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dvacuclo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3csqqcmjx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3rfkgxeoq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3txgbiygp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rfimyflc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rjfuanlv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ywplmcqo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3oqdhnsts.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bkivydfu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ucbfcgvk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cvnzdefu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mlrksdsq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3pbkljkqn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gotpdebr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fiskaicj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rfluepld.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pukqwmqe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pkpiqpwa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kcocspck.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dglwwzgg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gexmoapv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3eqmksjyg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3fjfkldcm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ldmwfoug.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3krknnyzo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tcykonhv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aczykvlp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulrkatpz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsgymmsr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hefjstra.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mufhagpo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hayjvrbf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qajwfkoy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kngdgggv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnsapbhz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cwihjtmb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3evywpngi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zdzlljdh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3igrjwvev.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zzbfdaiy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ngibhkgg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hrqtukox.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ucdpvquw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bclmqyrl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsrmujel.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nauitbjf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sitoeafv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sxkwyaho.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3txdloyzp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3tohxvgmm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3isgjpeol.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vpxmjviv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zgpkcowt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibvcqqok.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xdbxwazw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3crofqomn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qvqieolw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ejkteglw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pcwivtiy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hoitqiub.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3undpeizi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iizgwfrg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kdyzzpaz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iaswinno.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3duybifun.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oyodremj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3kddqfgot.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yyzssavf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jxalizqs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yiwsfjdz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uhzmesxd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfyzwhpc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrecxkvj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjturwvd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fcieqqxv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3dalkckib.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmszzzup.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cdkgujvx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vrmsieps.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wfvwefdl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xjdbgymv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3exatvdqw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwfyfgdy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3exgixujg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bpwdkznv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cktbowzq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3gbuwvmmi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xqrvocbp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3imlxgkzx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tfdrrrrp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zqebkqks.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ypcrejzg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ituujywn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3eantpcpw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jtdqzvqj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qwqlascs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bvohgppx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zozxjxoe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dszxazjk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dklowkex.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gqnabohm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hrwiiwhi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nfpoevcm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qpkyfoqj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ixhtzito.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3oymhyjve.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zkktfbtp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjppvwpo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ampwedjw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3atztkkxv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lseqnfau.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zehrrdwa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3povzmbbk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xsykmfls.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3srosquxc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3mtabmmep.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3veexvmer.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3krjzusdk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hacxfkuh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3btrypxgo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjxzubhy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlzrlybe.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hwldgycq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3eajvqpbk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vhrayqbn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bvmkdcwr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jetfawwn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xqzqnfqk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mnjhlqxb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zqbxwedg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lxzhsqeb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3biufnmsq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pfmkxsrc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvxhocsx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nujtwjka.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mnmqpwvg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fyfxwcrm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qwbtftea.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3aozhkknh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xlurdaqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyhoappm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3frwmhucz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltprcour.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ckprnaph.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3djydonif.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jdsdjpmu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qepmymul.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3axvkqklt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxphgjck.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ackrxati.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3liqafvnd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cqavsfbs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yysfgepg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ggklqbbj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ryhydqav.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lkcezxjy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gubwyxqz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3usutrdam.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejiqdgyo.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fmmkevgn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wjpujfze.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3axfsbksg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xxmzyrtp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vyysgueb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmzyrweg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpqkxrpf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gshxrwqw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jfxmkxxy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jafzgiua.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3okiqsyhm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yehojdrn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hkdgfimv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tupytzpx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3amlaunuj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hshcjyxl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hlwlmcbt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdrugsjt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kthideod.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3scemjmnh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wjgqdkhq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lwwjusul.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hicxzzcc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pesijnxa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lgwgdiku.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3abxcvrtr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cvhgblhn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ownuqjte.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rotzanro.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ujussedg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3anzfvzeq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3igeaegbo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xyxdzxrl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gbkhljpy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pdmbnhpd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3iqdfwobj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3essbmxwr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vmqysabk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rsxlxfuu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gqhhtqma.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpdqjgdu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nibsnaah.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3tasqstkb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rngmagqo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3uayewpgi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qxdqehmx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3obisgtgx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bxkjsswp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3msasxgep.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqaknbhc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jgtfwvaw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3siwphszs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xfdgzpmy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mmfzsxga.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xhlolezg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3asvptcyx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3byuaayqd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3quyiutcm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fslxtirm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3icodirex.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tdyxuaaf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3roasjrip.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vxuhutaw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vvhiybxq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3obyjigqp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hmsjwduk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mnuonrop.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ubzkqmwg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ophyilpv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3pknffhft.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eoayilln.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fvncbwuh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xwvujoni.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lkepmgxz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rtlsxkzg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wcugofgj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3jqyskfsm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cpjtbgmr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nlhusbbm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qyickygd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3evafwnac.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3auavouex.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cerzwmaw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3anxnvlrc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ryeshkdg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xaixkjov.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vmzjnqnf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fdymsvdw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xqohyxxv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3stddelgk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hihbajjq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uqkvgtyn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zkhtvzjo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3awbueqhd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xofybnij.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hzkmkwdm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjbalera.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrsmrnxn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3kvgemwlf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3olkmgbqf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3awqxgtnm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mgccozkg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3gimedsnv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oblqzbar.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zsnwcffj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozvovmsz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhvyqron.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3csbmtfje.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3typlfqrv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bofrecil.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ecrhkkks.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3erozhuzc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nkrlmnnc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpuuqaos.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3doctigmj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wectqmqp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wzvvptrq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yjpudwbg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tvabmrap.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wiyqpmue.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oscrsqla.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wfmsksue.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dbxnnmkz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zeikljlp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mcwvcarg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qghcnizm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qigdxufy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ogscngvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpetlunp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3uvhleqgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohakcjpv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rqxqdgir.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3waooogpd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qitcgtfe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ukdidlrr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gvxxbcvz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xumemofw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mrpjsjna.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3puduvyxz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hpkwztgn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wfcmffrl.html


<!-- 参考信息 -->