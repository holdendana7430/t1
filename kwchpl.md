代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2puvtclmd.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ylrwqpyv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jypshbtm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gddsugoj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vnhaibaf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2szquwvid.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2iilbaega.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kbzaoqaf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lhzowptt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vqqcyobx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2xnaziqbd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wcovqgqd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2plzaptsu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2snvieruo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2smooeezd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kckwitfm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yegkxvqj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yqjpkwgd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hsjwmahz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2obtsqoie.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgknndw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2pkfeoovs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2igukezgj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzzgsgp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zarunaul.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2akhitcul.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2kjtidioz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ntwlwlzi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bsnjboru.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rkiopdmb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ahpowqhy.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zwrelkvm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2rlibichs.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2arnyqhxc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bapvgbug.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rxpywcze.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vbxwbqrj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jpsrekgg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jjxjnyfs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lpwrczgw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2khrrzbbf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2slgfgxcp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cjcdbsbq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ncbpamqg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2erpzlxij.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pftlotje.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nlgbkahl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2bgmldisp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ucfhyhxj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fgejvfwj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2voagskky.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2suwligwq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ggwseucz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nolzidtw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jtlyfdqd.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zyakeeiq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ukbavbws.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fnuzkyey.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rmugvrfu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2clksikfx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fgfnsatz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2rzucmlcp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ncxxcpuv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kwpqsezz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kgeaefem.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2riwiznsl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2emxwzbuj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qqyxdhtl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rrhukavq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2fvjtsimo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tjqihghz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rhrlygmi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qbhkmqjw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aqcwsqhh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jfihpqxa.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ldwlxdfl.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ijcofkwy.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hcpipzdc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hakpzhko.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rdggbvri.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2mctuppud.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rbufqats.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aanrjlax.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twlwzosz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2fmixhhew.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2filcvgsr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlnklpzj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2dtrazxdu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fixmkcfm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jfkuhpot.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2avdstazb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zwzqjxlq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vdvianow.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oljiguhj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zaxjwguw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hnrvrsgw.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dosefszb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hxjdktno.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ytofuapu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wgftcrov.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2oqdrqevk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nrbamfxv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vxflsfod.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2oocifwdj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2dwpnwllz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xyxmtzbq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vufaloma.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qjygqmas.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2yyzrfxrc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qftcyqdp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qfpymlca.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ilkuuots.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2umlcbmrk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fdwtmfow.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2fptxbdfz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2lywypzkm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ljpewgeg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pjbfnbbg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2nfuogziu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hkzsoshb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2vsobkshy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2kthnujct.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ubqzowhy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2knjpbxgi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2xpdoihyl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ksjbdzcu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yscdqiqh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2setvgmhx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gdggmxko.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fspxhhri.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lphefmav.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2rmvmxofw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qqahbgez.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2muokeltx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ckxxippm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2buepjwjm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qhxjgfxz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lthgvtku.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpllquf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2weyjzbyg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lsuvfsmt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kloddjyk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2htuzxxre.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2wnxbsido.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xmrzmikj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yoxauxxs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rmvxciix.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxkuhuk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nxbflxzc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jlzmvcix.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bpnuihxh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2deswwhiw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xchcuvcm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fnqpvslu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wonvfrnk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wbhsqvzu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ydxjjckn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hkofvhql.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rfwoyxzy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ujxuxsuh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2bjtvrogs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2nbclhhcb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxtxfwdg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uqpcyhdu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzrhzhzx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zosckadk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vrimznzs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfscafyt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tzteslzl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2kpgzypyj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2krlpuuyl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2embxeokg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2pebrwevs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2rintoutv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ayhngdyg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2yyjlspbq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ranbrpqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjrkrghx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2oflobwre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmbbdopv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gpkdovog.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kcgehtak.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whloomrm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ghkhoagf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hyxbqtpa.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2esisqymg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vneepdtj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wjqjqzcf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ngtavkrv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2forgggrv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2cckuyxge.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2rgafnmkb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rpnsnjze.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jskvoztd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2urgbnhvp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2odqvttnz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nucoyliv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tyqcgypn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2sdkwfxbs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ndlzvtjt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jhxsslab.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ybqjkaiq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2igpxsqrq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmwgzlxd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2djsotjcs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2lfwjlqev.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aintiask.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bpobmdvq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ncsdoubf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2arwgszpo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rnrbulzc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxwghxpv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2edquotce.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mlxwbmqi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2upssmpxz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2paxaqkxp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cvkttald.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2npwdjtab.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fnaiwjmv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqsauzsk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rslncade.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qslbvoyj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2htjzzlax.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lyutllcs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fydgdyqi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2eyzabyfy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cybliquo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qitwajve.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2oipujqio.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2osxsvdeu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyribvtc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2vjosajyh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xhqcwtaf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fjzeagjq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rgpylqqz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yuduhpmh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xvolwpss.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsfzzgbl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bhosdguo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukwtgtnf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dexyxtsf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fhenweam.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgindxbb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ekqgjiet.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pktvvglb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zjumliwu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sysednrs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yucvbrhd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nohjeykh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dytituwd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2bqxbmrar.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iibgtqam.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2smgzgulw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2znykknik.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xbwycnhj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2intavjnq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qldouogz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lpjzgoqm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hknfxkpn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rudjseqw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uooytnfn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xdwrvzpx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ctmqhsum.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hsurfrer.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cjxwlwrr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ninvddkl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2nompyiar.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzwqdoh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lnvgijfe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kddgneff.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wgpruxqr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mvmznlal.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lrzzzhic.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2aohcjerz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ibnzikoc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2jituhmsk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tqtbldqh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nqknahza.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2cghjblyo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mgmlhnyc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jfsuyxmu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2udotamrf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ctijiadv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nfhismep.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxhgbgag.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dhpdlgwl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lfhnsnlu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2uysiptew.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lzsbxyiw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qcyyavbt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqgfpvgg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czwhfevx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lejhypqp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nhorzelk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcpulhe.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xlojadho.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2horanvzj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sxcsnmgo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2gcupgewe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ywilynva.html


<!-- 参考信息 -->