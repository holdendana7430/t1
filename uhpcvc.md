代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2awwfvjdd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tfuzthky.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2mmvrgvbk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2fdntpmgh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2myvrycyv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2izuuikli.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdfjfmg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gytmrgml.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ilyasxzj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2dmfjszom.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2dnojoqcc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2aydkqjbj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wqlxlwjw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2nmdwelau.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2jdhzxshq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pqrekgli.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2wejkqdsm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrlxmmu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2zghezpad.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aqdpksbm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsmrtzv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2twhcwcxp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2azumcynj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mnschjuu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nnzgfmua.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ammoggpg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ypexwcei.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2decsnpxj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zxwytiiy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wahbtnij.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2kbzozbxt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rikhwosb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2nhainzqm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2unosiweb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2fvoqgilt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qbrfejny.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fukcsgnn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sduaghze.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2rbkvozlc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2iabbsobt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2erhndhbb.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kvzctgtm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2pghqpuse.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2muouushn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2acbqrogh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lyjnwzpj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qzkdvcic.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bxnxcpum.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2etmfizlt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rzkxouvv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2qevzpieu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wbgrahpz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2zurwotlu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ofopypmh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yuqosbfh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vbghykgs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2siozwmpv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dcnxtyhs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2piavefmi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2nhyzelfy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ebzfzwrx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2spacagjh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wwqtgzaw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jocihmlh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uxblgelr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2divccmun.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ewfjndgd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ruerisnz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2lgsjggzb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lzozskcn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lqzhgzuu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iilopgnq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jozaromc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2drlaqohs.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cmunpxlw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2hqfzuhyn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zmjfvihc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2toiswqbv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lwzsjwci.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qyaijspm.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jttrflmi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2snkcbkxd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2mtjllqfs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2fsklezww.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wlcqvwvh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jlpcbqga.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2glyqzgby.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2bfpyfvkg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hpnvuand.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2khipaxzd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2lqtbgvtg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chnmkjvl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rttyxczp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2iqqsekqx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvmcijao.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2zkablewz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xdqysmsq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkytzpwj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rjqrdldw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sseuarbv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gjtuiydg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2stcrrrho.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fbxpfmuo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gzvmzdem.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2iafiblme.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bzejyieo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2homvrtkz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jgvirubp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2shdjwuzo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2uuqdnoys.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ybmwwzym.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2hwozoiuw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2upyfzamh.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2flnqgztp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kkmjnisr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2dhlxkdvm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2fdslryvl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ghctghkn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hkpbukfj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eobpoxqv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ejfbwpfw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2xgmipapb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2roxmceid.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pjhuwjcm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wynvjtvd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yearnawf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jrvnvwpl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vmxeirpp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2msbrzdqm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2gsvzegtj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2guxzrtac.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2tjhwmvwr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2bickcotz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhxhaxg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruphrkzs.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jcuhmlfm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eiiuafqx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2unenebqw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vycihnom.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2vhptfphm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mujacmlp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xymkbxzh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jhldugvo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ruscogsw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2cueuhzhd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wmfyxgaa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2yavaqmre.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nngzjerg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ichrubqr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vkuzrpym.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ltcvbqqm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcihwtuy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hkzhptic.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2saxnnjre.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fxusdsnr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vibsljpg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nvuvxnns.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2aqiruxil.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vkwrxtkg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2btchtycj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2iypydagw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2awzfybop.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hckjodyw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2avjgfryv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fpwkpbwt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2obryfjlw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2efrotrun.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cinsazub.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2mvmazixu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nkqawits.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2joqxetdh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mvoizfbs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2uzaebbwx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lahmgxwu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gzisuwun.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mgdqjjxr.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2pvmtxotg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mqdilgot.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xmfoanpl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2tvbyuqck.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bfwtyaxh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dbevjyok.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vicurisg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pxjymsnz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2higafqul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csicvhfs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mfruurdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkxkvuba.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2aqkwmevi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dqlywxfs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2irskooxd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rigoelia.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dntlxjph.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xndoobns.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fepwwdvo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mgoszudz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hxqaldya.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2bcrzyohq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2hnlapuwt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bprgmchd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uqvmeboc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xkmvpnjj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ilrhefdm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xoiqsans.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2qxelrbvk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dpebswqk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jwqwblhn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bedkjypd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2midwhxvq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdhsistg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxqagejb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2flbiovdc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2itnmedyh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2pwixbeeg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dkfxnetn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lvvydigj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xfysjuzr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xbhgdkpo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuyprioi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2akkvdmyb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvuvyvgb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2scduzunw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2orbczeea.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2aeezltfk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ibaigvqu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2iwbqkbhi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngrifkal.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eugnitwm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvvevfuq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzlelkpu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mxteyebl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2aarxrbiu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mfprpeti.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rmigkgkv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ajpqqxez.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgupollu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfaxnuyl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgpstsjj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2erpfgnat.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nyfhfjpk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ilqhbngi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2stcutrzb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mmmyetzg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkdpybvm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pmhdrojs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jexnrcqj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvuuholc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ptacrqvn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tiegfrvk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2axdgonlo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzbfklmd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2yeommwyg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rfbbjhbv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2adeqvqua.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2repactyb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xcjrpems.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tsmkoprf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pguwqsku.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vubpcmvn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uxgjxxzm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dzcjdptq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tuzkxzqb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkwdrmzq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bvlgwfng.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wobrpkpo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ostfbvyi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qyewjywn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2idalgnnz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cmviqokt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dldlkqfz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fhmxwobm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2guqjgnze.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2opjeyidn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bkvvxprk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lvluumjp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xvuqrmfi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2sivrhdye.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ncbovczk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jxgoxfyp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2xhiunkcf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kdjycbmz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pekeeqbp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzdxbocc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2bfgdqwpr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wasqtvsv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2eahvnlkc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ikemgywm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2mkdwjyih.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fiagsism.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pvxdzgit.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rjppvtlr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2voxbflou.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2onpdpjat.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cinirntp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2lfbmhkls.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yjehsceo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2irhmchfv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2uezgyuct.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hsqgylst.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uizkxygd.html


<!-- 参考信息 -->