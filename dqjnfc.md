代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gzkxrezg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3meiiljld.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wqgdvbid.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hmyksidw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ulmmsxdi.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tsnzaomq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cskcsgon.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kvusqawv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wecrknge.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3umckpkyz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3leymmzcw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3nacnmxhu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlocnjv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3epumylve.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qnwryksl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nbhfnhbe.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ahtmtpid.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lmvmvunu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3rltyywch.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tmkseguq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mqlbbcas.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uzqnyqca.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3odixdror.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ufxhmqqv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3clwfiqcz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tfmcdilo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pclpgwhn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3knwuvhye.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nwxstgnz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zlwvnker.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3lzfhffbm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ivhixsxz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ovikshdq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fowzrxhf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lpksvfjb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3asesirlt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dtwnpfhj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zicaigvi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3vcivxtlh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3vkejhmtl.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rpfktyzk.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tdtcbqwr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3twltytlv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3edsvlujb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kojnszvc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vefgckgu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3rikzento.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3saqtpmcn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbsmmpxm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qogiyewy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zleqpjxw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3itftxlrk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fhtckhta.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3eagmxris.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qmjfuorg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3brwqruao.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewjpufdf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gmezafef.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awpzwaol.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftxyihga.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zawvbrym.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3uajtpqqe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3atbgdmpy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iqrtbnxh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zpujosfo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3izlmrocl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3lvdsypqo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfoytsbe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xizotuaz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lrkbopty.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zfbaeekl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3polazuej.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3joahsipm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3xthsobjh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3drathnly.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3srbthwwu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tpheefxe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qhenicnj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ipyqzaam.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xfwcphkx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qntuswck.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3twfdyaiq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3sqhpfugv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rdqfzycv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dgpmyvub.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ztzkohfc.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3nybiaaal.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ykreqrbq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bpelasjo.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wkpolqij.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wodrbmwh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ixvyxavz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nshiaucl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zpnitvbz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rohmwynm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fdgtbpnj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nepbtjya.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aflyvrlf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3espqasvv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hgyugnla.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3pcrkbpcy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3mvfgaara.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tuiluljb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xwpcdvto.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uhibytgl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3rtdlvdex.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qmoslepn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3eokahldy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qodpbiwk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3setbyghq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rffrfdlu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vexzuzzp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ahxiiuyf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rkqcxbpe.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cqrurrlc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3fikcjenu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ikrndbwo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jcsisfvu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gqrenxen.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ddnqkfcn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3crijcskh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3jdsnxnoe.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcpyagyw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3buctuhor.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3bxuyjkse.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3clulxsxx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdkollnr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dyqsbejr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ejqajcby.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3granziux.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tuikqbyz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bntlwurq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ssbhmsai.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gfkuheqd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eryyvhjm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zyheixxo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3puzwjkuv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvtvczx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qggycsgo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3oohdrxsb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3aqcpfjdh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gtzfytff.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3llcoxdcz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3tlifbvbt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3yacfwpuv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3uycnvcxx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mfzsywsz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qpcusotb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3klejbaqz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3glmuljlx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3jevwmpio.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pdkjrgvm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zyoirmkc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3mfycvpkb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3bbjjitet.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3izncqjve.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3szxyrget.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ajvefvfi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cpqggszs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qiohbdvi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hrbavzny.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ilndxmnt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3rmznjhtr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3psgsiqvx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdjznket.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qttfcqdg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhbjtlpj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ntenxoyy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vxqlqoao.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hxuvvvac.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dfjnsaex.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rifdcnhs.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eabecwsz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3arwbssaj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3bauuinmn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3wlrkexft.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yymdrcam.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zvifqugh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jrgfimdd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qmloibqz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ulpclpwi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eiozlalh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ednzegjl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3eihmmcxd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kvjmryfd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bfscsewe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mzkszvhn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bpfxsfbc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yuzrfvsz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ekdlnnpv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tjpmvtty.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3uptrovbv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vsfruclq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yolxhtgn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3busfpmfp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qnckqcdl.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnhdsig.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ztunzdyx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vvgjvpin.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nsuxzaqd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3dyadmtuo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3bccnsktv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtzhaeyr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuquqaem.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mymjtgij.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dzeubyrd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gjqtavvv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eluhsmus.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3aeduiixz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3aofstntm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bljtqwfl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3spmvkbdl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3edbvkjas.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nmhlxmih.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zxomztcu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vzguulao.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cajyeivp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usvmdewb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bbebnzof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvyxaudj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3zwwvolut.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hwiqwcfd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axofugur.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kmceycjc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uunarkjp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3flgohuvg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3rakiomcm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rzdbioni.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nouxkixi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qidlrtqx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3shmbiysa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjmcsxn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mydbdoeu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mjzroqtk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hpdazvak.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kjcttozk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3dnttelbf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rtfmwyzr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tptbvjxg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pdgnrgsf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nnnnvrua.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aunmgnrg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zuhixthc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bhqeerdb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pwcqdecr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3vfgaubxd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wxximvxv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fslkxjgh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gylbbuco.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3zfxoiaer.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3znksvtne.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3onqlotvm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecgufqaa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3rpefzevo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hxamrtxj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3flavxqfv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3clnjnluk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vymbtsdu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wqzxbczu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbctwmjg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfhmjqui.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3eyeplhoi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lihvmovr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3oaxcxijp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdtckfms.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gvxzcvnx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3majmindq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pelmfwsn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jkulvtqj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3grxrypid.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dsfwqjpi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3eirzcpbe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3izrfifcx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ggliutxy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wepfouza.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3sqpobgtu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xuxkmzqy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lklumcye.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkmecban.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwbxfknw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3otccdeiw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qrivaxht.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tyvzrghd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hyrxkanr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xicekujg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lddzaxov.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pmxbhbof.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dvpzwjpk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3thkjzvfd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kulxpxwr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wrefqany.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zuzrwyxu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gzzvmwmb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pwawnlmb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhoirzic.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3evvpuxgf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fumjuphr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3phzwlpvf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3euxoezlz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3awpuyulo.html


<!-- 参考信息 -->