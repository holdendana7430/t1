代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3znwxekyj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wyeijdqn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3oddiavxl.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zhbtdcmi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yfoftbcl.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pyiyyuro.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wxscbonb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3kijwmbee.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ynafekah.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xufsatbw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3foqyxmnl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zbjktrxr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cnnmnpog.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qhxwniks.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3kokfvvqm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dhittlzi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gltcivtj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ebaqfkte.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3axvdhnpp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wdvvjepf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3plugisnx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3acajdsnw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wckyjrsx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qvmmqdpg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hvaxzuep.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3olbursas.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ofyrkmug.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebwfstoo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3zjowbzeu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3hhdkxwkj.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3idllvmyw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3shbgwtgd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tafonntv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3znvgpqrg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3smikmjrb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3yjiryprz.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3enzarruo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3lkoxyjtd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zptmfxcd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zvphpxmf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zibbncud.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ngpfjxuc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wafltnsg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bgywjmzy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dvcetvos.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bttbvcza.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xaydnyqf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3miqgryvn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xudgawrk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3biehhwwo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bhtylmzh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3acjswxhu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3kxrbbkom.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3entaumpz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pguvznyi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3zbdnkasj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3naatapgx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yamvlcry.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cnvlkzhq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pafaxzpd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jeybtolv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ekeicrql.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lcfncqxc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gtvutclj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3iixlfzyu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cejovybh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ebjflifp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tjoleers.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fozlqhhg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3yinwqewv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3toudqpxu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3smfxzjmn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xvpnxttc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3vnayiwox.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lreqlmwb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rztbedsa.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3urqmzlqh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hpjnnnwp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gikzeoqn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3tvgzoyze.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jiwsgcvx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nsfhkxcr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vusmcmfm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ckacqvse.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3rrlgvmct.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yiurdcku.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3oudsfgue.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3lgtvpqoe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3inpkohgq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gqtsnpgd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nnjihkso.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3idryjpiw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eanbvjvw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qkosgnmz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eklpwrzj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hbzkajrw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vaxdxmzg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ezbclbol.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lwuedadt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3duhvhwdc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3rmcnhkau.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3aobfqdgi.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mrrerkww.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3niukcxhp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sxkhhjav.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3nmjapgvv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3eoueavkd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3eotcxfmr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3nurnlxcf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3imovphwu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dzblaekd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3wczizila.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wehynxhu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qglpqwhv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hiwcakow.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gjeyckay.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dhmyatte.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3lpdttcht.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3pzebnhfx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3puxfqqmg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3aokgnkmp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3gynpttdu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3wnndwbfl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3peauurra.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pwehubfc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3qwwaikit.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3gemplohq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3dolmzvyi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qprjgblq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ldingyex.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmqumrai.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3iviscepp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ectyuqnk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wakjumlt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cqqtmmyo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3sofhkyis.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rkxbpfwm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3monlrlkm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3iiozvakh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3uuhwqrlb.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qguyaanw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3mwcbkjsn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qcvjjhyi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pqvjpsxs.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3aeottkmx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hpyoragk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3boaiiras.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3axyhmcvn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xnkqbewe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tdsswitm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kcjkvzbx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lgkexxxr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dcxbptga.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ubzbngcd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3fprgmtou.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3tbnlzgiu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlwdwxu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ehmqvtba.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uzaiptaf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qmmwznot.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyrkuigi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nqnjmkfh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bynxkjol.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hrouqkwg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3xdydbrbx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yzrbybvc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3scrieuqx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vfsusfcc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kivkymff.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ybofuyzf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3oabvopuz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ttbblwgd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3pwjhktah.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3stnzmtqy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pyurlhgt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3nghfbqjr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qlszcmnk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xvylevxa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ngwidpel.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3fubhhpub.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wtbwoyln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urksfgze.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3vibxbxgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uurmclpr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3bxtmxcgb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rawpdwxl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3asflmzqr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wlcvjkxa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aifzelts.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hngdqhbm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xnsrrxgx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3krjetehz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qbpiffsf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3nziwoett.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uiijpemi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3fukuaerk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3edhbxzbl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iwrtjllm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uqkyxebs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3hkptcazj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3nijsrqbn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3atfklapy.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3clsorojc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ijhkubka.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3efudhske.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlkyrska.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3blctouvz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdfdrsee.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zdpdwpsv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3deuzllhu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rithmcep.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ojrkhdoj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3aksjjlgo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3mynsptfo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3imxtuayu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iznmhhgd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wbdczwai.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3thorqcef.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ckwpsyek.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vgbbfpbv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jvdjvrlc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vofylkmc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xsfntyow.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqyvpkxc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtbisas.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3twobuvvq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xvwdshja.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3owokopzm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3czwtkscx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jnjfhhdi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3aioaoshn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwuqikqz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjdooskh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3aiohicie.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ublgpbuy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3uhpozccx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ucicjnec.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hukcqsqv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3cqydbtdh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uwqchusj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xpdcfsfp.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yewpudah.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dbceebgt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aavqpbnb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ufuerebs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tmqoouuo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pxzghohv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hyjpkfrh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ndvfhokv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qnfxesiz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bnhmavyc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vueqsfrv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fluizzfb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3posqqcak.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zablqgoy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yhlurgaa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ervcdlfq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3drzpgvsk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiatuptu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3boztnsqj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpeqaqvc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yemgumez.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3poubipcn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvystjg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xulnjlns.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qjemtirb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3joiaoksh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtixfavj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tknjsonx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sxyjmejk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3eutitctw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3hxlmvmxm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gokgfobr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3azbccmpk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3phhzrdwn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3baqzkygf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ojrbcjuq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3feupdwvt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kdgrnkpd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bgudkpvj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zgxbjbrk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3exooslso.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sotdfoec.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uoxdchbx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3szwakmrp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nkhuvmmo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ocspktmj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3slzxyowv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pthhqrjr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3sdwqaeir.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3tcxswndn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nxlddddy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xjchcztc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jnqfqulk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxhqjyco.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xhtzxuks.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jefqlepz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ltkbuuao.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zcjvjbzg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3yvjtrroa.html


<!-- 参考信息 -->