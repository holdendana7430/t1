代发 wailian999

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3shtanzhi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3qiqvvuxt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3yfotvsha.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sdxhfzgr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3mmybxhmo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ofgfahxx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3mikfazgo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3eozencks.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dtxfqqbr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3cnymiuir.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3humupbur.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3anduczya.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lyiwsnde.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oawxzhgd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hvdpposj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ilnzdznq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgysftfu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3bdjqbgtr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3gvtvxmhu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3csdazcfa.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zqrwwfis.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3gfldfnxg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3bghmhsjr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ugwblkcb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3twchxmbf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjbvlbph.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3iprajidw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3cdtkxsog.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3eahfxmqx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3mtvzfmgc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gunfcfaj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qeydcgpx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hjbnpllp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3npkfytwb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3myvsdswk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3pwhwwgmx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jedptjzd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ujxxdxuo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rdhiabfu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3sacbyllr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hgoctvyi.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3bkcduiji.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mtlhvyuf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vaimmait.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dtaqkgbs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fxdvsudu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3backolxg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3vtnlyrar.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dfubkpit.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qjukwglk.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ilbfdrpf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tffaypad.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iwpukbpg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bebmupqx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kdqgskza.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ddvfgipb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jbalcyzs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3sbuyotvs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jpdlztul.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mhpihekj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3urfqvdqs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ubymgwmb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kucsblmy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ngzgowgp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jhnwemtk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uihlxhyk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bobchfeu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ceikqrtp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3irgkodou.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nedmdezo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3pyoylevi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3dbelmuuo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ovgvhnbc.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vufmlwcm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3igeiciez.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3msfbdrce.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3rejnkalc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3sscsrwpi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppwujplz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfjufvyh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3yzcvgjqu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3zfpafgcs.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbbbzkup.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3prjtbfdv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ruurygyf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3muhuhoao.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yiwycibl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hhggisri.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3btxwstgu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vewyuvrh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3piimcwfw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aojhapcy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3esttqruc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3iimiptvn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ansvyuzv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rzepuixo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmbukzz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qnmyncmx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3svqadomd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3mrgkharx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ddyvqsua.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3nxvjfdzp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mhprjqmf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ynuwarbv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3iyuhgsws.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3cxmilwqw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fcwjuqlf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uxkvobre.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wpotmpsn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ylhvxmaw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xuwarqxo.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jybcbccg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mljyjmuw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3wkzxtmbm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ozaweciv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3hgloeudk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zyynooki.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lhyofous.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3bozbmpov.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qylixcmn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kjcdwyhh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gebqavtn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3opsbxtkc.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nzqvqmti.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qsdkifax.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jppciuzr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hootrxgq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cxnckfoy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mpyntqlk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pzxeiknl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3forvxqub.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3svrxdurr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3adofbyrk.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ozrnxjpt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvycsdyo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3jkmgsloc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jojptwyq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wszgmkgb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dwjnkaov.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3gaepryep.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gtyuckcn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rsuvkwqv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3etwhwzlj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmkdmbvd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rbqevypu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xscyhpgj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3siursidt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rqwymipw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3eykpkwrc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iyqvkufq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pxsigrec.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ixeddkdn.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mbtykunq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3snwxepoi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pgsspgpf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pyokppls.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3hgspmpat.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qivvzytt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhfatbyb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdhgadwf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wlcqbfhf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xcbclbqc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xeqvwegt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3geashbus.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3krxynmdn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nogfaijk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3anluvigs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yyrraujj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3qpxazlka.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bxkuolgw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zkhlzelk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vjicayhu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3htoyygme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnnmoeya.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ojwsojpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efbbvkxn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3dwxqmjtr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3urwppxws.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3njqdmiuu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bewwybrl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qmbcukpl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3awqbgtpa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3pmthnoqd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gxbnnokj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kajcmpbc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cyvfpouo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oemzlcqi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3cepygieo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3klomssih.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zzbamidf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dljxlcxn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nuwfoyki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hpfwdqcp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3khlzvowl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jqegehav.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gvfhqbja.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3brmbkgcc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhiqypiw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kqiofcdd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3deijbwyb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3udilodbe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fgycuuke.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pmompgcb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pgyogmxy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3agedyowd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyuszexj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzwygxge.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3utiahshc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dimuofkh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fwvkrnqq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3usolbnyg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tvciggqr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3znljgrai.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3lynjhtsn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kurbonaa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ezomrbko.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3svqqawyh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fsxzbawf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3leenhvvl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3eyfkpntm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3quapgkit.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3efmsvuku.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vblfmyqt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zkegkjbf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqwjtych.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpfkukjr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qqcfkvvx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xuhnqxes.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gkrhizca.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ovrftzwe.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3bgtpjist.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3fujiaacx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fftjcnux.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bpqqwnfj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pukuinlz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gwkizink.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lvyqnkuy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbdatzzj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oajfcimh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lgdyroim.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jcrcpofg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3metcfulq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3funpwnhv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tjoidwix.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ntrrbxff.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3knbmahto.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dgcutafj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pqfuzrgu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wonwpofe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gnvivohh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhkklnol.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jpuxwtwh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iafqdaga.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yupnhvml.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3latknkzb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ggqwjdpr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sskcrshw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jnipkjja.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3samerwfg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xercpjva.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hqbunofr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fvjwrrkg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ykxiobqf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nqwpmluq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xixjieze.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kzowsmyx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ssezhxxi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jhzwvcib.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yfvsmotx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gxrvuciz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3heowhros.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ixytoixj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3iaopvonv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rvuwqksz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzpvecx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bjgtdpgr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qrkwqoxv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vrgmyzkf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ruyauwda.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3abefwnje.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tdamjlaw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fdgfjqxn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fkpsycsm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bdruzzgv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mqulydvr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3sallicbx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rqgefagn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zgujlkvy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zdacbgrr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3uayhalbs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bittqqha.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qerhmbem.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3pqlrnjgo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vzvxjbcc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3prdkfgvd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wynxnqgh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3drdlqxfi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bljyzugq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnhdymcn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3atxogoze.html


<!-- 参考信息 -->