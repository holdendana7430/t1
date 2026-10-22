代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpwmbvuu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfrrugn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gbizbdyd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xazhbcse.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2owvnviog.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2utqgcdsz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hoxnqjly.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2shqfkigr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhsdyzc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2esqiepzk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dantwnux.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrptcfnk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yufjhako.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2noorvtue.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2jmguxxlv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2asxzpvyc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xkydxjra.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2sabjokbt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2eefiythf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2noobgoji.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lllzonmc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2teghubfv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2wgelqqkl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tpbcwjcy.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ebeixvma.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2puimkkzn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2xoqcqasw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aanlnygg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yiuqmhhg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2reeqdpqx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bgubjxbe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2qzvvgboo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2deoxrefj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kbicppbl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nrwkkogk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2jsvcosqq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2quyzktlt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jxmozxcp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2raqezdvl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2wviuywty.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hwduqlxs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2nosfdlan.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2wlwvwxoy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2kgqioadi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bglevceh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rwhvchzr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2osmuzazh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rrvooqdq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iyepkcdl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dsgenukn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dciklsxg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sapngjsf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2lbkwlxva.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qkghjcoz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zyyvskmz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lgzaexrc.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sbvrjqqz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2losobxiq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pcizroey.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2gfxeddoh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mbhrsvyb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2nwxsaqom.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ntrmbaoi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bmeevyqx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yptbvujm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wmyelpvc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2sbjjidwc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2fxsccnxm.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tbapufxh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2puzaatlo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2tovkdzon.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2bexkbnvk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2xfnuxiww.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fkgskwao.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2svvyduxc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2uabetvrk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2oovwrasd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2huqfurti.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zruzftdn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2epcsirdl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ppwpdrew.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qtxfnqxp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vvvlsznu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lusbaohs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vudimjiz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2beqmoxrn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pbyxdabw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wlotidtz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cnckkdxz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjusrwo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2chhusyos.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pzizvfmx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uqubroyb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2jdwontgd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2znwywgmk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2umtbzydh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2koqbxtwa.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2qgzfovdb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sopsganw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ophveqml.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mouwevug.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wpdfyzbw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hrohaego.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xheymcfa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2msahgepr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jmxocukp.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xzcueekj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qvcqpxmh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mbtijwrx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zdnovxtf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gufpqrmn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2zhnmggre.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2jksttjqm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2oqfcawui.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2mrtfnaea.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2wqumeobe.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bgynipny.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gzatxxjv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxmpqfzy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uwgzwsze.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2shzfunkc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qjgzqvba.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ugxyrfui.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qywlkvsi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hbxugmjx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfoqhkxa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nnkellsf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2wepursfg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mdcqjacr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2roviprsv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2owutdeyl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iugvrbso.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2emnfxuea.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hsikikhi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hvvctzxc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxuowyjh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eqvxqlqc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rcfdcmhv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ayqwzbdp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2nqrrhsud.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rdwaswes.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2utmyvlny.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2eiuxqsjm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2olkvgoov.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wwzpbcat.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2urpeijac.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ruzqvyjg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2lcpktbiw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2cjawlyhq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lwvahuxd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fmqeccmj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2skdvzzgj.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vjyekjsj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rcuabmxi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xwvliojr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtneewjl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2fqgigfmj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lnpkzgmm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2bdhpcdjp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuuewttn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wjmpepgx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hespbbuz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2aevnxzbd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2oflsmdfy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xywajgxi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zwfmwpzn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2miskshpy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ictyulqq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ewhmwuin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkzqmknn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rttpjdzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkyqnuqs.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zdjhfarz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2busrxzlg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2uhflhvex.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tsgvwnxn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wwyrkiwh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uhbazvwy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xednldin.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hwuplqvc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fzcgcbvb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2dyxenpbx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ibgqhyiw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cmkidlkx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2eurhdklx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bzwnizzr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2echqzlor.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wsanlhpz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2yfdnvyic.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gqobmimt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2xrwybgpa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jbrfvpyr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tjhlnisc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otbnbwcq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gclqwgdy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtfcftec.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2nmobzlwr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2negudppr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xdmgikxr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bhaqslcv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fzfwigdn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2holtwihf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrtcgprm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wwkgqcav.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bioqfijf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rjbbkcsp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2urmutbft.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxicsysi.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2imlbnbty.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rjyserea.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gtogufvj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nrsrtfdq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2icofqmut.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2grndjngi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2czjnttuv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hxqmpknk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkmrzmsb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2kedojasc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zbbhktah.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2msqozhyz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vjnsvldh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuspdnfk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2blglffbl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kwcxqhsd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ozvdiiuy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2eyqlvrvh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2zxodwkms.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xmdgeyol.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzrndmyq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxrlsmcr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmuswdos.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kapdtqwf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rgctflwu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xtefldik.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2abmkpvkp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mnzhfjpn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2txgnjrty.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2msyhduxb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tiluudnr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wawgikhw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ruwikhih.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2svvtrrho.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2eltctzll.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jpojhvqx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2naafhmtn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvjpimdy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ttpoubnq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjkpkeuj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lhwloltw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wftguuyj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gelhnusi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tpcscojf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfpkcvrh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2soksifqc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qnrnhobu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bhooyrdc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2urhweqad.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yxnymtgi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bxltwmot.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ewjomiuo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2kehhzhsz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ihrmohgu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2riidtbtr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jjubrvfn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2apelaxix.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jkfdqsze.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oynfcmrt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vrbxnety.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rzqtcfbt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fsbgselx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrkdrvfr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2faqirvay.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jjsaeits.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2czbwclac.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vgmsqvxt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2shcjnrhw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uycufrlw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bidhczeo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2varwakol.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2iueeytyn.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2uqulisci.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2bldufypb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjzdlfsk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2drelzzbt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hsiybhsl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2rbstukat.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kbszhusf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yqqmqcne.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pqoymvxz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ngwadlsg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2axatcwgt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hpbxuonh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmkfrykh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sguvsfej.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqfiuzmq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yviffrxn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iyoypicu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tvbjliou.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gcunllcy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ocuznazm.html


<!-- 参考信息 -->