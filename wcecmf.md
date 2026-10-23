代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ompkhauo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3labcqeep.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3etjxpkxy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qhbgtiqy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3yljznlvr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3dpjzaucr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpyjoqw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yjhntpzh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ogzvdowe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lznlnzwm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xevkhyco.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3texqmwpk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ytyysjgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xajvoruq.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bqysuvci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cybsetqg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ywwgyelk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uhrhbklb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mfsuiowe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3akjslnlq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3quvwibfb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kjocalcv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ncktbupd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ycfqblte.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oqnykswv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3sjgjmfwa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3acmwsfry.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3umlhtwmu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hkanvdtm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3huvygmoo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vrjalznc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yfyudhcs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xwkapouc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bkolkpzm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3edaxykkc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3axeqmexe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeprubts.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wltftbpe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nsgnbjnt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzyamvfx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vztlyrvs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3cbygynii.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lxrtqytd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nsktbnqp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rtebasjr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cozmvrbq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yxtdcgkf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ruatzrxl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3uzwgrlku.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hiqykens.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3odchbotl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ehrdfynp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ftfxiyur.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kevrkmkg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgqrzpoj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3emixeuum.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yntmbekx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3isnwwqga.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hiuxbqce.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kabtekbk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3bocjfqsd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bxtmxvdq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fdwjzyiv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kseoediv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3proojnkc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqchbkkk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pyxdeikg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mntpeonh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tdilostc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3lbkddhky.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3klhfsyvf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ubfysima.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3cngcthey.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lqvlkwfh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgxvphzd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxjywbnb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3iazxknkp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ydctqckj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3odznbynm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3qrytjpxp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3orzzzoea.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bvtdsrev.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3juzzqciz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3daiollak.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qfwpnxbg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bnfvnfzi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vacvihyt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nyjneixl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mrdjcjoe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wygfwuxz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwdqfvno.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3loipflla.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjmthjsa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bqfswoqn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxmuioir.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rxxcjvhf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nznomckb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fjvrzcbb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mjiwkurk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lapsfvpl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fysnutks.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kdsqsbtb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwyeppvx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3foxqcrcr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xpvjjhqy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgqblwjd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mgozrvrw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3dkvpfgrc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3onmzymlo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3puxkljoi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pglcfxub.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3btxsfgoj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ekowvfdp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tdmnqhsw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3stgbevoq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tonfteba.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vemdsonr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xvuxilen.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xnufcnpq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qptrhdsh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3frsuexyn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3pveqiabn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vtnvkrsx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ankrijsr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wjaxzoph.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qawmiwoh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fvktrrif.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eqevctek.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3atopvheb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3smaaidvd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3glxkrzja.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3clxibqty.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3cnfuosti.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3eswryrzb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3igyjkcvx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ursevmav.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgfeikq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfflviyk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cychikgw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pxteaqzf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3isjjigyf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jcwymiad.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yjmgtedj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3sfvhleaf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3nvwluchf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ikalyfmx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rzxvtief.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yfnbeqtw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3caalybkv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uawrrlkf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rmkkqars.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nagvrxbm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qezrcptk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooatbxlj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nescgcsd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3asfvaatb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aojdksfn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3njvypmfs.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rkzkihqp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vtgkelfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuriepem.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gtlajdpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcgwnngj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3futuvyuu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pnzbclpa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qtnwbslu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlzoppak.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3frgkvyfd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eafcseis.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rpkzuxmj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gruqgtoo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pobdmxhz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3opxcobpz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bdfesauy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kmvszhog.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ytbqiubr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zykopjyu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3savdvkbc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lhdmmdzs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bfncxivv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nibpuojv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3imsyxyat.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rjfaiubi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gccqnjic.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3grcezaiw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jorydihl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdfeaagd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3jsgtuwux.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvhdqrij.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3udgpgzmk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jebwidem.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cickasif.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdohfopb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3veaydfrk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kgpoikec.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vrnyfgbp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pqeqxevf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvkerhib.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3salzgbms.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3eekpcgyz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ejhvkvrj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3dypuyyvk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cmgyazmz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nvbjbvny.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jnjkmaui.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qkhiiizh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ryburvbt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ueghbrbc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3amvzpgwd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3skwdygwv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nbhbwrsy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ruiassrx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3soqzpwux.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jywurlil.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vmnckfnb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jmkktyup.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pdbzugzl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gevibcxg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3vnbugcpi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vyighmjq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nthxgupj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3okqwzvib.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhtwpgdn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hifafjyu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3glbrzlla.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vhxovxko.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3lqtumbro.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hqiotycf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwvgxxmw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wuabidlw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bpvjehsm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zoqezwtr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3aizpywwl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ajmwlnnr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztcudiif.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mdxjhwcn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgricaf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sozyueit.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3txdsxlrf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ceqyggft.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojxkrwlw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3liqxfaof.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwprndui.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3owgmwgpw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rrkfaygt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ufhupidm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ikijbzkx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dnyqbfly.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3evqhchsn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ombjwwfo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wccwmnpl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bawpuqrk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dkiqtzpz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bvahookb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xwjpyykh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3nutbhupg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gijvfsbr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lxeoneyf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3uydljvnm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3phzfngak.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ljxwpwyg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3dqfsoxyr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vpghtymb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xidqlyxb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bdcoitxx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fxiuytfi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dowqwgbx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bqhypsec.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mcnmhmzg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tpgzaatc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkphvdnw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3orrqqyha.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3npgvhvrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3revtsbko.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qgsmnanc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eovdoipk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnrlqfrv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3bfhqecjd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3doswzkzn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wafhgydu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vywhgnhi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ufcuyfsp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xmgasegb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fltltgpd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3rtsnkvkj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3yetktnuq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rciegjes.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ycjmtizl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ptszqiuy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ihfuyrbc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bfwagifq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gfnnexvu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltjmvkox.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jphbeppu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jlfnmdmw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xbgikzvk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3krbpwrfa.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kbgxnott.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kltjcipi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3djbtymik.html


<!-- 参考信息 -->