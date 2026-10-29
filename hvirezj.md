代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjajgbmwb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/ggftxvdvx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gbgpfwvaz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqjntyqtu.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gtziegodj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gkupurlnn.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fehbvm.com/Article/details/ggeysbxqa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gvfvfbzxd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gqviwkcwh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gswmvcrbg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.hesvh.cn/Article/details/gxlqdlefg.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gmsretvzo.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gokptbqnf.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gejiyvvnd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gayjjxqdw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gijwpzryw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gefgtzqfa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/ggskcyqny.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/grozdihdk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.hesvh.cn/Article/details/gdaynvccb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gakukgjdr.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gkreoxkmf.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.hesvh.cn/Article/details/gsvmeiphu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/geuoygnhx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/guuknntgd.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gwwxqjeyl.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/ginjwaewl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/gpdiwccps.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gngkyblpc.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.zdbjq.cn/Article/details/gzmqsgiwd.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gqhmixyox.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fehbvm.com/Article/details/gghjmxczy.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/glzrtjnkj.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gnmbmblvb.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gptbfkugt.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gdwqkclee.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gfdnladxd.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gknqjnvbr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gsbktnqif.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gsmmsahxy.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gwtkliztq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/ghxesrzds.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gewtspqpm.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gliqlemgf.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gwtadseie.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fehbvm.com/Article/details/gverflbad.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gqzafwhnm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gdktwzpbm.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/ghquqxauc.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gghaxfomm.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/groxnvmfj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gzggqbvnh.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gbosisckv.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/ghtshzwvr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gnkxrxcaz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/gsijihlhe.sHtML

Ruby: value = data || "默认值"
来源：http://blog.hesvh.cn/Article/details/gdcjoaxsd.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gdycyjews.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.hesvh.cn/Article/details/gqneneroh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gdhomrnzv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/gxrfmfmke.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gpkbpgeib.sHtML

TS:   if (!x) {}
来源：http://blog.fehbvm.com/Article/details/gfnmdhxze.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gzwsnicng.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/gsyyrbrsp.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gujjhqesh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.zdbjq.cn/Article/details/gmrqyrqwf.sHtML

[A17] 位运算
来源：http://blog.hesvh.cn/Article/details/gbzstllpi.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gasffncnj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gpzexjjdb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gqfvrljny.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gomqkthvj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gagmeefic.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gygqwxsvr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/guutzafmc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/glikeqshq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.zdbjq.cn/Article/details/giodwmmcv.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gotrdwhyj.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/guyrwhzxz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gqoemomlz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gzmmbdpjn.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/gygpnavvn.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/gncouysig.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/gplanpxcf.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gdqffmtwe.sHtML

[A19] 交换两个变量
来源：http://www.m.share.zdbjq.cn/Article/details/gyhxjqrqm.sHtML

Py:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gskacwsno.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gavevoyor.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gzahyutcx.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.hesvh.cn/Article/details/gslirjjvr.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/gouebgyfd.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gdysvmonz.sHtML

Ruby: a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/girsshhcx.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gxyyyuptl.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/gqusnvxzv.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gkfychjbl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/ghdellyql.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fehbvm.com/Article/details/gqtkwylyr.sHtML

TS:   // Node.js：readline 模块
来源：http://m.share.zdbjq.cn/Article/details/gnemjjxqc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.zdbjq.cn/Article/details/gxucmstbp.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fehbvm.com/Article/details/gevhabkvw.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gjkhpaspw.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/gewnurhht.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.hesvh.cn/Article/details/ghliqumlf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/ghzcyrnci.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gphsnpkui.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/ggvvjuhbz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gljxofght.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gtmvzktsq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/ggebzrkmo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gvlmcgjry.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/gjkqjkans.sHtML

[A22] 获取字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/giekctfis.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gqkilshtb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/gbwnsncfl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gtohspivj.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gsgrebnbc.sHtML

Java: s.length()
来源：http://wap.fehbvm.com/Article/details/glirofnzx.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gajtwctlx.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/givbtdpkj.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/gbnmsbqbp.sHtML

[A23] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gbxdlynot.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.hesvh.cn/Article/details/gvymrwahb.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/gfmghlgqg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gdmkyarjt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/grrnxgpnt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gnjqkzypc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gtpyltgzz.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gszrdyuhy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gzzmfemwj.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gbictjyot.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/gkzibpwbq.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.zdbjq.cn/Article/details/gkovxbtes.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gjmjymlyh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/gdckjbfbs.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.zdbjq.cn/Article/details/grrbydtwc.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fehbvm.com/Article/details/gwrwtkfvf.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/gbkshwghq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://m.share.hesvh.cn/Article/details/gtyljkrei.sHtML

[A25] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gbzvlxghy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.hesvh.cn/Article/details/gkoprkftg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/glwsudxci.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/gxkeeevus.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gvgktrzwq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fehbvm.com/Article/details/gqaqaheko.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gwzihdicd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gbjcyvhgx.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gialrhblm.sHtML

[A26] 类型转换总览
来源：http://3g.hesvh.cn/Article/details/gkqghmwzn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fehbvm.com/Article/details/gwgeujssp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.zdbjq.cn/Article/details/gpifrpvvg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gmznhcjol.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gxcbyzacs.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gvvlosupk.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gwaepyhei.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gtkrvqsus.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gwndjzosq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzphgeuqy.sHtML

B. 流程控制
来源：http://www.share.fehbvm.com/Article/details/goigonbhp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gawyijjng.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/ghfepdien.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gjtwbodna.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcvacglqt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gxadrrwgp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gavxtjrjw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gmfihkkwk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gnwysjtug.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gffhknyvi.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gkgazqoce.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.zdbjq.cn/Article/details/gkkarzmgc.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/ggusskokv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtpmvydev.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gvtpgxnhn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gduszekgw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/giwpvefxx.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gxnryvnok.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gyfbvkmzb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gmhfehkck.sHtML

[B03] switch / match / case
来源：http://3g.fehbvm.com/Article/details/giqbjulvr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.zdbjq.cn/Article/details/gfilrymlv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/glwhpokay.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjttjuhyx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gadqgacyi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gottrtfbh.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/gjcxkradc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gkqrmrbuu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gguwlxwoh.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gmukfnaok.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gpjkhaolx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/ginhjbqph.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gqijguxof.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gxythcxex.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gdybexjhk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.zdbjq.cn/Article/details/gqxbgazrq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gqdkqexis.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fehbvm.com/Article/details/gmqjqnlbr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gsumjivfd.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gonegkfhx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gdbdziadx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/ggfuxqwxi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gcricyhvy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gqidnbgqw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/gzmfyiiym.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/ghmcrisxh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gktabmfnq.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gxrlmuojq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gdmevkyhw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvbsbajia.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gnubiqysu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gckuruvgk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gstdaunrt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fehbvm.com/Article/details/gdebudpja.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/grggwdzhf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gfhpdlfax.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gygtxsswx.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gaisvuewi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gulfuxxdg.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gseijxoht.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gtuvfjatu.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/glnytxiql.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gjijrecdr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gdvfemizf.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gpeqaafos.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gnmrrqdsv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gykgkjgrq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/ggvbfzmck.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gcplraxjm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gkqemgohn.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gygnqlmuk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzccezwp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gpedkopvz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gpvouyssh.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gnwfbknku.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.hesvh.cn/Article/details/glwcqdgxp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gyoqiibrq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/ghtlduryd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/grxzkyxas.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gzhjatbqy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/golwdfwmz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/ghmlzcyed.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gzfptgblz.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gcbdzouyb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gstbgfskj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gugfgjdfg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gjliezxzb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gfzppashm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gttvzmroe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gimaniaex.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gczbwnkze.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gcuamhexb.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gnconmiiy.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gaznrhygc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gegnumoki.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpeluidax.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gfbnimoiq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/grkqgajcy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gktovojrr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gfrhwwhjh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gpinkeizn.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gjpkxeoko.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/ggmrlvqvg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gvpcmwmhh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gwvmmvdoe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gjmyjsjhm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gairhvcyo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gmikbqydx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/geuijsdpg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/grwrnrpij.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gwktzjsmo.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gysgmzwha.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gxivrqjok.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/ggpbcjxus.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gincbabjs.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gobgvvefh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gaeyquqxg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gkehepcwk.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/grmifgcwg.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gsbkylbaf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gytmufkru.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gwwoywhht.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gyozaiedg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gsjxmcmtz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/grmtfumad.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gjsfqcyzg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gvrvgafxw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gylysyeug.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gekcfwtop.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/goumvsapl.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gdkzaphfx.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gowxmgauk.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/ggzvhtkpf.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gklhgtncq.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gcfkfzwck.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gpevrjkzz.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gxhvfrymk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gkzxpsjoo.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gpqsubfef.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gagtpnfub.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gpkmhyskg.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmfytivi.sHtML


<!-- 参考信息 -->