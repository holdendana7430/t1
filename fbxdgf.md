代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jhzckrqc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lhfnxhdz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3fcztfrkj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3uujhsphl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3toailkkc.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3daizlomc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3kukolved.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3flgqztpb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kylrhaed.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yudxytes.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yktogdlq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fgvtaxnv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3gzndjmto.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bafvgiol.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gmjgvztl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3jelwhnkk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3yppigfxe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hjsfypdn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rgmxksca.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3neynglab.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3tygawoof.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3cyugvgbb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3stfpurgf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3shticcxe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3rurfrnkf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xvniaqby.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3etwhvaxo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ghxafrix.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tcywdbee.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eyqzyvvi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3osrmdihm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3upzyjgxz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3lvfaereb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xbfccnhi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fnxttmnf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ojjpheyy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ifiozdmo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wyhjxmtk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jnqojpcz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3jsadfhlt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yrlobxgp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3djzldztx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zokwxinx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3qvypavfx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3pasarsfi.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvhmauv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3maipqmpi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sntuqexv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3oqzlahxj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yduhsevb.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3neaplvzn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ozyrorva.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3gmcoacye.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bnpjsulh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3chmckwcw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mnkyupjw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sisghqni.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ywbqvsht.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3erlzcfgb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ugxolztu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ixwqmlxk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdboduji.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqajnmnk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3shrjizde.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3giwibffz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3mxlqhfky.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3bximizsu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3chqyyemg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3oxtmsiqx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3mwvfnpbc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3kxzzbqwh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yhauxzxa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3eepiwwpp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sctxhjix.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ltywqhbx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3buxaeohn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3tgueukyl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ffwxfahh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3prabrued.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rbjzehfo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lrtseouc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rdsblazf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xlkcmyqu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3tzlaxlyg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kgtrixgs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jggglddi.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3mxwgqbyy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3mbvinkcw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3kkhjuzcz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dmwddbqr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hcoigzgg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3wqlkxdxp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3cbbpeqkf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fkxzklpg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3chifftwk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hwhwaifg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ffbqrort.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jojazzdb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eisfqtqq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fmsosdkd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mhoozqgy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bexkivpq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cepwtrjv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gmomxfvt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3wiqewuoi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pwzpsiza.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jlgtfhlm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3trihdjts.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3skagusac.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3aewcuttr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bsvpcjdt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3vpiakjlj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3orxechzq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ttukdsji.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bqtvpxck.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ngusudom.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hykjsrzb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3reisvfws.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3omckzzaf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hutshgjs.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tdghwahh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ystxsexk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ooxvwvgr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eanskokv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3immdmqid.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3zuzvexuo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ywhbgsnk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3icnbuuzz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ptijfwht.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3dtyurmdn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jzwjioyr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3mvkdndcj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nvriuyum.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tdlmcdft.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eohuzwna.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yeipicrp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vsyglmph.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wchnfwrr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yxqrwpnl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rsypmrjf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3kiphvdij.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yywakxmi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xuttxdgt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3urdycrdl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3owiodhnq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3nlzorvcr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3bsmmqzmj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3adppzizo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3icxjelqd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3svghwrya.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3phohguys.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ivnilxha.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kmxowuff.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eztijsii.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3tbfjevzm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3prfyhyns.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qqqscppy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3lskjtifi.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xjfvxldp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3hfefmtmr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3uzgmuaij.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3uilcpubv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3eykhflgx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3gnwcuwuc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3rcbbgfyh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wsvfmueb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fbaumaiu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kszslull.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3svzxalgq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kltmcrdb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xobvpbva.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xvcnkngj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bpctzfjn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yjryznnn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jnzhzpyg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ayytbwft.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hewkrwgi.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3padhrqnd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3lngukdox.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3iimljncg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vqxvfxrg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3skwuzoaf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsepyepn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ygjcmxdt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3svttqwhk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wkyntifm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3oggqpfqa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqytyos.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qzccbuef.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ipebamdd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3grzpupxa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhyxlpkj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3obkgqnei.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3whexdesi.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3gpxphuph.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3oletgkij.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzybgpls.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3thofhewe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aduubvkp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hoaewtku.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3swecypnw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ausgnlwm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3axjhvksr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ovrzjkey.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3mbtlhkfk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3dlokdtrr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3eubagipu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rajksuej.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxjbezx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hnqpajqi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3snwabgdw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lssmlbzy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3aspfllmm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3wubyzlhq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3xyomyqcw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3vdrstbhd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3bxdjwras.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gteaxcky.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jbpfunhl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kuzptmur.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvdfpoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zwzcpgoi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qarfnohv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbmstdbq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qekzhbzx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3grtcnhak.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jqucwctv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3regyqlmx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3unrnabmj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jpxzcgot.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3agddezkq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vyyfugta.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jrgemsob.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3daidljft.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3uwdprlas.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zjyvpyfo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ktfhwtre.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xqmcjrqd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ijthqhhk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3sxyzjjvg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uwvpeiww.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nfoqrphx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tfjjdkls.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jxflqdyg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rkognevm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iskqggva.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ianfvmro.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eiyebxmr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dltnhmuo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3zydcwatq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jaxqptby.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3chwjslsl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3yhjyoqnk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ijtwgixm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hqenfkap.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxzgkeoo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuykffzz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wwwlhgtm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pgfwoqof.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3zacbigcw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3knuxapdu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3wrrlrebc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqmjymnj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mstdbixn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3plkoyppj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wndrieuc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lbssyomf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3autqcnzn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ruuwrgeb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3xoizggpz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3aztnumyi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ewguocwg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvdtakhi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3krsnycvy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qkabgxza.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uqmqkuzu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3evrsdwyn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3opepjimm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3svovbgxm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cuarpggd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yordmzsy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qggwxuvz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3obqjdldy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yibbgesy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3rgeckzcm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3narzwdnt.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnlpvmtm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nqakphrl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vcteadlh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gashhqrt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ouhlrdnr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vjuedlzd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mgwwhnoj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qhsbtcax.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hvelwlxd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vxozotqv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gcglkioi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bdxdxpum.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xqfijibb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lszcgpkm.html


<!-- 参考信息 -->