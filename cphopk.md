代发 wailian999

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzmvwich.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fcvmjmaz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vydeiicm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kalkbfvk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xqhvhthl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2pwaggaty.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cacegrig.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2eznjdppg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2unjzgmnp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kyzcckxb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwjtmzo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wovyjaxc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yuqggtaw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mwmcnycd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2lvecwuvg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wsrbjsun.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2azyysdgi.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rcfiqkoc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2vksteeoe.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vwvtmtvz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbppfdpn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvvrlinp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2lknyhbdt.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2tegadpss.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmgnczr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2mddcnwkx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hvdlqpgv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oyibfrsg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cxmdacdp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ymgcldjd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2eeqxjuuk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2pseqziqq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2egnbcbrp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pigxvtxa.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bbaosmmo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2rpjujlhs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2xfynesgh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2eajblriz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xeufgzvw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2lrvjrvdz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2azxpyoaq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2gwoazgmr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2zaqavqje.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xnxztasi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2reicnzrq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wihzvbtx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hellxoej.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nwpetpqe.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gzawvihd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mhuqaxym.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2najspbgf.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mflbgdbf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2pxszwicx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ynfeqhaw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rkjpfxyp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2famhagqt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2raunarmx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2aqvmbmmi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xidgavow.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2muszdyta.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dehzhddb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zohavrnj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xctoxnfo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dwjpyogw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cikljwuj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ubwqqubd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lxohdpdg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2wqmmxlud.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rctfkheb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tqraxxlg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2iikafoju.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nznhgzqm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2jwkxqmdg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zgsisoyp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psaiyfct.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wksaowvn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhdoktcc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2rkjczpwa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpudipmc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2kinlhfvl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ixblpitf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mspisrhy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uipkkkwv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ypotpyjc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wwykidzr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oekytmde.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bvajcpwa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jsfnbcok.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2midxrudi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxhshib.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xhmhwbqx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gehijrlg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rhffxmku.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2losfhuau.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2lcmzseun.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2fzdolykh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2roihtprk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2vemsvztu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zfuoojsy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2alnqapza.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2clolvxfv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hypwchpn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2rdlqmmyo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yffwboou.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2smrtgdaa.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2cbfthscy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2zovfqmsx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2uybrspem.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2sqzcrbqz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2npqwupag.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ctjxasxb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2fojrhdvk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2wccsseia.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qiwxaqnv.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2pjeizrfj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2xmxcuitz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2lrmzdooi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fholnqft.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltpogacw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2igblxhgo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2utyrxooe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gnvohcbt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qafdipyk.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2rrnqeonh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2itijngin.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywwxhwnf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2baggbxmm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2txiymfen.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qitwwzbf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2aphmjpoi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2mkacjboa.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2eynzccfh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jakzgrxh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hsltkurh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tflzuhbx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dkxoilds.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jatirldj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bglbhmjw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dpvtpcfn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2auzmucmo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lfxojltu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zjwhrxlc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2icxtodii.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2rroqyxon.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2irsnncek.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yvirkdyc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozjthqfi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2eyjrrhux.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llkcnndi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2nlbvfiyl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gpckpqcr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2artbqhyr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2cdgfojaw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccosuqdp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sakcyrnp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kzuqjaqu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujipeiln.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifbilatw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2nitkeevv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhcyvku.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nyknqjtw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2daziyfas.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wpetnfxn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2udqxtxjj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2teupuetx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dzmoniyj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2mhikicju.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hwpzwmub.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2eqfajrem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnzunmgs.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jwcidxor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgxuirfi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2mtdguvuu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2otjsccfc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ierjvaof.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2exertrvm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kikbnuzs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tqvqqzur.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qngvuvur.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cymmrcws.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2efdpunjt.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rbdkrykb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2vbtzqght.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqsgbnmn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2acdornco.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vebjakdy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xoolbgxj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2lwjkouns.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2lljydxcw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kuidrqgx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2bwqmrzmz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nntjdqwh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2skpmkhsu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jquofpcd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wwxgklxa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijuqqime.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jofatmyn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ohcpsdbo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vwqdawij.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2azdwirpx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rxfpmqic.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2itkrdapd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2voaatfpp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2udyxfkma.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qugjtfdy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2tmgrwwbn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cfarkorb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kxcqpxhj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qhrutgdn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qbdcmzmj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2woayzvfj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2axelzsdo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfzzctih.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2arzzdwzi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zcfmqukr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2keweyjmn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgdomkkw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2dxmrqadt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2cmjcjyzp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jwsgfbgg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpohgack.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ruhutlra.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2skosdmeo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rugxhfvn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkegpuz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dlqmcsuf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dzyexaix.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2wupnvoeu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kvqstdlc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2axltkuxg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bslhoipa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnkzimsw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fomtsbyh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ukcindib.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qjhuwzlx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2owkgvnsv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2uahgcwct.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zaohlfur.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wpvrydee.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kaysffla.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2akqulknm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ypiybrta.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2stikozjz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wndfzejz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2rscwzeqe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wauxvdet.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2btzrzaxc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mvxufqcd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2evobgpar.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2moiuvjwq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lhwjtlui.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2oakzsbme.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywlbjzpr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ciohbqmn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2htzbvrad.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucnpvbto.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dztltvjc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qtlrqtgt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dafyyfvr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mttgnkpt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nodwbiwh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufoiraoj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ytihwmgi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2zafunvio.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2shefvoyp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lhpeshrq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ckcingfs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lugxaspi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2njsotxul.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ziwgwpnn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dbnbizlh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2oogennvu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2aphrjdpi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ylkmbkrv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sgrzxfnz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ksxvtspz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iawewhqv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bniqsysy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rogrucqr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kixloiiu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dahzpkxp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ucxclevb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnxvvryt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysqxojqh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkbexcty.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yyavcnso.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2jlbjrxge.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ukcoyleu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2byjvxpvu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hflqeuws.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2edvuzvxe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tzraqkoo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wxionnyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iwjgsrui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tcofsdtk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qthtmnfa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqdetkn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zelkdvpj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2lxiluvqf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yqcdxebj.html


<!-- 参考信息 -->