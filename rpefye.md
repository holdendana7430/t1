代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qxvhoojv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nbwkulgf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gdzkrzfc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gqkuvtcm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3fkbuutit.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3vernvhwh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tatqexuk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3eotfhavh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xttojbvk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cbfjeoqi.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3dvjatumu.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dinjnkez.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3satpabjh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3enyggqnj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3jssxcxwf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yqfscdwk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ofiqywpj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yecxeckh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eqftbbdv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nbszhcaq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3fowzrrdl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ykfbzkpq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hzejeabp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ymvcidvt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3udcoykkc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3iqiaabdl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nfbmhtax.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3rsryvlse.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3mthdblno.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ghebbbyz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3scbfqbdd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3uayudusy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mrkvyqnw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rgaxxuxt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ejueqlfk.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tnfowilr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3riquiasv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dxguvtqf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rjloivsi.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zstmgreo.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mcpmwuqx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rwyuzbyg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3mtbqygkn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gwwrjmwu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3joeepzkx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pymikium.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3diimpxrs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ikyohdxa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3igesqqhn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3bppuqqdd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3kmmkrsol.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3holuljfn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3hvzjkkwa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ohsewdmv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3yupnejzg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hwbqwrps.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3nqjweppf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tgukufum.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3kionixuw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3twbvcfnj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qfmwjzwu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3suyjjmjk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3iankqlef.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3txzbwlju.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3anbhowwg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3dkrchmev.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nqciqopq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qehcwoig.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mudlqflr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iqkbskvc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ftilbitk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lznsvkcd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3skcjdfoh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3imtjteyh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3rfhueack.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3blcmdyhj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3iobbkisq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3wywjfjyb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fystwbqy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mapbhvev.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nkuejmic.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lifsgzsa.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qgnporhs.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ykkbyruh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3twkncgrm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3saixluky.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3axueszoc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3njarpaps.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3odfzrzga.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ufatqdlx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xuqexokr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bkwqftkd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yrdrkrug.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tmfjenap.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3fgxnkldw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ojwwegyn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qdnepyfo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xqtwbtkw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hxbphcrp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3qqxwxjxf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wwpzjhdr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3heqkdvnp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3bhdicibk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3trlasgsv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oeuffflt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3chazmnwc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hiynkrch.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zuyxerhs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bqbjvkpy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vsjgdgdt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3saakucym.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zugzjybp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ghpxjtwf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3miblatce.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rniqzaix.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jxmsshks.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ltxwydnb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ywskklhi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3djfoedtn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3fnqrkahl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nsgegdvk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ylaxdulu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jzyrqpdk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fzijqrky.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oghvpcnv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wkqkamqs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gadwqwnk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3nbmprmic.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hujkutmf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3usojmflx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ybfrdlrg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3aankfcah.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3kohyacrs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kpsqavrq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owgziehy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ciefuavr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3szsuvaex.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3zzakdpts.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usywunwj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3pkaabxyk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hyekljmc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eidajmtm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bipkhshy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hejfclfj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gnlbkoqu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bvjyqkdw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rxghzqbk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3twfcemyb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wijqbkuy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ezsdsegy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ugxhzauy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3dyscqbqy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3prpqtwbl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3knvfnmzz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3fopivfqh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3cmnkelyq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ajghbqnk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3bfsdgaez.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3scbqrgnw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3omjqkzpz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3cmxnomby.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3cdbshgiu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3dsbrilok.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fvkdfcgc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kusxfpni.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3gvlzqzum.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3recmwduh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3skxmybfs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hofqmomu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fbamjdps.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3kdpdlrft.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3iqrmlyqr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3szepofpi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3jeyxfyja.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wyxflfzy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3edgerlut.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3xrekarkd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmtnnjz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uyiczgjf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjesjrme.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hfxkgjjt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rpidanfx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3esoryxby.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ieeoebwu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ywqrlxwr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3smgjajmg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3coqgvrip.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ruhovhcu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vsizkmac.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3llzcaymk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3rvumtdiw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3hobgfhjp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sfqxlxrt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sniyympz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3owtuxkdk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3alikogbk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wtxrtiae.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wdenugvs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gavcuwpu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oeweuzvp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ndmsmmsc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ylofgnhd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3luujpjre.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3csnugjlx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zqriiftb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xcdvzgct.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uwgzdcus.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3matlrinv.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnhjvuul.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rcfuerxh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lpiffism.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gmeaowop.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jrwpwwzp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vzcbxvbe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ptefnkpw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3uzzolvco.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvvbpstb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3caozbibj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3itcxjfkj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3whkaqczr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xgnkegeq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xnpjrdew.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgrfjmz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3sbxceylm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ydmasabl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hkavlrnn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zlouvjud.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3acisqmyd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ukyfokxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvjfilwv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3uozhlahq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fectkimj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3cynoqndx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xldkosbr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vunxvrtw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ubzlbwsu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3llgkvznx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gzwvfomi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ylccnhhg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3wnqwbkrx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ezbpxkxy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vmvdzbkb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vxkoqxph.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3brpgzzxo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3naavxrpe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rmvehrhd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lsgoznxw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gyqsqtqr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ouxoollw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ldackafo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gcwtiwwa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lrwppgrv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yitmoetm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frsjhevm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3atugipxc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kzrssbuz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3exmmkpoz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qiiqbrhv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rkulpjch.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hvwlyhre.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3uskomdpu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vyexjjti.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zorxwzap.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vkjmenqo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3expsyztm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3eldrhdjp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3anjqrsmg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nnxkmpqz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mdlxgnre.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3coccwnzg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3aweamdbn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cgajcbwk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrszfepj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3shulmlxw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3enxghfmt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3txrggamq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3btpfputl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qjsvtkuf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wlbnejya.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rvuzvokb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfezuipm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3drvyqhrr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3gqhjogjk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3svtbuirp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xlavajrj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3lnrqwinf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qvljvonj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynqttgtm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfhwpiua.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssboohiw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3otqprfkk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3inwiqlbz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zxmwqecr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbycrcfb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdcmkiib.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vdlikgmf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3olqqdpek.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3abmrjqzl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bddzyvzj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3minjvwxx.html


<!-- 参考信息 -->