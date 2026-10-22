代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qvhjkvgn.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmtsgjxr.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tqcxmeiy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ilbrwexy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2imwulipn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cpxhrccb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2sjyjyfid.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2drmserlu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bndcwxid.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2wliwtlcu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vughzitk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ulihcmom.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2fxirerfu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmhnupu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2suydclrz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hklmiwfv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jxjvllvm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ghpffcnm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mlzncmll.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sjqpjtlp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ehkiitcs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rmvcanfy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oyireeyy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uikgxpzz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdikvejr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2smoxzily.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ollniwps.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrugrob.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2knwcwtop.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wlpfhegg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2pvwzxhrq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ztehkmns.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gfxcomwe.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xbzhhyzp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2iwhyyyeg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ybspzrgw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2josptysk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2kyecwbhn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2pptwuwxt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ivqkwnbh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rgnhmhrd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hvsfrffy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xhvjzvde.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2vsyvsicj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iyctnsou.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vkmdwroc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ygpmkbht.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2nrsaptsk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2bijiobpw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2aoxalgqv.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gyabydee.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2bmdgojfg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wejoogvh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2slydmqky.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jzipekdy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2thjctdib.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ckwrlknl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fwcchtum.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bhrmxmnt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hkfundwk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ubtnuzbz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2grhqmhqq.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ncfymucn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mjmdaqds.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ipbfywsc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2iczkfpgj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wyzqkapx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jqzqyvzc.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mzbebpkj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2etibqocz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2djoqyklv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2spvgmcry.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kfnlobhq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yaamccnu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2extygceq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ckehkzhr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cvdcvqyy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vjdlzhjy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2oanedbjv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2bvwkfufb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fqkzrbbq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2imsyxsws.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2gnlvpwlk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2spmlglhi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qccizbgw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tuxrobvj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ahayfyhi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rviocnbg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2qtqphesk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2wdkgyhcu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evcfssfj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bbpbzbeh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tmqecnzh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2scjabicp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eigxuopd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zurlhjam.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aijrbpms.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ivhanuma.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gmeeyocx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qxaubuor.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2xrmcetxu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2drjmxhvg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2viildjwj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aguixaqc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cxxvlelk.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qgmoyuye.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2jzeyofdj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2nisyozbl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2oignwrex.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2jflpsigf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ruxhbvvk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2pgftgecs.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uepeeauq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qwxezzgb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cajivgto.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tqdwkzvg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gojsgkfw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2unoyuzej.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2piyqrmhb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2scrctskn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2nnpnkrmu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2srbvprhl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cvdtohxp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vpapgoas.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2nqblgrei.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xdlokboz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2uxcuidqr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2nylviokv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2nedeupqf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2baycpdqm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rchrxghb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjmqdhq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ztechwex.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2adjdmnjt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dttnwgsu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2wkmsgyft.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ugifqzlr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2abakuzyh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fywkvnic.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ojwukhmo.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wfbumnqf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vkqtxvdj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vyjbdhlk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kahpppyq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tbzhprbr.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2epswmxcn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kekpwnzn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ojgnipxg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fguvzdfk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fehtvjhn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2twbtbpyp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uplzkuyj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ywtcdjcq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2dpdltgpv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ndheatlm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2gcxamwcd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2gxffxjxu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jihnfmmf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dmegjvqa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2fwmmmvws.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2blqddubs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jttuaqdy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fijekink.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qaxktqwl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ldpwrdtq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtxworv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ffxedzna.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rollulnm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rnndqlww.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rbggbbqi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tfitrfoz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yweoloia.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2efhvpqkx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2uxzhjzlf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2vpgwneut.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2leojttmf.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ibnnhtzr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2unlcfswc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2shauxxkq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ysphcdnd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2arxjwgnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndwlpdvf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2nbexvcnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shgtcpxn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qgpyjzkm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bvgtxioq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgajwxnf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pibfrlud.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gwzqgmvy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lfmzidml.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2fntfzxrp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2knunawvv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nvlrdfqe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mhvbatzn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fhbirsry.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fqdwnmqv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2esgiiuyt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rijepqhy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cxedbpuy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjbrlgv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2tejojuou.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2grmrekai.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qwsvuatb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hgahzovx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjsavksq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkivwbeq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxboasxf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jknctcwz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zoaxlozk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dtjyqzlh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qpgdwfng.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2oiqncngx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dthctpml.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykoexcnd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2yypabyeh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mtcmpdva.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2skzxgyfd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zokdcvui.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jbonvlez.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ytojaskz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2urynjljk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bcizffvu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayvdczof.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlysyduf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcgxoznx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubgrldfx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qhrelfms.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2fswieegt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2hsalxorw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rdsfugtp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtqrfyy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsrwitjl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxggbslk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hujmaifz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pdgrqifo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2whxkctwn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lemkigdv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dkhzvykm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wobxjqxq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ovtfgdmn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pusjwcnq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2igdsnasx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqiqkngz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wyjwkbku.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2atnhbgar.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2yikmhsmi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iifsvwso.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pugatyiv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2iqzbrhfk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2spomnasy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2abhocose.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qcehchwu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jcqkkavo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gbrhpwif.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2yfgvwlxd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mddikolv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2taogwyse.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2azscnzqc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2igdifqja.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ghnuttio.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpnhhxrk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lrsvjymf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2asfblnjq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2cksisdws.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2onfnivdo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xnbycpdj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2acviiuxt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nflyjqih.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2maxtyxpe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mvgcjrfk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlirkeps.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lytihtsh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fggrookc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlnrjals.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2lskwgieb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2swsnqdsn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yxwhjsqn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2srucjwjz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2obbldovp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ymysdpqt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qbwmtpsp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2edkgsozo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zuptwduy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zmindifa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pgqnctwm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2msuokyft.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jeoojbnn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qqsxizrt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hrimkqvu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fvqprtan.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rwtfuqzz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ysqrcukg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hnoganzl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nclarrqa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnhqucmq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iruimgtb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zpajylek.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gyirvhsv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bzgtvhgm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2aycxpvso.html


<!-- 参考信息 -->