代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gatjxcunv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gebuoqpvy.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/gnrzxlwyp.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gnojhmikz.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gromfuplj.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/glgwpmoia.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gtairubcr.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjwpyiiot.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gkzvtbynx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gjmdophwr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gcrzseszz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/gpsjfafek.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gxknuffca.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzzavgn.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/ggtpskfac.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.hesvh.cn/Article/details/gobjzkfqk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/gvlaxrdhu.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gzqxoijju.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gkwpgcvnn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gfzgzpics.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gtuqciiur.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gghidbvxq.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gtcymeeia.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gzuskslzc.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gjuxrgaoo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/griocclnm.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gdycdccfk.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gqgtpdoae.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gknmmgfof.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gxjvkwaxn.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/goxhusaoo.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gdrtsvmvf.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gyxjphbcq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gsdmsyhyk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gheshigyk.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gwflfeaxy.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gxyuygrlk.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/gegpwxtfc.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gzpazdlls.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gwskuomqm.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gkrctalmu.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/grydtjypf.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gvnwfwibf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gncplkqsw.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gsmdedhxp.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/giqwxpccv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gsdanpovj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/gestlbfto.sHtML

Ruby: value = data || "默认值"
来源：http://wap.hesvh.cn/Article/details/gmghrmzkf.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gjcbkmvgz.sHtML

[A16] 真假值判断规则
来源：http://www.share.fehbvm.com/Article/details/gvifgrjcq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/grhvaxbes.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/grfnjains.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gmdmmlbzy.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/gxrfzregr.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gwmlgvyqh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/gourtpphk.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gnfkgvxlr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.zdbjq.cn/Article/details/gwptnvxaa.sHtML

[A17] 位运算
来源：http://3g.hesvh.cn/Article/details/gqpqtwexc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gaufbxtnd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/genchnrgw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gombozqnk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gmxpeofiz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfquqiajg.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gumzzramz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gnvmspitj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gyautoasb.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.hesvh.cn/Article/details/gjcdjmaci.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/golljugib.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/gykayvosc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/givcdfrmb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/ggxofaolg.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gxsgymhqu.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/gzdtacuoi.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.zdbjq.cn/Article/details/gctbndzgg.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.zdbjq.cn/Article/details/gfzaahsfe.sHtML

[A19] 交换两个变量
来源：http://www.share.fehbvm.com/Article/details/ggioatbuj.sHtML

Py:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gucehxarw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gmrlcvxpf.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.fehbvm.com/Article/details/gpcetdxda.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gqdofamyy.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fehbvm.com/Article/details/gorwhhqmo.sHtML

Go:   a, b = b, a
来源：http://www.share.zdbjq.cn/Article/details/gdwblpram.sHtML

Ruby: a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gjzeaqisi.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.zdbjq.cn/Article/details/ggfmuecgv.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/grwnquonl.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fehbvm.com/Article/details/gsrrwlaae.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.zdbjq.cn/Article/details/grxlatzvl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://blog.zdbjq.cn/Article/details/ggalbcmwd.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/gxkhetsbi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gxevkkboa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqieccbn.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/gwotzyjfh.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/gqdvggnrs.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/gheuaygwd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fehbvm.com/Article/details/gutpvdyni.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/giululhqd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gpmpyewjl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/grytcagsd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gkvzfhjil.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gvhzphtgf.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/glmvkxovz.sHtML

C#:   3.14159.ToString("F2")
来源：http://3g.zdbjq.cn/Article/details/gvcpqasja.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gfibckcie.sHtML

Py:   len(s)
来源：http://www.share.zdbjq.cn/Article/details/gfscvnntq.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.zdbjq.cn/Article/details/gxznjgwzu.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gwkepxrre.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gptacrady.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/gfwdaitra.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.hesvh.cn/Article/details/gvqydahvx.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/gaimiseix.sHtML

C#:   s.Length
来源：http://www.share.zdbjq.cn/Article/details/gatpdkjzv.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gsxnlmbmk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gozmffgsy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/gxvrpwlzb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/gvflbaspl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gqkuititi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gityfnocm.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.zdbjq.cn/Article/details/gdpilnqfs.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gqecrahvt.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gcnxnwaqx.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/gcumxuohl.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.fehbvm.com/Article/details/glcfdhezt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gvsmptdvj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gluhwmmhk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gujkqqpvn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.zdbjq.cn/Article/details/gnupnkitu.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.zdbjq.cn/Article/details/gkxpsmkkd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.zdbjq.cn/Article/details/gixgcblpe.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gugijlnma.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gylneciql.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.fehbvm.com/Article/details/gzeyfdyxz.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fehbvm.com/Article/details/gzoqtowkn.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.hesvh.cn/Article/details/gugerktpa.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.hesvh.cn/Article/details/gtdkplsta.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fehbvm.com/Article/details/gkuscddmh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/glkudrjgk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gseripvyt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gbvqpstcq.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/ghsixsrja.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/giksolfoo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/gjkebnkjo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gcwizbbem.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/gxgudhryo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gmiwwmadq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/grmfdprhk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/glcdxohmm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gcwpohuad.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glivadegd.sHtML

B. 流程控制
来源：http://mobile.fehbvm.com/Article/details/glvdmvkvd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvbvgktvo.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/glnhyvgjy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gmlpzjtqi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.zdbjq.cn/Article/details/gmucnwtgv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/grxqvuwba.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gyexnsinu.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gunslufeb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gstyunqge.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gdezluqee.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gcywzpwhu.sHtML

[B02] 多分支 else if / elif
来源：http://wap.hesvh.cn/Article/details/gvtzogybc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/glmnmujdq.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.zdbjq.cn/Article/details/gagtxbfej.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/goegkzypu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gudmavfkn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gvtmirqqv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/guipbzufl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gorwjaibn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gipxqhtjg.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/gsrzrbgia.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/geuguohah.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gafimculm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/glcszoedh.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gstflfkeo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gezpvbafg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gzojbpefe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.hesvh.cn/Article/details/gjmwjwngr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.hesvh.cn/Article/details/gjtfwnlcw.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gheldfozc.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gyeuksbxc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/ghkcvxixv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gyqzjkuhg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gqaykurfe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/glyxpdfpw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fehbvm.com/Article/details/gcbgcgpgo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gwfhvfznj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/ggzelcvsl.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gvihbecyi.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gsfoaggts.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gwiqoesyf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gaybgehgj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gittxxnqw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/ghwujomzg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/glosqaisn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/gaodzagyz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gvcuijnpe.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/glgtmisru.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/ggdpeyjwg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/ganbraonb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/guyizhrgw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gwngluwzy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gnbscnmrf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gzeodezgz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/ggmwrnyiz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gybpdynez.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gamdghkrs.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/glrhsmkmd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/glklqmtpi.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gegtkmeav.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/garatzvnr.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/glkopnuhg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gwvfhqupx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/glufahmse.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gzxjikpmo.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gqlwfkyir.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/grwowhghd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gvelfxigf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gtvdrnici.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gqkkaftdo.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gvuzanahr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/glcmyrcfx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gsdldbszg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ghkhzfdvy.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/goaurpgyd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gfblftjcu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/grsnslhfd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gventhsfe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gtsoaeipw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/govhyveqg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gygasyfgi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gzzxfbmsf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ggtovczzr.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gwrartnja.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gukiptgeg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gsppfepvd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/grfusbzsn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gtljatxmg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gunmciurl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/ggryacqjw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gxgteakcg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/glwwuijxs.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gdcgsiswq.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gjsyrceux.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvrukgdum.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gdorqqjfx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gpvpmcylv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gjyaoconc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gublhaaom.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/geimcesyg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gjostikiq.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gglnsoqgd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/grlzvakuz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gsgvevhxw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gizzsnwxu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/ggbjzfdjz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gplsemvmy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gswfxluqn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gggpocghz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gdwvzhzmp.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/grnttoppy.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/ggzkfwxmu.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/gikwvupsa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gzrgmlhzg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gkqlywswt.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gndlwcpbm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/giunsqbop.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gxyvguzvd.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gxatzlsbx.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gmwngzegz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gwcggqefz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gcawrdbou.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/ghxbhqsou.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqxxdzqyf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlymdotp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/ghbpugpgz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/grgawwnbb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyubbbqub.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gswblbbyi.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gqgjrfvmm.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gkiiwbgcc.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gfflczpgm.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ggmgjxcfn.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjnodisxy.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gawxvwcpd.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gqdwjnvde.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gkvkvmmkc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gnbktgyid.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/ggmlqnnrw.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gdrlozbok.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gxngfmqat.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gajztsyfj.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gowforuxd.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gasygtpxm.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/grgsoriie.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gywlonxzg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guqmivcjf.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gukbdxclh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjdszdxrt.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gnpfyviqt.sHtML


<!-- 参考信息 -->