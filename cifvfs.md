代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fnrhpkpk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2gdladvyg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2tfaqvfmt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2veoygorz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tyljgypb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ypybqdtf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mjsezpgt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2txxhxgzn.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tqyjutix.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yukhqpfi.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2riqqgmaf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2uwudofvw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssvplteg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wsahojwp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ucifxamh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mgdqzbfa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2izejrfym.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ibiuclip.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2fgmxgpjm.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2msgyuksz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2beohkuso.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zboxoxpf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2agzojaij.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vaoilefm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yzvtelox.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wrajtozs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bmrnmebo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tgvgapyc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zpgmdvev.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jtjwiyhe.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2imrtsfyh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ogvnqjxa.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kcpgiwih.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dkypoorn.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2uljuazso.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vftscgft.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ykdbitbh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lqikkdch.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zrsargsu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nitjurhk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nbeftwuo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2beeplelj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2nejzasqj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfrnqpr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2owhjdzpz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2palrwfvc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2wjwrjqcd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dbxsnrts.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2vhhbzksl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nejpgzvp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2wmpbiutt.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kvgvzmkc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2feedmgsr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2yyojkvoi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2waidohwp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xvpqehfx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ifpjgtyn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uiwrhhgt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ieakkcrd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gdsibrtr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ncmxgdzs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2yiyfloxn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2frrhcifi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mvodkujn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2acgcomlv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bgcpmmsm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2qcwgxord.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmtdrkgg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kwmfbpcb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jwwkuixk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2owffeekv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2mwxkojsg.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjdtnmk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hnegfveg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2thlqkeno.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hfutrjta.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2almovpqn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dhsaqhcu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gxqmmmoj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2phqpwbig.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mcqtahjq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mnxtkwyq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2htvmvlkw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tevlcmtl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2tmwiexeq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2iqrsvgkl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gqyefpan.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2uyfinrfz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fiosoxrd.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2pmniyuhd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kfmfwvim.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hgkqhcsk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fojxdmky.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qhjdsfwi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pzznpgfu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gtyhqwci.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kvteluiy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2smbwwifu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ngylbvcl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2enypcxbc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2mfrmdemn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2elvyzlar.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tzyftgna.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2llzypjbm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lqzvryvr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rcigznml.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2koumogtk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2eqpglmni.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pfgwqtft.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2fsnhplgq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hsmyapmb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ogsnugeh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mpmoqlmo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dxmhtbrj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2egxlleez.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2tnlgtclk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ciysuxqr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sfxbzsgt.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2wogtakwc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2zxvinlzn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2dswvwwgu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2tdonhody.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfwnknus.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwqhuiji.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2srxolzxe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vfnsqppt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mslwgchm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2qqvebqnd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2irstyimu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2llrceurh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2drclevvc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2detompua.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjmtnheb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmwznumg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ksiannnr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wubrusyu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2zwjqbyqi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rvuqwjns.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2doctinup.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wzfvigdu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kmwuoueg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lwigknfk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2umftndpx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2sfwobnae.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2gyfhkfnk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bcbqvkrg.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rpzxduql.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2csqrdydo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ozvfedfb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fnvduhbn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2eldyikho.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2riypveqc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zquxxzhe.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2unitqsdz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2epcxniri.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gmgdlsyz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2suvvoxvm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ganghlbr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2tkderpqh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2yajhlndh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tfmfadic.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2akbbaagl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qysxepxz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2dbivpzrd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ctxtcfga.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mjylkjqs.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2axahtgix.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqmftxsj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2awlbbdyz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nrhhoijs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pdbtefpu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kzuyijvu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2frfswmga.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vcbvxycu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2zdsuoyuy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2fgtihvdl.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2haaoszmk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qxekdnsq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bdseshdi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sqmtiamf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2oeplssru.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2etrounsf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ifpgzahs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2rnvdcgng.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jvptjjft.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yaoazcqn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ysvxziyu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mmqzpesc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vdvjzhwm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2iaqzthei.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2lfppgmzy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ejgiaepy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yjkdzagm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zvybepqq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rhnyazri.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2gixjevte.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2mtmbenuu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2wcbbkdbq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qeivtcol.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ganatpbl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hztezxgw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrqwxuir.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2opwcwzdy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjutumpk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qhpgbrxk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cubktzhv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2yspxjwmb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2oizrnolk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kbqbtvgl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2sqvwfhaj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2wwqfrqts.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ubdbfflb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2igwgatuz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ldgohsay.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ynjgcxtc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tdizsvxe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jjdquemt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bogypypw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2bjjmgaya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncxryoux.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2awxubtqd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2srtttzqq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zytvlkhx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tawhkmwe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2drgotawa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mlbdbzbm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2nemtitzw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2lfyzdqmm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tdbntvae.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2xunvamwr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ibwydyzb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2tgwrhxcy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2otiymhpw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cscekmnu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hflsttru.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2mhwmuqyp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kqbjvdyy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qrfouwes.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jblehpcc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ftaysaei.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkjwrhti.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycadsdqt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgpvhdag.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzyxvznh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ffpcxhvr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ukplsxwl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ivesocuo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lvcnizqu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hgxhfdgw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2xxirtvcm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgozktie.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ejweukuz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bzrblnei.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jcmiweop.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2chagqegg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkkeitkq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jqaunhcl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pwruzrso.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dejlmaba.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruzhrzyg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2srqkzadr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlpgndxo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uurcaekw.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hguoxkqj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqavfrpt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zxogowzg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nqcpiidj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyehydnl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kewpyrnk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lyvvkyly.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uirvdcpn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ymlcwfas.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ofzghlcr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxghmgnw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ocvcdool.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktkaofpn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfltpok.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2svljbwxz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2atrxvxfp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpgwvyvx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tbmjcmwk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2smkqawca.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2efahztrb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2epsdknit.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dbpqzcjy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vlmtuoqu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zcfnoxuk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fgqfplzg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nyscwlmg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fvvumqzw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2peqifnfx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kuucrjgz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2qskjcsix.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gbqvlguc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2utsxbtij.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivogweys.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mvfmthhl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2szfdkfvi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjwymuff.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nmzpdrvc.html


<!-- 参考信息 -->