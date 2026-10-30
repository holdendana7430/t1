代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvskpyimf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmucpduj.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzmkmwsf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcjtwphue.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fanxiaobao.xyz/Article/details/gxodifpdv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowpzdhds.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoisreom.sHtML

[A17] 位运算
来源：http://wap.fanxiaobao.xyz/Article/details/glulljajh.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkzhdocc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gzqwcgnlg.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmgoovfe.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gudcodipz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gigshijfm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gmaybpevr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnormzzoo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqijktqug.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/guxprqclj.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuoqakxh.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvcfpusq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyryonmyp.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gtzoilczu.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fanxiaobao.xyz/Article/details/gamvbdxqw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmxtjkvt.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzuxgvok.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fanxiaobao.xyz/Article/details/gcesxauzt.sHtML

[A19] 交换两个变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvuhobuj.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvzkhhjj.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fanxiaobao.xyz/Article/details/glsleayfg.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gpoldpejb.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gyomdvwwj.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.fanxiaobao.xyz/Article/details/gheueaibk.sHtML

Go:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gejkpucoh.sHtML

Ruby: a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gxllbqyay.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fanxiaobao.xyz/Article/details/gmioujiuc.sHtML

[A20] 读取标准输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gascsujtg.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhtyfnrt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fanxiaobao.xyz/Article/details/gmupqsbqe.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxrptzjm.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fanxiaobao.xyz/Article/details/griluyyov.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fanxiaobao.xyz/Article/details/gbhbzeqwq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnraeiiil.sHtML

Ruby: gets.chomp
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkpyjxwu.sHtML

C#:   Console.ReadLine();
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqailjxp.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuhynpwh.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcnljnfxg.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gfowswlgl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gemsgebmd.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/geucvbakk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbajtwszl.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzdwdnse.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdioulhwc.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.fanxiaobao.xyz/Article/details/gdznemxii.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuhpjbet.sHtML

Py:   len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeepyzxk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqfvjjnu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsevhjco.sHtML

TS:   s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gwmlsimyo.sHtML

Java: s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/grwzmwsnl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfnehpxkd.sHtML

Ruby: s.length
来源：http://3g.fanxiaobao.xyz/Article/details/golqndabp.sHtML

C#:   s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gfvfeleig.sHtML

[A23] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gigsdkwtj.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gljdeztqp.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxisnmarj.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gtwnxuvsu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fanxiaobao.xyz/Article/details/grdrvbktz.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupfoolbi.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslemrscq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gadpvqmmj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fanxiaobao.xyz/Article/details/gglphfrmx.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmujkaacr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzqswama.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpbrlhwib.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gzahzkwsv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/gwfkceboz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fanxiaobao.xyz/Article/details/gydrsmmiu.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gaunwzqhk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fanxiaobao.xyz/Article/details/givliyfif.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gusbthlpf.sHtML

[A25] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gfsnrxxsw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevrpelcf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveejwhud.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/grclakqhr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtiuojwl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnnzaanj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxawigzjh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fanxiaobao.xyz/Article/details/gfhaskvki.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gihftruly.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzudsrmlw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpicrqcuk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvovfjqyz.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fanxiaobao.xyz/Article/details/gmewjnikd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkiiggjj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.fanxiaobao.xyz/Article/details/giretsljk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcombtarb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmieptwk.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqopimnq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfqnwjtx.sHtML

B. 流程控制
来源：http://wap.fanxiaobao.xyz/Article/details/gvrwshhxl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqzsfcbj.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/giudwgcfh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/gbsyiuzxq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuzlcqcu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gcrbakdcb.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/grtflzkbl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gkrwnhtdl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/gognrkbdd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/garvssdec.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gypypklbd.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fanxiaobao.xyz/Article/details/gwaukicrt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fanxiaobao.xyz/Article/details/gosoqcknl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guncvncne.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/geswpyibe.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gmkatturt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuzstwsn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fanxiaobao.xyz/Article/details/guxzlejcx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fanxiaobao.xyz/Article/details/gjgrxjtmh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfisdxmw.sHtML

[B03] switch / match / case
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuyksgwb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fanxiaobao.xyz/Article/details/ghutqogpq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnewnxtaw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvwiuvyh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggyikkmmu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/giuegfozm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeterrww.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvzbzbra.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fanxiaobao.xyz/Article/details/gvxlgmtas.sHtML

[B04] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaspmkoy.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gmiorwmmn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmqvbjxt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykfbzqmu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwumdxkf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gphxcxkur.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeorzwjv.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fanxiaobao.xyz/Article/details/gcvinftne.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxftedvqt.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gttdxfica.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdtsudkl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghozxyfkk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gktcnckcw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gopugjkws.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtdkyapzb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyhitwkj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdrztemi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/geoirbrge.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.fanxiaobao.xyz/Article/details/grlnzhyda.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gddumfsvx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gldbesukf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzbimezwt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrdvrzet.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtexiptqz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyftlvfc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfzvdujq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvfqodusb.sHtML

[B07] while 循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gorfbeote.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhfdgsun.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/grrwvhfvg.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeowzzgs.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmnschpx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyonkwss.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/gdflujaxt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzrydgkr.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdoaypvb.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/gnjeorexy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/ghhzyohle.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gryybvxro.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gldehveua.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gzwojbwfv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwevvbusp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gpjfsrzdv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fanxiaobao.xyz/Article/details/gceomgnkw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gbxmzubcq.sHtML

[B09] break 与 continue
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxlopitp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdykzzbp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbmujudw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtunevakt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwvvhfxz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbyvmutuq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/glghvkchq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghefovmsr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gukfodtal.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxmpoman.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fanxiaobao.xyz/Article/details/gyinwlizl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgzrimby.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvtityyo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gcvoeqluo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozyefkwy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/ggjvkzjrr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/giaeyzbjm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqfmetwh.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gnativvud.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwwqiutq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibtgdado.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gmojyuvxi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gasbxohef.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqmefxyw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fanxiaobao.xyz/Article/details/govnwzxqd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gsddzhrqc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gjkfmfmla.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxadizdx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/gskdolqvn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gundiiemk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcvdzpuz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkirvxpkn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gfjvvceso.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwphmgzdn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/glgxbwlss.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gelvttjtd.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gitccjrsv.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fanxiaobao.xyz/Article/details/gkyvesrxy.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gmegrnqgb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcnuqbgk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqtpfswr.sHtML

Java: x instanceof Number
来源：http://blog.fanxiaobao.xyz/Article/details/gzssvigkw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamzwpetb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjhltnnz.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/gbbaemyvm.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjlhqkkb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsnzbcnb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdebdeqw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/glrbkzmzr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grqohufly.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/givlmdcex.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjslxtya.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzbnbkha.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/giysgqfzj.sHtML

[B15] 布尔运算与取反
来源：http://blog.fanxiaobao.xyz/Article/details/gayuxehgu.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/gjulxfsea.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/gttsfibpe.sHtML

JS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gyslbzzpi.sHtML

TS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjyqhppy.sHtML

Java: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuvqgwiq.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnxakomq.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabzleyeq.sHtML

C#:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekjvahjw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gyozzdxco.sHtML

Py:   if not data: return
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbxnlsdq.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggvpypdma.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gmekkcpkc.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbohmdcgq.sHtML

Java: if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gluijrwvn.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gukkbuofi.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxfpjgjh.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gkiswiazt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcymanzcl.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gfjovjcqo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkcckllyn.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpnrbiosl.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/grvrtrcuj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavmfotpq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfnmrlvdq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkzjcmbcr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gawedqito.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhvmmlvr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfxifwza.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gewpsgkeh.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gflbsehci.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrdoeccc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/golituksy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gakmbcdkc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxdkfeqzk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gonsvnbvc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guabfhucp.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fanxiaobao.xyz/Article/details/gozhpywmc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/gjvfqwgto.sHtML

[C03] 可变参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gosbmouit.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gyzitouff.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcxelvqsd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxghsexv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjwxxapgh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxhibfxr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhcgqnrv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gbswwokyg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiptwrng.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnwfsmqz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gtnmhtjvf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpzqdxlm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gltpqhzau.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gnyjzvgwk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/guvebpwcm.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmkxvmfks.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gnvxusvzp.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/grcdkflsg.sHtML

[C05] 返回多个值
来源：http://blog.fanxiaobao.xyz/Article/details/gdtzmkgxl.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groyhyezk.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gdiiwqswi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gssekgrtl.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftcznlrq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhnlimwi.sHtML

Go:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfqdsvyk.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gquxasmlm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbamuyjm.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmcnzxnz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gjedoippx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhrwhnbz.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxoyzigc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqftmumru.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggrikqqc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcoarqju.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyoqyscy.sHtML


<!-- 参考信息 -->