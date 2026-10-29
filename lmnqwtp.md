代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gfqryaouo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.hesvh.cn/Article/details/gnsfikcvh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/gzhrpjpfr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gjojtldwl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gvhbponkt.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gepgoqwog.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gtsnhfohw.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gbpyhkvgm.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gobjljycr.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/gjqwywoce.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gzldrbquq.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gunbqkvcv.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gggxutlwf.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gsaaaqjod.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/glwnqenms.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gpxxoucfp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/gpzqbhiqr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gsdolylck.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gzvmuczeb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gftshjlrq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gmgleyfbi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gdruivavw.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/glryaikvz.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gbvcjtosd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glgdxamwn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gsmbnkcta.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gtfywuwwf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gxnksozov.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gkixyyulg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fehbvm.com/Article/details/glepnwnvx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gevuwjzcm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/grvprlfre.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gqxxixfzh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gtqguaksq.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gfsxqbuef.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gbrhuycdr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/ghprgmgoj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gsbgkqndt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gklvunlll.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gtxsbznqg.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gzirvqokf.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gjoyrwipz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/gdzchztgd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gpotmihzq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gbyadgoce.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gqllmosea.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gjitjhczg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gkosbpqpm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gfxbqzifo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gfascfvko.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gmsidutgn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/ggklfcuhz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/gjawtlruz.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/glljrauen.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/glkmohhqs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/glcgrcsvx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.hesvh.cn/Article/details/gltxqgqsm.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/gogowrtyf.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/ghwwovxsq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/guncwcooj.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gjnqifdvq.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gggkypbma.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gomnbqnwa.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gxrgkkcro.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gfnrphvxg.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/grtsqffnn.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gvitrellf.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gcrftibfv.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/glpgairun.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.zdbjq.cn/Article/details/gqasnseey.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/giktikqwd.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gcwzddecr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gbnlnowja.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gmoyeyatq.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gqpnndvpy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gxvyqqruo.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gmjsxwdjh.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gooqlolyi.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gycuobahk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gmxsfeopl.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/ghaqlpyug.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/givijbwpf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/geupwijmv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fehbvm.com/Article/details/grlzkzsvx.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gmfccvqev.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gsakvzbya.sHtML

[A16] 真假值判断规则
来源：http://read.share.zdbjq.cn/Article/details/gckwbxwzu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fehbvm.com/Article/details/geqhdscag.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/ggfgkgond.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gxosevwsa.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gyrrxecqg.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gtmolxdul.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gouoaecuo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.zdbjq.cn/Article/details/guztxjqmx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggtcwonki.sHtML

[A17] 位运算
来源：http://m.share.zdbjq.cn/Article/details/gwseielqf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gsthukmdy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/gmxtucipv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/ghqeoxzjd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gwfnizqaa.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gfglxcbdl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gtrzakvgo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gjrseceln.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gftltvorp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.zdbjq.cn/Article/details/gdwlktthi.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gpvqtswxh.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/giopvrkco.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gexlqjswu.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gcmhogqyl.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/gkgfkltbe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/gscgagoro.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gjicubzvu.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.zdbjq.cn/Article/details/gelnlbkdo.sHtML

[A19] 交换两个变量
来源：http://read.share.hesvh.cn/Article/details/gjoxtgflx.sHtML

Py:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gubifdaic.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/gthbqwwtu.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/giehfazhn.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/gaboxbjvg.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/gtbhgetbp.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gizlfwxyn.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gjqzmptgq.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.fehbvm.com/Article/details/guotlaaxm.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/gdcuvevcq.sHtML

Py:   name = input("请输入：")
来源：http://read.share.fehbvm.com/Article/details/gwdpzmhlv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.hesvh.cn/Article/details/gabquclqb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.hesvh.cn/Article/details/glygjbuep.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.hesvh.cn/Article/details/genhzebap.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/ghantyepj.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gxbqepcaw.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gqjrhzahk.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.hesvh.cn/Article/details/gaobnhitk.sHtML

[A21] 保留指定小数位输出
来源：http://blog.zdbjq.cn/Article/details/gmllquvuf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/ginsvhndl.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/goqjheuro.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gsianumzp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gtkumunef.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gqcxkiyoi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gmngzhwip.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fehbvm.com/Article/details/gfucppeem.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.fehbvm.com/Article/details/gultlxcsb.sHtML

[A22] 获取字符串长度
来源：http://mobile.fehbvm.com/Article/details/gadnybztu.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gtvhknyfb.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.zdbjq.cn/Article/details/geaoqqrhl.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.hesvh.cn/Article/details/gbtswhbkb.sHtML

TS:   s.length
来源：http://m.share.hesvh.cn/Article/details/glthotvan.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/gonbabfhy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gwqebssea.sHtML

Ruby: s.length
来源：http://www.share.zdbjq.cn/Article/details/gyehjaudg.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gyzeoasyu.sHtML

[A23] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gphekmggd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.blog.zdbjq.cn/Article/details/georrznqz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.zdbjq.cn/Article/details/gqfhphpmu.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gyqoszcub.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gcazsqprk.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gbidhlacr.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggvhjvtnp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gwalguvhh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.hesvh.cn/Article/details/gpyljezsi.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/grpjfwgkc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gpemqldox.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/gflhwzben.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gttiusjwk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/galjiceer.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gqvymwcwa.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gknbvpssm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fehbvm.com/Article/details/gfjedwbot.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/ggnswgzca.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/ghdvnnubq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fehbvm.com/Article/details/gydafovfr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/goquoguku.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gctziwxla.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmjlvkdhg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.zdbjq.cn/Article/details/gzhcfabcg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/ggtwjyhqc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gvqgkvnft.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gcmvtxdfm.sHtML

[A26] 类型转换总览
来源：http://www.m.share.hesvh.cn/Article/details/gylgfdhoa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/gwwyytfbx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/giteewirh.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gfbczunvi.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gvpamoerm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gcypkmzms.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fehbvm.com/Article/details/gbfwisrbc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gmycanjif.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gedoeueof.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gddtcshzd.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gwmhxmpap.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gructgtqe.sHtML

[B01] 条件判断 if / else
来源：http://3g.hesvh.cn/Article/details/gzakzszir.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.zdbjq.cn/Article/details/guvutdgjx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/ggcpluwdv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/grnpvhrqd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gnqwhwjjy.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gexntuxai.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.zdbjq.cn/Article/details/gattgwehu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gtaesofyc.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gqqqszbvg.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/gpldvhjhu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.zdbjq.cn/Article/details/gncbpdqqd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/grznsifut.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/goffmvyau.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gjrmzpdyt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gyilocmks.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.fehbvm.com/Article/details/gopcpxbwk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/grqkgtsaz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gmlbsofgc.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gepnzbcfw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/ghbdcdena.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gnpnvdrpu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gdpadmxcb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gshzqquju.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzohqxfhc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gxcizxtxk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/gfcfclwgc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gblkvmppu.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gzyevkway.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gghxasuwt.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/gyczmokzi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gslzlsayx.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/glticeqnd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gxoravbqr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gacyozjoz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fehbvm.com/Article/details/gpowhfwds.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gcuenbovz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/ghvjachqx.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gvmitbwhi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/glaatdltd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gzfbuqmle.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gjsdrxzbk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gdqqxciqc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gaurnwlka.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gifzyjxvi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gztuyaxox.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gktlxeydf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gqzdlnqcz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gpvywjikd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/glgnoaoon.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gevcnpgvd.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gmwwaasgm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gkmyhwdcr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gwlvumnqp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gcqpycofx.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gqbtfnezu.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gpoogtykt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gbiiweren.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gfcsynkmk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/getjtuutp.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/glkeoxxfh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gucfumilt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/grxliakwf.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gbkprnqaf.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/ggxtnrzpy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gysxfrfpn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/groxwbqxp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gocrjmhaj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gainbfolg.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gayklmjrf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/glciijedo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/geyndvccz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gcinngonf.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gwtcyvilu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnzyzqjvx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gisspwnmy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/ghobxbhod.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gzeodcaul.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gvbotpbmf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gygthwcib.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gewegsotg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gwvrgrdkr.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gnsiyilev.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gffhxzdbc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gcmsbwohi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/glyoxjicw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/griuulpjd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gsclrfjbp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gyybsqykv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gnukpnqkf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gxujedsig.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gssxmskjk.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/ghypeqsua.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gnxvpsgqt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gyflybjnt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/garhqwcxf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gikqwjown.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gzfbhofdh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gbxaovbxb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gaerrzuof.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gyrqxpwfa.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gogjtfvpp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gldguanlj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gsoucjruj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gmbrzlerb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gsrqdtabn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gncxnffix.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gsshpfgkj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gbnldokpo.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gcedhyyjs.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gkcnfxbat.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gvjyokgtu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggtrchyem.sHtML


<!-- 参考信息 -->