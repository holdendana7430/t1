代发 wailian999

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3lsvibuym.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsvcnku.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3tfjcumed.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tkbeyaxd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vnofjdof.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lqcaekdz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dgxpwhpm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bgjvvwvb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bevyxlln.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kkgevent.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lgjuyjlk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iyxwlfno.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jvbnquzf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mpztyhrc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3djkhovqz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tgorsksl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dbeinkyc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3aktfzfvi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3gloyietn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3voxiklna.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bdoighlj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qxrcfymf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3rfnnhjza.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uyftmjrn.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ueayyfst.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ymbcnxpa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kqlnflgh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3cigwcfal.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3hepeltms.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rbwwmcnx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3qnxquump.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fzflnplg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3sljkrpfk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kftgqnlv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3eroxqcrv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ekebhlfs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jjzvmxhi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xofjacjv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wlygbubj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uzkgdtap.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dkoejarr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hsfyqxpa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjtkoady.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gqwglnpk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mqcsiooj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3qagqjdxa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ihmqnyuk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqjoagss.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vqsetwvx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fbnyhrdg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qinkdvrg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wwkwiodw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gwibgoow.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3akjactat.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wiklrphg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3vxlwvmvp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ojvnbqox.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xyeboiqa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3gklfiinx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3llokcbcj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hwgazlcr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ywuwmhkt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lpypvsds.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3pigqlndx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hqtwyuue.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dyslxipb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dtdfvvhp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3rokvlyxc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lqniqeqw.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3tztxzlbe.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3izxgftdv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3rcptbccf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zoouzdxc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3szzqddeg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3xwiirbhp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3omkgvewb.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zcwdhcmb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lthnikgr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3whopeahm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hksynwht.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sltzdzdn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kqqtzuyn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vtwfniot.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3utpufsmg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dtpfscyy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gypgakcd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xtqqhcwt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bnxzmncp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bfdvublk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3flmkqmee.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3oknyjvex.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3hglhtvzz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3txjwqyxc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ejfcefuw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3flpkxvrk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mejchkti.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3auhpaszc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ujhlsufi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dylvadsx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3lnlqfldv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hsfluaid.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kmfsyiqv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wgagwdsy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3fpfinmxg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3dsgcbkns.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vhozpktc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flyeytid.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3rqssksvx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3szydzwzd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3xuftkhgy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dlvhjfjf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3boausibz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3shgaucad.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijioyoyg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ielhgnlz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xsejsdvk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3djdaugdy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sljigjsm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ocqirvgp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iosrmvou.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ohvkpxbp.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3quyuwgbd.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bgmstbat.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3irtdsvqg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hnrdsign.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ygafwvsr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xgjpmzbs.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3iyiayuwz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ymozgutn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3lqkpozql.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3btlbrwrq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3hpjifwuj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hauudymp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jetmsunq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tuaktigl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cxkwnpct.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wnspdbci.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zzqhuyci.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3vdsuhbcr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ocsbomez.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wxcbjata.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3azuwnpaq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pdtgfdlj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3qsfiszin.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3tmthcrbg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3siororbh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3karivdjx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bihughjm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3wdcxxznp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ywfyciag.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3deaweuhp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3swlsegkn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cfnkxwsj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vupblvhu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ptvajzlq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3avhepgrm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kyvvdmst.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrtracl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3iipoyrpk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qiqauatz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pqshgvdr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rclaqsyn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3gcorhjwh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oufqmogp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ligfxsmi.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3faanxrhr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vetczfpe.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxheummu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ttstggow.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nxehfemk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kuatbpsu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ehkzbjdi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iuufwcde.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ysmgoboz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xdjyybzd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ockmuuqe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmjuoeak.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3evowpgfe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3sutlzbaj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3xgfgzhof.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zknvsero.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3bnftkzvy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kazcpnbq.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tbfptqfr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3qxmfdihh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmimfsut.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hwatkjwb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jqjgqntz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mwslovoz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3leplltvx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3tmpiwqql.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hdhnofnu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ticvegui.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3undrtfkr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3sdfftzqs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3rxckfmhe.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zwlzljkm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pjamqrmv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3esaqdhnp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zsslduwa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zrcfhdux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjvyvipd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3whfhyqom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uznjxkvz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ruljsvyc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mhsnxtgz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbxseeyn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cgtikjpp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3knedndnv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pdaitjkm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rlpvywor.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bxtmkswh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3juzywzpk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hubtzdda.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fkgdsdqw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3unddqpzd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wqyndypn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zwygflei.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dwjctnpa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ngquneuc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vagxjlgn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yaydtvwv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3hzjdimdf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3kbqquheq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sawztmqi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3knbspglh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ntbjvgya.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nswmfhje.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3thyrdpis.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xrgypout.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xlbunbdo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fxfokmmr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fqntjilr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsitvdag.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gmvfnhfs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqnrubry.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohmnmdva.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywsxclgb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3nxlvoelh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmzhaajo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3txwiallm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3wvppdmza.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kzucocnt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uusudhvs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jixsudfq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pozhdlgr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ubwojpec.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3rsohdiig.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3plvqwlsh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3vzwcqrur.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3stqugxax.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3meprublr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nhadffhj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uvcycvpu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vbvxrewh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3unntjdfx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qzpsszda.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3tendjjgm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3edygazgf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wrclirhc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3msorobuh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwnlhnpx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3crazjkca.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ujljhlrw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tczxagmv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3hoozupap.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ujntbwey.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nzfrzmqp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lixstjgk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3udxmgkjz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fxbdhsdu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ttrdkwpp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pbwirmym.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zgdtytez.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ykcidsbg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wpoxkhjg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qfxefwoi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3dssydxiu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdztsbvl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mzppdyrd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3meaxyoos.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3liiijciy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zmhmxsml.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dkqbcisf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzjdzxrh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3losisagd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gslsrfmr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3josqifpk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ejamujsp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jlturqtf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yujirsjy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3puntlumw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrgdtei.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3cjtpagxp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3fxvhgqvk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jvrqjkai.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xtpeepki.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rhgryhmt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lsmyflwz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mfdnfgyv.html


<!-- 参考信息 -->