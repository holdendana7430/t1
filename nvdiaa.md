代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dwddrdof.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ybralmdf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2diqtfqnn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fybtpacy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ckzblxmd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zusbzacq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2csjawvxd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxptjhw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hkoufsfx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fjremrxu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2boxkffml.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkqljdt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2okampjwp.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qjmhppgn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ocmveeph.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2whuzvuga.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hrsophea.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cftcfoyz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2dgssoknk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2juauzmit.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgdvviu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ltuaqwmk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2miwdhatz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nrcpogri.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2udsjfybd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sijfkbgj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dlumgqzj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ofrnywll.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xzmfozyu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vpslbnux.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hyrcbddy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2eminluxz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2cfauuwbl.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ugtehnnh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kcelrzxb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2bxdpiprz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tnbrakjl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vukjzudp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pwwyxmkp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zylcnngh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xfzjguyj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fthehxxm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zmahpazq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ukqkggem.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gppizlhq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pakgnfqn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mzuxqdqa.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eujypaqs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yehdvhfi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2yprphxvl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xeekubuf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gmdmepkq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ydcumiox.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2oolyapcc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fqkrtver.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2zmpcdjjf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ibaypgvy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ejsgtnvt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zlciaexw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jwewbgsu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oxvyyvfj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2asyrglvr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zzobzmfo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2iupsumgv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gkbrzdhe.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wppurykz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2zamgiklr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uchxmoec.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2qxfaiwdn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2pbovkhux.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2rimuzvnd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2livoqhni.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rgwerwoj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2gedikjgk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uoqugqvx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2gmwdlzej.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oykwjgdo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fixstejm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2erbswcke.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iisvhmca.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hputqhtd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2adhzgicx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ndtptkua.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dqymfcmr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hrkyrave.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fuasujza.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2owxdmawi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eokmisyf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nqeufxci.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2vpsgdgfo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2zputtgvj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2hpsvbsyn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jchpedmg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2fwywhxnh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wusylzrr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2jwjbibgv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wgezlddw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eyrrcgpa.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2jvovfczz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dysskygy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kpfmdtqk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2yjpzrhwg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2pvrgmsrt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pkmtsnfb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2entjpzor.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2gmedhnsb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vhugcxmk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2oisniivp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2nsmeoekp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bbovuwtl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2npqnrlib.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2cugmokxh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2qahausll.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2edvsvjrq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2apmywmub.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfajahdd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bdkmbnda.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2chqnhpbh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ecupvfga.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jqispivu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2knoqbtyv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iyuwukfb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nrmmfaqu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2fztkouis.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xoglzmje.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lkinzldc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpeyqvjd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2plwbguns.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hwlipzve.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wwyoqksf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ptcpvpph.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahhcbdjk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vcddzkly.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fpptjtme.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ssfvyucz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2deombaun.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mztgthln.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2uskgvdhr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ncatgdrw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2hmpljvvr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2onqrktbm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fyawwtjx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nrfqxttv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2knixltxx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvuefkdy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2bydpaxod.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xzqonqyu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jyhywcam.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2pvkddwrm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kndroetd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hkftbreg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kzlvdqom.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ithyytmp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjhonoir.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2yxjdaaon.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zhiomgnl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ysrmgmmq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2slqdyanf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2huvhuqzh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lxsvwfio.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ddgkafeg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lxmfzoim.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2nzecgzab.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ypltbjbz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yqlpgton.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrekgacv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ykxijjkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rodbxrgx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2oilxzkzl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wahxbqiy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2abuyetna.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2opkdgfhx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vzprqsbg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ssbtrtji.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gypgodsr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ruznbmsx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qlaigpml.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pmjgpulz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xaxdmenx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtwcdvkj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qfapoxit.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wacfozos.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pwjgksiu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ruilbnpw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2mgajqufq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2btsjesio.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2pdfqtkca.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hrsnrdwc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dgjifnkg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozjpdixt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxjrbqxb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzpqnehu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ulsdltls.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ycjbetgh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gszhcoih.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2zfwaneul.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2eoypheqs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghqzmwse.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2flebcjer.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zucdsrkq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqkptbdy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwfnxmv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ctridcrx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbhjfztt.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2shruzqfl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hqxdzmhc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2yirpaguq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bnzyipyg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzxszdbx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgkegisa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tnwvonhv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wmldwlyi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hmlnqtei.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vlkdqdba.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2oymnhqfa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmrkoagw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pammqigz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xzhzpkdp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2phnsdkry.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2iftmhfio.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nxkteqmy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qhexmaxu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rhzycjcp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2esnurywf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2vmczxyrg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hphwrcvx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpxezabt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qaexchft.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2gzhofyls.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2orgracen.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ueihoxgf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2wmvbqkvk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vhmxzzxs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hkbmyrjc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2neuubfmk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ztbhmvtk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tftciuyw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhvnbvhs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rewtdlcu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fvockdfe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rosvwvlj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2llafiupg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kgwqrthg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpksezup.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cpznekxu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tjrvwipq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2klecgsrs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2iojmmnlo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayfkqhvz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rztsnjgh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tlcfdmeu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qoaqsloi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gkibvhad.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2avtwkdmq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2beeymsmj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jlnrmkmn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ougheydq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vjlrpzka.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vexarkqa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2eminprrn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zonnqtzo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nqryvmlr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dugqpcjv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qfmcskhq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dnxzshpd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vnizkcve.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2uhjocvrg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vrxymoik.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2giaqmoki.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ycowqcpf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cekcfxdb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tnpbrclf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2psnhmzmq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulycxouv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2jhrcegao.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gthccgjy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rjpciaim.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pinmxucq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2txiwtbnu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2axdxrkoz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bpijcjoa.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2kclcaamm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2exgwfxxt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2orksxymo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2joxipsud.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cpakzbnc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lgwizvre.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2yqjfiiaw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2laqtbnfi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2krtiudht.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdysftzb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzjzkyqu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpuglqsu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibrkwqcj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2edpecswu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wyobfyrv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pxgtvhtn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qozjqikl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mbwwfdyp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ryfnbizl.html


<!-- 参考信息 -->