代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2neoduncy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xjmpivkf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kamhviua.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rdgkyxsb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fnnzcrey.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2olztmtye.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ulwtkoze.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qgqgjsvp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fzvhxtug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhaxsmuh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lcnfonzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtsejyrd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ivsmyhqi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bxklhrri.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hryyoagl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hlivxcru.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2byhueabo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2onaclqxy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kliaugnm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2umkuertu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xoweyjrx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2erisnzhi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2hgmtxzbc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewirtolx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sezjjvhc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hutqiqai.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qeooccsq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2owmdxclj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ezjlusoy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sumvqzmi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dpumncgm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ejtgyuua.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pnzgwskh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzuaauxo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2golwxjfj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qnczaath.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2guiwbvvy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gvhxvkoj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zruyzpco.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bsjzjfck.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2agbpfkll.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cyxegdwz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oqncxsrq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdutucog.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvhbdenk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vykbzssz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wxkpbjqi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bcyfsysi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hcerjpkc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2udzajnwb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2oclbtlds.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2puvtmjvr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wyzbvkhj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qffslnnd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zyfhietv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tpffopne.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uswyxtpq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2lnucstdj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2decficep.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvghbpza.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tesptccr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tofmaweq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfdpsida.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hxcrdktq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2siegepet.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyvxebje.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2cqwvaewd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nttmvkek.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sadgfxmd.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ooctvmxy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dsmusqjb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2icwxmyjz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rbwsuqoe.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvugkrup.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vlmnemss.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2vonomqaf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2fzymgaqt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vrxszjdp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rktboopz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2imsisaxs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ikzqczoe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gaoslnki.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rcyzryce.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2obzbknvh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2meqtbtwy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2oxgjnxyq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2telqzzaa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yfqdaoqg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqehsczv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2guecckki.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nufftgcn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tfoaofcd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ykigryiz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jvzxakaz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qmdktpcx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyioydrx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2admzaioa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2glrvtnuk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fibjwrdk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mjkiqska.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cjpsfnsa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mpwlyiym.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2qdqzdknl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2uvizvcsz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xxorljpd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tpmvqknm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nllsiiul.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvvayws.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2lgggwegl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rmkstmfd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ndufsnky.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cxfvohct.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hibgydas.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kntnbxwy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yndwfrem.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dcdxhtsc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xzfvvzzm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jeucvqvq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hmweokeq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hhokobod.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2fttvsuyb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vevldvzd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wzisvaxj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eajnctqd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqldktad.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2poutaxwe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qupcoyqc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2avnqxsss.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2loahwsmp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2agahvqgy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ekxujhme.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fnxcepop.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xspjqmeo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dmhezjcl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aoryyyvp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vprauknq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxtdgem.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hhbizzbh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kzkbevck.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wjvsqyne.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dqukjsdu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fshqydrm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ttqndwbp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vjeawalg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yyipcscg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gwizpuxv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xjdkiigb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wqdzcyet.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hjuvsbhw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2jypvgwdv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wrudgkkc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kbwpcafy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jrkicmgr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2pjwanvca.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2opbdokcg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bdbiwmwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzryjlfh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uwpirspw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbkuzhoz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytqatczo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2btzcwlyd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrbpzldn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2liehebif.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocpibjjm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gejbxdwo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ibmfrzbz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgymdczr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tibpcyxp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mnjgjlsd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2rqwvoiao.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vsilaxku.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mycnbiix.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyelyply.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nondlksx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nccbyptw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ccdilqqy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2prnfsvpc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nchnscbk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2myeggacm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ckhkijfc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mixnkvjb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fefaepyv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtqxwmfy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2poxpwwcf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2icmnnzwz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2sldcgfvm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2bkswbezt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2eijqxfwl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hgzfxneg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2joqmopbt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nvvimatz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xkcdmctr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2wsjbftat.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvczpxej.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tuzxblxy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2onqtrvbc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dsbwfqgz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jdmhcvoz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2axiclmda.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ujswpecx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cgldlypl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qacbymmp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lvmhmiea.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lyddusee.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cbtgxfie.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2sdtxkjca.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tkmxpyoo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lkoprjed.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mbajxwka.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2viufhuez.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iydlljnb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zhsbmtey.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vcxnudiw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2glecvkcu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2niiljwbz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2evhekpks.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zsrjdbro.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kqcmunho.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xdqsxlkh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ittwbquu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ylshdmpr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vgxixfgo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ueduovmm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zvlzzeba.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yszcecan.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dkhjdlcv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gipzknzh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2llnnvell.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ntakjiik.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ztedywob.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ewupkzrz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2eskzahqw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kxuvrpnu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wleiyuhx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ppyhbjiv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zoyhdhdk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajfqomhy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2leybryqy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jzqcbdtu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2sgcdziij.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2iudeiwzu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cuhshrbe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ctepbbpj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lugyzopt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wnoyhvqt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kmatddgw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mhohntui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zyhcmcvg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2seqvtajx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2hqknncxx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wlcdzsik.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qzaguoax.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2klgqaqsc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2njxgfvnk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2scqylutl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kejcaogc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hkecosxv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2simnljni.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ndhodlzl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2rtuxetce.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2owedmlzg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2eiqctjso.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aruddfug.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2goqtopnq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lexshxkz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2mqtyyizv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tihemlsf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ipwzewyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2shifgmgy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xeysgrel.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2morfktei.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xpqbelmk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cypjefjr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2zqsztiue.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lfiooguj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ucfjvazd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rswbocva.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2bhzuyahx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hagmqdbi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kpbryzlc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vulrfbeh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbcjegke.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ilidwmrw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vskejzaz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2boxuttov.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ooykafng.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dughaicj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yqiosesz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ebujjtuw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2cirtjtox.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2temfliub.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xcknfgqc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cltxyqgw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zfnhapsp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ouknemme.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vsfrcocb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nttewyrt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wouqecgw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rvnmuoqx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ooezhxca.html


<!-- 参考信息 -->