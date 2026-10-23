代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bhbpjges.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vlcksoyc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3oajldrtn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdjxdka.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pgrosuuu.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ackaixuy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3khlmatvs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ydmvabqd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lptknsff.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vmtwoqqu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qksjhgty.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3aqscgqeb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3tugxprmp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3tpnsgxvp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3bwcdruvy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cuuhyuxi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ehdumdyo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iysgzxlu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bomqycux.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nfmtofln.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3grwvcnnj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yxiqiori.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3svxtmgwe.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3cffvufsa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rghfsbik.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3skwwxhhr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lkvmntkb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3jlldpywa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hruugpsq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3sqtwwkdf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3huqsauky.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ufzwauvr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uubrdtjc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jbxjciui.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xczltbvf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vroyrfiy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bwzaelmj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pgfbfynf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3okifkjbp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3whgoorhe.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3prycvvvs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3unzjvyvi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tbuphwnt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uhnachmx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mgkdgybz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ropavehm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uuhdrpcs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3swnasuqp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mvagllpr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zdwulumx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xhnxzhog.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gguvflvk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tnvxgotr.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3applisoq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3dwobiijc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3tosybgzh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jcgqkioo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gtuvzapq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ljfhtxhp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nouhmtgq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3kcrbvylw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xcbbssvs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qizxihzd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3inbpczab.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3whxcedsx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wxfjvcmc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzwqlwij.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qibfmmuu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mgtdxbwq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kpbfsrnw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fyxaonga.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lolncidq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kcbljgtz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3foekzhdw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jrxjtuvd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uttdltqv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nejvzwgr.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hnntwpih.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3aquhkqqk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lisuqney.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vncoxrjo.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gswixvhl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xrvaaurf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3oxwwpffh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3hivetdfr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3mowswsiq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jogpjmjd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qhjfjbfw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ogixdkdj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3loxhciyo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xctqwjfw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ktljbkym.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3eyjddvwv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3orioaial.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vuqmcgkp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wfgiunao.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jvbqaona.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3vbndrjtp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tseuaujc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ptaecxmw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3nhrucviv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ubplwxcg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3dusngprb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bmvnorqd.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3sfjnnsqu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rqqtmgvi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fltwhfld.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hagthgns.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bmrcrjcq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vvloipph.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eqhbxvjc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zggjorza.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rwayajjk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttxgrdii.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dprvovyz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ypotjryx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zjzvjowr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3belzuubs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3hvaumuhx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3nkmsbkhc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3grdwrkff.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mfqlclbn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vqozoiig.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvtzhhns.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3itozsrec.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qlmfzvot.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uogoojto.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3saldmwxt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xzgxnqqu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3iiduoxuu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hhcnpcqg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3xluhscxm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jstjvcwy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vcsddzfq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uvczcrcu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3degudoek.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3syytlquy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ynsbdjih.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zbwguudr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fplxempi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3xusjftia.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ydmyynav.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bxvcwvry.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nbpspddh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mickzcxa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xszdozqi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vglnsfgr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mmklpkfx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wemmilye.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3aqtrceaw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3cqnjtoqp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qtuukuus.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3nkbzlvuh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3srumrelj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3pcclwooo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pjmjojdc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gvenrhuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eckmgfkf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3rulokrkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gknypueh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3utyxggik.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ykqrhlft.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xauswadc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qxxapeyo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rvgrlhzc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3azmdktop.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vupyswzr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ddwfxhrn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ukbbaihl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3tshopgav.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rnfbkolt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3leerolzw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ndkyvlpu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3asyfkbvu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wkjyaitu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3quigelmt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wjizimvn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tqxbjlog.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3entotaky.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dxigzqks.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3issuhxza.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cwzbtwcq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3azlzgalo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jziibche.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mhjnzfqr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3lptvojge.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jqptgwec.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jdfdluia.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nvsoyvhy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3oukoxpbs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsphtjwj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ohlvlcez.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xuqqwyva.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3tsyigjme.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3vjawdecd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3nmtlsmum.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gpumutsa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ialxdsoh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jlfubjub.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ggllhbzn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvnxtsip.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3tvusplyr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxlpuvng.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ikysherl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgxgchit.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jtswexfq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ccitmnhu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whhhjzhp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdounmts.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3gqqkxqkc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qjztqeav.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mevbnjhn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qfikndnb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3hllhadsy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bdecaatl.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3togbhzpt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tehbycoc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vuynmhew.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eixoevxn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jisbgoag.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vqnkjbno.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fzuryzhs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bknodhtp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ntnqgoum.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kkzseqhw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qovhbexl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3djgnzprz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qpekybfo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cuprktdc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jokkilwp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hqqjbjna.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nbiyrpau.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qhseslhn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3kixkpflz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3setrtuuz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybwmkiwc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hqazlbyt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vvtomnpi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sxishtbu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjnpfsk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tlxrqpow.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ipgnkzmg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bjoxteix.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndojadit.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xncjvrqb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3anlnpkka.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojoqoiif.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3rcsfopqw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qbwtnujh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3citjnpnv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nwnlhgbj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zicuioto.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rpsbmpft.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ddlzoytl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3whrivsta.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ysjgodfs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3yeorjffq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qaoprhts.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ipnryael.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3stkkczth.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qykmmtpi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cmvyzexz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gqiszapi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3erczlann.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mllgioma.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bgszvath.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nvybxymd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kdhhrvmt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jbbjpgpo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3aphlwcmi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tswyhpqn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zplprfcr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3obhveqmh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wirwadau.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3rkahuuhf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3efcpzbjd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xhotyave.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sukquszx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3grmacteu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xadjxoej.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jmlqvydh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbvxofj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3omfyhsfg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qwhjokvj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3egzkxumg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zimxknie.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tyxshbyl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ddhgscmc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ruunpeth.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3judjnclv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3otcxzxcr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dwhcqgan.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3clmayehb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swqhpmti.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jdnnednd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3wiebefez.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rjgbkjic.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hifpudii.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oximbcfy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3buuvpfxu.html


<!-- 参考信息 -->