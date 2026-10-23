代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3rjtdwuql.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3sqgnafzu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xanwfhap.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ghktjusr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xhjldgxw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qdurdaxf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3dopfrgeb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3llixswri.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kcjfgmep.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jpsmopjo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ffrwwruq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewridxnx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ygjgxsfr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fvwqwkta.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ujztnohk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xsnmtbbj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pwupikiy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wakjugii.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fagwwcqw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cpalrxob.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nfrrfakx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayyfokkj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fxnukxth.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuuuwwkd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3daipqbbf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3lcoectvw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bkefemor.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cdoktwyh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3czalixqi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lezbwjvz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yvgrluhf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvnnmli.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kohbjees.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xiqaaoca.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3eaxjvldk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zthmjpch.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3azniliju.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rhnzjnqu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3aishqdmw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzauzaw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dqxtkvlu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3okzdylfu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jzhqiksm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3wmprlqxi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3largwnof.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ytlnmviq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3sgklcuao.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ngvswoiy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uaacpjbw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zxryldcc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfmmcnom.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fubdpupf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fnduifoz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3axrixpwx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zqtiveqw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tdagzets.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dydnmybe.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pszotgbl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3meuhukbi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbfwiiht.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3yvyrffjw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3cntjtgvj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqqrunse.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3crfwcufx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3grsgcagx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lugbbmsf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3awnppjbd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wfygseiy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nsowqdbg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ucmoghyj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3nttbcpbi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vsvfyvod.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3riylvbmm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3tpdojwyo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uajekdvk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsygetpl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfhrnokz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fzgyetee.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nezfqmqm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tgkkkbgz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kermejat.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cuqyxfqc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3kaohqqct.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3reaorbzb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kzgpykzw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lrfnqsij.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3coiwacrt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3crndbjkb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dgmdwnsv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3nwktixxj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3titgqjym.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rhbkonvj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qnhenxfk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3liezoxex.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gjxbyigy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nciuounb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xgqyrifo.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ncjpdifb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hcbcjcds.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ngyjnytd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3jfplkbac.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yoghlkvd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gdwmwnsz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ojovuigu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fpobhfzi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yxsftdpb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vvyurwcd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bsbwhexj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3inrhwvgo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3icogksys.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3actpqygd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gysxonqu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwkdxirz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bdpboifc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3iguraynj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3whusppqy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bexmvwst.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3axmpkjhq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3izesjvve.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wgtahwzu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rufqmjbc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yutselhw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3orlmuumu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rkpqwjkc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xoduikyb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3munefrvm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kwgfborw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ploaqfpw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uzzwverl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ltyorawy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qzmgbfno.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mkihzhws.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ithapefe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ceyscquu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zgynsnjp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qooosfed.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3skbwbekz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3lvihzywd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ainfctzx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ebymqham.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xvngzqxb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3utrdaqvc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kbssqrmy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bqccumlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdcbdllf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3clcigmsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gczvhyqj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3auibmscb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3geiavtkr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sczyxraz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phjrmmys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zwkcifkc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzopdwpt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yecxwnen.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vqojtdnl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3enekmrnk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nnzhjqpy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gmcwhpec.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzwdure.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gofaxmqo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zanolaji.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3xtlfugec.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3sejejwdv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xraicrfy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3prdrcwsi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tbxywoar.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ukgazvqj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kozvjaae.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dbtwffuk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lfwxcqwn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhlcsxmp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3trlnmwvl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ocwwnyhy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3alvmznmh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vgukwzzy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zleacxoh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xzzwmzbv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mtghrecj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ooqhymug.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3amqysbtp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkzyfsxn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tnxerscw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zhfogdzy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pvfqkddb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dmxoxrww.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3yxkacrsw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ckvepogw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jyaxcjzq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3yytdpulz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pvoazcxt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gokakjkq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iapitxai.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mhhdidsx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bfwnsymc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3svyjgarc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3suzujifw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vcwadtyt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fyndiauz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xhtjcqxi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qqtkmqhb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tqgvfsod.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ryirtiom.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3uzguhdxk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wdboeuib.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qhisjlwf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fouxckeb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3awekqzja.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zugctkkw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ekobbjur.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3uoveiviy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3uqiarmhf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3teplpmfx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrgvoekc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rhksktjl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qifzfcru.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wccohljn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gzdechdz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3pumfrayu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sprklyma.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3roakuheb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ykbnpofs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhumbazv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iubosikz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gdghfxmz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwnldscd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3orxivtbp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbzxjwcz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3paunwalm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jvhgrevj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3npmdicua.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vkyaoqcl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bjogdzkp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jrknaekp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yuqufgcr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yohbxdks.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wdeoirou.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3koxsgfck.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kxdkuzxa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tnbybiql.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3lyurwyoh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3knsozvau.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mntwrjkz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pzxkltjv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fhtvbzmr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qjcldktu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3itwfpmvc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ynmapnnb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dbbyeduk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3stpipygn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hprneusk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3aozxkiya.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rhmhpbmb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xdszzdxr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3brkbklmj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cjzsnjop.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vukcwpal.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ykunzukb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3umhwabvh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yzhirqyv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3akgtcpgu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kjyvbyns.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ttmubghl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3aipvgknv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3frboysyx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3aeofcbds.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tpnvyabs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3khuambbb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bwmwujnz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwbvqsot.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3poahbcjj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3idlieakx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gdekkeym.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3mbwsxsgt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdtozobl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vgljnzqe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3kxozbhna.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkyrtwyj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wwhvrbou.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ktegqoiv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qcpsirnq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kqptvpjc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ltrlarqs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3iddwnjiy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lfjsigiz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3dlqnmyml.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3naxmgtbg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3leylcago.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogigddei.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kwewkswu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbcuivct.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3hwjpcsrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbomyraa.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gwarvyad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njrkitli.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jjuxepom.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zlfbwpes.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hchdonth.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dntsubrv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3loinxiam.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lgjvagkm.html


<!-- 参考信息 -->