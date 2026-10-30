代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/grqqmnlee.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gfaflzjtd.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gcgcjtnya.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gjjozlazl.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/garyptqoe.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gxfgbyzts.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gllmajpqz.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gpmegjkiu.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gwoobppiy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/gynblampt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/ghdrktzzj.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gugosicxs.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gyvyvlfqp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/gvdnwbqee.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gjtoxxupd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.hesvh.cn/Article/details/gnjjkruhh.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gtrlxseme.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/gkaauzpsq.sHtML

Py:   value = data or "默认值"
来源：http://wap.zdbjq.cn/Article/details/gfjtdekwy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gsckfdeoi.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gvpvsebrl.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gpdxpemoa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/geumawkwb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gulewammu.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gwarrmyoh.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/guyzmenyl.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/grsurkmgw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gbltznkzk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/geuruogeb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/ggmrbamzm.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gbkjhkkya.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/gsowshipb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.zdbjq.cn/Article/details/gafxuhatr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gmbsgqcza.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fehbvm.com/Article/details/gmhddwahb.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gcezbyhjz.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gecsozqdv.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/grpduagsj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gbizxsbqv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gontaqffk.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/ghsdiduhv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gkpbocjcd.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gqskxldps.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gtmjbfbkj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fehbvm.com/Article/details/ginygroax.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gjmjddddv.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gchxegmwj.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gbqxcrwuq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gkcxizycn.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gcrvnwvlz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fehbvm.com/Article/details/gdrzcjlev.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fehbvm.com/Article/details/gswrxqwkj.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.zdbjq.cn/Article/details/gybyaufpg.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gufcmifig.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gxmbbrtvi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/gxmufztbd.sHtML

JS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gfvmlpftd.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/geqqntnzt.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fehbvm.com/Article/details/gexopaufy.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gcntbhaci.sHtML

Ruby: a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gtumimeil.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.zdbjq.cn/Article/details/gcuzdcrfw.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gtmkpgsma.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/glaovfxwr.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.zdbjq.cn/Article/details/gyedgpqdw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fehbvm.com/Article/details/guvrlifjn.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gofpusfem.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gkbvoijek.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/grdgqwumn.sHtML

Ruby: gets.chomp
来源：http://www.blog.hesvh.cn/Article/details/gvgmqmnae.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.zdbjq.cn/Article/details/gtwskbynj.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/gwdzqqpqt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.hesvh.cn/Article/details/gwmfuvkqd.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gnvbizpmc.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gkuljhuzl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gjawwykpg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/goekkccsw.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gedsumjwp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gcenvnyca.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fehbvm.com/Article/details/giiwoptkv.sHtML

[A22] 获取字符串长度
来源：http://m.share.hesvh.cn/Article/details/gkdphjqrc.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/gzvaimrss.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.hesvh.cn/Article/details/gtndhhkkd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gpqnrfpkc.sHtML

TS:   s.length
来源：http://www.blog.zdbjq.cn/Article/details/gagbyfchw.sHtML

Java: s.length()
来源：http://wap.hesvh.cn/Article/details/gdfjzqsun.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.zdbjq.cn/Article/details/ggghhgodg.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gveamrtby.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gzjhudjho.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gknribogn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gmwjpywzq.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/giufedcnb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gfzxjcaee.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/giygzuryw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gqvchrain.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.fehbvm.com/Article/details/gersxdukw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gihywybvu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.zdbjq.cn/Article/details/gfcdchsuw.sHtML

[A24] 去除首尾空白
来源：http://www.blog.hesvh.cn/Article/details/geirqqakf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.hesvh.cn/Article/details/gcdyniobn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gwrzcicqo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gzpdlyphf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gomdanbcl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gvqwqcnzy.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gmfaverxu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fehbvm.com/Article/details/gglzojtog.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/grjqdbize.sHtML

[A25] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gmobfenwi.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/gcmoukecu.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gqnlgkzos.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gphdujxbw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gcffqnaav.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.hesvh.cn/Article/details/goheuqruo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gsuatxzvn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.zdbjq.cn/Article/details/gvbwcveqh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/gbyykzblj.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/galxbgvew.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.zdbjq.cn/Article/details/gqinyuxlh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gqebjyntf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.fehbvm.com/Article/details/gaqrlyqdp.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/gekyfkcxo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gvjnqajjw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gzlxggrsz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/goggtmmzz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gloguzcgd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gspmpylpa.sHtML

B. 流程控制
来源：http://www.m.share.fehbvm.com/Article/details/gkutburdj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpedsuvea.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/ggmwvlmpw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gvtyomjze.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/grtdpggna.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/givnhswbl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gthdspsmd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gjcnktqek.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.fehbvm.com/Article/details/gjiivbxnj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.hesvh.cn/Article/details/gqddmbyxs.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gvnborgib.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/giioonnti.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gjdqkyqkx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gcewefiud.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gvcgfwoht.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gixfrizka.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gvytqyqsj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gfvpjwqno.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/glucyxgzc.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gwhwuneis.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/gkmutdppg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/giwkihytp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gfzdfrycf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gzjdujpwl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gkvoijhrz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gjfweezfl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/glaszgvax.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gyqyaetnl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.hesvh.cn/Article/details/gvjwakfqw.sHtML

[B04] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gtpxfccjl.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/gjejnfmrj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/geedgtned.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gcoupsosl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gcxjbjxif.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gzbfiwdbe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvknupbnd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gbqiikhvr.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gggusmknn.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gzhhewwzo.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.hesvh.cn/Article/details/gihuvqrtt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.hesvh.cn/Article/details/goilstkkt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gdjuyeowi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gryljakai.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gjbqobnaq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gbpoidxhp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gzgjxtxqf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fehbvm.com/Article/details/gwrbydybg.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gvzmerwtt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gdpdcfbee.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyttgthju.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gfbkxpylb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gadlabmhg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gojamtfqj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gafalcpjl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/gqohzkrkl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gsptiwwbt.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/ghbpyswqz.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gpenaclre.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gcwxtmsvd.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gwklnpcpz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gzryqxrxf.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/ggyfmzhej.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/ggzmccuug.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gpiknzrrq.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gmlqadodw.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gwqccreds.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gulgghwud.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gcguahrpc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gqnrulxdc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gpicfxtbb.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gautziaue.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gwneuclme.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/ggjwhsdnc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gzfhjtcgd.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gpsqgwjcr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/gjvbvoagj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gziuqbkhg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gzkbwwmgr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/galxgaijd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/goumyworr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gbvrsitzl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/godzhrpml.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/guouswvfh.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gzcxgtugh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gvqugqmaj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gohldkdiq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gaiwuiuzh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gchusntas.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gzdotkdfi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gvizztbav.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/grvzaxlda.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gumoqgajp.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gbytnfabo.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/gguifxvmf.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gmhubzqju.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gdysjiscv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gzhguxxyt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gxfjslgfq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/grwnkpmtz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gftmyypqx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gizsvdzto.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gcdzjfhqp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/ggiudimsh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gveraeppo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gfivfqccg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gsfmobpfu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gffoueeco.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/grrqetcvb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gsuhhmetw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/givdrxhip.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gqrzmtukw.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gqfgpchwl.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gypflalga.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gliislktg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gsrwqzebc.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gnzszrika.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/ghcclxzlh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gwgjabavv.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gpipojpjw.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gseemcrbb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gkcqtlzot.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gvyaeujtx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gxncolxfr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqahdnvv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gqyktdyij.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/geofxfgvg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/ghmetfxcs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxbmwvujv.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gfjxraxgc.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gvemyrgvb.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gxwpbbasx.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gkvtxllap.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gyziywatn.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/grkwhlxtr.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqzhhphxo.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gzqvkzboo.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gjdeuznva.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gayaqdvqq.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gnpcmnuyv.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/glcvfmrhl.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gzawojxmk.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gqcidgafn.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gpynsjnly.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gmvqxyjee.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gfqgurrle.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gbjlwjyuo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guwuriehh.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gpqelaqcs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvfyuybah.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gpngppbcn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gtyjnqqyu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gbavrrqgf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkwozqwcr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/grfkfbvcl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdfdcgcda.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/glevkkgma.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gfgesazvv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gjkmxyalf.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gqjeegttg.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/ggdvfucih.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gflhndasp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gxszhgbyu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gqgoprxza.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gqrggrqjm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gfcsgztmu.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gnwkxsccg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gzhffqaqu.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gocjgsnxz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gvprgwjol.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/guvpbxayq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gkmzrexvg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/ginvxuwih.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gxofryweg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gyozbfcyu.sHtML


<!-- 参考信息 -->