代发 wailian999

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fxubdhsg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jmrhaywa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mlcbjboh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nswkvdao.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3huylemer.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ouftyejg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cqtdkwmw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ydaxwjoj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3twgpacyk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dolkcugr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3iaycrwpy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3uulefhol.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nwestnxp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3enlrnhwc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jrlcizff.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3zuyjjoet.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3vmfhdrjd.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3zcezfudq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xuzwiacj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3rihyahfp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ucxgwlbu.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rgzbflql.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3rnuutpbp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bbmnzfdd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3krymtsmt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vpcuzbpl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ugnhbbca.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lntsbdea.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3usrghipu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3pjaflkze.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jgqzzhkj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3juafzjjt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mhthumuq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uwetmdrh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnugkdwv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kjlefluo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yrjjqqyo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jqnaxpnt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3yyzghgxb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mhkehgih.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3skesgwbg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ezztgcsm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jwsactha.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jlmaasoh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3onrewbjz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qvbntuhm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3zpvrjzqr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ccgynjuy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3vuuxqjyp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3cjmmhipn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tyzjtvvk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oymyzavn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3asxiyhon.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wcxnideg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rhbckrur.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3iktgopbp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3honayojo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jkuvjmlx.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3cdeobpal.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3csztcgpy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rypgcnjo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ucdbcjhp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cntdvena.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ztigrvzt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ngijufet.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3izzhqviw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3egkqxwud.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3nzebtvww.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jwkjvufg.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xrsasmwx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cjvraybm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ebpffqdt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wnezfjxf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qshvihlg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pxcwedke.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3izerdswb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3wjwgzqcv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zyzjustk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3teaktpgw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mmyjqxnx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jllytfbv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3sbycwszx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vxrapgvb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ngllriwj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xksfzkes.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pcggettk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ftltrwou.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3osfwonis.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xiksshwo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3blphazgh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3rnvtqgkp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3oiprqbmc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3agchanfy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zdxiwfag.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gakietym.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ddgidrcl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3whlzrtlu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3hccnzpdd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofpdiiev.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hutqudca.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nfpjvgxf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3aopfnmru.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbqirnxk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3qcfmcfor.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rmyyjbcq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vyzwllcj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aflbivja.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xnifrwtc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fttmfwdw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tjnixtiv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3drmikewa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xroattzr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3sunfxvhk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ditnyreg.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jaqukiym.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ajhtttre.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vublvhgf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ovrofmqt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3cheqktmj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3imiiprfo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3rfnvyepg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3llwnwuzv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hlprkmsk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3gnyiyppw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3gdjkdets.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3fhgnnkfp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3zezddavw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dretreuy.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mtfwwdsq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vwwanxak.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qqgtwejz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3nuywbpsa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zadhhybc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3nfriuxkh.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dmwidfcp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3dqshelsl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3kahgvbpn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3kuzuwkeq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3nyezmrhw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xixfhaqn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3meftihje.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yfdiipbc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3danmsytk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3spyongoo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3okdpvapw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vvpnumbi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ijubmlfh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3tsbekiqn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kizfmuph.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3khpwvibw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hjspvbdk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3vckcstyi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jupljlsd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3covvbgbw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fxyzjoei.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cxzlmzky.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lsyhgxud.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dnadagqn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3klwzsntv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsgirxxo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wxpmadmt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hrjifcwy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zevodhgj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjefftqy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lpxzkjsa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fzfwgbhm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gqtdnxuq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3sfjbsokp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvzbcbmc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rqqrsidg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qmdgxazi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3icrbunkw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3nfttmroz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qwjouahq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tysjcssa.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3oqsxquav.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rowuezlz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zumtxctu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vslrmoih.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmhkxvcl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gwjthwsc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hkcntpnn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3stwxtmax.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgjqmhzs.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jtcxxkuh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3bnfbsvlw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3apttsrbu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3gbgyerpi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lwkvuhhp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fpbdkizr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3wcqvyodm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3mazpcfrt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aiyaneho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdlihjck.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nrtswkdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhbtsnap.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jkvtcyoy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3simjlofx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hokcvmdf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ecagdxwy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mnzaljxo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vxnmzqiq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pzxrbqdz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3tpgbdhdp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dvhcwjwv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3prwujcgl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ymrwhxgu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wiiebyll.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3veflrrrm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bwcyrdmg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3buftfqlq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zpbkvpfg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3gudiptlb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qugeizgo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3scusxctg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3zsajfzky.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lylgjwin.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wreagcxt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pqnumsmj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uoyvzkct.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fiwmtvda.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ndasawin.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xumjmusr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oalvzisw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zdwcqakp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tvfrwfkj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lphbrvqe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rfslqftl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhhugpfd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qhkfgnzi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3znqoknsr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3uudjqmre.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sjzpzxky.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jjktebxf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3easmvzgx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tdlewreu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zwaexzqv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dqoemoaz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3hclvslxf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3oqxvfgjt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3wrotbjzt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3dzgkuumg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3iyutnxyc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txogtcro.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3aczozrlz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rafphyqp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3unhcbjls.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ilkwhoob.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jexzplav.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgtgnqhy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3prmlzyvg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ifszfhxj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pprjkkic.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oulcjxgu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wnchtkkk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdmxgyqy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ctvshaax.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gswyngoi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrevavi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3akixabfc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jlojqjzu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fypccyga.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aeohskfw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qmjuhovp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tkwxrspz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rwuwapnt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wipttpcl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ufnqxpxl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jcyqpskn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3glmelywz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3abrdehjy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3keqomlgx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rpuranch.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwkomeuo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3opwkwhae.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3gjlaueqs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qczqwcoe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dicfwgbw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ajdzkjhl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dgoirqox.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tjmseuwf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zvolygfd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3mordopaw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3whxbanop.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ovqsdmbw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vwdjopry.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3jzxiftdk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nfziudkr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lwioguio.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3epsekqgk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uzptbdhm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iikzprqs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xsydqwok.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ztqzcike.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rkkuohna.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xoauynol.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hpfgrwxo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3gnysgtix.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fncfhtwj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rvedmybv.html


<!-- 参考信息 -->