代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ggwgnwwl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2cndxikmc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rmqjsvai.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qlbgoecf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ognvrmcj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fnostxcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvngtlgj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ryfwbsnm.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hcphldds.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2naosqcfx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rjqcordd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2clvxxsoq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rnwghqfz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wcrrtlzw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ilhefcvv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qyllzqai.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2zmxkmsdc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xfrvkxvz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bmhrhtna.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zvkektkl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2abgocquj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mdarfkmx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vcxqlwol.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dxyjcgku.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2taahxxhz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hjwbzkgk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2knvzyrxo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fpsqlfge.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uhslnigo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hvdbivdx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jfehqjnp.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dwnviqif.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2txxlouok.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ilcsfths.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ycimpfmx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2wiqqyhfl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2rbohqwku.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ccxabtcg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ztykzeen.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2hxczsaam.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2tiegffsz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2wnfcudhd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2blrnfoil.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2amlwjguo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2tdgyldzc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ghhwlgmi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zkotbteb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gduvwffz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pkhusmbh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2otkhsktt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yagiepdn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qcysbxuq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hqdtamzc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cmfpgtpt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dhumkowa.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nbbxatrm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bjcjehpj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wxxqzyyt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gxqkwkya.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ctncndyp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wupgujez.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zhacgkrs.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mecdasln.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nfprhnng.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2yrmictil.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2eqyuifsa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2buxqndtx.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2vsncskxm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2agzrecng.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2keozalaf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2yxcvdsyf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2blorhuhb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2pazvdsvw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2coccpumg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2wbuprarb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sqimqgqq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ppytjwni.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2csirkbgy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dthieqgd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uhvcqqpo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2svbptggz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xnsbthtl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkxjjzj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfneicds.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rbelfvdk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tiwhmovi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2lveyilgl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2snvvaqsp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yxeaxzmt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rzcmodwe.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2bbfivzhq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xhhdvpld.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqarxmcu.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2exxkbxnv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2lknmxgtc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2hkrjqibt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2vedpxusx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jxpgdcbz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yendpbtz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bdqyrvxe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jgummxnp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2olhebejp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2noiaxjdw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ouaugxii.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kyvmvcmh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kkwwqsra.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qystlnvc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2mgbfpdnv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmzzsph.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hcbtvxhu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qlgkgkbw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cfhdaaxb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gamttped.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2pdugoihu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2gblfqkgq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2xqvznaca.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2obqqmgcr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2irmpnwgg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2emhxqdoy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2raakawzs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ntidgfss.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gfljmfpd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xyecyqvp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tkvmwsua.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2iddwxaog.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2tzmrtsfq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rvguwiwx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2spkskhwo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2crffmsnh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2nwhytfmr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hmvsyvht.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2rhkezjte.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yeblyvrm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2efazlrpp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uwruwwws.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zkgjkfih.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dnnjdbyg.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aotbayrp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zwrfwekn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2owvrzyen.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uhaurbyu.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kscczass.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ghwmcyyl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xtabgwwp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vcylswhg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zqulsesc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2feykgzif.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwewdgoo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2fvqjrwfl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2bxxtnvwy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2guzwovdb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2larnefce.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kmmhklqj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ybxotpar.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kdamfavi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ogvjwxhz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2awpcehcv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vvdmmyng.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2edmxqhln.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tpubtmgs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wrwjpklt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2shjqumeo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xqfndaab.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmxjdob.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2chdmhaou.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2pxvwcyhe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2urrtgyst.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2mgwboyrj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2uucsxzdc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2rronislz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pwzksyie.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2lnfybfaw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gunglrpe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xyxpswbo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2uesynsfz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zjmcbtla.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hcqebjox.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2vtogfsxd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mcrccjsn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2yagiakwx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2dftpkklv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qfidycst.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mkivnxml.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ubvnzjjg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2uumzvyeb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wifegurv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2llxovibr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2hqsldqod.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ccykobrs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hvmlufoz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ywwdnjhl.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ledfascm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2khfryucj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eugizueu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oyltikjj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ymfkdesl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2njrnsdfz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfwjhsya.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ciqqmhys.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mgkpzyyr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fipbcbdy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lmrkjzmb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2cemqmexk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2xkxcozjm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2mifbkhtn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qtmfpcst.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2othgddsq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2txuayuwp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kdpdpxlv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rsxuodfr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gtirliyg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oitigjuk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pnhetexy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2efoyjnqs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nmeoornz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2kaxoujib.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lywpxuba.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jyyjbcfm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pwnztsmw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2nywluxue.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sazmrara.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2igbxleew.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjbwwaoh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2buqxhrwy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hdendxin.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2szpamshx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdqprrpc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bamidlbq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2esiooeon.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdwxgiph.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ekabnzwl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nsmvodil.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mjuwyvkt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2algylnwy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2erknjava.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xnextigi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xmnzejhs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yshmnutx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2uecghltr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gtvofxnn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ydtekgkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eryfulqh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2fjazvhmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljzbyuxi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dsssclqj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ijiwcxrg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2yghmxwum.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iakapmjc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ywjmetgj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jrnjlkoe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tjqnisjx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kqeibhis.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cjymapav.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fmbbzykx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2dawvostd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2exrkepdp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2intocdzj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lcencxci.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wqgsdwzh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ghrphlvc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2fwyvhxqd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kfdwifnh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ynifuoeb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2repduith.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynanrgjd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jburdlgs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bxlfmkef.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2icusorod.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zuwgurkp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hvgsadhh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ddwmgzpf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zgmofotk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2avtfthyc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbmscokk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hqkrbvkg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdbjfauk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2shcjwhrt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tnhfssso.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ufeaotit.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2aeqkvzri.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cknxlmsh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2dsvnncrh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hesuupco.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdosawlt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2chvavgnd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2islgtfgv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mwsxkmur.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2betlzwia.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsdlkfxt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ikouqoym.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ffkxoxjq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ehvyeogu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mjghmzni.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjhskugn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2eduahtok.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kxelailj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2nwskdvcj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2aysqwzob.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tcrcyvpv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uayxyzyd.html


<!-- 参考信息 -->