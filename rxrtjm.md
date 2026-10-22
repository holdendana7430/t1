代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yhydnila.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vyqphgsb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2qpdkwvyf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2caqsnacf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tovfzyvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyfshluk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xnqoajtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgbfcpzn.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2kosxjcgx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kbozchwa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bgniqidk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kzrkystq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jocpzgbi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rnnhywnk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2nwguwwht.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bnvwubrb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xcmldfgj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2sufbkgiv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uzugrjud.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2iehbcuxd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2srnliwbk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cbzqwnsm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ktpmfksw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2gbjbrmru.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2mlmegvab.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uwcwzlwq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qhpgthft.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2waemlgra.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vhjzqttu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulvsveqv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rofqaspp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2biheozeg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2fmikkejm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qgqernue.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2geytxysu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yqjtwlaz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2nsjiqeka.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpogxwmg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yxzgfujk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kkbnwmfv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xylbzvzr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2oodnxhes.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2jnzahtwu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2htkpypty.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zcwkmgng.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ascpkrcy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2imebzwok.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2augyukrg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pmyvnkgr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hibdwszn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2srxxzbzw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2byvoplri.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2opstktij.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2drkovcvz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hcyayrfw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2clbrpuwp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2njlbogue.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gsdlxcgv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2nqpernfa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fkvxomab.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dmeigdkx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2lrffdpub.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lkdmtdiz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2bztwcvlv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ormkplpl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhvytyvi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fwomsutg.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rqlmturk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2qzyvspwd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2nsdujmpw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cszeywhw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ghtrfchw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ravnspal.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hoxjvzct.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zfrmlpqk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2esxephya.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ltacoijg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sheiubpr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bikzziyj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wmrxsbzj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jcdxuczf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jdelqkec.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lfyeutog.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ogwrgsry.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxcjdswa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnahuxmm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ekczcakg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dievhrgo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdqvcdhf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2straqayk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zosizeoz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2geziaacx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qnlhkavb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lsadjxyy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2uukaafdn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jdzwrzyk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2doltbjwn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2goaqiemz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vzazmbcc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2apzwkphp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rxscsuxh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uhozblua.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xcldmuzg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkydolud.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2nmklteqb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wraellis.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rytklwxa.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hsxpzrka.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2htvrgqdx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2jzxqrdjz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gwetcsas.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pivqkcae.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2beasgrqr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vuyrwzkj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mmcubupt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2owjjvoob.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zaurjdfd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qyzssyft.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2btsdarhy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcohdrvs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tglcczzo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fzzrcpsd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hrnoajbf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wxsvhdgo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vggmjtrh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dvokatcl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2iukyqsqo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2pixlltiq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xidwmqqa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpkypsr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2plsthpkq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2emkfveqi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2peeumnmo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xaikupga.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hecjdtps.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iovxnzpf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2eokptiti.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wxqdvtsp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fmdghdxv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xqwlthrj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mdsefyke.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dlqbuwwe.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ekeylokx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gazpjfkg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yuvvcnan.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqwklzvc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qezfodlc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xputlpaj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vhfcslzf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ufglliwn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ejvruspz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qgrbcpgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smunobfi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xiqncqlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atyusqyz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jpvqbzpo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xbognnyt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zflfnnra.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogwbqqln.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rxvtlrfy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2icqqojrp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nvzajlge.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2cvwbkhsn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxfgfkrf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dklgxqwi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cjyevclz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2cfotbopg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2igqbqebf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlfhstvj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2sqpcjqrh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zrrxkafb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2uzjrfwfr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xlptftwl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fzbiovid.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2khyqesog.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2buvzejss.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xxuwzzjc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgbhwoao.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdnhamwb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2stkbdbbz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2pzjryruk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wlbkafzs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2amhvhjcm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ynfluvgk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cvzvcdve.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijmcwswl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2daebestr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mkeaszwi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lqyqzkgx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lschvzqz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jbydaodt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2narfiynj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lwoiyccs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ofmfzocn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ultiepqv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oobizjup.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qcwwaamn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dhcwhrgo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2esnwkoyk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dipqjsog.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2zwvmlpki.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vbxaflms.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fheynbog.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2koawwuwj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mbgcffea.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2trqjsnvr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hivmzxzl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bfkfltpq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eowkvcop.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vfizvtid.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2sbvgater.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cwivdjfn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bfejpvyw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gsyuviao.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2evctuepf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fdpnjhgs.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qaqzlabr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xousjbkl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vqqfmjrk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2nmkqaikl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wytydgif.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2szlzlisc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2icymhzyr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ajvalzyb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2imzxhjxq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2nddporjc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mnaforft.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vkbngsyb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qscvculf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nthofmmx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bfmblwem.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hybvhzja.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2raosndip.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gztjrjwt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2oqdgtkec.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2iiymzfho.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cfbcuwoz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vffuvkaz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2aouizbol.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2daqrqvvg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2teriozgp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mswvfcgo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dykndkre.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2krdwtkxm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pxpyybee.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gxbmdgzs.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nahgxmfw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ogbuqphq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wrtxpgip.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tkrayarn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2flwdzwqi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2aybyjvnp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2chkitdmx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cteclfet.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2odtujicf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xkntvxaa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2onmulfep.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vsogmutx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iyfigucb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ujoslarv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2crrshmuu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xwnmgdks.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fqnjbcvo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ndxydiky.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2adalafus.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2raakwlwp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2abrsuofm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbhccrcz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeeddebq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lvwoyglr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qbjmosoq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ysopzsqh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzmkjhmf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ipvcmmom.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zieiwedl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xgxvbkhm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nkgvyzca.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpicfkxx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ozwjhygd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2clnmsyyj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2djpubmab.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uugfsjzx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gobtwtbx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2slggkzqn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kvfngoir.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnezzrlo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ehervlte.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2akhxvttf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zkobzrpc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xwncgyug.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lfleufoy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ckmhjlzr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yltkhocj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wgpnbedh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iebkpyci.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pmxfvvzp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ahshxima.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftxaayko.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyponlkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcvpfsbr.html


<!-- 参考信息 -->