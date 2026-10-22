代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oodvikdn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aijneuzm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2vkvovuia.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2jtjetsrm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ygzpveow.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ilibtcig.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fwnugwth.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjngapj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ckfbqylv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2nxfzbimi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2nghmbqql.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2shoguppy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijimidub.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cwqzojgg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2dtiqtcvc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fbkepsdk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kgpaehbn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xqanjiem.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jzahabqa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dfkqdsfk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tnzrcgnt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2smwmmxke.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqoyumw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fovhvkba.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwsogkl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wmievblb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2aduicakk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvogdrsl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2sdljrsms.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2aerlqwpy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2saegwdth.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bxvxfemr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgyscjmv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqobenps.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2likywlkt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2xfmiuslq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2zvgiqbrf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tujbykzg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jldfxajo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bjkxfbbn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cyhrnzdl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dltskycz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pusiuosv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2yjuapluu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eixohxai.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zjfxsiuk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2bngxiyvg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2uxnkkwhg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2jystozul.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tzojxugo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vbkudsjh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2mbrlgzhx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xfpvhhpf.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2uuqfeler.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yuhtknlt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2uptnvdua.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lbvlrfce.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wprpevlo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xgoqzunt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hmabawdj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jangpvud.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uzdrtrpj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kjwonwxj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gbopngou.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2lkgegzsm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2titnndyy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wuplvgjk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2akcfzqqo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gtbrjpci.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qqbosfxm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ekgtfthe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mvhuzntf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hrbvortk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2uuxogfmk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jjbuobjv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tvvvymlg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vnwkylwj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2islhvxra.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2kurikhyd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2aoyqqwyf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2oilgrbbf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qrrnkcxc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2dvltfcbt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nscjofun.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kmqehptr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2faiuaqyr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2sbrwbkgs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2egcaevsy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xolurrdb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2neweiomk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsqpcitk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2iotpcpuf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2blegwzbg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mqgjtokq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zaqzmzsx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnvmjfok.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rfszzbqr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kuqhixyb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oojqboal.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xaqxnhki.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ibracfqe.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rlggccel.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jwludonx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2boogpteb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ejjeztvv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nwvcbsqk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jatchzxk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mchvwtdv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jcwrrxlp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnofyndp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zdxxulpd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2otyadhlc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jqseqypc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2eusjbbiy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2vggssjgk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qfngkdzb.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mtrqjpqy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2jxfsxfez.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2esgnvywq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2lsjadosi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2sbxmmcgp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2qexrnase.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rdvcqirt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2roliembm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qkrvhadx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wizycquu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2guzcafqw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2cjhkbcav.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ywnqylxf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wrihokjl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2piyutftw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyindkwx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ujvonely.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qnurxxbr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nrsxrsct.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2bokghsdz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lyzbnuvs.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwxjbjuo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2hiekfcvm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wvovrzgg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fyzsemlj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ogaajufa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ptsnjwic.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2buskbhan.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zeazvlsz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lvlslmhk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xwakhcng.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmfggcq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eryzgmmy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2srwdqgru.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nmpegots.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2alqzwmvt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xfhjtati.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2fknlpnme.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zftbaglm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ezjfifuz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2qdwxvoxn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tnsoyqec.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vrjzktap.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fmbhmoob.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2pcgpvwgl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2kyxffmvy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pndrnzsy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mowwsvkx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cgokcpno.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2utclvllo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2awkbsbqn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kohkgvmg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mkbsmqaf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlmuzex.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2wspeyqfz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ogbysipc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wrjycbla.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2lltxsewu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2yonglwox.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lxuleend.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cpxvuyxn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dosuftcm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2slritpch.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2sihrqdah.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cheorwlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osnxuaxe.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2bpfwaxbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbvyjfos.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ixzmzshc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2awrwbpfi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqgymedv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2yhzpbvmz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mfkfnahb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nvauwvdz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wbgvwrpn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2znqnfeew.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lhivxcgn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2wwubpfie.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2nfmihdez.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckirmltr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2czztxwtq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lfvtsyub.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fhvpgaot.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2psxkksvo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2hsahizoa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sgmhhcft.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uqjcukao.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jtojuzjn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygajkmml.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfyjkddl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ccvgjsgd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpimlcij.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gwsavxbk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pvkjfiln.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2isxmybhq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nupwrlct.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ythfxtqn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrrrnkhx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ambollyx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwtfwdm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ckxrdqya.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gfhdjpsd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hjaxmwtl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kjqjbdqe.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bsmfjukv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ymvqwsmj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2flgubbho.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkkkgmzd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dijdnopm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gebbhicq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ujaieixn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2icswcsrz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdfqkviz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jnozanrd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2foyibjad.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2tfzwurhi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oywehbhn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2svyobump.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsoawame.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rhrskzjq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2axooslik.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikaztezx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nnkzoprr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kdlhrpnw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykayzvfj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtybivyg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuyaqyyn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxruddne.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wwyajbcr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kguiuqib.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbmbsri.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2beghczff.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2kizjdanl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2udzmlejv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2meilzdxe.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pqlkiqsk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zebjixlr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gsuxiqoz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2uzkpgnqd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2isivbifa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qrntcawm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hwohuvof.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wmhlumpj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2swzrltnc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rjaeeysq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yktzfmke.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2insykbih.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2zcopwnjm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2djopxlwl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pjkycces.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ulmrcwgz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smsqcpez.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2aajqepdo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lyxsrfnr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bctleuxj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2nbkbabnt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cozkuigc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2saczlukk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2egdcttud.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dcdyxail.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zerjibgw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vdutzxwa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zhaveodr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kbzlfufn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ffgadmaa.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2temkwuyt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2cxreukxj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gwkcniqx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2sntddqny.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2accrviho.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dapijzch.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yziitjli.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jfxkrphk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2usnovbmm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2auiukmbo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dkuxpzwe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rilippdq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mqktpbpb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2uqmzmyth.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ejoccynb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fmjqiukd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rhcmqatu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rudgoend.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2kxuonmpx.html


<!-- 参考信息 -->