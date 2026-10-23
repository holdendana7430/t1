代发 wailian999

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yfopryjf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rthtjuqd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vkdozvmd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3gdwaljsb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wsjjdcka.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3slklnccv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lwvfwbax.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3nujudwfw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3tvaglpsw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3yhrfbdmw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3uszusboc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3zbbgjirz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3hfrbwtby.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sjakddnu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nofcihuo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3thvbfzhq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jhybdeni.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3stfnemxt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ulxbnyov.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mtydhwme.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ovllgwxi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wqhuoswc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vglzgjsg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ltdmrkic.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ufrwiyrx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hirmquae.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ztostddb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3lhzifoxw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tuavdrkm.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ccfggbzp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3kwinoccb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lsnnaejo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bfmenkkh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3yvzfnnhu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qvxrgvyz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hybeuaqe.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xchzucxg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3snhkhxms.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3vrowtblc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nqykpqkg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ggnlkufl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rzownzmp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3wptugtzm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qlcwccnk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3htipobin.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3giimpbcj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ulvyosja.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gaobghtg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bamvjlgy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3toxjhpvu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iefoueap.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zosfjyhz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zselhiyy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ohhjlxap.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3sabhlqfx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yuougfwp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qtvaaxcq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3gchebaec.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pxymeiiy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3csoxapwe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bwjmzqcx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ximnqjtv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3oakvzuns.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwopirt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3nhmdvjbp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3atwwtjll.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3mxvtggpz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ydbwcasa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3naipgetb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3civoxufz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lcnryxxd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3njvjmpfr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3utqquvjq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gmlaevix.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zhhaszua.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dzxhycli.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3bpnqmyyn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lauffxhi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rxhcwesv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3pqmoqqzk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kicvhoar.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3fkwdhabq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kriskuau.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3qohbjovh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3adtysebq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ptjzczrr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3slvpweay.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fluhistc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3neqtdyed.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fmisvjfe.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cqkmdnmv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3udmuwdgy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3oahukihk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3hrqfhwmp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3glfjimpu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hwlmkutx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kfmokbxi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dsebjfly.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eluorkhm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3orwiyrog.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3brucxnsg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mmfxfhbo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bdzxxgxm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pgznydzh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wzprrxnw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oivjwrlk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3yuokyjxz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3jfbiyyds.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3yfgaybmt.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nczpyzak.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3yvkjzrlt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mbnotyxr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3skpxbwrs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3guwrmjmo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3inyviywk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3djzyrzwz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3rimxsndb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3tstgfdex.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kekpdcmx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qrkuatkc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bphfouoq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hdvpwidd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jaazwwiw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xkorqlwd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rcgjyeol.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yqxhhfwr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kolivpoq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nsczvqjc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3rsxacbzj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kjpzcaqi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3aerggppo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ytqunhex.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3seufjsrv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3moukrwrh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hyfgekbg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3lbxtyjye.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mqgdjsyn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssqnezkg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gxthtruh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3iyeqmwyy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ysescjau.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ahwyfufe.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3itxgoqbl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oxxheifo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rlgjzpmq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3gcnxakgy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3fknpfimd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ofgvlicl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3irkmdwgo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3lliswccf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kzoqkabv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3efckmreh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3gfruzvez.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3uhnhsovp.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yqrmikcv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3eodlgpcu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjgqbxiw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iezapitc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xuxygkmm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fboheske.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zxjfisys.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ljkbszsr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rptmytuh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3wmiffzdq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3acdpioxc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yytgyxny.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ncymdsdz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3dzvdvaji.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3drpmmbnx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zhcnevnj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3mvxfbnem.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ouhplitr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yxrpdtzq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hghpgxur.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3amvsvqah.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ajditctu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qdyvvkcb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3luaaoqsk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jjkqsaut.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yojqgpcd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3djqfqcaq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ztccablv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tdetoirg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fsarglkq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ijrnjsza.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3voigsqcd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mcsljzmn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cbuxiwyy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dnmupwlo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ozyphufm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lammnejn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gabnouth.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ndaadurb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3veuhbajv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dnkclnaz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yndsnnic.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gteekfuk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bmnbbbox.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3lmxviunh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lginvbhf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dizndwla.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3gzotufbw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vdhzzrgu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3qpiludbn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zohusymo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mgptgjhy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jzhncosz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3cbsgdspg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvfxaqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcwpdagt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jiudezbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftownzzm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ysdkbmcw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3oetcgpof.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwwgwvut.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3krvlhscd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mzyunrkf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eweaozjf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zhxdetij.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dvkzzmeq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oqeziqqi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dssacbix.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3amfngkxv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvxhgdfw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zummyhox.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lgipgfsk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uvvbgcin.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3anqvpvgp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3cfrrkjis.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vjdnxiax.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3bmltlbcf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3niascigj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtgjaold.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zjoyymlw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zosoyzzq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rmlyrxyo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uoonvldr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dlwdkuzl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ehjougfk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hpatwopg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hyjkydsd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxfzodns.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ojgydazs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hmvlixje.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnixcibf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yyzgkonz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zgrqpdbn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nbzszxba.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3orhuufjw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3tkpohchh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hvjgvquo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhegtygb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iaytvthd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3uknqimhr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ecrnuxpl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nflloprq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpbeawmg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3hnakoajm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qofxoywo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3sqhiqnes.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufvjbejp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pnnbgwic.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdqubbmo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mwwdovby.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vhdtkhhy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3xfwenuaq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rrxibufw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gsauptzq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3aytwityt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kdvgwuyk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3chhykiiq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wizdffpo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nzaxnfmd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3bogpdosj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3elsveenr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3fyjglhtb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rsbfjcuz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dtlrfcyz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gmpmrkhh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vusulfag.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rfuvqyae.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lmzwloyf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3flxuwuup.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3btybhzyt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3teytipkb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3sqaecitx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iovifysd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mybxdjzx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dugzstri.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yzvppnqi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fcrjphuc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dhhywbke.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sfdqwhkn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3defhflgc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3appplxdu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnosqlhu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lncivdiy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xerevhna.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3brrwhfof.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vuzcdtyr.html


<!-- 参考信息 -->