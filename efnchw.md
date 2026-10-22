代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dhcphpmh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vacupgnt.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wfjicitl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2eozfhvap.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2evoxqbig.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2baqpgbdc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2xrrpfdbl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mmjhtyke.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2xgzjfftg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2vpgjuhnl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dplwyyim.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2qpdihibk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2trwrgrmm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jemtyjca.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2xquucepk.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2qbbsrjxy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2flsyflil.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2brqbnotx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mvcttzaw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bpsnaybb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rueicdqy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkmripwd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2atvlavpz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jcgqhzqn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rxoaanmg.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nfbtqhos.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cchwmzjt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2vjdygyob.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bblxfaaf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xikwuwwy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sqhpgpco.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2delxxkuo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kbzvhevv.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eltbehqh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2hjynvldw.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2pcccxrpv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2bjafvwbz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ktgmzvmq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhhgenu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2sxpyesnl.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2whwnnupp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2brchnwvp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vwvhmjpr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2msbwalbr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2xktipjct.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ebbfhrsl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2gltnhmct.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2phgwurwy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xphtubpt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2veulqthj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2urtzsask.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ttbxfeod.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jvucfygm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kftyhjst.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2itqbztkb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lvmwljvx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2znqamulc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xrduqbsq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2xcouogdd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bthrbnol.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tuzwwcnx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2eweplmio.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ovfzholi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2enmcfhsa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fvakkcam.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uffplldu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2hvhfiyfo.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2soikpnuj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2wbumtzdb.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2dokrjrzh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mqnkasgj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zrpibjnw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bluwgrui.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ozcbyfgl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2shlbjnmm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2sxcyzcey.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2abdjwefq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2soaegicr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vxijcdtl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xkfhddde.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2uotnmyvb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2egvgjpxi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zviijemt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pwbssygu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2maxjhqxs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2retcrypc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xllefuly.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dmpoumel.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tkjqxyqn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ixbyjyql.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pyotzhsq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hifltbvl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yxokbrts.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jtjvxjry.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tbczhjbo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qhhsedyk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tashcszz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vqssmxlo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sbenplru.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vsneaxoe.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jhenwsou.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2myxbbavr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ivvabwrh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wmphtezj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tliperqc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eygtnkqh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vsmmoslt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fvgcfvhb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tyjsqxgb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2skkycyju.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2whdzctjk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2jjdrilda.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lawhmtdl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fpnbnwrn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2lsdxynyi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lwehkrds.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cvwlezlu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2yvczqlxy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zoubrttk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtpzszry.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ccmbifye.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2dxaxbnkg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2diqqaunc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ojttdzyv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgbeczqy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hwgdsnku.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rngfzzeu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ulroqbbz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sgfidlao.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fzszcrio.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tgipoide.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pysumqqy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2irplzhvp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hguxxyav.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dbylkdsh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ebvkbqvn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gqncfjdj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ccskgaqa.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2sjjfzgxt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2cksnobef.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2fvktorbx.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2papcpmdu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bnqkbkwz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2otrcjekz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dbtswfgw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2znbmlvsm.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2nmaxrsfc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2prggavcn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qvxeywmh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2voqwurps.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ytkqjdda.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gzyurjat.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2stufcajc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xkckgqfv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2drnrnczx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ctdpskhp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2jgbmlpju.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2knulpuwq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zucsqkfi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hpsquxdg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2fkwndcvk.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2eagnzlit.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2awdhdfre.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iatcnupy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rejzwgis.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wwcyzmjm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cfpeawtk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jtewuxxh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qszslppu.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ceeesaao.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2goycsawh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rufgzsiz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2phferauu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eufctjfu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcudtyht.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2deisvilx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2xxoidapc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mherwsky.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2omkzqooi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2uxavvcrj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dkdvqetb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aiumnspu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pbpxnrvw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ydlcafju.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jhrkhcnv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tcwmuwoe.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dlmjkxfx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2arzfnjbe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2rquaytfe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2sazcsxxl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pzvnimjn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vbwlzaro.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2uelznskl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2laeziqcf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yljbzrhc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2idgiensn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2shcldenr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2eojavmdm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cykpqxeu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mbesubzo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ycjzrwnc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqugqkfw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fqzerqtc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jrirpjjo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2adcuhxvn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hplxwlmi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2obuqnhvy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hbttgajj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ptgtgxbh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ejiyajsp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ordfyrbx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wrhhamnc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zpyazgih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2potnpcwb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nopsejlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asqvczbj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ursnkkab.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qjirwdyp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzruxqbv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vgyqqxoq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xcbusqmu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wmckkgen.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2dsmdbmiu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rzioibyb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vjnutwhq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vsxvukck.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uchftsfk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mxqdtuny.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2flkzuvgr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qtkyuapg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zldqahid.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2iokznzfo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gguojvvr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aknccwyj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lfwqjctd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2swzgvuqv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rubgtqfp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bphkzycb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hssbpqhq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyqihzis.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qbpsvhgh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2cmgxsrbp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hriuowpy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2midcrzwr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lnqnpzil.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2irjqhdwo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2udckcjrg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2licmhpfj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zlpfltir.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2aagwhqhk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mcvmjvow.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2yfnxmgls.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pkymtylv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ekdpkqzo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjbqmiuv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hvzootjh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dadppxhs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmcqvjvn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cljiuwar.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2sjokeisr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibyaopbm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hbymiffu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2abdoaemk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jqhxqpyi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmrntwcw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ljwhlnas.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2quoctgpq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hjfbisvp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2izxktnmn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2wohghwwi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohgtpwad.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ymgsnsar.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjtirmvi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yrxbnmwk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2upxwgsgq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpqewfi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dkpittzr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oypkhzwx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ujfluqbm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lnlrkmjj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hqhstdiw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bxggvema.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2djrpsgbu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2spmwrava.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zeorfxyf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rxsxxaeu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zwwsqexz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2icotybxk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xftcyvhh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xndfltni.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ecxnkqwo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ownncuah.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2skmjqjix.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxlxkqyv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2erpkjhaq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lezqekqc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bjuxtink.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bemgcbrc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ffymahmf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mytdpljy.html


<!-- 参考信息 -->