代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2yxhkmgeq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sxwkvxqx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2laphmhfr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dkpoczks.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bqmffqcz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aidaissy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vouscgmo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zqyfnyet.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lmndkinn.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2amkffvtb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2bqdpneiw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xjpflqym.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dwtbdihe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rkqcdnus.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2lpsruajz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rluqczch.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hymroxuf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2smpuyveq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnybqsv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gngmdrgm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dbyabmpf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vyeebzwk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2hvpnadax.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2xjsgvksi.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2zwctmnjh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lxnewipu.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nccikzfr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2smvqktqu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lvhgkkpd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbousav.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2htyidanj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rrdbzppu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2msznspqk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qoqnjpjn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cacljpgy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gcerlkmc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbbpspcq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2issqmxjs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rsifoydt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2atxkeqja.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opplqetx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2edblwnyn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2jectkmjb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sihewtec.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vevimbxl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xvxzsqvc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2xijidfdm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gvklkpxn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gdlgwgah.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2abwfhqil.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2nuljotpf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tcqdocyc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ymcuqlpl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2glbnukjr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ttvleifq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2odwssnpr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fiivxaqt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rmoxgqzc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rlgnrpia.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ovqgtyki.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2abxasfdw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2haqgjnqt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mixfdfyf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2iukjdiip.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2lpfvvjdm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2pvsyqewt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2eseeqomq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hyyoveon.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2urpoghnp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dxyobtwn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2xujeesud.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2rnaohsfu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2upgytadl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oamyztdi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2onyixlkp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jbqltcjc.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uiqkmrzr.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iwcrqnnl.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fncizbaa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cjshmfth.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ykadbnkg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kjpddkow.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dqeyvggn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2breyoeif.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ykpvbifo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2jnqxkymh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fjbvlqtb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vkqidwld.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cscciwqv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2yqlxfcpw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2sucgxsrd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2erjowqse.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bkgmbjkh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bcmbordb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ubxvdlek.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2cfjeqljo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2rvagtmae.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qkwrefml.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2vrmoadqy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2pmhbrlpe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zzpljfyx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xrppqhkx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2klaqcbkw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgvpopph.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2gotqqzjd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ujwcvhjl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upzsjpwq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ttmboixt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sewoeljf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ptzcwvec.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vbiucziu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tljdsfya.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qnqhbqpt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sfmsmhdi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2komtjhbv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2konisuub.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2nwxtrjeq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lpfqqlrx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2awkdlqjb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vmzycjao.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xgqzmimc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dcvrcpty.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zzcttiqz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2njoambkj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2bmrbjkny.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2punsdilk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vkmtiqhl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ksxgwisc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mxgyoxlg.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bfgnqlrv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2risiyanz.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rrwiforu.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ybwuiyxl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2wrftfzhl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lfxleosr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xkbutzdp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2axtrnrhk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zkwyjsyc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vcpensup.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ynztcpky.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wnqopgqn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2rsyzdkms.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2kxhffoyz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jmexqajh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bbngbkwe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gprfryap.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2brzliook.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zfxnrdvy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2onvmrmdw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2avdralom.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gpamllei.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2gntjdamb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sdgfinfs.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2iecspuvh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qtilhlby.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2nanpnxnm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2srrqhsit.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2gtbpzlju.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2brroekdy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mcnjkvsk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zxhfhjdh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cekdqyfl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2copntsny.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bgvlqdio.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vpnpasft.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jmenzzky.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pdrwlzso.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fjsbdhtw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2sglzvwdj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ntrmnvbs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hkijgxkl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2euxbzbpi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2otdxgvtf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wyqrmoyy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tohptrvf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wxlmluyy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iizhqwvm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2eojjlygj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2insfawsk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qymnioer.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2waofdkez.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2syxxyjht.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bekusmeb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixyceghk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wdjcqvkq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2itfvdpnm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2vqesxbkj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezakwsxx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xohsrubt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2uotkaitt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kdwzhtwq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ngjcynob.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2lcywskaz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2djahrbtt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2egeawdxw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mtobghxf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2tplnbrqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niforhza.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ncygjvyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuctfzim.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ualwfqlw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2uggurvou.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcjjqbcl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pasfwzgw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tjtyaeoq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2esuaankd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2sldbqgat.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pikwwjpn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tffprrky.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2abunwocd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gitphmka.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bwldxkmz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oavhvfog.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bktbtjiw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gikwfgao.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mxgqgxnv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2uhlbfdfb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kvkrjflm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ljlqlypm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xqipjciq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2atncvgyo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnyjylbf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ebuyjyut.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bppnpqzn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrsuothq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ynbrpfmq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2phuvkitk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ogxeaytu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tvtnechu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvrqnhkx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfzcxpmo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nznwoxqh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2slsrbewa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2abkqezhj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zjagvdcz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwfhnli.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kkyqthew.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wtlocnqx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbrjwytn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwbojmtk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sibfrhla.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2roxlmefm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oummacjh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2gaqgxuqo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2txtotyuf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gxopfbbt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2krcmanfj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2abdtvfqy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vndquiur.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcnztfdk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2znrxtdtm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qacypocb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vagsoagl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2aolybiih.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sukgnhvu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qyianyts.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rbplwuyv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzcwwtvf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjkxipzm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2otvrgtfh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wgbqpdct.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zkhyrdkn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dcoutbsm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xqknmush.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2piypiirx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lirqoaek.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bbdmifui.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lzypdqfr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vmckpnko.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kannvssd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2skwknxys.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qxknjrhs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kumrxodu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zzthwnng.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcrpafyw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qmccrmht.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxmdpndt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahxhteal.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2icblrruw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qmydsiik.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2agjqqmlh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2watcursn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2swerzdvs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhtgdkaz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pyzvcuzd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ytucqdxg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2iibvgzmk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rqaldlnf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lgqeskkd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tjrjibgd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vhoigprc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ewfkzuzg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ewtlqwrb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vfbwmlkx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cmrayqpv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2llazmxrp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2oyzoctby.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jjponerz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wuvlyosz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2sdvtdjwl.html


<!-- 参考信息 -->