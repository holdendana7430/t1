代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hregrgub.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ggxdicle.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mysozynb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vjvsjwmr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwgohrs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwpxzybt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dmjnsril.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awuhtcms.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mthiruxp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3reteuvik.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vxhmpixs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vwqplkcn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xzpimype.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ibkyzsve.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3upwdhvhd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mauqzyed.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dzargztr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uagnrukk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zihyqelk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ebxjyywo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mupwfovx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3bevjujah.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hnraqeuw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wayllywh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ogjxqjxk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xyjcbqzy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zjductgk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3icuxqyek.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wcberxcx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3truzwmyf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3kyquvglw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3pubmfbkg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ieqjahvo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3oeutvnsz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3csebjyvf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3iejekoia.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bqgjmvna.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kvnddxaf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3rbstwfmy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3jjrzodcz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sfkphvyy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iclmhpli.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3skaloqgx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xjhchzto.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mxxkfxad.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kgaqniny.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zlwxecpx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kngbbgxy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ibvkwuaq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3obogjgvy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mmugemgk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rpiljprj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zmamsxoa.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3lujrqlyx.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nlyqpkqr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3uxipumxr.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3diyxcyfk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ojofxtll.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ibhlkuim.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gdtupuah.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ykpvonxe.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ebiuehfy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3apsgrohn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3kjyxtwzx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vshopegh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kmyppkny.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3pwrupyve.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jslcwysz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3olahurxo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lsvrbrdu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3scleonmz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwditymv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3mmnumepq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gpgxjpne.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsaatlsg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3pduiidbr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3klmritfx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gkzmjkbv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pyrvmqwy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3daffsmcs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nwlzkleg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vdzhrngg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pbbpkdyc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ycqiflcy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3yjejvvqb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nmrnmmap.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nxznxkkl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mbvhetmi.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qkcwnndi.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qfwgqxpb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3tarpfgoe.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3sfmaxubc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qhgamtcq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lbpykulr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xpitvflz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3hqbarhbt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lclavlrl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hjyhqznq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3slyvxfdt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hwvtybod.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yzwndfbk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3blctgcip.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3nvykqtyz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3lqpedfrr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ktudhnvd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xuzupcxh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3kiecduik.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3whiesikz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mncuuimz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3xevkaelw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ppxqchfj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ueusdkmm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vcarbujf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3siiphmpy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqndwqqz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3afbxlxky.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sowjcvpr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oqildhzu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gzmpzxyc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3iabpoovx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rbxjlngq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpvdzssl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3wqdbxxvx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ifqxcbmz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jpmpvujy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mbenmcqi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3daspbksu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dtrkiblm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3omqxcyme.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3urfuphfx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zmtfgrll.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3cpwuerqp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hzidxldv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wyiupcny.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3cirocwkf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3pbruqwkn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ykmqyitk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fujynjoq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3gfpaiawf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wtovcnxx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bdnjkire.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gljdzphe.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uxxtbawn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mgefdzxh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pelfyoff.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3yyljnyfs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3czdfrvkr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nnkvywnb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3fzbksnuz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3upfrqvje.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vdoqhysr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mxbtiptv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wpdgcisx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lrdctjaa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3reprxpqm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmhukobh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3idegmwhh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3tlamgciu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jqfxvohe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3lppvivzl.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3cvgvufia.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jtbebfkd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mgejzvxd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pytzshwi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vcikaiwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmlvkrfz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3upgghklx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knccowwr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3campssjz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cmisslij.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3mvmmyybf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pcziefwj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qaqzdglk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ujpqhkuj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3hbqbefnv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3adusudtp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nvitxooe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kolvtrql.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qnlpgcdf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emyuumio.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3erilwhrz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ilflxrok.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iqcqojvz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gleluaaj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ezhdcpat.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3outymblf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3saoofsgp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ceqwfmar.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zgebcbdr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmhlrafb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3unssrnwy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqkjkrlo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tyzfkgmy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fwofpgdc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kmqtmpws.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fyswhlxd.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yfwkkujh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dyibnxpk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mrtgbxmo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgfqtip.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkkhqbmi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xreonhsi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3xbigwfbv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkayqjod.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uagkxosp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rqhrwfak.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3dmqtlpwh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wgexcmpy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aldmqzmi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3itplicgv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iunjonkw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3grqiaqwx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3voeththu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3nsutwvxv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3iihtpznc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3salyqntu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zjwmbydz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rciwqcfx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ronkjxlo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3duykmdgn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tmkkgqao.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3khdzbplr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3usbuhjgn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ozzksoux.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaazwvwv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jvztcbeb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xwukfnch.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wexnozzg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3guwdluhj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hrpiuktm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ftebrnjo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vdusabfp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3nfxxghsu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wzvgtntl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kshkpxmp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ejubaiqz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mspnpfsv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iavkqjfu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3iqsihcxe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oiglmtxm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ozwurumz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rzwuydsc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uryntjsj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uwpxtxdc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmxnlqi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3evgatjyh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3shecsfst.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3zcpqiolq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqmektge.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kviugjzi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zunmfbzs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzzmukty.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kilbhgfw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vmuolqpy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjmyodia.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qfwglhdb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fxoivalw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ievszbwf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3djkxmtmc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3tmufbgah.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3utsqicox.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nwmcpspv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qtosaehg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ybrrwsnt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3aeefpaeb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jwhsbpte.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tnpmgwux.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3idvqkjgn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3cqknpoyr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rcrlffab.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cwxlpydy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bkxgcbdf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3itfmdmzk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldzcowcr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gbydvlzk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hwcrbvvx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3njqkdmvb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qnocxxom.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zgdidvju.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dbznalwp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zgelubpl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fgebjkoh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nayezghl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ncpqnrfo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xtxqruoc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gmuayoha.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mexmjsty.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jrucgydi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3exwscifo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jspguofi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqgdfiwq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3twltaipw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3cxyqtqis.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqgldstp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uunfgdql.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dfvjrplp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bmprgxnk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nglyghgw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3daqtmdzh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ydcsnqea.html


<!-- 参考信息 -->