代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gwyscqpm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pzgdtibr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3vspolkep.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ljsnltlw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3owdphwpu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iyqnbark.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3aikvapwk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3awiqtslg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lozovlvx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3tobvqmwv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wixwmesq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ucpjvscy.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3jaqsnyip.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fwvfsjxv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3jykmzmqf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cpcfqldi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ewiltgiq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fdayqpns.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3bzeolmsf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qdeucdzw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hbfmmwwd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vzlopzgt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xdwnuvbi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zxwgwdrh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wybtenhh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xcujpfvm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpsjqer.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cgprwfud.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxfqnvpv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jhleervs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3khmqupcf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdxpmenk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3lpvbgrtv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3icvmefyd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ieheotcn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3hlzrdsyp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cnzfmykj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bzerulkg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3iklgrrfa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rongbqbi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3eodkmesw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3qvjtrahu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3skmyuiuf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3srpfwdue.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gixqayql.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ocmrwxsr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3thhitzco.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3priyoxxp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uaotkgut.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aqxnszyj.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3keaixqsu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3mkygvseg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3unldwvfx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jqqxmbur.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xbgniear.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nvzddfmx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xwslwctx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3hioamnky.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bcmjbmga.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3rxagoywq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ndvvoosu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3chnzvnkd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3drjwhwru.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bvtwikkx.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3niggxdfp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3luaqmzkn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gfbnqhai.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vusoispi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xzrtjpns.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zgxcvqsi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gqkxmanw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nvgdupvl.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wahfgaen.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3gvlhxlvs.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lnaoukys.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ohxjolhj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pfauppje.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fstuzhtz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3goqcfquh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zqkxgbiv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3didmvjdj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fhqzejra.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3rwghijxv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ifjrrgcf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dwwthjmc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3buihuzyv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3fgbduyqo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3oscmnykf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3hojgnrdm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vrghxpss.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kqfwijsj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdmbxzhh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3agxapvgw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fareldbq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uivunuwv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ogpdrwim.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3suhncwdj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3obrwkout.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fetnvauw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3spmzvvbi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xaifamfs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3egchzqxe.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3etenubfq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ynexgaev.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3kigyvojk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3aszaknmv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yceqxxcl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fgxhbveg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3llxjdrnt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3icezahdy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3uixuuurc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3vuwluagb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gjwvwnxr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3caoxxvyy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3pkevspdn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rnjuuogb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hgdrceai.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wwhdnpxf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3nksvndzc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rohcfhvt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3sjtlkqhs.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hqjpwdkc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3kiglnpka.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zrzaakxy.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rwdyshqr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3fftzvkmd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3odnndexi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vbtymbfk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3utaxhwqa.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3kxfbrngm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3itpkqtci.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3nfusdahl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3uqrhdqch.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bwnghiwd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wnswyypg.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zphjiwxe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dugyttjp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvjehrl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xliqfatz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3dewqrhok.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kpxlpbes.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3oiqkmjkd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3nlosghyy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3xwqgfyqp.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qucddsxj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3udjqqqxl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obltyiwj.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ylqnnsuq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xyksdvhp.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gesyoyhu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dtmrdkmo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bjnefirx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ffoqtfze.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mwjktrjm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3okwgllxw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvplykuu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3phncyalr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3prpmirgd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gmojduww.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3euezbtxa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3scdbslig.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3islkrmfw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lseepgyn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fdrpihvc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qmlogkff.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3sgxjmfej.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kewjhwlw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tlvwsbgj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ejzprcyv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eccinnrh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kvmiupor.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3erpsyeud.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fsupyfhj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgbrpova.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3odkaisqw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zthqpmxz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3nqhfldfk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3gnmvehai.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3iwkfucud.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3uqnxzxqb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gerectpv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ftlncwht.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bekdurda.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bpaplqci.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yrddzkuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dflgjpee.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vckdmscz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fllpbwvf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qlcvjjls.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3gfidfxud.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhdykczd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3esoscbko.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ttsllaau.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3czaddnou.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pumzfems.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lrigydyz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nhbolwai.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zvnblhit.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3uzgoelex.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccowqcku.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tgvzhcrl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dwzboetz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3klzfmqnh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3buqglpev.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3juivqhim.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ahoxmrmi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3psluoegf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xypgdwfg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzwwbswg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3briaacsz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgemnhap.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kslpcpvk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xdnmsshc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wczrwmtz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kwwbezen.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pdntapaa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3dkypvjqs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhhzwctl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bqbnxyca.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jgzgnvgg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3juhaixeg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjajsnce.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3grwyfdck.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlyysvjx.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gzqpdiuh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3folphzhq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zgsczmdi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uutbspco.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrpdepwf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3xsmahohl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xlvnlltx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3fpgicrgb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3yowwddjn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xrtiuxdn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gupqxdfw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khbvasck.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnpuxygr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ewafloaw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykikjuvo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bivuizpx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3voxnnuto.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3klleuejp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vwyutlmp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3voxxnupn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwnszocx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pzuomnsz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yogpmihi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfvetbrg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nsgekzoj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3dljkeftg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bzsxhqgr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3rzuqgpfw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3imkgnzkt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fiskrcpo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3brjwwubd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pukmcqxg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mevmaihe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3picsdcvf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mwsejzlp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bnxgiccl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ooqgckvr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3oyxunare.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xqnlvtkq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkacmqjf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwnvjxhl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3anjwlall.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3edmmfavz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kldvuwrl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lrhvduer.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jymtpofh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3slufedmd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mutrusrq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vmhqxngc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ffdukixf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ekulllrz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3eokbpamr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lataixtw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fheqwfnk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nmvcuhub.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bqddvfkz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3dluyatmg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fowvpioa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jucuiwmx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzsyvhuv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ymxrzhlg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pnsurgyp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hmshsbov.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3msvkiaio.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ztacdatc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bozetfgw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zgthipgn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kaiyfffq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wmtczpyb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzwlgkyo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qwxhetmd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3pxhdlihp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3kkzbibzv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cgkdqnrz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3fmydibxe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nbnoetsd.html


<!-- 参考信息 -->