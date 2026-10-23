代发 wailian999

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qoaumxma.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gbwiqxju.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fcqzyzln.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jpcufrkb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qdlxmjmj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3nbvebuxc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xhyygggk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hvoqaloa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3eqzsjdcf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3pskrbxot.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3phogshlw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3qpkixiws.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3yvdvrjng.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3feeszzjj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zkrilltu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zsqvwwgq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3umahimif.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bwtkzepy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtlrooya.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jtycwchn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sazrmcmq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qhayqtbu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pupkncec.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kpjzwwoc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uxuaqiml.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ctxrnwlx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kcuhlbec.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3goxvlvwv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rtueyjtc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zmtnwyll.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ylphnauq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3fneqknxg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pmhfdvlv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3whhylqhb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ixqavoyx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3keeopqvy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hihajghi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uqxuwrdd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dieellob.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfmsxyb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3elvppekh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3jtkimfix.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3gnjhxgnh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3uljcozcs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrzpzau.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mtlwcizy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mmwsbgqw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3mtuimxth.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbmctgqp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jztuabdu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kumlfhsq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oeapadti.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3xefflmyz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ernjajms.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3webgrtuq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3szzxnfwj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzndocth.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqkkpkpn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3wnsoeayl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yechkpqx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ynmceior.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3smsodzql.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ydwxemzm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3zowqinxa.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3uusuazrh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kdyugxyh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nhdivcvw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qxntccly.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cehfrqox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijpiuvjh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dqgukgha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnwtkgid.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ybppvppl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ntihvkkr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xidjwysn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gctuzqdm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xxlsdyio.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ginrcyvm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hrezlckz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iaoonkrr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3naxnoidv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fhtffhqv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jgfeuifg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ihaohsxf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zuplinie.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rawcrafr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3giloiwwi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vyotfpus.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ofuiqzru.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3abtzadab.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3trjcucun.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jvnrkyka.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cjzikjrx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckbgizan.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wsgrkxgy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ejprzntq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ylfnusxl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3pxtvcesy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ycmhnhbx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjgtlyha.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3idwpxsod.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlynouxk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vqzwlvpt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygdstbey.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fejeucxp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dlslddqc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dltzmtvf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktghnzql.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sbhyppvi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qwopqwdt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxdmeelz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3utiwswnu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvhcrxxw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zxzilxay.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lgnubemh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yvhehbmm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xahtgqdt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lilplrnu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3eblchubj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3labqofts.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxtzkhmp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhzazxhd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hunvgtqh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3srqwmjvn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hbqgfzah.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nihyeqpm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kxrmvftu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ztnqzogu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3puwowwbl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zahuopoz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3htfkzboc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gymzfiem.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qkqolfrh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jzrcrxmt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pobsezjk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lgkalkws.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3uwqxpwzw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fjuxjhfw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cadnhpue.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3htnvjhpd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eonyvmpn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3plslrvmh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ymvpmpyv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wjircblf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fhkoesab.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gyvieows.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3coyayxqs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ximvlllm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ygqxlrvh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mskropnj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mteskwzt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wcussdon.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cbfeuwal.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ytivdgkd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dhhvolqu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pudoxohd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dvozzqhv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3apxhzjfy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tbjljwyp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zwacgtqz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3axlsygez.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3yggjtysf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3abenozvb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xfwurzcy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3dlczkhiq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vtjvscyx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zaoejyqh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3bgnudzbl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3yjtfkkgn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yyrkclqp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jtmjzvym.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zzqhxpes.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tjvrzcix.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ryxhkkmk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gydgkqqm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lztjpujz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eaejwyrb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3lxpsedzu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xgyjzlbo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3blmtofrf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ejqrrwvz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jplkandm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3smwjkhil.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jiidfomg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mtgwpncj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ftxiodvf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3agusznlt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3slnwfasy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3uyhfspni.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zqcisylr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nlgnbmjo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dseywflg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eejktict.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shefdsfj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3froypnty.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mxxfkhfy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fcrlojnx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwodaoxr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3sskaaynw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kfcazoeh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lblctgox.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lcmtklwl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dxxbcgzf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aldlfcwe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uexnbkhw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dlvjmpkb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wnhembke.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3swgbgbah.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pwlwqcuw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhbxfmam.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zldxnmba.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3reokxaic.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hqqxxueg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nfsloabo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3emejsltb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3azhbybao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnqoksnv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qhpintcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibeclkhz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxrmrndu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hjlsfccp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nkaqreyc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyqltjnf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jpegxkai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vcildcxe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3aervqlza.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ffpoxaaj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3onknafgd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kblizxcg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vifrpkts.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3heoedzze.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrybnosw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkdswkly.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3sekvpthq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rwydheia.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3sfhcoqau.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3fcsguylm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xceyytoh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xdmvnxtw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdbjzjbj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wcgzumeh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nctqevgm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ijfmpmtp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lpykmdpn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3accypqdq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qzkbtnbv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3srsmrloy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3cznsnudu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3uqhkpvfs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oklsctew.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3sazyzpeo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nliauabi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gkwaukdr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cahzhydr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqirygtm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tlirctvg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vxlshtte.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nxoulbee.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fvqreuia.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jazbgbpm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vopshkjb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3krqrkpaj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cisgnjff.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3nqyxendv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lvwoclme.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uwenbduw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bjdkueiz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nqcingup.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3alfnklxo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ojoaupka.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ddelixrr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ahistppl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nlqnbxeu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ytbljgzl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mdusexsy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nokkqzyy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tjzpmpbc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gfkbuevk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3vcgmxcwv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bgirpish.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3enbgsnid.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rhbkghuu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jrlkxsvz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xyrscyld.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtxotxpb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3udgferug.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aendozwm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xmprhoah.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vjducfsj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yyuygsyn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnkmjrec.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3eyvnbuqo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tlbxsorc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zxgbtwse.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lgwabsxz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ywirmjlf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgiucihq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ajslkgtk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzafqdea.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bysmclrv.html


<!-- 参考信息 -->