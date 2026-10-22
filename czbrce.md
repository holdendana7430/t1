代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foqjblgl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctjwatvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibylxhrt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tflqheqg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2srfwubig.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ffmyovwj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2panpyyck.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ypqiptdl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2aamdgvjx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rjdchelv.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ddqdzbws.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fftgtapv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2nkjgabdw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2iadnwxwg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wajzysod.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xmrbdjrj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yzdxbesp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jnhgmqdu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2nwxlrfbz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2iyirumqb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2igcndikj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lgrkpdnq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xoawjutg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fyzxitcu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2clnudbgj.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ovbtrvwi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zywbmldx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2geiqdijr.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cbqicngk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sqlapavj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zdvbcqcx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtnrpes.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwfpakc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ctfqfbjz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2orglcyto.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jnsaunjf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2paurlsdd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2nhemznrj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2khwujpsp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2zzftojme.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2pdacfrxf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hdmafjwa.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rnnrerar.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xwcogcit.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2urzlkgfp.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cbcvchhf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ogvtbhes.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2oaqohero.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yxmluumr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wvpndbao.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2fviejslg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2vammyeqc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lcnpwmyq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2aotzptkc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2enkifuqf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2uxoyrpqp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hwmdjgfn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2cpzedhio.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fnwpnenb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2koxrxeem.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qyygnsnr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2unglctzj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2viwwwawk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2htidknxv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2aegfwjze.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2hlaxhlmj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2bhxytnge.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zafukwjb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkpdjgcm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jeaflrmg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2mkiyvfzj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2azpekvyk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bicrlofr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2eauuuobu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jeisgosj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2doyzgmso.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rbrcpyba.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cafmrile.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uymdfpch.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpyqkvsq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jwruauxe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2gtjrsaox.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2dssshefx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bqbngwda.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ohhdsudg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2eqwiwvdn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ymzrjail.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tmtipiif.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qxqhqvyd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zhyotaak.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2gstnvleg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvshvcw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rlaasyaa.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2jlyzoulp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2umtbckgi.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fzchffhg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bbzmzizo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bzxzbgvl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2webvacou.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2fcqiffjk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vlkfaujk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ufaidzxe.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2zgtnhnbh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2xdmkhoeq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gazphips.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mwjsivfa.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uyzpqqtj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2njmgcbin.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2tixuqbos.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vhdfbyyx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ahdqlpfv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rolwyoor.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eimcgwwt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eypmdmre.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pgmnrgwq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tnfpfbsa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bawhhhww.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2emarwgte.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2asacnsra.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mxgzvgto.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2krzmzicb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2uddtkvgj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sscaozah.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2orcbthmc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hiiycmqt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ezptxiin.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jbdqnqcp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ipotnjsx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ubvkloyn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2osbjglbl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2creqrtey.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bepujjdz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pnibtbeg.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qnremjyk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2lvqshvyq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2jbzkpboa.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lqirvwcm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2acppgsza.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2wnqudjqy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ptrakufz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uwzawxch.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2szcsikcw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2qzwsspds.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zngwjjiy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2nogucdza.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ijzicjsh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2syojbren.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wmkyyjle.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2udcpvmry.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zyfkcgsx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxstmvkt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2utgfmexz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zdgvvhix.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nnjhtjpt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kltomfsp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2thyudiuv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2yevrjgjn.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tfkufsvm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xgbmiirw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hafibxfj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mytavjrt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rpklnvcm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2mvhhgvzb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2rmxvnlbs.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2coxyinhf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2yophgknp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2erwkwsmk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2vfwvnpsn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2msmjtsze.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ipdxzulc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2lxdludns.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ujaxsgib.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rxxbtrop.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dvnpjjco.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2bkisgggb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2hxiinvwx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2rdjtqzap.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2lpmzkjfj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cltfprwa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2lebyoiyx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2mxadyurc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2fjuhzkes.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2asvlunok.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2okaplxji.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2urxskwid.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hjdxkspd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqfikbih.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jzatbxdk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2muyhqimq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dfuonitw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qybvvlsk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2hjvbtkfr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gnjneyff.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2pxrvhgyj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2toopawxs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2laewdapf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zpbhsjfj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2dzbwnkoy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2noisvqnp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2hpjtafzg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2jalvucjh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2efwynoth.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2cbxkvrmt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkfcprbg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2blqwptbj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jjakogev.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ncopfmwn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gkixsdsw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uzbwutbh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fanurvmx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2sphimvgm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fugwalox.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgtwsnqg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jvewnjho.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fwvodfgf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2shwqfwkx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhblswv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cppvnsfv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2uuoypknv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pqcdxiup.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zwbjmpxz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2zlcfuoir.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vmakqhtn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rzzceyjy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fzqifvfs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ysusgwxt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lurdcryq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiemgqrc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2kshgduru.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2cttrhaui.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2zirekyzu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2vobcfbdz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cnjikzcd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kkgzshtn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jxxrqwut.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jhzyjtsy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nuklaswl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chtwkgrs.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2fphccwxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtafvlug.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2scqhovou.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2izxukwhc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kqgjhein.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aeyzaogg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2umtqrqza.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fgmkdood.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ddezhvxd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2poduvuno.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2itnhsgpb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vwgttuzb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2wwqcypue.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nacajaeq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ytakegqk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jnnnzeva.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2okbcmbrs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wmavytnn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2myfvbiqs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jdfjdgjq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2munhgxzk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xjlfiapi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2utzslpdf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpdbskvg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2idmwiggt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kkgzxfau.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2lkoweatf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mclhmffy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ckuardcl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hwruwcjj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cluitjva.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2spbdvkco.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2szcduflp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uhyddhqr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2tbegayba.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2yabueept.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lhdgghnp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2isfliiis.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sifvtusr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2bhelweyc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwwddyhv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lcslvyoe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vpsdsgmi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxkswsuz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2trtbooiq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ffewxrkt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zlpscxhy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vtvfeqbm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2khteoovl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egdycmds.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2agmyusoa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2azkzaacp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgplrusw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tyzlybqi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2heqiunod.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zvddlcxs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2znnfxqzg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2archliod.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kigwxvgb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vroibjns.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gahsjwoo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oeitptty.html


<!-- 参考信息 -->