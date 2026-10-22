代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2umkaemlz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ykwvdyeq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2xyfumolp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xfvuzgry.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gcogaucn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hfvzdefe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2frsduspo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ineffzaj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qpgjfpiw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zogdzbze.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pnaxsnvr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bcgciwys.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2plkjveid.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ctjilril.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xzuogowq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2lxongvvi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2nyxizeys.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yebaivbo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2hlwvvxxu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eipyfmsj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2wuoutncm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ilrxnwzd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ifvtdibp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uocmonns.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lnivvruo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2veemrjap.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2acdjrgbb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rzioafis.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hdgzsixq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2emkdzbkj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kvdokppn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ocnpbnhu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2apeyofte.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2comhndyw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2cmropzcm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mnbauxbm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pyrizkus.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfuvkfw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2nzgboiwl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yphotrfo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fendgdqp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fsunglsk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2mwlrvsiw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yzlpifnv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2fnmznbwf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2pprhozrg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wsvivadm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2stdahuag.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zyfjxlfo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mrozbsvo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2apfwwwca.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2iaqmnqlz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kdppwxam.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2khykudha.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dfjbnjxq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zvfhhfxb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ppyecehs.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2clxivndj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2owfvkiep.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2docezfwu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jehigzry.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2esfgatjm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ybhvqtkz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lazzkwbo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ohzdbfjw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vtilerue.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hxwsfqol.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rqnopvld.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sqnpflpd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jrfuylgu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2flfhdnyh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dvktpbgz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2qzpoydsz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wmqnytol.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vlqiumow.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xcqnwyrt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zolrgiin.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ikjhptsp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nsdsbdgk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2drqskhpc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kdxhvnku.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nwwhpnvd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2drzaildx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lqlblyty.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2djteppym.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dtawqrqw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2kvdzoqup.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2dhudiasq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ohtluzfr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lgmusltz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2efongjeb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2zjqpdnal.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2xlosaujz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2wzgaevvv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2tidlzvpx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2vefrrkbg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2dzvehtyr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2nrwztcas.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bmydyjcn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2kksthtbq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2strrkiqv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hyxltwhy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tsuwmikx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2feilenbk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vfphmlhs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jdkxxkeh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xafetmql.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qyfeatob.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2poovfpll.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zwiytfjl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rpknlmsk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2toexzfkp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vgfzxtom.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2yaobjyll.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2locqnzcy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2btkdhmxi.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2mlllhtdp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2mwuhkfpi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2infgqcwo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2eqgublhj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nqhsezzo.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aqubrhct.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2kpglrfxn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rxpfhecy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lkewksrm.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zgrnikro.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2gavkrxwt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vvpuguml.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2fiexxbac.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jisoqyov.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fbfnzvcg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2sslxegrk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2mntscbdy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2zogozhwf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fiiwppdt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ybhyyrar.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2kltefcff.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvqnhnm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nppofkfd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bdloqrta.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vudgobco.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uevqmpix.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nmttlrgj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ujpkxufb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gbjnloeu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2oafiguzl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2lfclxxpi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2iqvmkglq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jfvhlelg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2icorcrhq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2kdqctkbi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kxoszzmu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qijdhpyw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rqrvfgcn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2giaajxgw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2thamieok.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mldcllvl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2elodqaya.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2poixmxgq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2qrsjrjji.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dsvicqle.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ptbauhqg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2kkaudxpk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2exihauyf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2xgwdybqs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vphhiidu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wdyhztih.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xjsmxubz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzgavlw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gimyqbip.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rgliasrg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tbodewqh.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2lrsicyuv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2xzuffbqh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ryzgrile.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2whmwugvl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbriumuu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixjytmfc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2urfgjuce.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xuulmmmq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zfsksrtu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kkdihbph.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qlgzuvqs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2fgxzjmal.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xzfwcqsb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bmndjbkx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zfjkwfnn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2huvvjrpn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tbtegncx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlbmgfoq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jwjkymvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvflzcoc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2oyrnaumw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2enejtayf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2jqgefskk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oatpzuzj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pcclukbh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ajhrcina.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2usgwaxsy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2uznhexiz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kqbvhtpx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2sbfbvtfn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zmhxecqj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qahzniky.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uhhudryr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nwssyire.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hlsfvpvm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2zxavuzkk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dnlfcxsp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2amelsknd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zspwuzow.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2rkszddfh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqwfflsy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dqujdqap.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bwdmuhvt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rrzsybpk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2infuabzk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2avnpdyqe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ebrtejnv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dimkphca.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nquwcrcl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2gdvlyhxe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2taxdtoqc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uzbgzmlg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2vfqdjfpo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kubnsvyg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2nhfxikhj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2jtydbiou.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xukrofgt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2laxdvcjh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzogletm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2etakajjm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2thwhqbkw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxagtcaa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dxzjcvsf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tswxlefc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iemukkfb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uqjqbgxu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ihvkkaqb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hekulxbb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pekwatnh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2smutztrh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vnxljjve.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kmutmxog.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mjtxebnu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqdeklcw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2yeonjyeq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2caqbujhk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pnjlqthz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vjiloqog.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcryonjr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eneccdce.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gqpijhxj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2epigubpa.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovukrtzz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2oyjejobr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2izqxqsru.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pnhauqnf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qtedvuxu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qfmhhuam.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2blnehewo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sbbrrmyj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2grybaclb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2njqiyftf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rgapbkfg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vbqlmexu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2igwdkhai.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vojwoeha.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fetvzymu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyzdlwaq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2npdqegme.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2coduveze.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wpnfhetg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jqxmfvry.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2yhntzqfj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdsawcdd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ykmukgfb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cwavxwcw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2awagcxxi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hsfnwggb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gsiwyims.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbmelppb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2dwmgxwtc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hphabzjo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2otibbubl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2byromehe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yushrtjh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2qqlqwwil.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ilgqtujw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wvnjdkta.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mcvanpqq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fldppnyt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qeerewsj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2cqgkybun.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2khzibywz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cfmjxcqh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bipipemy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2asvxagau.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lgdvguma.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2irjhkuwx.html


<!-- 参考信息 -->