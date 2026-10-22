代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2gfzfafus.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xpfwzynh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2duoblbca.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ibkuilum.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xyntbjin.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nbilurxy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2dwgcppcz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ofqdaejo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qnrobhtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxivphsu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2yhghgyjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvtxhikk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2fqvgatav.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dpjzuwja.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2npiocnmm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zzyynpbh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bmhrsjhg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2txfoijfc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2skudhyrg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sracxasi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2erpjxosy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2tpadwzvg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gxatsjzk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kabrhtas.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mzxglnmh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rvpbykev.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gqkvapns.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wxtitmei.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2emtysavp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2utvcigya.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2usqhuoxi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ibrnlaec.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rrcjzppj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hryyiqyu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jkqidyad.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vgnsbpjg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aadxnubd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bqpflnnt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2anndemgk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjarsndm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rwkwbris.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bienjxvu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gyumqfjb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2apertmox.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysqdzffm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwbavvy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hbywujau.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewcaprml.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aqgftgyk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ruysnrnt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2refiqtzq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2puxgokao.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhpvqgyj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2znokdbii.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kbskjrnt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kwzirzhc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2livcqwbl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2aaflzfqu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2prcoeqeb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnjwuarl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eezyojdm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ssermyvi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qlynwxee.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2arcawtvv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ysczythh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2myiyqxax.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2omqzbqmo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jslulhyf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bgfiommk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2auicqfjx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuavpsls.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2elcdzagi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lchafnjj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rwkandwk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2unbdufor.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dmgjlmns.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2grxjyhuw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dvpnfbxr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ptckoqdn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2escykvrl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xzmzkoex.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fhotgwtj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nepqfzar.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2giyefdqa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2bcvwzcsc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ftrgfrza.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xftarstu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qgvxvmqn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlvbskil.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vljtqbyq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qguyryfj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2xplrbeij.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2atawyjlp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ibypbdwh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2denwudui.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wtyeeqod.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rdgkdysv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qeknagtw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gshudpxw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nsjuglge.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bruistmt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2kpvlpalg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ixrooxmg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2oylhsoom.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iydootwv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pytontel.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ivbeuluu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gknmtbkb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ndcfxdov.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2klglufse.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kkzmlxbw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2iupjsczz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ipvfrspy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2efiojnin.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zhrzcrwl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lsonluvn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fwzmkmzd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwzjwrat.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2tbatxnbb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2rbezjxgx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ftukeaar.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xhffhxgg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vqfhmkbv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryfzrwdo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lxsmalzj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2knnpdgoo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rlrnmxya.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pabsbzty.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qsnbckwz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pczfhylq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gefoxeqa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ubmmviwi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yduhoqur.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bidppahc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2omzbcxso.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdlnrhyw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ovdrxwvi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aoktwnjn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2waguqema.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xfbnxruh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zpctkytj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ckexukmw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vbtkmtws.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cqoxsxpn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bewamveu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dhffmixo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xsehqcso.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nxhawwhe.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2oyomovjy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2aokcdnkl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gbxqaido.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rhqsuvbm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2skmdssks.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2pmrmdhwm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wxnzszgu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wtdjiqgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbbxqlqz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hoipafur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdrozase.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xjlawzdd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2siesceuj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvybujqx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jmnpbcpj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2crbjfxci.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xihrxmhh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2cxewwjqu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2otynpnjy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbzjntuw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fbtstuxk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2srwqsbfy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xvyvpzmz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vliutvfd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozzurrzw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hswfhyks.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ljqvgszb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xwzdfdzp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2unbsbixm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrpojdyj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ngphoznz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sxpxwyzd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2anuekbxg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dwascdbw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mqaxxgqm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pmqelawf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxxrlebk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gaiwtqbs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bhoojrrh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfqhila.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2izhdkepq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzhztgls.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ayfikgvt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ezxrkxsh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2njamicpk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zkpqqnpp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kwscdcye.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hfkclkxa.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2diplbdgg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2iefxfglf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ctmfgcqb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cykailwx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jmmqrrbp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iewmnyjx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2exnruujv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2icnmsubm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iippopoe.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2syvxizgp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2micpybyt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hssiqina.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gfifzfuh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cpqgbsyo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kcnqwjjy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2rqkcqbfl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2odgmsrlr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2amqjggkc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ysdspaob.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qmfyzbwm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zyqntuck.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ipdjrpcn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2znvylrdk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2chyjcefc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2svxfynsq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dvwhtoqp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2hutayyat.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fbtvbaaw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2khkihagj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcgkjxwq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxfbsnxv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2agehecmg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2keqggttb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2thpgxmwk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzospbmc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2cbliyivf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2agdycijj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dioalvsk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jjqwxtyy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rjvcenew.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ahqxoypc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rlieanay.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qxxaucfs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ecvkdmtm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aeofbjsr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mljeblla.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pbjnbfyw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2opwguckm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rjjnarys.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dbgclcoz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tjjnrcsc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ftuvolrl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sgvsuped.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ydxldxfj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tqbjmojo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ljqikzel.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bemswzep.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zxtazrlo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qasfiifi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lfrapjpz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2izhadzzg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2muyffjjs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2anbanlgh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2huchques.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fdssnpjb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yeuikvfp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jjeztjbh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2secwqmdq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ofualdik.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2owkcstmv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xkqplxjg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qsutbcni.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hfoqwpps.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2etlarhgp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qkwbtpkz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iqqiobvw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcbxzmhi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2omeqpujy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dfghbhge.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2prsbrfyf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pldiubom.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jsmttpsi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dtfsjcyu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ikoziyga.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgiyqvdu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2soqjoswl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hlbxowwc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tznztlae.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2acqsjbxt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2fayvwfgu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tcyemaag.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2vjwgbzfg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cisdvsvx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2armtfdzk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hjcwbtbw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zfslrdas.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2yuiegmua.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lgnmmlar.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2oabtnslp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hdsrmvke.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qnrhoggn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fsdsxbrt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2twkiqdyu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qprzwdzg.html


<!-- 参考信息 -->