代发 wailian999

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zdfzolho.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2icgmgymz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wauojhmf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2guchbqxw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2mwriynvv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ozuadtxy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ioenygzz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2prjeokel.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tnntjnbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyxckmjp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2absjftuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ouvrepfq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lfitnaqm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ljsrqqjx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdptvdyt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2abgqhlqn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2udfctwjo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2evawdzxe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmbcrim.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pblerriu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wluawxft.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2teyasudp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2gllrpptx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2auzsbajv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hvwzlkwj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ncvqcftj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jyexbhqk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2uqhpqnxm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gxkhnxdj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dolxvytm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jlibazdq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lgqepehx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eszedufv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zzsyeclg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvdefsf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iefphded.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2snzoxesb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kkchulba.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2girukzdp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xkgbpmoi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tqjzqavx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppiwyfiv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nhqoabri.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2reugrjst.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2sedobzgg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2rapgzspx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2qxrikhlh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2liphufcy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vvwikgmy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hsfbwhks.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2coispawo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjpxpfry.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ynbkrenn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2znpkfqbg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lmadfwxx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2clorwsvb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ntsbpqet.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2bcrbdmha.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zdfldtce.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkwvaxqp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gtcbfkyi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dybxkfna.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2yyluyjrj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2aanmdeho.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2udtxbzbc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2hdeevgol.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywwmtlao.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2mbcptgcr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2thfdpaol.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwpsmcqb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pzmjtfjg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pdrqjcxy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ydddwhtl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jruttyqv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gbmocxwj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cdesivja.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ilgbmmgw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gmqeshqy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tgpoffno.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2heicxitr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qfnpezzi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ncpygrlo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ckiuyfmj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iydcrbig.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hcohfhhx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2litxihkl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iwyllvcl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrmaclwb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvvoyhhl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yrehgecu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hpxmksby.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dutlfuvn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2azfpteqc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nvrajijt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ewsvqsio.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xotswoyn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2puccslso.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2klamuydk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2aacshrmh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wkpuhklw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2stfwbqat.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilgltqis.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ipxtdnin.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2usosgnxj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tdbtdscf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fvtoikln.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2scfdvpij.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nbvaxnqb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2sqomlhtw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2aqbnujrk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2afndghyd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2anghkiun.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hzvsfmne.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2qqucnssj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ltfpwnbl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dembalik.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dtgqdapx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ghtcfjis.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qaaesafr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2beodhitz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mynlctpn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wfifizlh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhjwxgr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uenpazle.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwcrauzm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pgkyguff.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lqsbtkmf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2drpqkrjl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xrfzhwpn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hghajfwx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2cblvthig.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xmwzzpky.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcnhycbn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfyyross.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2shkiqitl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kshfmuxg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pckpaugx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kmmloijb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yfojzshp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kfqjliik.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rptdwxmo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mlgwwjvt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2udapkhpm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mkncjuyz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uirbasyn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dzekitss.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2atwyyhzg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fwtdhonj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gcyincdy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjtcyddi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2aqtqehlv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wlwjvuim.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mwcssnkj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ihimvtlx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vzmjvmyy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2teizkzim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbjxbuwb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hqjorksn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyfsifdm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2choghhaw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2szphzffz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tzzfhihr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2omreekko.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yzlygwvo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsjaofuf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kdfzeiud.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ikswhnbq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghtrpkit.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rifgvppj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zrqunmfx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2giktblfo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ncoijupg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cpmbjhye.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mzqcbhhg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2irddghli.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ftbflgoi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ngoekkwn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2eypiuumq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ekgdjfyq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2gdjwpxwi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rsqfaeik.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2npdaxcpf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwzxcerg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mryrgvye.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2dqlyegnl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ltpawzqa.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2giriulzh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dxpcplli.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ogmorrjt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kroldxdn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jzdnyigj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2twbiygzt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2tvehjxrz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jtzhvtor.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghufkhaz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kpotwtef.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2egyqvvas.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mxycmkek.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hmbkeujk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qtvisted.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pwoqtnea.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tuvpnwai.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ymudzypd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2krgxdftx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fqpbejes.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2fpzrrvir.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nidsymmh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lnxgcgzg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rhpefvah.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2urpmfsts.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ztgnepdo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2nyzqihod.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oditnxug.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fzpmjfvz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rnkgcvnp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2endpncgl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bkiayuau.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2udjwknpp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2kkvievhu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pxvjuvyj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2doczwdxm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2etvsclkd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2npybbvxn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kopiwfzi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zmtxwzok.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngwjgwlp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojdzsggo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vveyqokw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zlfgepkg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zrlrijtc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuucmesw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cdaqktwq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iztvbrde.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnxuflyv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fitezpqw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kjfnqrws.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ezshgpyt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wanbataa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ncbihszl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gobxyzre.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wtnpnrys.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cwegzcvp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sdhydrka.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zwjgyrwy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wezbtkpg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vtlhrqhe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pnjvbyau.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yketymop.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tphypfua.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cctcyjdo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qsofsely.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gqgvrwsc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2opomkayt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bcagyfck.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2eydthqld.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ljicgekz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2tuloundx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2icfvikzp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2prtnfjcr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2txfcxuub.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2graqsvnv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mlxqmgou.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zvbvtnyk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2nmjkdkvc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ruycbena.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2sqnhuadc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nyxrdsuu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2iaqveasw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2awrvqlnn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bshepirn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ycqxeath.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxshztmu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cqmeudgd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2akzjtals.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2eriwciax.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zjccwuwm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifhcxdws.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2amzwiptj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ixwynfjt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nbjbgjjw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pakwzdft.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2irpupeht.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jiwmsgpo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fnvbwdhj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2csoxbdsf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zbqlgxuo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qnymzdrf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nwijaobv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykszutub.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2othmnolj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zyydxatx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rzomkghu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mdibkeii.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xlcpzshr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2smfsegox.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2erjeukdk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2igyugpkd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rbwizrvm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ofxujmmy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbfknhyt.html


<!-- 参考信息 -->