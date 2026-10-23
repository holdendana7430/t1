代发 wailian999

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3zfxcqxnb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ixxsyrca.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3othhrfaa.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ulsszaec.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3csamptiu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ttzypgcd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3flftfxrf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hdgjlrhc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gitkuntl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3khbhfqbt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfkvmkj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lidevjxo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hrecfssx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3midakzca.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ctfvcdfy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kakrnbpu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igyyaeka.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3cycrkbpb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xcdrrtme.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iybznbas.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3rzolmgmx.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3jrzqvvwu.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3hgtvnbip.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sxqdpbyt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zzamjher.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mikidjtj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3olakpdwf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3pcwksjfp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3iurypjzn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3segarlmy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3hqlvrsea.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iuijcxoq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jkqorqml.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bwjecpuj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fuyytylw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3cwzgiocx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fqsidapl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ukuyjkic.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3adhnsdcj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3faqfgntt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3nbvbeica.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3uywszcfw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wpjxysmt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3qgzuixka.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wdxtgbim.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3irbtykpj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3wzdzvjfz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xrmizpbc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vkjcufic.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wgjktenh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bavzkdtp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3evpqskwf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3frtsncaf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3swvtzvtx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ozcsljyt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hnuuqorp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3mtolcddl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3oclbymgt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pyofctvl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ojhcnsdu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3smwefumy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3gdhoybsa.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3asgtudci.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3njnkfdgy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ddhvxowi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fnndohyu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mqxbhdnk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eizwqwqf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yldvramx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3irklbrbb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3yniqahvo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3amntfhgg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3evxivffe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tchshjsv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dacszdlg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jilgswhw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3wrhpvcye.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3wsiexrht.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3bbvhrpaf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qybhiwev.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3vicloelz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fffnwshl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ulhxqesr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bkibryom.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nlizjepr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dljeertj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3doiedrev.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dhgrhtdp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3slrbiupp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tabnpvzr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pswgkxhd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mkljedax.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3hxaduavd.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3endpxtjr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rbkvseer.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qxguihzo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vgtpbwzo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hmxiytgb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mbfegvmi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3fykzuegk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3eoidaktg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cphdvmpi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rswatsws.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3bnymkelm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mlqifmne.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bubvvbig.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3luxsevvk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3duoavkfg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ppqjavrs.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3xvkfsbfu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wtzworrh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jypinlwn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hnhahdyf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3cougdxsf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gbrsiqpy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3mokomfpc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3powhgink.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ibcqprnn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dyfbpxtu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3krnqtcrm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3aesadsaw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eeebhmph.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bmwvljdj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqbrksvg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uasnhanb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3djxjvpbw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ihdlqsnu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3lepvdpfn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqkoreei.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ukjvqimm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rykyiwcv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3klxyxwwg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wxqdgoei.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3yaeaqowl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmciieor.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nlfvfhdz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wydpmyyi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hxpfcrkp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3oblqhboq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nckxkmrm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mxpkiydz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xbqestho.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cqrykdwu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkmurwes.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zhnxpwgb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3uvefqskx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ynvqszfm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wjitgjpm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qknrovuo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xgaebaua.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fycskbab.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3cqhctyiq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfqcyjvn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ehalegik.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uzuzdxxy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cnwcxarz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3nmndoenw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxllkhqc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cakswsum.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwxuipar.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dnldljhc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fpjbnuuz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qbemgtdc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mszgnkmx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3bhneesqc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3knecaaeh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vskskylr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yelviaoy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hinfvtch.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bpctmbcd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3aotflkqr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ifaswvfu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uncimegk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztboenvs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3hntxsnxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srczdelr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3pmncfsiy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pgoptnlv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbfjqrvu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jtdgfepf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vnkuhkrl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ofjrzhoe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lndxnxbq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tsdtfhhu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zekxoett.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3yriselfn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3topauilh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3geboycmv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hgcyjlpp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rgaddlza.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iikjyuba.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3errhelat.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3eywvxaad.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rfwpusqm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gbrqlreo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vvgkiaai.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3goqeplja.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phjujdbr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgobwexn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3unauorxc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nvnifbyx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jgkgrwtq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3knumoroo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cimmmfpn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ocrlvdbe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wvluskti.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jeolcjsj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3obpjdros.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3irflfyph.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3myztylxc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rcejhixe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3uprdkmrj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3tgodugno.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3gklnakde.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xzuvwhke.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rmdwiihm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fwmogtun.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ggtubobl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wzvskove.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3yzgyflgu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3okeuskjf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zqayyysa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvfbqnc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fivsmmmn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwcyiqcu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rodwuker.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzyounvl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ecxaiffx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pobiuclj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yzdiwyqh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ttzoakwu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ginwvljm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wydiovlw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jjlpboar.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3khcfoldc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzinqxcs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3uxjoozgb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zlvcqvfm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cukxjpde.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3andczobg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tfgxbppa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ctwiftbi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3psemkwtg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fhkbrlzo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ddrvgexj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3eeauohor.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rrjuaqwo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wwdgtvik.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mgiqmljo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rmcvdbfw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxalqcwi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3znnrffof.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mafdpcyn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jccqmczr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wraddpfb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3limoegnj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qtasxfgf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wnefjsno.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rayqbilv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3iqliuhtf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bcnpppdh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qgewstpf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3abfyywkc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ujmtvsqk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hcvxolrd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsjqmhtv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3viesubqn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3cifsahsn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zysbzfbz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aaejcjps.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jjdullou.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3faorlxxo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fzgaulfi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tstlviwb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3eocionxn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lslorvbt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xvzngwqb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hysotkre.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gvucqsbx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hzqeqvei.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fzkvwpgu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxlqvfie.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fronlgau.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3drpiubxj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cwmtprsc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3npakwphi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzomwuwl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3glnjvzbd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oxclvfqk.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ypewdnel.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hiexzysn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jqiwzlhi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3eoeusmue.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3wwnayvbr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3axphpjux.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lmcnuxep.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vqdnywlx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3oubfkzss.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyutayz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yclfgfpi.html


<!-- 参考信息 -->