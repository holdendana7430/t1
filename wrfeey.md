代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lmveutxj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2pncuhgiy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nfannsix.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2hfqlnzlo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hvtxevff.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjtnagp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ikqcsjhi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypjmuchq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgoxteng.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rvzfllmk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2saadxdoe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2codafpuz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nhvgovkf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2mgupftmp.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2vucbcdkz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sdnptkei.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2odrbswop.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2atqefoug.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wtrnsiry.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2cjoctogr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2udvgxinr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kqadvifh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tdwtfxmi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mnvzimgr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ejvsgjfk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qalftegd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qsprovga.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jebrkaxn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mczmszoq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ickzcows.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2avtcgoxd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgqcxbqd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2fnannqkh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hahjbluu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ryuwvkiv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zzktvjek.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xsrhjkpe.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qlnttwec.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2jbvuiyxa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2rzgcuxko.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vkewofsw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ggrbqwpa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dqooixrt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uislrjep.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qgfpfbvg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2osppveid.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oijqwxmc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ueyctmoc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2dmbnddgw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2asjvlzpm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tqyqdvmo.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yyuechna.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dqnlqmdf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2enrydwvn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2abmwxzsb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2tqjaoqei.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pyhwlsks.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oxzhouel.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bkwjeswj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mwmvrdmk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2baaearcn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vwapnrba.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2srsodrcq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kzuqkqgd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vdicjurn.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ymtqtius.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ejxkyprq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sjgzhkuq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wggzupiw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2adahqjhn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybbmbqlt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgburnjv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ffpddqyh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jqncsuzk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsvnkwuu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hmnrjzkr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xkmtmryu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnnzsaxe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hlfpnrzd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aougywhx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xftpsxhd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vlxxrtje.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xuuvbntv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2siavewlm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2lkmdlzny.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gnqmxutj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2subosjhs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gxxkwkgt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkkafvg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wpzlnakz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2diznulgx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2buvkvncp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ejreievv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2sylslisw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zqkrltov.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2fomnoikd.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ixbmkfln.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zhwrtili.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2qrgxatle.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jmxeqjve.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2pxqtbykj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2aedgptly.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2juitufcl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kmxtblkp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2vahqqxrg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wkbvbqin.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2msddpwci.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mxcmogfr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqrwtvf.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gtxwmbmq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2qbuiqipc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wjmbjxhm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2tucvgbfh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2opsyyncu.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fuyjvyeg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rznhzqpr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rgyqtqyz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vjgugvjz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xmzyqaco.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2qmbsoubk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tuhivivq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ontjumuq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2kunfvtev.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2doabrnol.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2uzlnixof.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2knhtjyfw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ptzzxbvy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mycgftsq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eriktbsm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2utpuvokq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2imximsjx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ukhryyvg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2upxnppkr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sraafdqe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fnjjtdhd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iedbuexc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2erpbymsv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bcziwari.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ntlksjku.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2zgptbcrh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2sawebqvh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2utnegwbt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ohcgzseq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2mjwwrahi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ohncbkeh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ulrlxzwc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uvygnxtc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mbmvqbsi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2toarvgwd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdgoibai.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfzcydye.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pzrfofnw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aaovznmt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2abquyfrn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2wdvmfabn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wxgpwwzy.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2swxcgbxt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rylyeapb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uefuooyk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2vjczuhvl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jvunjuyv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tfsfodzj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2gppylwsk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2uywkptje.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ozxtodco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogryobhu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2skktbzdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjhzsdak.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ytpppxbw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2auxuajbt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrgjqpag.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nnlyxyna.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vgrwlhnu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2igxracfg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kajnwoof.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tttxgzcc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bayutqpr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hylfscfe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2rvoordze.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggzyjunt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2shkkjrvs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yqkmgzfq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2uunwyezk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2kwfsiure.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2cecloumf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2inyfikqf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wauhnczp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2stkzaqfh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzpyhfgh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rvksqxiy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egmlqcxy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfhjrfxo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cuuaofft.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gqhqwgvc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ntesudjx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xjitbciz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cwkeqkqk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2hdzupwwb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lceaaxfi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqirobzf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecsrkijw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xiwoxqpf.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xxyyngza.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2spyxkfil.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2plsegvtd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hcbgfkiq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bukwkhpu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqsonex.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcjipgsi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qckjincm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nifvzdhm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kfacrsaf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvcgenvb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2odluvqah.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2sekjdevi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsynobov.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmhmidm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmjdsmeb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzvrgxjb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jpinqmpe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zlkdscwb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbygpsiv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sdgoyyhv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2arayyeiy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lwfkbolz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxijfrqy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vqnombax.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gunegldy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2gmnmghee.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2marsvvhy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzowjdgt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bjxiozxs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qlvkktue.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hmbjgkxr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wwkxlmxi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ptkgfpfg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hracxgoj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lmuumflk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2juqaoinm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gpddopbq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2crzccsvg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2etfkuenz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjebgmqr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcbidsod.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tipzxzgq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdkubdh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kowaclco.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdrisko.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2thslwvkf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sddxltzi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2sdgfgchm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaoirkyh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2svqthtux.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zcuqriig.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xeaxnckc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xyzzwrnu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ajfmekrd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lnqrcoiw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2gmcoylfg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cjyvqadb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2odquhhvg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qhfmlaoo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cihigwer.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2hmhyanrm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2uafraicf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ipdbtyvs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mqaeaxwl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hytwdndn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2wobdzrzz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qdvbxcfc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vokearko.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kafimcvl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qjxfsdzz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzudswdx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hgzkdhix.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2quxkpykx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dppbaxee.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xoregkso.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjmowjnk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2isgeoetr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rgknnyrv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xldubmre.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ijyofyns.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxkqxvw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ohdplfpl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2keagbpux.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rkwzbpan.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pcnvhgxl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rerkliab.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gnddzuvx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pqihujql.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oesoygww.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nveilyvq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gvrkpwjs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mooumbeo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2fginplmt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2beisxbas.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xkgoalfw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mdcvvkgx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2juazdzlh.html


<!-- 参考信息 -->