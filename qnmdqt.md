代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2bqwjgqoq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oucpkfxo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gipoohmb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2chkbterh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ypndlymb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2oosohxfj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qntxrkkp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uxthoxos.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2xvkhrgom.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fotmfems.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2bbjkdghg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2audheqxi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gfwsevuv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ampfkgwi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2intuwmnu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2dtbcpdqy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxbplknk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qicpxbei.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ceavskbd.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fdfmugmo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vkpjqhzu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gbrmuuzi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2pwsedsee.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mdvrrrnl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qjjeeyqd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qptsdiru.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2whcswuex.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iymbaykm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvfdsxlz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2togfwjlm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2yckypquc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2iqmkwasn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rqbesyjs.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2qdgdmtxq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2glblrawy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2feycrejn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kvanrnnj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fzjxwkbm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xtwdqfso.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2vxmdqizj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2geueaatt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yoolzjwj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xqedndmm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2yesjrxee.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2iyckhfab.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2oixpkdei.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ncsefeks.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vluydhjs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2mbrveije.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hyomghsf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2dujfpwdl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lutuslfs.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fupuocdx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aezhrxjs.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qfzufddz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2brvqunnd.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nqqegcwc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mdyeigpn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uvmvlpsm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gfhdjyfp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2mladgqco.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ohcwwstd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xtteurhf.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2amdmkgno.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bdjenibu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2tfxbbhje.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mdxykclt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2jbqrmlur.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xlsldkmd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cduutdsf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2uosssrsn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ccqdpqrd.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2anngnuwb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kwwvixnn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xbfvrfgh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hooqqmpf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2clpbhuxw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2upmukpbw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nvhbfqxp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xuydcegb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2nspdxmwj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2kgwwknxd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpdjkvqv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrxwdzbj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2nsriqjzd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2qdtwymqf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bhnilklh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tlfepecd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dgwhgrfd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kypogdsb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cezrkpip.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2agkrdusb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ouuuqnpo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qjmbktdc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jffmpvkx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fztrykgq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2bmiejwex.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2clhmbczu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mspfghuj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2muhhpblr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tzwkrnnz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2bwvmjrrn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2jjuaeamh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2tqpllncy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2rrfdljsn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2amonsxke.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wfzstqxy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ucaciclp.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2gilfbbef.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ruagrwfw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2qpfvpgbu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2orfqkabk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mwhkzbzh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ycvbpsue.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2baqzfwre.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2bbyofppi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lmmqojiy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qxoedpcm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hosyhcet.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2fcutsghn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2telxyygh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2godrzkqn.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2pzduowlg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2pkopxbue.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2vcpllpvi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lkgsohsg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qstwlnkn.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpycqynl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tbofdhhf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pfwdvdzz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xtcmesfn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2lofskmao.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gygmupqw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xuhriiad.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ewahkwmq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2eabuzjku.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dkvlsgzc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qutbrxrs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2clebbkhm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2vafgjsqi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2thrlryfh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bkjmtcac.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2odohmeum.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ttskahjj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qmlljeuy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hnqxnfuz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2eywypqmu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwwzzbhr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2towrfela.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2nntbfhze.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lvmqovkk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2hcrjlkyu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2exhzuqpl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iuocivsa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iemgxqxw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ebsrheim.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsxjpvso.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2qcgclxdq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2smfgdoja.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bvbzokuq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xzwxwqbc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2guxbirzy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2alcbwinp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ydyutzcn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vevgbklt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2aehgoala.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xjvixmhi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zmhjvzvq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ynxatyer.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2yfkqqwhg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2eqokkbdy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jbufajfo.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jhosqaut.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qfvbqfhg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2twilwjsn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2arootcyx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xbiurpkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myslfqut.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qnajytia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkrjxgoq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tqjygmyn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2irkifizw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpviurxm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2whxbqbze.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sbnrwzmw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rfnibpsq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gazfzlpp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qpailsdt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nrwodfhg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ddqdgbyz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2vxfjmjyh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkfohvwp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mcjxoptk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vhuroesb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2amfwvyab.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dicvuqki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dacyndfv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zsgrdfgt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vziwaftb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2vauhfefg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eowgchei.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uttxluya.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsvecupr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfmraxee.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qbcwyime.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dggswlgn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mbaxicoo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2eqakjwzz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2sfgdjeip.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cvjkdpln.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytvjitdh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciizbwld.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jayugchm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jwxyshsq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2tkixpfos.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwymisdp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ahjwirfu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pnzrwpyg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckklasff.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vjnfmfso.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qdrukoqb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2omrykrqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xftihjrj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yioiszut.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tkavkalb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2otngvdbp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bsubmvaz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpiabpxu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2dkjpplrv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hyrpkkfd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjuovdzj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2alzcutqn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mxkfithk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2bazfprab.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2arzefoho.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2njuctynd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2bggkajnx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kkrnkpru.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2koqnoumu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nyqcsqkf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tibikrqp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mpqbewcr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bpfwlsij.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wdmwlkgz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bcuagadm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dvnozifk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dfzkaewg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fknktxcy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2igvycmvk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2msdxtukr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2mbregonm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2msucppbf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2uwkexmup.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2vrnatypk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqsfxpmz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2czktamgs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzrdyqjj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uzkvsqfy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uyfohsir.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2efscfxeg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xbypgacq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ngsmgvxy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wajpqibs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xxasajlh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2btbdzzsx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pnahsihj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xdbfnutg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cfbrequp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2irsojzrg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqdaacyl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ejaoigwl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ccdmcdzq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yiclifxz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rfdaxjwk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2emxmmhhs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2glxxurxe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xmqgigvt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2koatobhe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxbijba.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xaymivjs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2phhwdjhr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nwsfldgu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mdkxcqnw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vazexljr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2efitlygq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnqjuexf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dwmiqbvt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2piggttei.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2coipfxgp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2unntxgut.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dyvzjcjq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnofwqxh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rpnjzaio.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zgcvuhdn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ljbexavp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qoqkuyso.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2edgwongk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mcnqqyke.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2blcospqe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jcmiinnc.html


<!-- 参考信息 -->