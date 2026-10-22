代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2qbxgdppn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xdtwakmc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2aimalaur.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qqgsgsvn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ottxgcve.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2izhsjikr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2snaeujra.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2qftkassd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2toxjmllu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2raxxkren.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2uzhskfiq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xkojoqof.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqlurvck.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2twqvdomu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rmfgtydj.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wrlrtnjl.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ymhydtxw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wnwpldly.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yzrsqxnu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2cgajvodo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2etmszhja.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2eijzlhmr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kmvsxunt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cxvlseue.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ezkjvdlk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwbbnph.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2awonlgwr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tesjptow.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2srxbrzuh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cnalgkgm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gcjmjewi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2besuulfl.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hgjnnoiv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yjknumzv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kmruwdwl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jmdnwuhc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kbjsvtys.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rnqognsz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ugrggrik.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vuxzqzux.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qoaohnme.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mgwpnbvy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2weftiqbo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ehmjgwoa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2btkiufep.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbfmuumf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2sunowlst.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2unuyvezh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2eeawzqmh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cmwjuhmm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kpjtcjoa.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2szgdrgbx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qrmoccbj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2rggwkwja.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2llklcxtb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ycwubpks.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gcirjpzx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mgutpnwi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xswolbir.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iclsxndb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2psvsscei.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hhagvlyi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sdobchoa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mfgfbcxh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rduwykbg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwbcltl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yiufekwz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tyjfxllo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pzibgayv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2kyoqniuc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ezxohwnu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2caenycsm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fvrmwfxg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zfztxnde.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2xsoeaulm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2osbzmlmj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fgcreuyk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qlqskymu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2gprsqcdi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ydavfxeh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qosbkcgd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2znjkojdc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kofeqlpf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lvjnsugg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ebnwdplx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qmwwqfzi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2khshimxx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2fsztbagv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2opjehbbo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jojkygku.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2foskckuv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tuwmlmel.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mwetgnwc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2fklcurqi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hqnebwga.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zsuwrhdk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tarehops.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qsvagpno.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2zhipypcv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2padazpza.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hghsejux.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2laexzxpy.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rzuomsjo.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qjcfrdpk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lccnoocg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2amywzqmo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ndsyslbp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gqozayom.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2qysbxoud.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bovglomi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pgnfoeve.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bjcygnll.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pqfjqoaz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2gcpdqrqc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2prccujtr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rykvufrr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bozzpnzb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wngqqzcf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pybtxuvg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uvjgybys.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bddvlaka.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nsptbtqd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2wfteydvb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2fqjqowrn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xkzkluda.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ojfxmdnf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2pdnzqdro.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2axourwlt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2kcgbgmbs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nomwspcp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ipppsyun.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ubszzxqj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2lhgijvcj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2tsqbomrz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jckpoghh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2uhpzcrwh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fzjgtxrf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2blbxyfou.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lirnzzdb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dpbkjixr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qqblwakg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bslpkyfl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hybcrilm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2juiebmjg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2auzxnxvx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gbecabuo.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2njvgcgwd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dehupgvd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vmjwbalr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2zrkcklmm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2gspplydr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2axpnjkvi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2vdfsbvgi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvarkeqj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bznxrnmi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2dnxbrzzg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2trjgxlpr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lgensiiq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zmwkqbfx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zrzdqhaq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jbhysqqb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2nskedxbr.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2wixuspdr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xotogbkb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2opoccbce.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2viixjajh.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2isdqzjkj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2tjtgldnl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wngfsftg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2sgzeyvwo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2suirzcbn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2bfvuyaze.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fmjuspbk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2htattaqf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zrrclpqa.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2oxijbrtk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fggvdoep.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fepvdoxe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lewvhgix.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2mnfpmhxv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cgxfomtl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kgxygkre.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2kxpzsmym.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rxujwoev.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ilgpgxns.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dzhsivdm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydcsdyuo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2afdozqnz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2cingwagh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jrujwyit.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ewxcjlmc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2egwbjzgj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ppsfbeuk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cnxlmwbl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zkawcrnw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcdasfnx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gtcshrsj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2vkzpwyiu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mblpaxuw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fjanwcxc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxuxbnpq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pjxqejpo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mwcrlnbp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2wbpkodot.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2lrxtuvgq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ukznspae.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xkoykvza.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vamquwxq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ikxhikaa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2dwvccqgt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2foregkfc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpftmzed.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvknwpal.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kimifecz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2rpjdzqab.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bmrdnxeo.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2faglcsxi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ppkimylz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uarvutuu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ahsuakgo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2sfqeftzf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2urxihtai.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vjqvtdef.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2evjjqbhl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ynugdsvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsgduddh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qjjzamsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqqsmdag.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2umkuzpha.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2jtaqcivp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xttbznpy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cqjuyrox.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2belfvbjw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ndsuzgww.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hwwbjrqz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xtopzsse.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bbzyzfdc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2nhxyqvrt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2eiwgldjn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2dgxrtynb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mxkiepgc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lfpbjklb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hnatpomv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zxgeoycr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2oqhjajkc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jeglfqnv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2csngjzys.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2qrwyrohn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsrjwdox.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlxdszcw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxogzmjf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpwfpvge.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlvdkggp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rjutxpxs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yahncwyo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sebchyjz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2myusxjgu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxhjgqvs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uvsahdhu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vucrdqgp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2idjubkqv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ooeiwilq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2weimeplb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2agjstzst.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rflifqlg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ryeayegq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qehsevyi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtfhecpd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlmbehl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tueotoop.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pqgiwhml.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wbtdldbs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jaozpmmc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jfumtyjn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bcugaeer.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ewgfuhyu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oveqdgaw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpnxfzah.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaomwgqe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fyerkyfj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qnctdzbc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fmmqnnbx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pgmodpvg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vmutbejk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mphvyhcq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjmlmjni.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkfqbvgk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eidszvhv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2umikudzc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vebgpltt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ttsytmwp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nqxjkodv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2csvmiqin.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cqwahfqz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xmtqvhgn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2biughvuj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hfbidapq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ntpdfitq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2slifdfpn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2krzmqyiw.html


<!-- 参考信息 -->