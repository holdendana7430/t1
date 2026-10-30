代发 wailian999

[A10] 生成随机数
来源：http://m.share.zdbjq.cn/Article/details/gkodsxxdz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gvpukymmm.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/guxyvsbbr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gmbazlbkw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gdowuharp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/golpuxroz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gopgwoggc.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gufzsuckt.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gookgdyrn.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/ghrwvssms.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gbbdmpxls.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gcytjzwvy.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gsaopgxba.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gmmtxvlxb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/giytvdmnh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/gjghwyvmp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/grdexzufp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gusavdacj.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/gsjumxkla.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gqcirbexf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gruauryhv.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gqhxtfyeb.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gwmmasxhx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gmilndrvj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/gxjknkmea.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/guaphsdta.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/ggsdgzpyh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/ggbshlbpl.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gimoftdti.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gvgwfgkoc.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gintjghoh.sHtML

TS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gfoxsldeq.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gxosvxrxh.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gprmocmmc.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gxataoldc.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gzqhnbdkw.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gupkuqcwp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gdlajtvmi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gzcovckku.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gwcvkgkym.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gapyzistq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gbguseutm.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gbuopvzxz.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/giwjdymat.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gtrxyxifa.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gqtlqnbkt.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gdtephafq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gnwmjnduk.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gqgaxzdtk.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gisurqzea.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/gznbsmywi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.hesvh.cn/Article/details/gkqlycjfp.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gvdaydzmf.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gioocrwkk.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/goepawkcx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/gdvdinsya.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gyrklqlvt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/gxfikfimz.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/guvpzmhad.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.zdbjq.cn/Article/details/gyhpnqnmd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gzpllpvpx.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/gzfxzbanf.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/geqzqtlid.sHtML

[A17] 位运算
来源：http://3g.hesvh.cn/Article/details/gzingconl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzcexoijc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fehbvm.com/Article/details/gqbxvmuct.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gxmtrhexz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gvhzvduug.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/ghhtfmnga.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gzadwwdjp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gxojybbeq.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/grykgfurs.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gglasypsn.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gwoxmujdk.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fehbvm.com/Article/details/gufwaudom.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gkzgqwict.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/gexmoafvv.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gbnqvrnif.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gwznqalss.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.fehbvm.com/Article/details/gtdhvyokm.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gudmehqmk.sHtML

[A19] 交换两个变量
来源：http://wap.hesvh.cn/Article/details/gbczbvtmf.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gfddojrqz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.zdbjq.cn/Article/details/gupbemvgn.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gwmxceaxp.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/glswnztwj.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/grydfotaw.sHtML

Go:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/goykjgeix.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/grijlxfga.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/gqvhbfsbh.sHtML

[A20] 读取标准输入
来源：http://3g.hesvh.cn/Article/details/godullbsf.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/gmoudkrhh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://blog.hesvh.cn/Article/details/grdfheese.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.hesvh.cn/Article/details/gqneboqrd.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gdctnjjvg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/gdzuaehcv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gmnhhbrzb.sHtML

Ruby: gets.chomp
来源：http://www.share.hesvh.cn/Article/details/getzzwvur.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fehbvm.com/Article/details/gjotnewfy.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/godwghdya.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/giestyirp.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gasjxypio.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gimtotnvr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gjvknqrum.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gvradwqji.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/gyreogqin.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/getpqpywr.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fehbvm.com/Article/details/gasswdqnf.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gnsizuzvx.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gwzrcrycs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.zdbjq.cn/Article/details/gkhelygbn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/gbkrwsxwx.sHtML

TS:   s.length
来源：http://www.share.fehbvm.com/Article/details/gppnznmck.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/gqlykfqal.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.hesvh.cn/Article/details/ggzeucmhj.sHtML

Ruby: s.length
来源：http://www.blog.hesvh.cn/Article/details/gzyojdnnn.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/gtnfsmihq.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gmysnmmxr.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gzmeqvnez.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gcwcrshbw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gfdmisjnk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/glnlmsapu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gceizleux.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.zdbjq.cn/Article/details/gaznjttbk.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gijarkygk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gdsxrbrfk.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gvkolwmvk.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.zdbjq.cn/Article/details/gufonviqe.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gthglsoxw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gosiewpvz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gdbiwvewz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/ghubvozcq.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gdjppomwb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.zdbjq.cn/Article/details/ggvbotmjc.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.hesvh.cn/Article/details/gyoqtxlok.sHtML

[A25] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gxvgyrudw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.hesvh.cn/Article/details/glebwekgb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.zdbjq.cn/Article/details/grtnpmnok.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/grzotpgmd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/ggzenfzcv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gthppingo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gdhpijayz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fehbvm.com/Article/details/gegreplvl.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.zdbjq.cn/Article/details/govvamsao.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/grcxbwwbh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gqccmwhne.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.zdbjq.cn/Article/details/gdefhayaj.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.zdbjq.cn/Article/details/gptdfzujx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/gfgtapsza.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/ghujredvj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.hesvh.cn/Article/details/gqoogvhki.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gbniynzqx.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/giwgetcvs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbnlzxltn.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/ggxmglwap.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjgopeyvb.sHtML

[B01] 条件判断 if / else
来源：http://3g.zdbjq.cn/Article/details/ggdyyqkjb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.zdbjq.cn/Article/details/gcclulkut.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gknhyvozx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/ghvnvwwnk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gwgcflmim.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gtizumuil.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.zdbjq.cn/Article/details/gsykrqypq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.hesvh.cn/Article/details/gzjvxmerl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gmpxjxkpf.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gilpbrjuk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.hesvh.cn/Article/details/ggoyjfmna.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gsmdpifyk.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gkgziwdcj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gajbeaacd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gfzplmmye.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gxykgidtm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/gyhxrjokt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gktikzjxv.sHtML

[B03] switch / match / case
来源：http://baike.hesvh.cn/Article/details/gcgshzsja.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/grfepohkl.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gmveatlmy.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/ggkhlxuax.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghaknwxxv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/guaqtnmuu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gkckofead.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gflfxgrub.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gchqxiorj.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gpnxnosko.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/gauyermix.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gqbtofaij.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gfuxnhotd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gsjvhcmxz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gswojxrmg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gkaaahbrc.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/gcbbygqil.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gzfnrwdiw.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gmkcqawez.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/gzzogzakr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gnuqojpqt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/giejrhifq.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gggrecanw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gwdhxonux.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gimfgiopy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gksfcqkwp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gimgjaxhx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/ggnmgefte.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gigvuovfd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gngjqzzex.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gkkweebzt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gwcixcpqz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gxluxhsmn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gbywbrhmo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gcdnmlffv.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/gupwatbgk.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/govkwnqgi.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gjmaqhuny.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gmpmovmeb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gyhchuvhc.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gyhrwuzmt.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gyrvzjqlc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gngbbltfo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/goyzbemmf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gaimnmiai.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gfkdmfkdz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gqswwarry.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gpbtegznh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gyjjerudp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gdwzxljae.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gdplndpbl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gxgsleywq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gjoxevxpn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gthxdzygg.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gmfsdcgwb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/giuzzoohf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/guvkntmac.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/glqessept.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gcysdcvfb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gxxvurwsu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gzrguffuf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/ganhglqsu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gpnxsdcus.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gsgnvzslf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gzhritjhk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gltovcguq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gokcdswnx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gdgliqmgu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gwustcgey.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gnkfyacpj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gevhdqgvx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gmahsgqzk.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/ghfdqkaxv.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gdjskbrsi.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gcrgzejnc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gatajzhmu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gvhhlmufe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbiejhvss.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/ggesjscqf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gtxofysed.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwbdiwuxv.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/ggfmuvscz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gynqlszie.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gsxkeazhw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gtnbrehwy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gczcekojb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gfcvldfag.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gphjhrwfj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/grikfanil.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/ghisftztw.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gvmdthnqr.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gvlmhevqy.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gnpttueqq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gteryoccu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gzmjhtksn.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gryfetbmd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gcwpjpfgk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gwxntkdtf.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gfddydwia.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gkhosdipv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gkeofvaww.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gzalizwkq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/guncgpsdq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gxrvroflx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/glqdywcej.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gingqaaln.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gokcxsanh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gowcjzmza.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gwzcqwpuf.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gpqluowzs.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gpzlvneyj.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gtqjslzvz.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkncpmmwh.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ghaxaencq.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gidbpupda.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcqfzifhn.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gvwytwphz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gcpcazcwt.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gnyytfjek.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gtxjabaiv.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gpdwoyaqz.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gcbxvhxar.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gyfhezwyc.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/glkxvgkni.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gnvjyzwsz.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gtkhbrqqp.sHtML


<!-- 参考信息 -->