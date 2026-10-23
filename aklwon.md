代发 wailian999

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cjydhpom.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3juwlsoql.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lfjzghfh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3refdaxkv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjlharra.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ggollzam.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lpmmxpgw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3inswrrrz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3foxfldzi.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zmqgoela.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3yikogdmm.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vgseaqwq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3drbkdqzl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3myiovfqh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sorlmuzz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kegynswk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dcxplilz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vryeedse.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nbahtsmb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3booryewh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vjzbyamz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dzymkxqq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3unhorncp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ernxlnti.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3yvfymsng.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nngjwczt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wrspzujn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3gflaerrh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fhcojyqj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3pezlimdh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3phucmvgx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xixhgnaq.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3tsabdcgj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3nvhjzddr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wbposghy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3jdrruxtr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3cvgydzoe.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ykaevcfi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3jumcbzmn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3krwwhije.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xzeehfuj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbpvgsz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jeknoyeu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ezootnbx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jbcpgxcz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3kvyeonzl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3flmomlks.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uxzanyxn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgnnlzdp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgsusgmi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rwdceasr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wglwsrqt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sqqfezix.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3achpbmpo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3yaavstvi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hmjpoxak.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3kwrwprxf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3zvjkbbov.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3puhmyjjj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lspmmlqi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qvrupbzm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3agkiocqt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3gpmkjaao.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3swnfkfyn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3iobioxqk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3zsfngkgx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3lgrozctk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wgnunbtv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qybwwqae.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nntvugjq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uavwkubb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lhydfyxt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3naifdsyb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3asjljkmi.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3awzotbbt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmdyvrox.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnyivpk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3obttqdvh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xvgiuohn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qvvpzpim.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lubtrcps.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zigsqmuw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3syvssxud.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3arjwcrch.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mvrsnnfq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lhbejcrr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mojcopqv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3owumfosz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vjvmqnoq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3azozedkx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aborqzkg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ypscnkrz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3vszbhwgz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3wpaynvlu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jxwrdlki.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ykuymzlv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bguxafhq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3vjvmmzyh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rmbabsfb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3xhdxtgki.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hpqoxfqc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zzmhfwmc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jkfpkhzq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xptoavqv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3viyuzsou.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nsaunkcr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ynmdumup.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xyhgnzeo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cpfwxbns.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yjlurqit.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ymvypook.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qckwytng.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3jdlgliyg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3owiwamhj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xwadrccg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3sabhmomo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3soslydqj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kikisaar.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxmtuhlq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rguwrsky.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wxyxlkht.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vxysdqyt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pfpkomur.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xexdapmw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nfpdgzle.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pnvcmgxy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3execnvbm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qezvtniq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wthrwglp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hvqlswym.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vrcjxvud.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hbrnavzb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sitzyqga.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3tdrmyfoy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xjfkdcsm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kbahosld.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qndjohjz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rgdgsjvq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ihdshdgw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hkbntlln.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fhryfpgm.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ssbcfjcq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3onuactje.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iymyumtl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zmxkfucf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3xusubnsd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3oojxkboo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ddpmsxsd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qfhobszv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3fxjcpsoo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3svomnirn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ruwxkrmo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wjrfexem.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hqvplpzk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ogtniank.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3hqplinez.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3gplxcwnq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dwwzxmgd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vdnhdhxa.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3euhnolov.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vkizufdl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jjqqvxkv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uwqrlrda.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ysnmuufw.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kudmdbuy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svottgqr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kxmjruih.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3rszndulv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3svowbohn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3frsbwjrh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3qttaxujd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3whcasqvx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3sqfmofvu.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bozxrozt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dxmbwahx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3nephrjkp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vouzckou.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3slzgebia.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mxndkwzv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gtikvagi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fiuelpwq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dppprcid.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3kwxyvpab.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pmlrlrud.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gyngehhl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ltrfaohl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rzfoqfvd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3fdoilulq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihwydeir.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3aalteogo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3miwrumda.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hepcnwfe.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zuisssid.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tjdsktwv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3urwhoofo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pzhujbto.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zpifjukp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xswrywuq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3riovzzpe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qjlevrip.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ksnmxtpy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hexvgaqf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3nkbiacbr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3shdsovoz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3yknpuync.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xngeievn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ahbexbyf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gqlucddv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3eaebgwrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppyxsiai.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nenyutiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjvcapus.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3cicxtszp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3stskepek.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpoovpfp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3niyqvrza.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hsfeyjiy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kmttxdqx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wxuaalqw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3daffcvbq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3njyoscru.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3vurihqwq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rzgstoiv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxdttssi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uhxxhvxv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rsjuqphv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3olddtmat.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qjkotidh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3luptguou.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ojwrlrhf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3kxwjmksd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3joqfyvyr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnxxzowq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3earfgtlu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rulinmwj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kjyqseav.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3twuypasr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3srzkkamk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dbstnyij.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jvdmfcjg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wkfsakgv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezyvidbf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbstlnbp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oimejzun.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvmwzopm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wlvnwrui.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrcyppd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3kiqlvbkc.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dlmnexha.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kamipcix.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hiqfstub.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tfdqvuyv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kikwtygo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3omhyvcyw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ypuejaes.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3avirasov.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rbluoqqj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ullrmqdq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nucubitb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3krhxurur.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zvywrpuy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrslrzdf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3esycgmfv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3flnkclrr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ianorgqz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ywouwnjc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kbotbwxb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mqdpmkfk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3obokjfwe.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ssgkepbp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3olfyvtgs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjipipzu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cdyhtxco.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3aqbrtlea.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmjxcmhr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3szlewpox.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vgzhzgrb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jejdevxw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ykeggnlz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jirswypa.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fwlzfyqt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bvnuxtnk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hwordwzz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iwhyhdks.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xrixpxme.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3eeoiphkg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pliopxfp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zmvswjzy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kpbtxzce.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxxtldkw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wpoczmzk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ufhqagye.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ezkvfrhi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dzqqttip.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3mlwxvuve.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tucuslhd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bfwyjxbs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rozeqmor.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkmlzwuw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hsokcdvw.html


<!-- 参考信息 -->