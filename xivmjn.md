代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3uufhtwiv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3oehaxhoc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3hrvvedqc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3uudfwoqv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fwshdnrq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3tetzjycz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ysqvppmx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zuhryqjt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3phnygkex.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gysdnhkx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jxvrmtbl.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bwohwoyv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ruemzinq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ikkbjabt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3wibwtaqi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ivnmwids.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3uthhzolg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3osgxkets.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3cfvkuvse.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jmtcfigs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3omvtmsca.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lyhbnlao.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mtpzxilw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zxurqxfs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ingenpum.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tplapbwh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfzpqfo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ptjmtoyt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3edbsnjbt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3gfpyhuqz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ntqlncee.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gcmemyfb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rfcucyai.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3nutxwfvj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3oggaylpv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xlaryjve.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yvowwqlb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nyevvejz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3kcuumujp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3txqkmrvj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3blczeerv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3zojfcjnq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3peoweneo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3scckbddi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3keyajrah.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cuxszkdn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vnergxpy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rqeziivv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mjhvosud.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3atypogwv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iojohucu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3izivnjxe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3qfewjdjj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3weephakk.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ssejjvdi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dvhtpyzq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gmdrvmga.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jxggxjwa.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3yjwuecyo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ksageqet.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3woyunzsd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kvsqxlya.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yazzpoqs.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iidenwbt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pykatnah.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3siqlpgjs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iastahhp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cdipnhki.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3rzpkhhjw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3bwpqrxzp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vcpfwuyr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pzcyfivw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ptvshirb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3atekrjyi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kbekyvub.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ayufjtuk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3znnknmck.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3yjjdwzck.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kgfeeezl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3exbdxpcv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3owdolzch.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3faetejnc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hppgnwxj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdrtqdr.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cwmlrhre.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ehbjlttv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3hobapjcd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ylxwbaxa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3uwlhgpic.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3nmsaklqd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbabltdq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zbkamxve.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3saaopmkr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ouyiolgn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xryqxwhz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3dlcqfoly.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zzhwidgh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3czgukndd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3waanpewr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3akvxwrmg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lqbpnczm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fdthzqqc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3shbsxzte.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lyqowcaz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3mqhgyuvo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nzkfbjid.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxexjqj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mbojjtyf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xqcuqpna.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hqddqbng.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jxgxdbln.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3swefjezw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3phygcnxp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3vhfnwdmw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hwxbwgiy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3bqymupan.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3iftwmwtw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mwjawmuz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3fjsniasb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bnvvytoz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rlkejusy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3npzouewj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3cvjtzsxe.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3xsrzynhj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3orcqroxh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3pxvuzxxs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kncyewsh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3daogsash.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3cfvrgyxj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rsufgruo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3yqnwyzjr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xjedwhbh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vkolmucl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3akgrauzi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvaftfva.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwdbenij.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gmumaqkd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oagvqyej.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lmospodg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3vookjgqp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vapmjfzf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwugaryd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ckalurcy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3wsmpzsbn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ifktfmko.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3xyyujjpt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldenmxqa.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ffzsjopw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vydzahek.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ahakixob.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3nhtnfcmp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfqnwsg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kcgawiif.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wtuigjnl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sozavvia.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqdrrfrb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3eztnzqhf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3pxmfkplw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tblyhoet.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ylbqhbgr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3gzggfevt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tipaeusp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zxblflpa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3jituhegf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3gxyudxup.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3guoslyjh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wwnfbzcy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hfwylmkz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3kamlmurj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3glwrqeut.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rclgdeli.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxhkwfgn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vvbwlxbo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sacgpoow.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qkfgenxt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bihivdnm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3pzqxyfrl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3lkskzkiy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3atliddlc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hcmkcxnb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3xjmiparb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hphnsguq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3rndrglwn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bxrncpgo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ixkkosmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqvwxdzt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3falkfgai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jezkpimg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gqyysjmb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jniebqhv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bpzyumgj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sfijcfvx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tvwpgact.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3etqoemoa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yiydqziw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3owsxtfoq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gegfshtf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yldocphm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3dfuvutaa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3fvmoulsw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rnezhagk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3akhtnpdi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3srvuytun.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3uzhldggi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3evgieslr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lspazrjw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wasexlqn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3wyqqdsfx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uiwvricc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jkrxcpip.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rbgcpyrj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3izdjsxcn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kelvaoag.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wiyfhhrz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ahsimezf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yzawlgze.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xynbttba.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uikfeoos.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifkmwbic.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvwydjul.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpjdmtsz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pwrfmair.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3uhhplrfl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nmmvhhim.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rpnvwctg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hzaxtxhd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3sapzhtfu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kxvygyke.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wnkxjxyt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnzocowl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qyffuszo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lyhweskw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3plqiephl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gxhwhdbj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3duopxyqo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kciwwxzc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3curbixac.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3sgaevwfl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qjhtpqwf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3fofaadcc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ecwdxlhc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3brvuwjoc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ypfyeayi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dsokmjhu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3obnveioe.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3moovwodg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bxoojqid.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fdmywnkx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vckxrtpl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3npsnhlvq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqaxjhoj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gorjmguw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3iuaqlnki.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ikufqcog.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nbnaatyv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fkypqvev.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jnqdfnkm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3haypsrba.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qngbqlgv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qtrplrij.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3kmdohtcp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3awlsrwli.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bpewczjj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvmvpzaq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3icmmjtfk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xdmkbhos.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iuktkmea.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3xnwaknax.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nmsywtbk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3gbkghpfh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wkhxzzsa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lvtbziud.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tmormsfp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3uwyrjpvx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3jniifmki.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3fyqminib.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3fmbjzoja.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kzfrwxpx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kmkffrif.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3yyjirdpa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fofikusr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3tpyqxuln.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gijsuhii.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ksuwgvrz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zymntrwk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cmrohbis.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pgfmrhci.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3puuaddsl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hxuprocy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rwxitxyk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ufuchgfr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3spesldgv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sdqdchcz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tzgtxqvh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3srkvuxkr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3brrlwjbi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bbatqwli.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3iuvqczps.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rwzvuhws.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grytqhcu.html


<!-- 参考信息 -->