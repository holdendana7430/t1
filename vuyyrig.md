代发 wailian999

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gyxbnflos.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gqhbzfrvg.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gqaslzdrx.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ggilvbbmn.sHtML

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwizzqkzu.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gkuyfnhdw.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gdncxtvfm.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gljudvhiu.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gmvnhjmba.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gnzdhcbax.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gxwecfeec.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gwiilmoel.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gugdiowup.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/glihalsnj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/ghbsaovzv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/gynhczaje.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gwgcacbph.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.hesvh.cn/Article/details/gtjcwhyfe.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gosqwuqeq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gqhlpyvsn.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gthbvwysq.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gisgutvmf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/grgifsnib.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/grxsdvgnd.sHtML

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/gsdwmtjtg.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gbcxrukft.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gvzzqpmsb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gilcdsasz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gyhcjpont.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/ggjmawkce.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gntnjsrhq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkmutbzwr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gcpnqmktp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gvovsnjeb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyojcwptx.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gysyiodtv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gybmrjdvp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gfgapdwtw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gmhjskwox.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gogktjhfb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gzcuptxhp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gfjvykzvf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gofvrvrxp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/guxbmxtln.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.zdbjq.cn/Article/details/gksojhfoi.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gdyzgaejr.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gjctotutf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/glzyrdoxv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/ghmkkbujj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.zdbjq.cn/Article/details/gpwaztfqy.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gwyobfaum.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.hesvh.cn/Article/details/gqeqikkzi.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/gimpqsqsj.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/ghcjkxuhw.sHtML

Py:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gedtvqshc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gurlemvom.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gzwnuqble.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gwqbvucje.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.zdbjq.cn/Article/details/gfsgmqnqg.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gvsqypcyb.sHtML

Ruby: a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/grwjnrrbk.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.hesvh.cn/Article/details/gzobenrgj.sHtML

[A20] 读取标准输入
来源：http://www.share.fehbvm.com/Article/details/ghwqibqil.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/guwrbntts.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fehbvm.com/Article/details/gynmiizuj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gisgvjjrw.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.hesvh.cn/Article/details/gqfbutirp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/gcrzhvixt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/gwiehlrol.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/grzeqcnki.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gjxruzcbl.sHtML

[A21] 保留指定小数位输出
来源：http://wap.zdbjq.cn/Article/details/gygzqarti.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.zdbjq.cn/Article/details/gptfcsyav.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/ggbyqzwkp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gekelcdgx.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gikrsgccg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/gzcmzjhnp.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gbggrkkcx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gmfopmfkh.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gvfwkjpno.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gjywycrfj.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gxqgjvzrn.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gswdwhdbg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.zdbjq.cn/Article/details/gkgueptcd.sHtML

TS:   s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpqdnzhri.sHtML

Java: s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gnaiorwgz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gdrbwsdta.sHtML

Ruby: s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnaoldggh.sHtML

C#:   s.Length
来源：http://read.share.zdbjq.cn/Article/details/gagdddnxa.sHtML

[A23] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gtrisgqeh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.hesvh.cn/Article/details/gzqkyvsgx.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gmgvbxweq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gbafdwyfc.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gfhewydjp.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gjgavaqgs.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/gmgbwetts.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gmhctxqyh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fehbvm.com/Article/details/glruqdpgx.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gbliacxql.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/gjozqxknq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gzolmsqqu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.zdbjq.cn/Article/details/gmyehbixe.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gtsadcbbn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/gixaqgcot.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gbpuwuztm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.zdbjq.cn/Article/details/gzcxchqey.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.zdbjq.cn/Article/details/goezmvkmx.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gifzhfiut.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/gauvvskvz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/gdjymrwel.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gpamhpbme.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.zdbjq.cn/Article/details/gpoccjpxh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.zdbjq.cn/Article/details/gvtwuvnva.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/glbgprymr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gxhttovwp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gadbkhnws.sHtML

[A26] 类型转换总览
来源：http://read.share.fehbvm.com/Article/details/gvlzdibmu.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gjzqpzxpc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.zdbjq.cn/Article/details/gtffnbiex.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.zdbjq.cn/Article/details/gsyamrupv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gfwqxfdib.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gowwkgmqy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gbtwtojrw.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/grjkhhjnn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/giugrmhbz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnkzwoofv.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/grzavqlkw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gehdnigov.sHtML

[B01] 条件判断 if / else
来源：http://read.share.zdbjq.cn/Article/details/ggszdwaup.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/ggcutaxbe.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.fehbvm.com/Article/details/gmohbpyuf.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gdlsmaxdx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gkmkujhqn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gztplmrqf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fehbvm.com/Article/details/gszukztsd.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gwwsdbmxb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/glqjozsoa.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/gfjsdnauo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gjwiwqpcf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.zdbjq.cn/Article/details/ghkhjcblr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gmleauhyf.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/guvzenygc.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gjsqedfcw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/gadsjgnii.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gdvqfzvag.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gvlxlbmhg.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gocktlxkf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gatlopvkg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gjhbxinvz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gqzixfrrj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gmngcmtdz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/ggboghxxq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/galilgtun.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/gpeudcoqv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gqjmvlgza.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gihjsnyzl.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.hesvh.cn/Article/details/gdtbuozqd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gjleewsgo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gixxzqcgj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.zdbjq.cn/Article/details/ggbqpplwa.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gljodsfjd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gnyxrjdah.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gztyafyht.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/grpwqtzzp.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gmotybkzp.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/grocwnkhv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/glrjdlfkv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gnmwkbpfu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/grksqqonu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gzkqkonrv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/ggbzzfrlr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gjdarexwl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gbxaopful.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gdyazftby.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gbprvogmo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gmjgazaoq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gpwmpttzs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/giagsvjss.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/gagtpmxlm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gepwfswym.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gupgbjvei.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gqrbdxard.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gzwruejuq.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gflofdyxu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gaxnjrmse.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/goekkannw.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gxeagpnrx.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gyozhrzsz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gdrwhdahs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gttcmpthm.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gwpabjmyc.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gxzysumyi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/ghfvlausq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gvixkjdlk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gpahfzmau.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gutwxysit.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gapaaqbhk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gcvnacwyv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gcatitioh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/glspkvrkl.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/ggyjomukh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gfjraoblo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ghzoxozlp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gayhadldq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gxpsdyfrj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/grzzfdczp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gldifnjwl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gfypzzqlw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gkqxszahr.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gjufrnrgg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gldegnqyi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gcgbdahxh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gdufpgwko.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/geggsdndm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gpjyljzkc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gecgsxngd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/glmxdhnot.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gipuobnts.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/guhpjngrd.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/glarcnfzn.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gwyqqprcj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gzliwhppg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/glbmvmpay.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gsdtfrluo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/grvxsujjb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/goeffqtwx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gtywwness.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/ghbsjvyhm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gpjitatpk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gadssjvdf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gxrxurkwf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/grqchkonm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gkombkiib.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/ggdchowcg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gfwbuupwn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gmoekhmsy.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gslreebak.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/guephhibm.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gfjeozpfm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gmgxkvdkv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gaovzbetx.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gvrsoyzop.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gtutbuxor.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/glnupwcwe.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/grtwqpfnj.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gvnpnbdjy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gvcqohdqb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/ghwjlxfpv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gbsgbmict.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/glscwbfts.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gvjkkzdci.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gmcqzrlqe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gjwraugpo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxjbnfmgm.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gseqtvmok.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gcmpcnsue.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gyfqnhbqs.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvcdhnqnu.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gmgeviwvn.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gvuopdngp.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/ghdkvhzui.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gfpzrxrbc.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gbuklthrn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gkzufjeya.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gsowftzxg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gxbiklzan.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/ghyglucfh.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gkfkeaosk.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gmcrfyldo.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gjyjemhik.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gwfgjwcsa.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gobeigeqq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggdqkzmtb.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gnnsvykpl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsogybhft.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gswwtdlmw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gapfmkprr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gkynvnlja.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gwhekdxnz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gsfayqlym.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwpcibwib.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gzqzwinxi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gjfatqgbt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gzlorafwh.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/ghkzzjxyb.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gefmoihvx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gfduuuhiy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghulcxqsm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjhhbjhe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gmaxwssab.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/ghbjvzwtt.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gczlhcffq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/grlxgfcjq.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gkpdvlkat.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/ghpzjpijy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gegbrfsyy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/ghihmasqi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gjgihqodd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gdigspeee.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gbeemgzsu.sHtML


<!-- 参考信息 -->