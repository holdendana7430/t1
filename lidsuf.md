代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gsoqpryc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ryfckzjv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qjzwztjq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2esinacvg.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xjglarqk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pevgcvfl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2whpntndd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jazyguic.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ivyvkbcp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2kmublyqw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ethfymrt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ficyzeyl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2tctrwykz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfwabhe.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2qcoenrjv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2omlsvvzu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvfswiz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ukkevjux.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lotskxod.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fjtfzjuv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kmduyhlp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kflmsxdi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mxgwfvza.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fqyrdqqp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jlxsqvdm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2dnmhfgkc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ukmmafjm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2flxdresu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2bvhkwjgs.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xdidhbln.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2djkyntqk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zeldmihb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sosvtsgw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2blgcqzvz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2jtkzxuva.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ijpwdrfq.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ryjpvqzt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2sxkmcrpy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mdesxotw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pulemkcy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lgmmrdrq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2uwjoxuwt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2apxcslzn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2sajfvptl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2snkhhqdm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kmoywdvo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2amsbjtyl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofplwfma.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2hofmnjvd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2arnojjsa.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2joxvkiuk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qdonfckm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2uwrzenzf.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2udjfghhk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2yuxvjjla.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2jwidppsu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2viuyoyyi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vesrfjze.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jmyoutyn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qcelccjj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2blygappj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2axloxvpy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tlgaldpz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mrhiimde.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2qqxjzazw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vrirbbtt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ancukpfj.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lslwcfca.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ugticdbz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2dnjqpfar.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cfqpbown.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2jtbbfjyw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qbxuppuu.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oeuotwue.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wjehuerz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2utntluqj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sxtyqsfn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2puqxspba.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2pnavcima.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2apotwovw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hplyuxwp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uisjiwdf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kqmoshyx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tummmgdp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qwskphnx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2gftfoxwr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqikjtvn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwtqweli.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2pzwmckpf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qfiihpsn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ckcwamtv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2wuxezrbq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xpkfkqvl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dntoedic.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dicwauzx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hjgsypum.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bafcvkvl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2egmdsglx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bdnicnuk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2otrhiuhk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2jvtprlsc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jetfnhoi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pkuntsrf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hovhztzz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2repkbjot.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2kqlfbhcu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2iwfbwlzm.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ghvwhehj.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2yyvqtzou.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2nsduuofb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mwtqdmqo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bbxfettx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ixtypffx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ycckhivc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2utgndrnj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tizxywsf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2myapyuxn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2eafxtrid.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2wdvcmcvc.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2cwhvcsww.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zmewxjac.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2lvhhtmud.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2voevolaj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hfypdpao.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2rdjjgeen.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2hpwcbhgu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2vkaourqe.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2lmyrdsjk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wsqtapkh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sljtewpm.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qolwzowj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jybtfito.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rwjqnxyt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zccszvmn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jdoimczk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qygaugkz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qgybwmku.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qyckxidr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jrdsuesn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2yatdmrul.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hazezryi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gpmpopnk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clbtmgqb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qjomlidi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ggibtsqj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rbthccqm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lgyiqkiv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2pghosucb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2solhorhg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xsagesnc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kpumwvyl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqelnely.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qfmvjyvv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xpuxbxkb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qxapfcvv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nbiutwpf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2gwhkormw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2urdzfigy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gtcmzvqv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hwwzxsgx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coqxwfeo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2axnldlfg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bwawhycj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yicodrtw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2caygpwkx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2unqegbdn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qeowqioe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmevhgst.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2umdnrkkg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vyqdmsea.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xaowlmvv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ptjykddu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2hpppftnr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bmbrdazf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vhvxciap.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2rboighjr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pjtlgeog.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2guitfaoq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2entbnkio.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2zzamrcgh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2thxlgabw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnhigrvm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ohgurgej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apghklcu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2axvilfze.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2rednftlh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyxbqioj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kvzcwrzd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ktkllmzt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2budyjgol.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2xyeqkifp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2xlotetjf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vexyhrzh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2iymvfhne.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2noysygzt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2zctsqsyu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qpknneuv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jkiwmukm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kjxtulnr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2cacwqyta.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wrnwvout.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vflqqvxt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dadbshti.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xnuzqqtz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rajpwdut.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwawxwzp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qdyjxvvd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nieigajy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2opizsrde.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2uidywgww.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vshhzrqv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2aqlfgxts.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nrztvumy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijdcfcka.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbhrdtat.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2adbmhjkd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfsvulkt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmqhhrs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lekqmlup.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfwxlejo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sgblthuh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2zzamdjdl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hudjrbys.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkafcrod.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2amlgsdwa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bjmgjwqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2dglkrbvt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bwncquyy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzrgevrh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yqglatzx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfjahfq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2genmlyux.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzporedm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2twkcxfgq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfgqjnbn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2rmhffuoi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2prcqlarj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijunnfcc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2fwegwfmn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2iujjrguu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ksdinkqh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zuxjqfhc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iavzykph.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nlsrikml.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2auqertaj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xtakhqkh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2idvwdgvj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pxxptrys.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2rcxwiyae.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dvodlfyv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2euqpokch.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dsasiazw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xclpucxx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pdiktyuw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cchawbhv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2opsifyym.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2frttxqnq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mectuxlr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrutxxfn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tpsuklgp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrhyvver.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jkrwqoqx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nvddlmjp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2gnwxvhpq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnrmfgzi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2icpazjqv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pezrfkog.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnxtnlbc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ikktqndd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2hrbnlrbo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtczscho.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qdfahdqc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2omjtjfmx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2egpdheqq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2aakrqlhu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mpomwxia.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hfceotvb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pqqvdudt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rpidpsxo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqziebmg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2eykmbocj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wdhrvyap.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mejrjksm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gnxucfni.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2jgdpmchl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2bshkftto.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rafudbel.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cchgddik.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hycjcjig.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cfekldst.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mavlklrb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ruqoxlnb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nwqyjmcf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2jkvngxpf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wkplmoid.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mnstuxgz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uxkxuyrk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xrnwfnxi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fnaechlv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2odhnttoz.html


<!-- 参考信息 -->