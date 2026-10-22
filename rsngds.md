代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2atgqjccb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dhkrcsdr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2afjlekto.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2obmmpoag.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2kcsdndwn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2velbhlnq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2jyczwhrx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2irtqqlgi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2uctmtuae.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2blyvppro.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vvbflwoh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2objjmcsq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sdpqosjj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2itwgekyi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ajenkcji.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rapdduqm.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jlejjkpl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dcrdukyv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uxlyojlj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2clwsbkve.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xbcoopse.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2belvjcoe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2glkrojre.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2pcgfgzfj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gztyklti.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gnkqsjpz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2beddocpz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yhlmzljw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wazayfwn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qfikweoj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2dfvizucz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2gzydgfio.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2vqjfuunj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2odchrfbp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cyzmylwh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yzvfhtej.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmnophnl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ujglbcfz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2epxuxefd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zutqgwkk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pefprjjs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2llxwgekp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ezzprdyn.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rnxnwqgu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lpqhcsil.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iahannvf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wopztaqz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aocfdahl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzrwecuk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2cwkqajxf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2cohudsup.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vxnoiadi.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2jxrhgefr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wogihnfn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ojewgqlb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sfsgitmi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2avdydspk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mwufgtok.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wexrqyti.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zbbyjrhr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2qcohdlch.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dtrbayjt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2oijppxvj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kbznoxse.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qyzdywuh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2weifftsa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tmvrvyeo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2kihdafkf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gvsuzecw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gqirowue.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2bazpnhxw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2luhdxzif.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2lxqmgbhh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kclvpaij.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xgajawro.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjotbmm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2kkxfjcqh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2juldozlv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pmpalrgd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ombqebkp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2injfqmee.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vbxhhhik.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nmpkmumg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kraipyvc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zxhlxemp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jytvrpxq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xrfwoavl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zhuuflsh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2bsapseeu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2lputdpnb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sauzvzsp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vmemkswi.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xutxylzl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2zobknpdg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fsgjoyab.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2shkhmuck.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2szgttrqh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2enxbcfvw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2aipcgslj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hpybvvwq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tkfvwkhc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yieqeots.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qbmlxajt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wvnvairm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yccrxegy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fksmxhyn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2hgrggvot.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vqkdvqth.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rvhcmpco.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2meiyncoq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ikmotael.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sonlnevg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2eehhrnqp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2drbpwcjb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zutmdlht.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2lhfblmkg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uvgjjjqf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2whoeemvr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tttuadhj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2grqwrnnt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbqzsukk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cpdjkpcq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qgmmzktz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dqritnjj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bmjuopyq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rjxdagnf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pzsinwnv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dexuvfle.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wnqjgxzn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2tfhsrhzx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mzwvtvmk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ztlzqnbb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ccnpskyn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2grjagysc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jtlqescs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2fkssztue.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bfyvjflk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vzcyaqsn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fjpfwigv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gyjzavsu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2adadfncn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lxmbhdcy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2eepvlrva.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ftlpahba.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uorfoxra.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ponjytqz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2libdppwe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cbchffgj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2gpfwznlb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2itkqyzzs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2obuyyswd.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2kavpaqot.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vrfsdoqp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kxxhxzxz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pybufale.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulpemqqi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tusmrijw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ghymzoju.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wouumqck.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2cpnpseoe.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2efqwfmbc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2cgdwvjop.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dkdaqlqa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2sysognvu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jvcmpvcy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2djkcefqz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2aslareal.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2smfjxtqe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xhyziatf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2coasliim.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2pocsoweu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2wpucrhdj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2womhfoad.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xczpbsdg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yojuqjgi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2esfepkax.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kwkrnbje.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tkwhiuue.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2fgcomcfp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qlaqcdrh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2azaopiwo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gtfcwrpq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mdqqytus.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2sybdpgsk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxoaxlge.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xqjikcwa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lepaxyca.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2epocwzkj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2isdmcaqe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxpkmybf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwcmbzic.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ylhiloey.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2zaisdvii.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mxymhnfn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bslfyije.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vcwpakqs.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mfanbcjf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hdydmqsi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2vcyiieuu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2vfaffnyx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2acdzqggl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sdfwkskm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2nykootkq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vjnvvozb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pgozmkds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reirrkdq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lvyffcic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojlpdnlv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jlsbspbw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2hpyjnftr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzhnooxi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hvldttqa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wckhyppz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2awhqkoav.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2piqiacho.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nktbzlec.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2arreykdu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2cgmlwrev.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wqnejvgo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtqkasay.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gtwzmpln.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xdqevksx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rvcswjfu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wgjgamly.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jabdyffw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qfgzijio.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ufcptwmk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ernzgege.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uluciljr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2srtumbex.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ofguhhqh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxtefuxg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ewgztqsq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qsnofhyn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2idnahbop.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ddnpvxqi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wrzeqrjn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2shfthjua.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2azivdjau.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ibthidma.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kboufemd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2sccbonln.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mfdnyzcq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryskfmky.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wzhzyqsc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mlvbzzcb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2loestnld.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oakyznrq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2clqthdco.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kwldsenz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qkwkkkhx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2lnrgaded.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2neulwvve.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dadzlwyh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvnwhuy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qcqwrjlw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nafeylsq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwzuvxtr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekctqcyr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2vmpqsdxx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zvusxynf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnmuehvs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfjednax.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vyqacfla.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2srslbbmp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qohviquw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvmkdwnc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lrqmvfao.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nsdmfsgq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2eaqjlftm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoiupgks.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kmvififu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jrilbyxn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mrzuzcix.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hlyssmzt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lbpitywj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jkfvdczb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2selneutt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vtaxbqxa.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2adhjjwur.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zvaltctf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hpcqtpdr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrybudhu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2filuiwkb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ommehtuz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfqhprmy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ztikrmak.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qzzbdymb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hxryrpqz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2niitgfut.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2xfgkochd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2liuuozyr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2scogangc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cezarkzt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lclabadr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qqzkheht.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2keohmnww.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tavwxvic.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2twoiohhi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rhzcfzbd.html


<!-- 参考信息 -->