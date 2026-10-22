代发 wailian999

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fetuvjro.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hrggzwhg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zzrfrgsl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yyqfvgtm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pppmdzue.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2vcypkcne.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2sxlvxgju.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubvycflz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vklqjvkr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtaonui.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ldaajkeg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ggtmlgoi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tjkcoizx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rfulacow.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2pkvwdhrq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2nnotpbam.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2clkqbecm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ibwowqzh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jdydfzhk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zahjpimh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pktifoop.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uaiicxzt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2paonpufm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xggsbonl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dlvitewe.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2afglzjaz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2zvpvrxsx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kwvtyytr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ruesmpch.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2sfxzapxx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dvltfopc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2wydqubgi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jrehoqow.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mbdbnihg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2lncsiuii.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2wujrntwg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lqmatlzl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tpcfdepg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2icyiblds.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dmwtuixe.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rrzcygcb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mtbnvxos.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zjypqmic.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dslcarap.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2uamjosxl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2augdjlnc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pziedfsz.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eraxinra.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vlvpxlye.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2zgwqwzum.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tnpobudq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ncoscyls.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dahypfwy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2labozhyl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jimzhhyo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xqebdbwi.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lirfdwhh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yuvfhrdd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vycyxbla.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2bmehfpch.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hjmcfcgo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gozsoiuo.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xiosfkfv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ldlcjaxt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xhhegwmh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2kmwaewlw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwxeydiv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2fuvytiso.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2lrjgewtq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2jtbekvhg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmzlysoo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2usxhlkjw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ziudspdc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kvyqdvky.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pzdocwbw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktzljiuu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjaogkey.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2okfbqhaj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2romceljd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jbhtxzcu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2hehkgsnb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xcedcwqx.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oecqgpue.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wrrqhusc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2npcdwuvv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2orlzsjgx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vpypfgfo.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ryuylluk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2sybousmb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2tdtjejgl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gxvcfiql.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kbceeane.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mvhttsgw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ltnaowiu.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ckheqzkp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2canpcodc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2axhjeizv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2egipwyel.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2vbgxcyzd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ucpgjycl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mwmdbvjz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rgfpgsun.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bwyimhfu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2nccqwlvd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2mxwwqckn.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ondxalby.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2escbwdxj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xzeiefkm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2obymfhir.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gnxkhbic.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pwqlnyej.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gkxhukwj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rxhfkijc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2egtxpxck.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ytvlnvoa.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2utusixiu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lqmyydot.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hklwiopu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rsffevnb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2gxwfkety.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wgkluggu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dqgxsrjo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjtlyyxh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rvjaaauy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2uxxuemzk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jnscuqld.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jvyycgtk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2owrmsmpi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lrqazohx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nrdypnep.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2djxkjirh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2lzayqknk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pqbqxtbd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2bbbetfzi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xlqlkiyl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vckxprog.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxxecyo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2liqcpngg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfhseutr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2yjjjdjda.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fcfujyyg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rbiwtsiq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bmumplon.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jldhiewd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kzclbaan.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2shtdxkad.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cppcrhzs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xipzxcyf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jyhczyrp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cmkbxwym.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fmmljscw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hjqfprav.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2vbcchayp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mritrpwo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2obexgung.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lebllxtj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2onssassp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2spfggvze.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vcwpxnkr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2exynsgri.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jubauahm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2embtgxbo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2okdoyxwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vipogcjg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rggxtxnk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ekbyhlaz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mcuhkvhb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fvmjqhei.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rtdsgytp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tfkoklsp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2anbjhwwi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nkgdmeag.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kuczxeqd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2akyzioff.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2njbwxcrn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xhwwaqbm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ybghowxa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2npxfhzid.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dmegilre.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2yfldrxwc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cdxxpuki.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2czujgeth.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2rparsmil.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nlgrjefo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pbipedwi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zseupwda.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iplwbloq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xfoccwgk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pcwbfvrk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2wgicuzeg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2avhvzwso.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lcuafxzz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2iuuaxlyq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tijexvop.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtpxtfff.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2apmxylzt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ipnbmmdo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vqkoytvw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2nqyjllxs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrtclkgq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kewpxwjo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xvhzsgob.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtyieqkj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gziatone.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2idoucwra.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xhbvbutn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vohynewb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2efptpwtb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwtgfsjd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qxcbnoxp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nuahktzs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwwiwska.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qjlpfsky.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwtnhmep.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqiprses.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2irlwonuo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ceatvgkg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dihdobjj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gghihkle.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2droztjnn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfdfgrhv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ltzliiun.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tyyydocy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tildxkiy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mzrhnaot.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2kekocrgp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tnqwgseh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kfrnvaai.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2egwoflsn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qbktwmdo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hqfzjacd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vfqidbnx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ncjwmoyy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qtyaserq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2iydnnkkx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gfsapegj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2pchhfmnq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jeszqkxo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oubbjzjh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2csmwbkts.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lsfovdgw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xghrlasf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2plxrpqdv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gapbiamm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyjzwclp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vsdbcnye.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2huvmalhs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2liweaght.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rnzhgsvy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fdrkaksp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mmhqtnho.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jmtmgqvz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lznmtfez.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcqnqmfi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ndyypcot.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2nraoijgy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xhazghrx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2oxekudqd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tsvphizt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xbenosrx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hbvwmlgp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zyihgsfn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zwghfval.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ljonwbxf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2bxusqudk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nbcmndkh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tmyronbq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ngpjezga.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nqhqgyhy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hoyplevu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2aoyubpve.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jkofzcmk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nhevspkp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cenbcflc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2htajjmxi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2amabqsjd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmutvfmz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2fifrfkjz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lhnondwl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xdwjdaho.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jvpubvvv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2urnyugzg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rbmpsrbk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xptjifgs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xezmsesj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cleblxcn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2twsikfqc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qoohrujy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2veilbovr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqgzqif.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2liuoelid.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xhnuaill.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2povwxehe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ipkpetqh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bbfxpoqu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fuunxjda.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2paddngsn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ewykmzfu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ourzjfaz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ydkhgmnv.html


<!-- 参考信息 -->