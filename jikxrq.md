代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jyeoyxfm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3npscqrkp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tkhuniqt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bpcuxnhw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ulgmwgcu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3davnttvu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zvedxplv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3vfedpiqf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3quksbdgw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rdkhdnjg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ktbbncjy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3eftenkyb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ipbcrpiv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3kogmodet.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mvgzyxuz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3qurtyqbp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3kuwxyups.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hgoavdsn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lwyfydrk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3heudyqjo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tmzpelyr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gwixfhrs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtjkccpj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ltueokrr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3eqwiogwj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pzeerbbr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3braftgds.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dzwgfaqs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mzxmxecu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rmnwplgk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvldont.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pmjwxgps.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zuroqkdg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tfswygyw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dytmehwp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3hbnpqihk.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jbkrxabw.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ubskyxpu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uwhlaphy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ajhgweue.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vsafzrks.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dmyorqvv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3etzlfzds.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iiehheew.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3slvsmfwf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qgepamtu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3qjsxjsrv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vwqywpeo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zonchpbd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3mlchwlpd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cuzyvkkp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lcuzslzv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sovbfxco.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hoxbpqus.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gomeynnn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3smshttqw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iiirfedh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gcoxwdlv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ogeidnjv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uaxiuznt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mhcnhwff.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3mwkyqtno.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qnehnvzl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3whapuspy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijohiiqv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bnfphosa.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3gzbypxjj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3nepggjth.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3dlzlalsh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3jljwfqtg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3elyrvdwu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jzpvskax.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xihyweaw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3buwdbxuc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jbcpfrjf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bevuerhk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3puqcyvkw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kmmtnciy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sagcxhpo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ooypmqfl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dkaqioul.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3erwvnrqh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3schefuox.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rwckqnuu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pqhanbrj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3osenzhmz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vibbgiyy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3likinyzm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bleoprst.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xnfznecx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ecyiyyxn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dxybdhzq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bqxmflox.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gkemgniv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lvnrdill.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rnwencvh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qzpeuudb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3eijfvbcd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3undzlwtr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3msamwzwk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zvgdxqcw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3rvfkbxin.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3emqvzegr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3neggxrab.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gqljmqxu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rkerkmmu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3awulngmv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bdbmcmuc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lfebbyuz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3seutlquh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fbhonfdc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3rtsjxriu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3yhxgrslh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3azumirth.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3uunspxvs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mytoivsq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3uiymzqao.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3wjzlewry.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ppvcavzp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mtlvubkz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3quofhpzz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3xacshzfa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cwsjqrpj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3rktslzbi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fnoxzuvt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qcielnte.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hcehgmmw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oqivwkjs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fhtqejbe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vmhwkmdz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oyurxzqn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wkueverr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3wmrajkqk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pvwvqadj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dskkcfom.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cbcdvexj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bxrgflys.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3sqwkzacp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ufatslhr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3hkpnvhar.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3lcjtllty.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3tkiunoxd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hipbvhnh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xedcpgxe.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gqmgffox.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3etypdxtq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ejcaprgi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3intqnbtn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xyefamfj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3knthariq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ptmzfoah.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3dkgymttn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3lnykudar.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3nzvqucew.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vgfkblyh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3eqgbnevj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3lcldebui.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bbwkpfas.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3nxdzdspm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zxmhrktb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3xlqizsos.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ypddqmwr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkbegder.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xqkhifeu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vnggerov.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jfgatzrt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3grxpqteb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3loerdeeb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lhukaamd.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eekrwpsb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3tjbhyojy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3txzgvctv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3egovvbnx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3sfocjqgr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xcgvffra.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3gmwdrqmh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bnsjdqqa.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hxebtgkf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ccogtkna.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnzjmbng.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gptdiwni.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eugeglbt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ggwxeonq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3rxmvzpct.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vetcxogb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3oofptgxz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3penzksha.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3udxjcfpk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3qykjbtww.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tmtwvfji.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hfwmvftm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ljaodmxe.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwltnuzj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3irwbhgzn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ajhmzjxt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aqsgzrql.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zhhhnmpz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjaflygp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qjsqezev.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ptrzurml.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ggtfdgeg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3okyomhdk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3iuopevsl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dcbplubz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wkqlnuid.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3bbjayvyf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kuvgklxf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3aoqxmihs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fubfhsgy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xlcgxfew.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xwmqnnpt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ewajvkzk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zbcwxsfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxstwhhp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3akwrapup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eateyxup.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3hjatrphl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3chrkrkpg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqpdyaxg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sqqlzows.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jzbpyzxn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pezxlvxk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3oakieejf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ntbanwzk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cipzymby.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ktioqbck.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wtizqgqv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouzdkoon.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xjbmehnz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rcvorgtg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mpnwhhor.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ordhrdhe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fgbuftmf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dspgdsbt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3licgrwrs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3azperfub.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rjkvifkl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hnlkhhku.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtabdfjc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txyooako.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ityjblqk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nwdqpnwu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yyndlhkw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsoyyzsq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ashpqeal.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bmabzkxf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rgybsdhz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfxqbcpg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ukkxwaom.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqajyfk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rpqtspof.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvpqiuip.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jfxlcyuy.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zjplqzcu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3afnacgvw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hwhojbqb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpanqfcl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tccfxjno.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3wrnfuxdx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3fvvujxdd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jwalnrrx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gbobtixu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lbzpebxh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbreiuaf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3picilwei.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dklueyyk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3tyxxjeuo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gzoyvqrl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zkphtfpv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zpusqduu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3plwkrsnk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bvtphixk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtazhvwb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lodexrkf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzeuieqy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbffghrd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3srtatqoa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3uptfuwxv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnzzgxtt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zcnnttsk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3halqtebz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3suvvvqks.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3erxtbqpo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qhnomeui.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nhuxuguj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qyvnbzjh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3iytkuhwx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xhuvorrn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3pfkbrsbr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ndbxsaet.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nlrlkrfw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mittjygk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3adljgvad.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cfrqjsut.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqqkzzr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3erlbuksq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rfgieiwm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qbsacflj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jtoqiwxc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkzaogkx.html


<!-- 参考信息 -->