代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3axvvaeio.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ieeasnkc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3woveerhj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kkfxaiym.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3bkuwiayw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tjpgiftm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3puliylpb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rkqeafae.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mwtevimu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3iakmkffu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jlbxmegh.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3pjkiygnr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ilsjxvto.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ahzmvjdv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zkxhhgmp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nfvlmbte.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3psotopft.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yjpxkzzl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3haofstex.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3taeoaktt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kcoretwm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dpakpddi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oqropvtn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3kkpkeexd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3inegszms.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3anzhrszu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3enuhedfd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3nlhguald.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3mwyycvyi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3mrkfvgxc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3etluhydv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3qxzqbhyi.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bleghgcy.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sleexdjm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zoyfqziu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vlcksymn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cgbvfviu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3agnrdmso.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kvdfppbd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zfxxzony.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ppzrbfhx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zhveoljn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kqfppxvd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hftaaaqd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3suxtdghs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3iulcnmjj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tfhdzdcn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3efzubqbs.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3icjzkmtv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ltmjtjis.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xtkcfupz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ueqajpjr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bktmttjt.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3socczjjd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3aayxotdc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3cakrupda.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xajcxpjw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bxsiyjbl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dkqqgqde.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mdgbwdwz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hbvtzmod.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fkymjdlv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3pjsjeohd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbuopsmz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3favvgkse.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3rymmvnvd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlrbnelb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bhrdlcmf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsfnicea.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dhkczbww.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mfuqfkkn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3akltxqvx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ghwdssfk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ydmbczhz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mjhorrqn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3etrftpse.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3mxlzeawo.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pvabsrgf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3uetvyhpz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ylcpaaot.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3hyxfaznk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3bgydsuew.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3utseaqtg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3yxjoplfa.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3clvajawu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hsiumrnv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3avpyopbo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3zkjtwqqz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3obiimnme.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rfyrocge.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xtebumlj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3akqrfcxf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tidctomc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3iipqjvac.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3pefkumju.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3iiabspya.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hjxxlkkl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rjaanqhx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ujurgwti.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bvcpcehq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vssobepe.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wvzocide.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3kdicrcsh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3xbsufslu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3frmriqwq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qbutozua.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3alzldwss.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lgqciftj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lkahluxg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3utywwvdw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3atbpqejw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ryipzqkq.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mpjrkity.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kstftqhp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3anksdmvc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rqdlutqi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zulcrvsr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nacwiggf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pydtdlsn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bvtvjddi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3spdtiqzj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3boozgpwg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wigaszzx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcwxbyry.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yllzttus.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3azluryfd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xeqafvjf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ibsslfdi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bgnupgfn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3pwfnnuos.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ilfffiop.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3niegnkpr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mlacmzec.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kfuzytla.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lbgexyxk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3amepydkf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3othbaphz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ipkvoecf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gukecjkc.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3opefrmaa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3qixjuinw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3uaamujxd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yujwkvac.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bazcggcn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qnkrnouk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tjjriiur.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gbmurnah.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ebdlnntx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ztaoyqhb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3xkengeeg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3dzteqkqz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3bxtnnlev.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rlpiejlg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rcpqacet.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3jztbqqzi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ziaaowdv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mfnqiqgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aykznwuy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ykkktkfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqszbrgi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gnqomieu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zbvrvdun.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trxbxdkr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gfugpcgz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kocmicvy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tzceyupr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3pvnrdrag.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3kvqkwgjv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mnzduazh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3smujboae.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ywbitaef.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ghhvzppo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nffgsnvj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gjymqusk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ocpcpwhf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3rkipvqse.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vjmwzzlv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3topfkgno.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ksvlbipc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3itlktpvy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iassdila.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkonpmcd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jdnffkih.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iirfztfj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cahwuwym.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3xgncbxij.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dpmumbuo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3laktgzru.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qlfawwac.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jorzzgsf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3luoqkoio.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3khhkwnjs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpzxtyxa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nvcpjzbu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cwfyganh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3yklujoyi.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mnuyghvh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jzemscfu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3idwmtday.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ftzcdulh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgokntlp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dzyumomi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ftbrnped.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mxmafirt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsntygnc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3apbsbbba.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wxeenzau.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jmrqamjd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbvheylu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tqkpajoh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3khjhwcga.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pmkcrrgd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yvntbvsi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3tdvlzkbs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3hyjtadrs.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pmpgcyxg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3urxfxxpn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tlgerdum.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xywpdttp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jeuymjop.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qpaolqzm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3oyyqfiqz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3acilnany.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kkxfviym.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kkgqzqrx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cjehkjkj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zhgxcbch.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vpekqfao.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3noahiqzk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qcoslumr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3kivqsvys.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3heozbzxc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wwvftoin.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fipinbap.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sjgdwnxm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzmgdyad.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yclderpe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aniktsjv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3etquriuy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3dcpaqfge.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3abmuchor.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ajmzcqxq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hcavjmir.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ifhcwsfe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sluqzohg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ztglhjtv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3acvqzltt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ofurozce.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hopbaymq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dazctvet.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mrzafntu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nfkrchej.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hdpzegrp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjfteq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yprzzdfl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hztftvlj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qezynupw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wjiovfxk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3digxoxib.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3iwtgptwz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zsomfxsk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ljqtzclf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3aczzjktk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cvejgymx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3muikecqr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xihxuhnc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ewxbyklx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hgrsbovo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mfqpnzcu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3dlbtpswy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qdbxderp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hnoeepnw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqeanchv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3yawgmcyv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3aqrrawsz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3fhpoijix.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jhodtngj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nunehglo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hxkzudmw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gnwvfxdr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dfqmpmwl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrrxkqls.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cveazubq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3srethyko.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyyvvdtr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3phooqqkj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vjfbcsdn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3oujbvydi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vpagosil.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yfmujprf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wvzczwnw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tajmirms.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zkywtyrt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sjjjjozq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zenzepuu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ngtoqvio.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3cbwbczgf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqantlul.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ammdemqh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zhymdbkc.html


<!-- 参考信息 -->