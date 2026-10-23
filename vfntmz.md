代发 wailian999

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3qqyqtkqs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3yiqjulnc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3adhspmlc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zogdwnce.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kvvxbqvb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zakhtfpy.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3tmjmexzc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3xudlnzmr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oktfutqw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3eaydarvf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3aoofaeja.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zhmxdxmq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mlowjvxu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cttlliwt.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xpgoupqu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hjqzmzra.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xjdikzse.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uesjyslr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qpgkkuyf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3bsfjsfyr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3tzsilsfr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3awowoqko.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3whkrpkuu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3luabrjtx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3tsonndwh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvrywbe.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ujkasfdr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3qgmhsuup.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3fsoqhwuj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bpuijyrx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zfdsyjyb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hrnqlhmz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nqzlyjud.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bxbgtisq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ztexiyvr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oxpvluzs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3welyxdbl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jfivipwk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xheozpuy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qfdwvbai.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3alpltsbz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3awmvnaey.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3buhlmcux.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3uujdqyph.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3myhvqksp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eszqbjkc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ceavxnnb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwwsgcu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3setadhcg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfeqwwp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ywilioow.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3pdnwfjjh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3rqcnjyzt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kmmxabqy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uavfmoif.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qitkjbvi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3evrrvxfp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yioxejfy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3gcwcbtui.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ulkeoxrv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhcobpa.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3kitsdich.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ivpiayyb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gnmdkpvt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qgzdgoep.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rkozhkhs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzlfcbrp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfygsowg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3irxomitu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3sfgiqmng.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qdvadbud.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ojjlqjju.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ljdolpsy.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3dolmkyaf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3fnkjoydd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lmfesoeb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldvzzodw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rutwsull.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wqqgydby.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ajoxkohu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3arkdzsvc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3menucgbq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3bjywfqeu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3telzmdqh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bmntqlpv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wcabpazx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rfulqhxh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3bqfmoqsl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jxgcgmeb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ytimnerr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cmoifkqh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dztpohfm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3mxsoqwnu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lrazvrsy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vjhsmhtl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3moagnxlm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vtvljqis.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3uiresnwi.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3hzxaeudx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jfjvxgth.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jnpuvbiv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jqyznnui.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mautnkmw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kqffxbry.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cncllmys.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mzxjbnpx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cqzgkfvr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3obwzxcuq.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3oakavrat.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3mbcpwmqz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nhtjwbas.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3olswmlec.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3eiirfbxo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3zajvzwut.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dwauhaoq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lqkrjyal.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mhxvtlks.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3exmqlvwz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ezzyiwiu.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mnjmqheq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3igrudllu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fgkkhife.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zsetuuda.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ggdtlvcp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3qslwfmms.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qznzkfku.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3lceatgag.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3gvoempxs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3qsedzgom.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mhrjbepf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezrtbxar.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3prajobrb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3aqwllabr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ydlskckt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3djqfbekh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3rylxskfh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uxusyqsj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cskzetoo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hyaaoqyu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qjikinnd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zzjlqtwn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dgfzzbou.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zioczrjm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3imcnqjrb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3fidzgnpq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uttcrbgw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3quqtzpbw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cyftlcks.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vitqfcas.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3xpexiuph.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3qhuilxwf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3btgcusfe.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3egwitgnh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3esbgtqxt.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kgkntxyg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3wgxaofbj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cacolazx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3sukajekl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3mhtuotny.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3utekhbxy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jwhmvlir.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xaneqqvu.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3funwgnki.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qtoelpey.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3itmcgude.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3tylgrznw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3thmjtdta.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3lifuvjzi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vqlcvnwj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3gcvcdmid.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3yejlqqpm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xzvbsitz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jznyxqoa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ohtnycuw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvmdzhtn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3reyljcil.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qflraqfk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rnuxdqqg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dvyghtki.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3cvdggnbf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rkbafpkx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jadnrzdo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vsfrieqo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3aaqijrdd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fwnywkpw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cxrgrced.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3mybfiyea.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dkvhpgsi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ugnjbgbp.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3acmlbfap.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3egnzrnbo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3puaosmwx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zadrtbxb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fwpugouq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3moywhvtn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3pgrmjzfz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xnyqbfsj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3xpvonkmj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lgycdqlb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wqtoombn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3edcwermo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ovyzmltr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lxvzpkhg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3iaxgzhqi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3otebarit.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zpgggiec.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qfxjukkf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3acodgdpy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3sletbyyx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmbxswl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oslnczmz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdpsblsl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3amareljf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xfrylmtk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3dmfqpkor.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3btbsebjb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3phhakhdy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3kfwmqjsb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qlsrzstv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xanqrzne.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3naunrngc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlbsagu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3szcdnpcp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3phxstobd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mfldsjtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyromxcl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zfkaxmuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjxxzacf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ctovnmuv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qcvdsvrb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmdxmauj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nfdvklxo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qwbnoswq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3drrdlwok.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rpljdjon.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xjpftxoo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zdiabcsj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3snjmfova.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3eavqnult.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3dpskepdj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aabzhdcu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zgehfxks.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fhhobxfn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vyfmegon.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xdbwxuyz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wooksmwc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ndmqtpjd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tkqsklgf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkkynatj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pnesobsi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggjxfhlm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3higpsmir.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yiudfnpu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xtcuvdvo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wermvzkq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hvzodbpi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3yoyrxtko.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3cisirvvl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pukzgaoh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3leztmuxp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tdaealwx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3bwmqstbx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3opatwotc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wcggqxjx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kbpgdfsz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zgbfkajx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzxibgxj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqbjkduk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vwprxeye.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbujwrxm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvuxehe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dydvdnqd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3egiiexuz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ajttxgfl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ofwmfbss.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3aueqkrts.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ylqeojrq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3blhcvftw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjwgkvvc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rcywwodz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fgbyzksu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jlgqcznn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3lfvdttcw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xtvbfffc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zjxbhyrl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yjqxlidi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tofnuspx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zfspnjfq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wxwevpcc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vixnkjqn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pqpnjfix.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ikghetui.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3uhnoddip.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mgapzqkd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3swbjhwus.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3irodjwar.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ddxqzzgf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qaebukfo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ehopwoyz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pqpofgbr.html


<!-- 参考信息 -->