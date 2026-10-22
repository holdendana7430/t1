代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bgbxkpsm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2qpahuavg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jhkkregi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lktndfcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vadplmcg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2omocokly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtenndzb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2bagumsmw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sqmygwkh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ikgvlduh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mkdtqqpn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ntkbteil.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ssydwivr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yhnfdmct.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2gibvnivm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xrmxjmkj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2uiezxbly.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2wxggtfyy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nciijihj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2aouxwifw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fivqcsau.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vtuipozn.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2lwozksab.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2uoehoafh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oywclmsv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lwhizktj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2pszvymel.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ulhujmhl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pzkebgxz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2relfnrbd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fizjpmax.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yopgibgd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tajcnmbc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ayszmunc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2spgfsqfo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqhiwmo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2enubilti.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wsjlzjqh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hwvnyqnc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2qaqvkool.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2zflpspmf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2uhhhxhbg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pdjsatcd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2mbdwiqph.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2kngwkvdc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xyazkgik.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cxcrsroo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nnxkmnde.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2htspljcr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gbbdaunc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2afnsuvbo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wvayksba.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2krmuuukd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qzzblynb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2aglnobqq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2otxokdfo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sxijwnya.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mgphlbzf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qteshzqp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2psdtuvvc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pffhbfov.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ykvhbjbh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xqnymioz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2bgyxtsmy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ursieljw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vggzpvru.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bxbochmj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vmjseqak.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ezarankp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gageyjxz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2kdoolvps.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bsnfiynl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxorxyo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nhuboftq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wkzsbjch.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lskpogba.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ywaaiqhm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2dcdxilat.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nctphdep.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2txgcgudx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yonjfqql.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tjusoltm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2juxbilcr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2owruusui.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pmmvhsfk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2vejniysh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qpijvqcr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wilashav.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2bfrkmbav.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2aihgzvro.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2hdopetkh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ejlgixqy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gqqlltch.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2upabxadf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vhtmuost.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2hxhxorlr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ilpbxmgk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ndydhulg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2acohgzis.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wfviyvmp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gjvbcmxf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wvfhcvuv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2skqjctif.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2kealnrag.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wulahupl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ujjguxgs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xtdzhvfd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rxycvzuv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2bdbvmgbg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xecumdkr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vccvsaaz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ullueeef.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2sqqrjglj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2attfnxyh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2lzlmcfic.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2zgthysjw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ucckqoas.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bytcjxvs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nztmqoax.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sivwmlqp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aniizykm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yzwumkjh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yjluixoq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2azatxvse.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2kufaqojd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2gdsovmro.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dmueccmw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xskmqhlm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pudrqvtq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2tllkrzem.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ydrngfha.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ovbskvoq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hvylrlrc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2swssmwim.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2igubqhyb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zvsyxzgv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kafjeuwf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jjqdwcgc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2uiotucft.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2zcivkzqt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2cfiedziv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dmrbgwpw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qqwtbsga.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2duhunfcb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2bcupfxjx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nwzucoie.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgxrkocy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwjmrvrr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2kuwtewbk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2dogwupvj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dizylrzg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tikqezer.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yizzjzer.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aslyggiy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2exuibmmp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2usqbuunp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hikmmnil.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yjxjfykm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mdqpwikz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2djikbhgw.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2lbifyaql.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ypgtcbrd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pzbqnjeb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2yaabzzmj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gbxnyqmd.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2xovwsjfh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2dxazxupy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2pxywlpdw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2eixktqra.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2hofufepw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pzxrcghg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2tcadkguv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ifhcbfsp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2tcvdhzve.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ypfcbovz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cmuecyft.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nrohrchd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2zhpohdgj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ddnvrmho.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2vaamsalx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uhpxqdmv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2nobwlgpe.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kprbotwx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2bxvmrrtr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2evvkfkzo.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2sostzvwe.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2jjfciktl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hbqemohq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ldvjhvvk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xkuduxsr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfyrxjra.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2moqebozd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gadmybtl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ejunhvxw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iovkuxbb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2akknrnkt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zgodbzvh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2bzxluqmh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2phwvglqy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2uvyrikjv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jsdgjxim.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wntcnqrz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2weshkcmw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2efwqzcql.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2uwpvgeto.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kzljjzsa.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lnaodxul.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xcjyblsc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qhkkqemt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jlzifijn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2iahvkcfo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hxzriquf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wuznqseh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2giikipfq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2fntaktkc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2dwabhyeu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kmnqgiul.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ixzlkwog.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nuvviuvu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jnzxihwm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ivyxregi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2fvewipof.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wfzkmcxr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rgqdreja.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2iordslbl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2egjglbfk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bhhckmyz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zceedyhz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2hzdsqwtn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bsadvyjb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xkzaxnuq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kewejees.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2egtdusaq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2eqhrwbrt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2crhvlcwm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2sdhklyjb.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lbqmxslk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2arsqdvse.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2assjrgwt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dzptmdll.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fmklvoul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qttcwnoe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2thpgdpze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qducscnc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2cwnmxyow.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2khynbflp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2usxybknm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sjvtcwna.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2roszwnjl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ctohihrn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2cizgxcus.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2tjjuawuc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2atkvmyfn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2kjixzjoa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2yhqnzgru.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmndvzjs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dtjxzahu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iwphdczr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mcwafxju.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2uhkvnaeu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2flbjwwsw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iedltfic.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2subeficq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ohoighlr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqnbelwe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jhpastqs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2efhsunsx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pvsrbeyw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kdgjupxl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2atrmhbtr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zxbhkunr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vpocpzja.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2awsxvzby.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2umtldcvs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hhfcobkd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuijbalt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfdzolxp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2aqutgwhq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2neoulntm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdckepqp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wrgklazt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2iqdckhdn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2xjhzxguh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ryxaxeqq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzttwjdp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fasekejk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pxfmxmlj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ofiqbryz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2uqsjvajl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vhxsxcyy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ypkyscxi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjclqvpo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2niyrbdbh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hystzcfz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2moxifrxu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvufnpxq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hhiqmfge.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dglwmtvq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2iszhmsrp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2aadqyoiw.html


<!-- 参考信息 -->