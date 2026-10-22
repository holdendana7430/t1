代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uecxmqpb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2slczlgyz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ivawazmq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wllyylpj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lsffqbjs.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jqhvxtle.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2klxcngdq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hcojamku.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jdohbpbd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oguyjnnw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vpcejjcy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2sgfotgrf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vekohvrj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fexxrozt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2txpsjwvl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hxeotnoj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2zvpiiqkq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ziqaeubh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2htqbrkos.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jvpqqusq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2dmfknxdb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eygjgcqy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dytidyuv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nzybwrxy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tmeabhno.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2esklyjnr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nqnxirfo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xzognzqr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yamqbjjc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kjatzbtw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yeaunehm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2gdxoyryo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tniftpaf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rvzalnvf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ekhufulm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ihmbctwi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2oqvnyhah.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2vodcdjyg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2diinnmbe.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2xozkrqfl.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2pcxmsitu.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2rjjfubak.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rsyydkbc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnzcgct.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2gfxgnhza.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ltahxcus.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2iqyyxvon.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ibivkuni.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2udmujyhv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ytagbkex.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gmuwsctw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ngynxfkz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rgrdqobe.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2zqbcroaz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vtwmmovw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2iijjtzth.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rvrauliu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ixsagjwg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ufpddtzp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayfgbfom.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkzqosqq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2omcubazu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zbfisozu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yncscuan.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cxfwjgdm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bjdousbl.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2nugjqyrj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2spfuhyab.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2uoibefzd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2isayizyf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fkffenxs.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2mjgzpdsa.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2nwxeyhoz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2gmrcwsih.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ofbggndq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wyrxfomt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zokradlr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2satpblba.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rtgqcfij.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2byatkdqh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pagoybsj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2doqjoezl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2haxdcnrj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhyufdwq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2honistma.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2suqqgzsh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xmxtuxii.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gtelbdsv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2czitabtk.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2snjmgkim.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cmjlrazw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ycpxfdwz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dikwrrtf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xmoccjwj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wkipbuka.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vergrbkw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aoeemtft.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ywaxkzkr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aofivxyc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qnppdjcl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rdnghzbs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2rbqnxevw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rqrbpzua.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xuobzbub.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gsbvyzwq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2womtmkni.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sdpsywaa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ljqxzwzw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sszqvoxm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2wxjbbruz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2dsoxjikl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hralhfcw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jzitohiq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2scbwpsvx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2mwuqzdlm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hegfakxw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nlncwumd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mmrullnr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2yinqazzy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mpcrvnnh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2tafgsakg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2tvoscrqn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jegnizox.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdujdjrb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2nqaxxsdy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mxjehzbb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpejixxk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2petknpdt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zvbudhfj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvfpwvbi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2twagtvjx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2edcliglh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbxqnevk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjgfwfkv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjgyncvd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ilqwdaed.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2wvnitehz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eyybmgxt.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lxhwjlnv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2sntnbeeg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qhjtexyv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lilrjiyr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2wnogthmm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yiztgaja.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cjaoffmt.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2znivuosh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fvwrlmmw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2uruonoak.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qmerngpj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nvdyavsb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dsorupkt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uhxcwuym.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2usvkziho.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xmyjogij.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2vkvtmuwy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2cjzdjror.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2fapewmoe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2hbqfdotr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ojpuzhbr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jrehobyq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2bvrfbfqh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2tecrfqin.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2rezjpktb.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2vtwlidin.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2nphgyxzc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vhptsoxz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tvtdczhd.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gajqnjvs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qywsjbdn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ferseffp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dqluimbr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2fnyjeial.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xmjebrwc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxcqihz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2relyjwzd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ffqzyftx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2kihedkby.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oawatoyy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2bzrklqhz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2csmcumcf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ipwpuhpn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2evkmoron.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2thzuhylg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2zyahizyh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zryqadwg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bxemghsn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yldjqyij.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ppdswjga.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wrxeddtx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2oateenup.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qvcsrnrv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2dgfsrkrs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ofwntenm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gleykfvi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mearvavb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wjdwejhd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zepqlyqf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2exlaogxn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gulqhnud.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ichhvyhu.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2otiwtbrl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lksgxwsk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kvmuyaby.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2raprdxil.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2iykfzped.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xoqpqlbx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pjpmknsh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zeuszsmp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qzxejncm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2wlbskbjm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wbsajhya.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2muxqnuwm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cobyzqjx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ipmrnrra.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2whvsiyom.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rrfvtftp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hwdknzqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpgkpylq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2sqlyjogw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duymzgpt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2byjxyygh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2yhjvibgs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2qvjyoemh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qmhjeoha.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ozqcerbz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2drgqsvcc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2dnmkeusl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mnhjzgmx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ecoocjfc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2flklaujz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2hgitkjdk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcwxhket.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dfogcygl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ikcgimsq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2reoavxfz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhvgza.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gnjvhqie.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2iumtkfsk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ykumtwdt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2isfgrsgf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2irnagyyg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2emxkefwn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2blezurgs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hwylessx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hxbbddqv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mjycnetb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2renicbne.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2etopefjo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wzubaajd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tnmwjpee.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhxqempj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2stkonnbj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lswbpmfc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ctvwwleu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mgnafstr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsivfjfh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gulaueap.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2osnqvycq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gkwszbza.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwrtfpke.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhoobjsq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rivaxhqm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2orgwahbs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wdarpnxc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyocxcnq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wuyhrddn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hwizemol.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdfungix.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnsrxjow.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2msollnrd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ivqpxxvo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hjmqcujh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2inundpkd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyfpbsnq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohyumogw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fqmxsbsm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztrpylyg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kupgenut.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2odrianec.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wbffjidm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rwtyvtbu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nlbodllk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2djmdtqtb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wbchnohg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jwlteidf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2npoiicwr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tfgnxavi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yzeloekc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jkbwdvsd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hudqvgvu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2bzsaimcp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mvunopch.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2mlnfynzx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2usfjscrs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtmajail.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lneuxnhx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2udurhtvw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkaisnty.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gytreebv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rbdfnesq.html


<!-- 参考信息 -->