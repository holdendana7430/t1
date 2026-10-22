代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ycynvrys.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2zcefifco.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2acvkhnrx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ehaprygr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ukxdwxcw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qknohzvx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2krqcvjdu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2sxnyxlet.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kampmdcv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jqbmbgcd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2zoxtcvoh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2udpdcrsk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2feaulghp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vxgygtnr.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kesnqcof.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hnpfaqmk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dipnhlrt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2utpzotmh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lnsccogz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2litwkxnb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2udtevzav.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2slbxrlxi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xnbdttuv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2jukpboje.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hkyadirt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tzeioovh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zpabxgvk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2sbderxue.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2tfukvhbe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wdbxnmbl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vpibulfz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ilctdfkw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2desfjcjm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2njoottiv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rehzyozg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vkkexqgj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zrtyaoxi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xtvmiiwo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fspcmsgg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bizabdnf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ndaqutly.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2smejwsam.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2daodznta.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2becaecwl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bopayoch.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yqatgfzi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rvrybgkk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2csexonla.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ecgyrxah.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rjaqlcqa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2nnprcuoe.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2brvfpbxf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2onryvuei.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2vnxmvxbh.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ucjryisy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fzlazbkp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2xuwmievt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aodwftij.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2lmtlhaca.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2egcochdw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hxpyolhq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rfoarneg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hzqtffia.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2bakxuryc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2baxlcqkd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sujvqbxc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oavuukuf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2anklfizv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvqmypcp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2sgkvdxek.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2nbistjdj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2afbckgwf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2emqpbnmc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2pqnyxwbc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ggcjdmjb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fnuefihd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wcddnzqj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfclhxwg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2yjmtlroj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jmbmznzb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzprevt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2xjehokzs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qkkfpywt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fwpewvmp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2umcczvkf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uhcosztk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xqipyouw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2awzqprbe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fzoxpovc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mekszqox.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mmoyyfzd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2smvjqsnl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2wrzbpabb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cqryutin.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2sybucvwj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pomdpdfc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrujpsw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2msbgutbj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dtuvoliy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2fqwzpllf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bhnlrojf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2laojtrvw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qwglrjqm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xqvodpvx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cpcgddvu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wibamucv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pucefgtv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qckmycci.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2oygyqhgj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2tirkzygx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pyqxksec.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aaqumdtl.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cmasgxhe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2isonzlui.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hwgkjecx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wneppghg.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dqyuryil.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2thvyerjp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xghyyhxn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sijhllot.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jagvseri.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dohyaktc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2yenkxoex.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2guapelgz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bmjyjjou.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dyyavhpf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hxrhergl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lfkzjbxo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ytyrcavu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nyrbttjy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppeuutsl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2outetutb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2sbfpqylp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2czhzfaij.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgeyyzrc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ugmdtqhi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ppsispzw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ufnebivs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ertuaaoi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ssatbxkk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jmesawkv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kzvjdgnr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bkdsgjrj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dgvogjfb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dmxizpkp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2grqkgpmf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2twripeod.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wqkfvuyu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uzanufer.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2iogkmtsn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vxgmcqmp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2gbbcxmha.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2urkwnlih.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ufyxcdyn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wwawugel.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2zjfprqso.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pmyxwjcg.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xioqizaj.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2syeuzprh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2htpqyihf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tmltnahw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2sbgyzovh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qjironel.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2timgmpfv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2rmejqnyn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wxbhdxhr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2yilimhno.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rwepjpqu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2xbbeyzfh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2vlrcenzs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2pnowxlik.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2mdybluci.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqaogdpd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2runkitzo.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2byalbfcy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqqwhry.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jhrlsrfu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2djnmehgo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2woemjwgr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jflztbdh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2voxxumtm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2guptukom.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2yjsgjiir.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2wbxpwiuw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mbpzohri.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xakvdmoi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcabqkao.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gtlvbkvs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2azuvkcjv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yacvtzpb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xpwrnvov.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2kkcjvszs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mgpihsbj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uueytiov.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nmsmqabx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtolisc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uubijxxg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2litotkzo.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2gehcqbyo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2atzrfexb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2knhyokgc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yrsnlxsu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ouyyuyee.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2buiwfjyi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xbgxaten.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mudieytn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lejuzgyc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ekzjukbi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ludslfoh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2clyovnfi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnndthrt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdqqvfkz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wneytcbp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fikxpokc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xsahpmpc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fspbkzag.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2yajnuwvc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2edkswqik.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2aiqyqryk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jmwegint.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mujorkvl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2memkgvmo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zqunhebp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ouedlngi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qjjvgnjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yorntber.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2esgiidlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emsnwwkn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zzkvjcdg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2twcynver.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nijuwmzg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cjhsbrei.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lzzlixiq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lfdecalk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qhjrutoy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wkgedebl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vyvcshcp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2uvonkdbx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2irmlqpxq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnuhdrel.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qhvhjfua.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uafdftju.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2enfhauei.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2nrnemdrm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xwqjfcgs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jxaeimwe.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2taseopxw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2sbsuzxso.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrndnrnu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mmfzldqz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bzhxcozn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nqharzrv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2kkewtysy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2btlcpyri.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xowmgmnj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mkngfadn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2obphpwjd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2bjnghzvb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dewijlop.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cqzbkcjw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxdivrwr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fpcymshe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2udybkgrr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpvqrsnx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vnecpitr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xmllofge.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2envgzbzq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yxufcnwf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fwaufwge.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fnhgtwhg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2woliyocs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2femvjfvw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvczedkz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2odqjdisl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2rhhqrrnj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwakziss.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fmxqjnsi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vbrkirtm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxczwoav.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tcsrpjoe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ngrczfkc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wokqtfot.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bgcsslks.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2viiezswf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahpqtmoc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2esabxche.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iyntxraz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aimykygk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ybyvvweq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2anqlhzmj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2leanecrx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ezixjihr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ryoblqbk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nupljztk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gwfdpjrp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qdmozuxs.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pqboxtsm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2psyxayaf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cgheadan.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ofhhajus.html


<!-- 参考信息 -->