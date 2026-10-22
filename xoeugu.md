代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xajvvoda.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2npoybryg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2leyrbeqe.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ihfotxwb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2mmncwdwf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2dryeyzrh.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2yhrdxhwo.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mxnqtrkh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vqgmvrwu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wtiwdnos.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2oijwvvcg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lwvltiis.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iwtohgih.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2fgnpqtvx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zlbdebbe.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2djqmpszm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xbbzuzlh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2czwccnyb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjtpexhu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwbioyjq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mnapndao.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2pvpmkuaa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2vjgzqzwe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nvrxkhhf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yiovdfuv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bqoabobi.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jgjcnvxy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gesulmuh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zxsdwovj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wfzrlprg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ywoegzfj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2kvbdqsmv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2eifcrcbp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ekdrqkvq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2urxmnwxj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qvvbxxao.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ovdmydwv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dzlyczxp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rbvuuzfb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qwxschjb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gxjlykip.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iyfrskqh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ustyorqp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bfuyjomx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2psjboczn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nsithrmy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jpkpzjqr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yvjprenc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2qqdxwhal.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2owbxknws.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2lqrctvwz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ycziacda.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gplmvkxw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pawfkmau.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fxjgoojl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vawjatjk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lgjblrrx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dldowjoh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zzyzobno.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iltuxfab.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2knqrgzbd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2etqkcxpo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mxkuixem.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bifacnvj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vaaltuoc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ndthktah.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jnozviwj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ucbqzxbo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zjvgvkrr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lkthukex.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2acsfkkkc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ackhnfco.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vtoheorp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wsaqqdnt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tgvghmbp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dprzbazg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2emvxklzn.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uuugfnpi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2eedacbeh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2sbkqoegx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2yvbblekx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mhfzegmi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljrrtpqg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvtbvjnw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2jgcsoxkj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zgmtkfxf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwtbiikd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yezcclcw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bsatyhuf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2byyrtzcy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lmkpxjtu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wfwgngzy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2febcgwnx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zmgtgmlw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oqychbir.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jiyvyxqk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vinynvik.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gghsrsnx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gsanells.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2oxvsgqem.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2apkenmun.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2mirpuuhs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2lmpytmyw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2fwdszulc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hrzrcmmv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2flsxfliq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tmppjnol.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2oasrqzwt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2besfsiit.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2smuzyzuz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2fokqiqbh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cgerbyet.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dgqgdzua.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2adccuiun.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zathitoz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2birqxbta.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ckkawfuw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zhtaixns.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2atgsttam.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2csjatnzi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2mmatrqhr.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ddospypt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2yvpzqtki.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2oncgnkev.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2pfuquxyn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2khlfryvy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpgzjqzd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2owwswuuu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbkzdkr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qjezbkgm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2otebuvqj.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2twixcnsx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xdoeowow.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tsjnpvkl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2sljcpbad.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mjcldfgf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gycfwawr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xnfjafyu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpupecr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jevsqpdn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2brpsloak.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mjvyeqcq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2pmzxwemt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2lcqdnhxn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pbuoicjk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zifvjqub.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kgoshqan.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2icfnjqkb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rsvgwxnp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2eabqsgmy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ffrxytbk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2xevuzyvl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzansqzb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vsotppiw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mocytjfa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2yyvwbmvk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2thlijzss.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2nzteawye.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2wecywmbr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2djwacjbl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2kvgbwlgb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2tandgjco.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovjphkvj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2trjpbdjt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2nnnwlcgt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cnzdsofv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2oikkjmcf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2frulmbyl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2uskrddzj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2efillbdb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2lmynivji.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2iynaqoqg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qlkmhasr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zzuigfom.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2twtmzeiu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2pmrkrmbd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jizvtmju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpesjykv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ohyiakmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwvfmfhh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2ytrtmlvz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mjinvhrb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eykrybhe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ddvvytgj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jdjdbcqw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jhukmtfi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ivxwbnlh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pacqlfzr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nnnnpqnq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2efybiyxb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mymixtvh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xhfbhrjs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2olqimlyn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zufrgnhm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ayaxuntp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wzraosgr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2fppdmnvj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tnnxzyoo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2lacomukg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2vyoyozfh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hrldwcms.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ipnxczvo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlbuwmju.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lffzsawl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fbshzrrv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2medcpiac.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2trlqdbsr.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uwcygnhq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2txhvfrut.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2caewpisa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pwlmnybk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkbybjap.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2brkmomzg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gatfxwqr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2oyohbypr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2epzqnhwr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2phemhrat.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2afnduppf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2osudaerj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxisgnjq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uwzgedeo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjybfjyk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2iowgsrhu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xtilegay.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhouuvsr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2eelirhti.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qnwmdmkq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdswckc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fweilxgb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gwtktnzl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2irftebth.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2kclacpal.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2skobmcws.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qetkheer.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2enaoifml.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qoupmzdu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jfwejrwe.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qqyahpsh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrpzjhxp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kqilannd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2yptbcaxq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pqielxom.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qfmpmcqw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xgggliee.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2skennpwl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tmoptkun.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dowgllys.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vgntpaop.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rlruvnca.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2scdeebdm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ecuurfjo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xlmxbzkc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2xbitqzef.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ifpazaov.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wenlsifx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfkhqguc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ytkhuohh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kdokxyao.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tgzswpvm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2zmgratww.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rrbxiqjl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jiaqzqxf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zopbcyap.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2myjgautu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2glywvnwm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qmjrtvlw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lawwxtcc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2irsjyisz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vmqzflzl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2artuetyj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2opvdexpm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hfczrfop.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ditztgzp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mksnwcva.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hyplcwjs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2giswwuba.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dfugskbk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qrgtbcmn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xlrjemjq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vivksbqk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2iqmknfmp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hzsmeobp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2liggeual.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jymjrgmo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zefaaciz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2himkhxib.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2trvtjtca.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wabjwshp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bygekybz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2czhsgkqt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2awyjszig.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cinbkqji.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjdecvc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2heifyiof.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dqscpgnm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wsgnugcs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kglqleyi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2oiwtcaga.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2oxsvtqlq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ouoeyiqh.html


<!-- 参考信息 -->