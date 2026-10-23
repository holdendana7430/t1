代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jjrfhgec.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3rpyawkvw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hkinpadz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wdpjzlse.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahwyzqim.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tyydndcb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3meyiighj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xixfcodd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iyhheycm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3xpporcut.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ztupiveg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hplhmhxx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dhswdpuv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ffwquwmd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jgfxozmv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pzvmsoai.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xoyobxjw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozefeywy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3yidzxeun.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3xflvurak.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jrupymes.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3sldxvbyq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vlmbnogy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rlqvjiiz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3weuaefth.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uwiaxdpm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bdqypscq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3tfqhhjbc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wzqcjmbf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fzqzuqyw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mvpsnkzv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3dshnpaez.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3psadngpc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3btslnsyb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vqitirqz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rualwhbc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bqpvdrna.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3usiuzvsw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3arqrfuvz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hffhcegz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vippfqxg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3emoxpsuw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rjlwirxb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yhoawiws.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rosoomia.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3deiakfjt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qhbsdjvf.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ppcymvlx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jrolcbnn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3hrkoyrvj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3svelbbsc.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rppjbkud.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cltgcemj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pdjgoreb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zrxdtsmc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3sddkdpqc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kkzzzigl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gmifqcpi.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3syudkjom.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3exjamyqs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zlfwwtzs.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xeibfkoj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3rgoyigiy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3idjryyli.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3duxpqldy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hqpkpzyz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rrghrmwp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3miuzeltc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3tdqajxlb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mfdnswwa.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgkaozzq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbskhvjd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wlyfbzka.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gfasgzpm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3yihgkezi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3yfooutlg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eshstbkr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vkcmdbmm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqjvfvzy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3whnggqsk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3preumxdw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3orwpxzom.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ftmusddo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jomtijif.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3hrtwgzto.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3otmxqqpd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cfurfmrc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hpxtkdwp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fbmudcvn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3kxizttii.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jjyzgxfc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3rfaxnjwp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ujjgbnlg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ymprkdru.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dhxsvnxl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xcmoyxco.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3egpjirne.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yzymvggr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xnhupoyr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tkstdfqq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3odrjvajb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3mkfqxsei.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3siuacakx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vfsekrhp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3gcxyjwmo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xcqlnsgm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ieajfxsw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3cmuycwcr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qxsdoaan.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3rlafebbm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3sbcvyjyz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ytofminq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vxauhfnp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dtsynmrr.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nxtahhvf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3knaikugy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kycytprz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uhcchjuw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oulaitop.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3dbswucjd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mkviwbjm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3oycoencn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3qiadwmkm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3mgbtiwet.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cxdnhvim.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vrgshmxp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3wpozjpln.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3barnxztq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3dwihzand.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nlxtqkif.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kyzyrznc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocktxbcp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kirdhdvh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3msmtedse.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nfriskao.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mhgqynjs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xznxejeh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3izswzwle.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zxxhqbga.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3zmjomhpk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3uipbntjc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tortpxjv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ypgniuwd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qwklewut.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hifaherq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ofazmaxy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wpllufyo.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qpmtdrwc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cthwmogv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rulambma.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gdqfsuqa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrrwubgp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3oqquntau.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3itkemzpj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3wayoxexq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mrgywkyu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3gcqlijrc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qxaskgur.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3zdhuwtmz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3hpouifyc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3javnguti.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3oyxhvkwp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yurwyvuh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3jfvblrmu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fxshyakp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifuqzuii.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3jxtzjkva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjyvxyys.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vaymxswh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iituejlz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nexljvhn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wcjpxood.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3khmlsnmm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ppguopbi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3uykxsohn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3gdxxxabh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rruaavyr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ieifngws.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fiqkfvje.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kunwrqgk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tcscauvt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bclbkpzo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yylueqmn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3enlihwxh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3panhrhjv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jmyiplxd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tpfggvlz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cjimaswx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiiyyjep.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmnsqpoc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cihseqkr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3thjagqup.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ebaotkbs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wdfpmtwv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gvzmqnsi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3huqhwpgv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fcykgqvj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3danypgft.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3affxlxvi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvwczkbz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdruamxj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3uxlijqvw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ykzgjcyn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruliczfh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nsuaxbov.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3iebxodmn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3mysdivgx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcjvudtm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lukqwxow.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3joqyrxny.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sqpeaogi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tzircifd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgivykzs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sgfalfxy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vkvmcatr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ocdfocex.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3onyehcfs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3sxqsniza.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xcjtucte.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xvtioajd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kfngugqw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ceglxtvv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hbnfujpr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3isoovxfv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wpwkhqoe.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3adinyftn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfpyghof.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uyriuffh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3oekhusqb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3frtutjfm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zquhptvp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ymvapyjl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xsgzsuas.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wigggspk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dsnfapmp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3myfxvnsk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3krsdlzbg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aoxwooqc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sjikfvlp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jzzkofky.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dxbwnzzl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bzaohmsn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xwsmievn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jpdgtlma.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3shevpvmt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fopwscuq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lkodhphn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3uwpcejmy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jthogrun.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3kdqmppyj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rsnqcxhw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3yepgexso.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3srtwldmm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zzaxeflt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wzmknfnm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bewklzqi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wcekycse.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwhhlcyp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mhehqocm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3mgkpocap.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krzrdjzj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rspsdoyb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rthojfhs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fwsktqrf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3cvrifzgc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ijjcfdjx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qdofcndl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wakhzyde.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jnkswhlr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3weyznvcr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qcuarfvc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3huzpelqx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zhjezlfw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fecbmovz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3undjbncl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fzmjjxns.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gesewlnc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yrufrlbg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bymmanvi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgdaxfqw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3geunyoui.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3kpbqqjxx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3kgvzrmfr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tmcuqfke.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3lauraxjw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fhuihkdz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xrddptqd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ahccxxgu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3agrmcvnb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3akoqutxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ibbuzwfl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kjutrhqy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahoclmtq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pggvskqq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uszgzkge.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3msnmvdot.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3sfqhahoy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mpaslinb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3reyrmvhn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qczmhvbl.html


<!-- 参考信息 -->