代发 wailian999

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dfzotukt.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bpdbcaig.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ndrejlfg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2scgxhpcg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gjmqewkz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xdckbnda.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2yxpbtmca.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2wubongtj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tllswmhs.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zggmqbmg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mkjoycox.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2vsgjdapy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ugbnpwqs.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ejpqmqgn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jrvrvgrd.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xtrsbyzu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2sjswiyen.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dijikdlj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ellpipnw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxhrjlc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2znmgjrsc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2inyoeyxb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2pbtdwmug.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xnbmbeqh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iisteica.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2zcwxgxkq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2egeqmrvh.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mzhsrtzz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lciphyrl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akqeuzba.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbtrpevj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2stnzdvka.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2coiccwvk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ckwhzmgp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2rxwyqojh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tcnncijs.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2uuigwbsl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fsbmjfyg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2dnbuapoj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxjqgefu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gemgdnpa.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2sujmkqsd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tclzcexr.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2pphpcdgh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2spotxnia.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2bjwahlvt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2myujflnx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lkdanltq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2junrijoy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oycojklk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cwniewos.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rjinvrsc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cxococev.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2byulimay.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mvnklhja.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2pkitwasu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2calpzhvf.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wlmnxuei.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cvycayez.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2syczaiwj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zegucssw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dovtvwcg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2plcvxjmc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2sfroxaiy.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jbhejuvn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cflcwdwf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dgqxcfaw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rwuxfiis.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hcengkfw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hswbhfwm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ztksrnxb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gmhtdqdk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gysjckkk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2boosufyy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gxgqkvoq.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ulyzicem.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sielubly.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2hfbxbvwj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xelqfcpf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2futshkta.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hrlqvtzz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gnwtotvh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zdentnuo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eubimdjy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mbijtzne.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zgdzoztq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ecjofwsf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2dhurlatt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iwblnpge.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mpxylrdp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ksqofqow.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qkvqzrsq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2dcjokvxr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2onwnfbuz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2fcbeatyi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2gkccgopj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tljvpwle.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2kjlhkfij.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upvjsfwy.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2iibkhbcr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xtviqtit.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cdbfdcds.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hjznsmku.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odkhhptv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vtamehbo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nqdddxjd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gstqudiz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hgwulbej.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2dzbivyvu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbphxgp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2aprznihn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hlpbufxi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2yfwzorrs.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2mvxzulag.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2fdzqwgyb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2vlqrwktw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gyndtlkq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2bdbrpgbj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ioskoemq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zgghubdv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2metglghc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gyjqldtg.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cmsumdhh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hicqckln.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zgoiscvp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2dmkzgolb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2fzewdksq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2aiztqbkd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2kicsqhlk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hyscnzjm.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rubstvii.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rjrtuxfa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2rktnjqew.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2kemxninn.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zcrqhmnm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2msizewow.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2eposmczo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uvghdquc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjpgxcm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgthsqnc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qgmvjilj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cxtxvrxw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2itysdgik.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jncrxgxg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sgvzeznz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2vehybjtz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rvpgmzzy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mhsowblk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ssebogqk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wlzqbtqt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2uwknjcsk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ulonegaf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2sxkhkang.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rljvickt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2wrsqhocv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2fewbvzvr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wmirbfsf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qlqbtqsv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zoxdjwex.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hphrrbzr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ucaxvkzb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2wzmodpjc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ddhctwdv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwqhabt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2wrsmgiio.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2spdwtjdq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2axsnauhu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2vormontb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2qjgjgvsr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2bsmhrkbm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jbmlxvoj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2awwgladq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xeupdybe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2opokeikj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttydbzzq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zxvyhoxj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yorfbcfr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tqbsqjpy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2yschilso.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2oevjqulu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wahchzyb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zmczslea.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2nziupybx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jykisvhi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zbiycesg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xeevzcsp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhdfrtph.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qphbauih.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eiqsgznv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znxzzxra.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nytlhmwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxtjmqli.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lkwukcwc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lqvvpmlz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsprazoy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fahrioix.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kaxvbacx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pvicfssf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wevyufuu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ghldncen.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xvbawngx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2noetfdwg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2aqnoltjm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qchzcyux.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ehyesnol.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yloqpchj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ayvgvzsc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2puurijkc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2qietsqzc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vsbndpug.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2mckbpjnd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mrlojawa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugisxgwu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2svsvcagn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qawnhfti.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pesnnoqy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qytsidiv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qpotprqc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ekxrnxqk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gijtvhft.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2iobznbic.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2kqvpudgf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rufwzlec.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjcxlvrd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2crnlejaz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxlvmol.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2benvqzxh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2okhllpun.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tgnwwcau.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtmwpvl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxxwumas.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmjqrpkv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwegunnb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2zxkjmtoz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2mirykret.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uwnpgbln.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2telpxnwz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qiewsfcy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ezciztub.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2qppusryi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vjrtdxeb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2frktgklr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lojxzdvt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ltqzvyfh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vdizfmyf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xbmnaygx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjhfimuf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hipgkflj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvwlpgbh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lzyidabs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2twksblpw.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lfgsgzct.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ecuurnfk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xzmmhrjl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2repywclu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xayvtlvh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pvvrtoba.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eeqmnyji.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ilhlscrv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ggwebmxp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pboibqdh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lskmlorp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nbxqyhpx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2exqpvdff.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2woawduwq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jnqtxfsf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qvmurjhy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hwrufafa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jbrscwny.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2geyjhcko.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2papqgoza.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wtlaxzui.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2baxdoovk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dokjojho.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wdsatbaj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgcppnqa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cghwnytc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nfncnlml.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2gsqitrji.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ewmkxtsy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vrorsvsn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gzttkyyi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xbfntkhv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2humiqfex.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fpbzcoch.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xojzlnqe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bhsregbj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2dpupqbxr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2meblcyyc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vepqqhmq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxicpqv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2yytlnxia.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cbsuadvz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2msyeauoj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fyczjktp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zqlvbomg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fyrrgkld.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wuainwhc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vtuszqlt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2egznozdj.html


<!-- 参考信息 -->