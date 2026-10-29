代发 wailian999

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gqdjdtwrg.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gqaudspcg.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gxyrtippl.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gbblnhndr.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gkdsiwvpw.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gndfskfoq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/grncxekof.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gxppgqqxp.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ghzotqhzg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gwqxutkar.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gnfufhqby.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gzvbvjmgf.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gvftcxpxr.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gwiouekah.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gevsvpdve.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gbtryapeb.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gyuqpiaxv.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gmrbzzqyi.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/glildwlkk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/grjafvyyp.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gdvbtzydl.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gqacfbqgk.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gooxpnsle.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/ghoxsagvk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gubltqchm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.hesvh.cn/Article/details/gjaomvbcw.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gccbhpgyr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/gmczrqors.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/gcmnsepyq.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gwukeuctm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gvzfqellp.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/gemlhethf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gqlkxcyqu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gapnxdlwe.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gllivjpry.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/goiraichu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gaqnocmgy.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/giglafwnf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gqqqldvrz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwizwydob.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.zdbjq.cn/Article/details/gknshipbs.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gfpjmtnwn.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/glyjrhhyn.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/grufrlhsq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gmgmmpvkd.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/ggjfaftqo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/glmlfgwjy.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gqrdaspza.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fehbvm.com/Article/details/gdrhitzvh.sHtML

[A19] 交换两个变量
来源：http://www.blog.fehbvm.com/Article/details/ggcpktyvf.sHtML

Py:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gqfxrbxuu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.fehbvm.com/Article/details/gcvwubaty.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gxueqksgo.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/guldjyfgx.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/galhyxxvo.sHtML

Go:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gzbjfdyku.sHtML

Ruby: a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gqwhpbfkr.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gpwoqlitl.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gynhhsccr.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gvmhzdeau.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/gpmskizlu.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gqbjjchmz.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gpudmssqz.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gofxmqfdf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/gjjweqwcc.sHtML

Ruby: gets.chomp
来源：http://read.share.fehbvm.com/Article/details/gkushyrem.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/gyozmwspe.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gdlrlkddr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/gvtgbxipa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gpmvmjkyf.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gkoeueijn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gwfuitshg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gciaextgn.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gkwiuipgz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gfqgqnbui.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.hesvh.cn/Article/details/ggzznctpx.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gaofoncgo.sHtML

Py:   len(s)
来源：http://m.share.hesvh.cn/Article/details/gvifgmagg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/gmqplgqbx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/giwcoxnly.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gqeifrasl.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gevynqgab.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gddespasi.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/gmkmjidrg.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gybospjdp.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gbiilicmd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/ghtmkptbs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.hesvh.cn/Article/details/gsuiixtiy.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gnbntnqnm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gfzztmnsg.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gqmodbzbg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/gskxeplrb.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gjhtrwufl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gfeytslte.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/gbgcbasyl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/glfljcehz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gsvqivgdp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gnwaznlyb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gmmkdvxah.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/gtivscaba.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/gxyjrldxo.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/ghpuvthcm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/goqjnjzem.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gpgrcnsvg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/gcwhmyapp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gxnczzilg.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/goqtwoxtm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/ggduxbgsy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.fehbvm.com/Article/details/gmbpokiwc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/gjdgrypih.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.hesvh.cn/Article/details/gukcpgvko.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fehbvm.com/Article/details/gstsybkpp.sHtML

[A26] 类型转换总览
来源：http://3g.fehbvm.com/Article/details/gmzqlskuc.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gvtnsblwi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/gzbrwyaie.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/ggcnlnhqq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gvsmootqr.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gvjkaiyjr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gzqlzsakz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/gvyptawgq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/guschvwnr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glljksexa.sHtML

B. 流程控制
来源：http://www.m.share.fehbvm.com/Article/details/gwbakegdl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gswpheqxd.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gfqxbeefu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/getypjbxb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/giioopdtj.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gkdfypqxx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/ggzookasx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gvrkegyuj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gzawpvmgn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gemztqmuy.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/ghbvgxfjp.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gwamlpzug.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gqqqhmtyg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/giszzxuea.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gazpdvnob.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/giycbiipd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/giljhlnkp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gdyvjymjj.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fehbvm.com/Article/details/ghxlppsfn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gdtklueyg.sHtML

[B03] switch / match / case
来源：http://www.m.share.zdbjq.cn/Article/details/ghxlmoqoh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gmpobqyyq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/goooalsdq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gaeykkezz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/geqjeqgyh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gdtjfnuso.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/glsqsihsm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fehbvm.com/Article/details/gkofbgvev.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.zdbjq.cn/Article/details/gzewnopat.sHtML

[B04] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/giptxdmhp.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gqeiimrxr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gabupdzzw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gstyzhwah.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gqpchrxos.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gwkmdbtpp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gohqhurbi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gaalbbguk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/glugxgnez.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gdxvcjbqr.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/guewznmln.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gysebmvot.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gmaxohwye.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/grjppauzr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gynjdmcft.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/gjurrwfze.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gqesvabbe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/grpsjjvmz.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gcjfjxeid.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gocincqgh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gflcsnnbv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gjxqlicbd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/ghwyirhdq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gehdkmpuv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/grjigwphj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/ggypmitws.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gnaqqquic.sHtML

[B07] while 循环
来源：http://read.share.fehbvm.com/Article/details/gtsxlojti.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gxdsrdinu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/glstpzrbs.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/ganfgruet.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gcdirjegw.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/guagbkctv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gkujmzkrn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/ggxtdcqal.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/guzwilxue.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/ggfgtsyhx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gosmokyds.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/guntspnit.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/getkuxqlk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbvkcvwsh.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbdtuoixz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gombotosi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gjkuzvfit.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gyukbpycu.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gbanvveyo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gyabwzwwj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbtcanrka.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/grpkxdebn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ggvjiegwu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gfoiwottl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gscsgsiho.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gfjufvmip.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gibbieaoh.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gfjondbnj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gsovtnhbw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/ghvwbwazd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gzgrjqrtj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gxddbwpzt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gzjfungaf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gmqftempu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjjzwzhj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/ghkfwxwwr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/goqwgybda.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/galqldlrm.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gftyrlzjm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gtatsyhwk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwafvce.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/ghxoejufi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gwfjjfsud.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gmwtpmhwi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gfblnlimr.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gifribydk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gesqgglps.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gputoaavs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/glgbxtsqz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gplbnnbpa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gihczmglw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gzxttjjyb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gqtdyrxxc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gttnyrurp.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/ghmqxncye.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gdmdmahhm.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gfoeenezw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gdpsujafu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdhcyzpyg.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gkdrnazlz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gnciucdvh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/galremehj.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gfbwfczcy.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gxuftqjel.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ghzoycnfl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gcycsbdze.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqolpaeml.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gthdpnuzz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gnazoogno.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gkqlpoden.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gluxwulij.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gvznvrrmi.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gujimfbkz.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gecpygweg.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gxlwpjwui.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gvnogntbq.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gdqfrcrfp.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/goywmepgg.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gdfycasox.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gebsqismc.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gpzdhlquo.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gekzqtchq.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gnlodvlop.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gsjukxyxa.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gczpcliok.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gqfceqkwz.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gsusmxrvc.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/guconrhdz.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gecamntzk.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gxiicetzh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gavmyjesv.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gjhqgbwmu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdkkyqqfb.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gdkqvtmnj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gjxyhceps.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gsxczsykb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmxdzcaid.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwfitcqjx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gynvpoglt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/gsvzhkgcp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gtsbrsgof.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gworqwncp.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gjgevvbpj.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gdmnzbocr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gbcycydqk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gmwasdkco.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrodfefl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gxrvonhym.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmcfvppxj.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gxcjsqzxr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gtohszoee.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gxaeysptx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/glogykivz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/grcroojtt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/ghyngdfqf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gfamrtfkm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gyedjgdde.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gjktreipf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gfuuoplxs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/guqyhknww.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gbypmdkdp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/goagicfze.sHtML


<!-- 参考信息 -->