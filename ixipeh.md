代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hutbltmm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2oeuqhlmy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2yuwsacdm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sqgnrpry.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2zcjkflfl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zeydtbpj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kvkwylnf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cffearhf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qkqstabs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2akyhiqrv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2mwowmudm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2znapuwcv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ijiuckse.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2exyegmjt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2bmcngjqs.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ophblebj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wrxbhtfk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uevvzjbk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ypdtkyus.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2dqvuuwdi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2bdasxxoi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xdoxkshc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2exkdmeri.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jmukcrkw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2itulgufq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xvcqukcg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2axifdvtw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2tuhkexso.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2qignueuv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2nbpheshd.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2xuenepwk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2bllsoisb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2xxawvwqr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2comqekeo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rbrjzlhq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnmxarwy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pzclydnt.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pqefofjz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ktdfmjvv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eqnhmhtk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2iduxwlds.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jopobtyw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vornovkq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2avhkfxlo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2icrdtncc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jlpysrgk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2qoaynisw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2damuhrgz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hjpxwgon.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2stpcolet.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fzqsgapr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bhmagepd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ffwwdwdl.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2vfyaowai.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wfhutdwd.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2yfmnrzfb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2zodcwddh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lzohebvj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2ogyxlksj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ndifgkgg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dmhscbzf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xndtvplh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fcouthta.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dttnzvjp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sawtcbrr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qqwztcax.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fuxhgbbu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hjwqtfhf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzhpabey.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdoidmrw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpllhgof.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ybivzcir.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjbwqqw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2izxicvgp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2lgfhhjsb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ygpasnlx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2oxfsndkl.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2tmeerwnn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2yizxilym.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ioiqjwlp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2axdgmqpk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2idclpdwb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jooslhfp.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2hhqtauxi.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2stkihfoh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2jjqhesnu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2uchnhngy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hsjyrgik.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2azohztcw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kyanubte.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ouuyljch.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2hhzqhbuc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tevudfkv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vacbhorr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2qltcrgox.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2lizbbkrt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ylqaolii.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bzievevi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2egegrjto.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ecuidzvn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oepusysh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bkfrqruz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2nupmjahd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2dvjmztnq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zfkfcinq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jmhypesd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ycjeiirs.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2caeqedrx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ftypzhmv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xugcjncs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zjaeybrj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2woopqnrg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2wqgrtjus.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2riyfdgcs.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2siysdogy.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ldtzhyyk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2idbpqqko.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qtbbdjki.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wxxfsygg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ofejricd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wsfhbfzj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2idkivutb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lckmzrdr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mvizuktl.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ktptckip.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aylkoisg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2cqwlgljq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2grgaoozk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hgtglojo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2stsehghk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2dfgyqodk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2dwjljnrn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2nqcuhowl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2svcsjcja.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svtthpdk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atcmfrtg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2pivatpcr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vorwewjw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nnqckgup.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2luhzebnv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ccyvrwkz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tdhaoizq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxphwrwh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzckepoh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zulnvsaa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ytlsiumi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tspyljtc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2caqwyhjj.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ymkuudsh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xgaboeke.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2shzbascf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ljkytezb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lnlndqab.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bnneusxp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2rmhfsjjy.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yvbobrif.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2aeopnqee.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mvsavohx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vpxtxqfs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zzetmfoz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iycchwzj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2uguojfse.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2uzcegeik.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wnomxsqs.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2duqvvzpu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2awtgxnqh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2pnruzync.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2pxcjixog.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2dgpcjahu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ghaxdcnr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qrtchuml.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2okozcuzf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2jydcgnne.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2zxgvnlkg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2njpahiuo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wahzqvsp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2xgmhydlg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2resiwvzp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rfdlahlx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ksnkntxs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dajupnog.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cysyluda.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2shsuqdnp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qmcblwnw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2icsifidb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwdjzssq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2qbksotxx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wuquyqun.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iplbgwyx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2auireqgv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2nlwwcfyz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2njsbsytl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fsjktylx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2dtcettdd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2sbkqneru.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrchadbh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2itmjxpgt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2diyrvytq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mgzrxhhk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mrpblzvt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fybzskwl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2errttyjx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2eectueyd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2kmqaikfm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvemorra.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hpigjptx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2smggtnvp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2szcrofrq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2urdnhtal.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lvgdqdju.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jshyxypp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xkmfqvuf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xumztcos.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fktrdjpv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pqmgfsof.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2dvmtlqnq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xslkeiux.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsnpjacu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ldkmrdpv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cqogacsm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2lztngwbk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2lwdawgao.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xyganfen.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hyuqtwot.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2dlhccwoe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vrwqbsfv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2oqvaeutq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ctsskits.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sexeodue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzjpknje.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vvydoodr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhrdzyzj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2jpnazsml.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vwfefafv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2qkfwktux.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xxpkczou.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kumrrgpw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kmaxcjfn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2siuikgjj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2nekwojlh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2usljlpwy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pwmpvcbl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ezbvcvbz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydfmejji.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dfzjuncz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pgoyulfa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cqjpbvlp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wnofswme.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2pdkivlne.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2daskelep.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lsaoudtu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gecswrkz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mnvakjnw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgxkxqpi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfowbyte.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xnlgxtaz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xzkrqwgg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jkvucidi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vpiiwvrp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ljnfzdmj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2aptzvwbd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciipzgce.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvzwnglb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2couhjuvd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qxqhohsf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2tlbmjfur.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2dflaueqo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mpxavczx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uyoxecaw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ebuqayji.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dsdibfre.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixbdktja.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbbsueg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovimjnpm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2bbdxzmmi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bgbztnyr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fklgchon.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ofnhmajs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2sntqhjfp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2welygdvk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mwbdhwon.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrvbkwl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfibjtoh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tdhvohuk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uzinrjqb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2oiwlkhcy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vspayjzj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lmqlkjzl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rwsgvhnv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kbpiqqou.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wgrlceav.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xewrpvpa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bmyvjpyt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vgdpamco.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vtywtbte.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2drmbzixn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wwtvzvxs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2euvvpfev.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ybaivuqr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kyybuykm.html


<!-- 参考信息 -->