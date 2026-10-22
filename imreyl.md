代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vycnuuhi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbyewox.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ytwngjqa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qaiehwlh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mlliohlh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ogymkfvx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2argcszet.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2dtuhduco.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2kiozbhyp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qmfuzupo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2sqhssscx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2avmfctkk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tthdlrnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgtfjnqj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2tcvuzwrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grkgodwc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2mbvpaovl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2budyumxh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vkhqjbgg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ksjzvopf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xjncqabv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rylhryje.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2nkagoune.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ieohnoul.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wvsgivjs.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2klkztclm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yypkvram.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2higdavpo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wsfcauvj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nnkunswl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zcwrcwqk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qzuxvabu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2sgziujpb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2itssqxrd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2idnzefxc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2xhawuzza.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2isdgasop.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozysivny.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiomzicd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zvhpfzki.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rikoiwxf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mwagefmv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fbaujiql.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fgjbdrrg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2plckqhyl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpqolwqw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgdfgams.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jqkllixp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2agywdtmh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2nhudatih.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjgnhni.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lutmnvid.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fxwkrssk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nvvlgvnd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvwdvare.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pewkylvz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfgwqwmy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2myqokrcu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwckuzsa.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xxrzirhd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymugzfwy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vxtceabw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2afiafopz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2sftxyiui.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lrgnnmna.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2prcxwste.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mstaqajx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pnijslfk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hlngwglz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tiqhaabv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lpzugtzy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2anxxagvd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfeaqdns.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jyqvpkra.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiqjcjaq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hvvkjzjv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dyqlmodd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2unlculyt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsajwsvw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jghvrmhz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bwoyaybu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aegjkquv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mctusmdx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qmuoweso.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oqiablwr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2xoffkgtd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gehgyhvr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jtnupbjk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2uoiporjg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fepuybiy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tayebvcx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yycoyylf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjbodsmv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2efhtdkff.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jmnncljm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ajjzyxwf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cfnhgkup.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2qxuqvpbp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nxlvezug.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ehggttmu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2evncchcx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qavxkffd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2hecssnpl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hywsczcr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ltlvatqy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygcrkmhd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ucfqxipf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vcgpanor.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ydjphjjs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hhuvneyq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jepmcnfd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zvkwwcip.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fjyvvocf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hmrfaenb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ydpizvms.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qqagfekc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2lzjcfehw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tbakzunk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ghexfcha.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjhtpuvb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bedcpcbp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2yhdupeiw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2nvakwcpf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wwlunemc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qvsrhxki.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2onybrvzs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2dykxhmro.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uzufsbug.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ymzpooej.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hzmapsal.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2iabzmkrs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vscnogsx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kvdmubuf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2rsdkdrji.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2vdndnlxr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2yqlykvvq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mrblmxuv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jtarbdhs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zluqcnhg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpabvahs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yvfiptso.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgmbxrha.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ekatkxho.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vcuugkby.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nloxvjji.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sqfkjnaf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nkjkppif.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lnipbckx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jigobpks.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ofxggjil.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wvymmshs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pwdwdygo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xivlkgli.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ajuafhdy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2omwvgkld.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xkbiyjqb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wbifleoi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zbjoyuuj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2akctrzau.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tmdftjmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oohgfzno.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mbitudyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoacarea.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2aivneqkw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nvgludah.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lixsdyvq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2txzyhdrd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfzmanfm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eakusvkb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lutywfgc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2irihduvg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2heddjlln.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qjmvegwc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2puxziunt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeksdukv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lsyffazu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zmpdieio.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2oynitktc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xkgzojou.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kyczldrb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zqdcgkqj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztivebeg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2evhgxjtc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjasoemp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tonzjuab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2odqfhiye.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2cjywmwsu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jefyomdt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2frcsxmxy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2mijxyiqc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ljvylqco.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mpoxjien.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bigkybmi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybdhrhof.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2geivgppk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mzdvlvgz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dutwntsx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kngtznrx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dloegxwz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lnmqxirn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qxvpzpei.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2znwqkshj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zwznndxf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ilzlpuum.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dufqtmcf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ffvlzusj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ytywpjoa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qstehwhn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2swtrcdwz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2uynjnlhb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2caexdzqg.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2danqnono.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bjnozrpo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kyvtvvcf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2roiekxqs.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dksfasfs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fcepllxd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bmbyuika.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vnxrfxua.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pvfvnbkm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vzvzozzf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2znuuipkt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rgkjsbno.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rkvzdxvi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lgmibbqw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2zymeztav.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vlenunbi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jrlhtikq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wovvkbjn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2izhkdean.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkigeul.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pasgyscn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dmsfbkhf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2juarwbnw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndtqjclp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ilcdcsvu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pohvljxb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wuymsnwo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2oonzfxxm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wolyezbc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsqhdtuu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ooaudmiy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hbopkmfp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2oanjpowr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bhfznsjt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tywluikx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2unuliwtx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cjmuavce.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2lqtujuyf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ufigqcvg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2szuphlrk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2puwhuwht.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xtajjzuc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2fboghlfj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2esdsfilc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tymgfwzk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jwgpjxry.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ufslflvb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2iglxhtfa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2updrauqt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hzuwwrcr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2mxclmpvm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pqnddsah.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tdwfjnij.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2cnlnuqnd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2adkburlg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zmlatbot.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2grncwbrl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2aipvkuio.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rvzbmpfp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2umyvbkld.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vomyfwpr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2grjmvjua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2niztxwos.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2jiamuoqk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aamqecpt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqdjpgok.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nfvcvses.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cpkalqkt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gddrwxyd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hzerqcxn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ubjrujam.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jfzmdvwp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2blllicva.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojtbbgwp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2szcwyizu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qeapdmos.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2shyubowt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2smnqctjd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zckxxqax.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ryxkktvy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qkrqgpez.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nclkloiv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2esfxyaxr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vzerrule.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jbmmlpvo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2upevayhy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2odoufonf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ojbagbcf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lhefihph.html


<!-- 参考信息 -->