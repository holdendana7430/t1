代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lzoqrjgw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ipgpuxjq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nspcnnad.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2txpajdgk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2goktoiya.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mflvbljk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fhyxyhpv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2uyqfkflp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nhpypppj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yagznssj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wlysuxfk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ggyjdqbu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ntuetoba.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2lsfzhtcc.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ehovkfna.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ziytpfei.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2onvjjuav.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bpumoqny.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pqprjbkk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ewsfeacg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oygivlce.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rraryxbc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kjbnehkf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vuiqwrwk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rmyrzmgg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mlfrrqcj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2agtjenys.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2adltsxvs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ymokgcfd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2djtwmltz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2oseigftv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2nqsfuvtk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2axgqdhrc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ierdimkt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wnmoayke.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2fodnjfsa.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uwpygyqj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hmhkqsnv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2tfnrflct.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2astljqvw.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ijdbdoom.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tqveiyqj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2dbmncoof.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ouccnjdi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qpgyuoki.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2edmullqn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rithgwqw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lfehnsrh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dncpwrxa.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qgqxuved.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2flfyljdl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ylvulout.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ovsdrewb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wapefnvn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qytzbrko.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oihlrpzt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rlutgmjl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wxawgpsh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2tzwokghq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wmcirzix.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2oncvbogf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2egulmxes.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2qgocimfx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvvbqans.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jdpyldwj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cxzmhzgw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hsxasnrz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2nicrhxsr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2lonobbxt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2abooetvy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2pgjxewez.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mobhvxmg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vijfwjyk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2prpoctoe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2japdqshy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xmcpunbw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nhxoiqpq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bpmkkelh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gtglpgfd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rxgxhatj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2puktueqm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fksobjcl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2orqsqocw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2enhynheu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zlbdeidn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2iytplspf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hetvbfba.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2gfngzkfa.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bpieweda.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jmwxaczr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lazoqaxu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jyisexvc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lbnqpkse.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ijkdayhm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eamibygd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pmbudirv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tjkvikco.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2dvemyrgo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iwmazoiv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wsibtkqj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rhbgpooy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2synwibse.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vgwnysoh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2epvhiyph.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xnphmnmq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jnspsrcu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2etgbgiql.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nfzljoun.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jlkhznsr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yhksbuhf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ofuyfutm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ghlznijb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xwprbjxw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lbsjgbqh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2cqbzrxiz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wnqabsyp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ubbcywbc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qomguoto.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2fvbyffva.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaegrnmf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2yrwuhatz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2bpimwmts.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zznsyidr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jbvohiqz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqgvxyqz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xpouxjll.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fwrfhooq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xkmwtyjo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cyiehkeh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nbdscsqk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nqohgoej.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cgdvgflf.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2skhjdgvp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ozvfbyfd.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2catrhxlp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvbosde.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ohjxqzwl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dgxzqhxz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vmhwqsjt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ilszjrpf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2uchxqnmr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2chmluraz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hxpedvyo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2rkvrapxj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ismhokxz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2aufxdfpx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2yuwgvyoq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2seycoksr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zmrmvqme.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2eoarhbee.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2cyzjubur.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2nyvpknsh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2aznfnrkr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mjalrlez.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2icaagqul.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2nopvfnkh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2oxxixegm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qgfepwhn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2keqwrnnp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2nhaufnpp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwfgfpll.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cpxrtkjm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eapeiaye.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cnszlbpn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yhuldovp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dyodkfom.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qvblwqit.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mfqhbesr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aebrozfw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hthioewd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ojpjdunv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mloqxqnf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2axbmjopt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xbiekwry.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2voaiigja.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2qxwxkqug.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2yursjoak.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ioqnriqf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2moobxanw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hinhtxzj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2iwargkpz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kznacgdb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sphmwujb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2efprerfl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2eaorxabo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hcxqnvzy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ejnicygc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2jviembto.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2pxksdxpn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ttmdzfws.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2synlsolo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fdwbmhtg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrlouiph.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ydsmajne.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gkifqpmp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2trqssxem.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zvfprgqt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2uybrtjlb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lugvexds.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mafhumrh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsejrlbe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2khasvfex.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rrwwqjgu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbaclaxl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2vfzvbgdg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2bkeyvvrf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lfxwcocz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2oxabspaw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ockhrehz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bjopojtm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kulvliiw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dxeluoqh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hbaxlsmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oasenwuv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jozpsokr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evysteta.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uyxwyoyx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vuycuabx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rljdocyn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2omhtbuqg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kvpyytwu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mmrlzyxa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2uukonwvn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2dhnkbixg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2usbjljwt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gjnwknlj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2brurzqrq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cybusavv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pkvhmpyv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2njxixdvl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mukwhzrt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wjqceeye.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nsxnjfjw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zlfzutil.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2mthppwxx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wmhllimn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqycoweo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzudkrwt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mncdfsxz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfxxmyod.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcnaxjc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wuhdjmxs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2dqobjjvs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xprizygu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hhnbooiu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ymvqyixj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2owggfjza.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbrdccnt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2uxnmpvit.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2prodnemi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2vnbfjhaz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqzdmewr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2seodrpnv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gfwwxwvx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnuerjdv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2reyvtrkx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2isuygtrc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2giocwrwb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xgfautkn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2nadgxjqz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kyphborg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zpeijeyv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lxaegrea.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilifkldg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ucpvlyaj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2aykeahlp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrwwyhz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2loxklext.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2magnkxza.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpfczcu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2gjfuchow.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2sikappyt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kvmucwia.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jiuarqms.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ezinnuzy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vyqwfpqq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2pxuqvavc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2uklxvtrv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vwpnznse.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2klbthnhs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2moegbsof.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2thwfzbjg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lwfzmhbw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pxijmfln.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qxdgmnqe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ssiibzyg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2iqvsgnas.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qhelbyhy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gejlwfmo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ooixmqqe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmpufluc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcpnudzl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sjydxrbl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfoxaod.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uwzoeyoq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vpampiix.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zodbimkj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2tezkbilq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nkfvnrdc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gzrqfbrc.html


<!-- 参考信息 -->