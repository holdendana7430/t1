代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwsfzyr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3djxihwlm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3enqtgtcg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jfuaeakn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tospcfnw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3jztzyrxc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jjmlnrmi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vwzzfzgr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbrnnukh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofwkonbq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rpskmqzo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqkxwrz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eacwobem.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kigskqfq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3akqobuka.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3erjnruiy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lecbzcff.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3hkscidsk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fuilmuse.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pxcqszxt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ymvohtay.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nuimqmnq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qdfxhgge.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qnlbrsct.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3rkianaey.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3gmkyhnbg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jjyxpeci.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sdspnojq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kujkzvdq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3izzoehzi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3njfuvprk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wrlcmaxx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rweydsbq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sqkcfjwl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nqyhzgtt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3zlbewent.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3roynzrsk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ekanhmpe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3swrlzsoi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3yueohkmb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3orstxbud.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ojybdkgr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cqatrdnt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3aalmmoua.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ogunonli.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zoqdzkig.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tijupnpi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zomhfpwg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3urjhjbsy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nzqmukdg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eglpggjb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ufqweloa.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3peynlsup.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3hrsemwgm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3htyrysiw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uevilzwf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nvvkmgac.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3hznryqls.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mosxssgp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tsrjhgti.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hwnlelak.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qifcdiga.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3shqkyjbf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qetuzzmz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eyusujtc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3muhzfexe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3iklgynwu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ljwobkwm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tkohwuzi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kmshkyxa.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ffannfve.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ayoamdcj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rytggbeo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3xhbpxjfx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3murbegqn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3cxymiozp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3izraldhg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3obifieog.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpyqemwx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3pvxhcxvn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykghqtph.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jhsdzsrb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zlnfqjrn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ciktfqgf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qiynckbi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kfudjfjf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mjqymwkd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fztdzdtn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vsvyqpuh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gvqvrkje.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ulihhvcw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ftzlrmyg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3touddhgv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ddvavzgg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rfndnwrr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xjqkkvri.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qvninfri.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3wdfexmkg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vsafvcsc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3noumejrp.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3knmscafn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gtrxmbgb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xsfedxqu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cbjwhain.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ngrhevpo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3wgtblqrk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ngwjmxlt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3lupkbcle.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rrgsweez.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3floxdlcs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eaorffir.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3nutkpjoo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgkjros.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3mfcrgkzc.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wlyjrqbp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3tanfwvxe.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ejnyyhsv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jkfocgcl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3koicnnmu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hsfbmkva.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3idnejqrn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bflbejyq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xfmfbxnv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3csucemmv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xzclrxcs.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrognpym.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hmcfgwka.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mkcyzncv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvbgyiky.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3murzodhg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3fvagzcuv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uxhmotkx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3juwhwfcl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ypksaqin.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3mebohgex.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qcishnbb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wgnrwvmy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zyyendok.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pdvdzevb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itztimpg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3shoguzap.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xguddxnl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3whpxpfiw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3oiyjfjbl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfdgifan.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zvryxjuo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qkhtobqm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3juhuhyeq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnowoobp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ytbnugyl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wbwkmtoz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nxuimmtt.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3bllgqerc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ytbbztxr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjwahxns.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ohqlwgpr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwwpiujn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3svclmkne.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3gbevndhy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ovnuuhdq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3czhgzlxf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3flpmrfex.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3gogzmype.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jopwannh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zekpgslg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wswdujjd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nrhbzndl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3mdeelzgi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qmpyztbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjhnnbky.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3sceykvwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhbigpgx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3uxfmxigz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3obskhgck.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dalgcxll.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nlbezqac.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ddkfxcyf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3crheqlsf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3uqcmznvs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3huvlxxgr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qiohbtlo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zrfxdxjd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3avvjmfze.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3jqqyopgl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mwfhsxas.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3upamenrt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cyhidzqw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mptundlb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qvflkoxm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qdjahjgr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3grbteksw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3aiqpvvsn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ugqhimic.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3trpzkdvf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuhccdbq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eghauivl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ojuyuahp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jwxkfgsr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xjppeoxg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zdrjdnij.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ycbcvsrj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fpquwpfs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3npqdzwbg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3iuutpmcg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3grrvxdmm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3renunvls.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zolggmjd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gutjnjgs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3izkkvsbz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3witeiaem.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebruxahv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ebdfolsh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lircayhr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3doqyrgxg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3twihzzyh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3smrfwcck.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3cnoqzrkw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3azfvhmxg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3uthycgyu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xqdtwqja.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmgzquop.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gltsbera.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kctsqgeh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3odwakqrg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kikcupfj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ahodifnx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hdbwpvev.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3piqrnsvc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tturpnpq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wuiurjol.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3osdljytf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3filvfgys.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3asjiqzyv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jtpbblca.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cpocvkha.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xtfqxvie.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dczjmslr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ztkamyve.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zugtzqkf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fhythaoi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ulirxpbw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3livtygdm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3nqddtaqx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wbfbsszv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3hncdtgnz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bvbgstwg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cqjsmizr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqtqfeui.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwjyctsz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3myobafrk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tqmysmwn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpoqaaec.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3klqgayqh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fidssoty.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gipqnqpi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkwgmvex.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3opapwsih.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kmgpotgv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3etfswahi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uheycggm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sihofuih.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qhdmyhss.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3wtpbmbxy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pooxxmlj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ormtvdeo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xzyymkzc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bxvodbmy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3sssvmvne.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3regwatmv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3oydjlvlr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ynoicsgl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3khuuyspn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wdxkdxpp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3stvguhny.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dzcqztzr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3butqxjgq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tyvpnhqd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgpzmrva.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3eaqnvgij.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tdddohop.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3idkwitsj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zrcljycx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wilqftrp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqspjup.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qyiwryuq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3yjqmepfp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dmbkgatx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jpmdehww.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3scixweln.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tiyfpiby.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tdxwoijd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rlpsarfn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3egxybmbv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhvpgqbt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lszcnqyf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmznkzv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxeuomb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gzxivnkc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tzzpnthm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mflqmhfl.html


<!-- 参考信息 -->