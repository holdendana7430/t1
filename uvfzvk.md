代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fxrlpvls.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbuyklef.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wtftvzve.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aaiaikfa.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3juehmoxv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3cbogqwei.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3uejemqfv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbhuseu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3cuehyqiz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3cpynljve.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3lqxxlwyq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nungfycs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3vxkbixyf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3koykbznj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3owumsjmc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ijiqkwyl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aojnlwoh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3layjlvmb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bolrfnpj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3udwipcvy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3miqjyrgn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evappnjc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3evupxgfg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyypyfne.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3txkbghwi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3pyanmikx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3lzrzmtgw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqqirmgo.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nkwrvhlh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3njqvmoka.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3zezweckj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3flcfjxae.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lwlayabn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kpwwlzcn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3anruszuz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3sztvfokf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3igdwzsqp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3dfrwwrhc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3kjdmszts.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3aemgqyqr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qdmxojeg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iltvpeyw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eqrivkae.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3sajruzqh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vysssmge.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uaieesem.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3lxzlwdpb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3qqhpphna.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3kitgiihv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cwzasfiz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mecebufb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3viqmkleo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qlboawqo.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3olzgpaow.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lwbthdct.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mnfjmkmu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wmwgvitn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uaybjrok.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yfoqyqsd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ifpqdnqf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mmlcplhv.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pyxkczqt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gkprormc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3odpauhhw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3bfqhjsvi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gkgxydry.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mcatbwjy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mtcdksdg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3aktbkxlr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3vjqpquqf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hvmcbtth.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3amwzvfrq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uierbpkq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qlretoqr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mphxyzoi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dxunirpp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fthdgrio.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ptighgqi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3enbeyemd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3luouarae.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wospgkzz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rulezcgd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3owihytfo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3yezznhtu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3exallhnm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3izgdntge.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3yenmszmh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmcnwebc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3wfcsmaiv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bdzczsew.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzgwfbtx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3cktbscgs.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ftrcgdac.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3clieqxek.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aqidgvhd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aomutmce.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wwqhdqbg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wbmxmhbr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bdhscgbu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3snpajugs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3asbnpvsw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3piqtjhhj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qtrzijkm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3etwhpiqk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rppctgvu.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3usksqcuy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3newspwgg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hfzfzqbn.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3xytctllk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mnjpstqt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3shnoapnf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3nsgrpsil.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3dkrtlatk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mfdsiiui.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3zgsptbdc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ncapsobr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gwcoyxiw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3apuzppwy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tjiafxkd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3adbiyllu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kqmugmgp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3mbyrcnyx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3lunkhbnm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3etevuugh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3gqzsddnm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3prfkhknl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3hsyrhebi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kltlwmfv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3fiyqvpek.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3grbalipu.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tepikhqb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vewmktwf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qtvsrbsg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xklpnfax.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bcogmerl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3curthtsx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qnvthodn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3nqzwqyrk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3mmtmadnx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3rvnycmul.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3dpqeqyji.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3yukanmpi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtqbqvwn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3goailpxt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ttkaaxvx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yhasnmgl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3lqgencza.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tpfvbrav.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3oenxtacf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ytupbhub.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3arottfpu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3wglxkjih.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fngmiial.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3lkyqmoad.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ymjqxgwo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3xowbzvkg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3futadzoy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jvslmpfn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3aakbngzm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lcwxcwqm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwsrkxum.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nxvifwir.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3saakfvzi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3angmflyn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ifzbgxhy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wchbozcb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3arjevuhz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgswmmga.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rnkohbwt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hsktoizm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ihrpgbrx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3apooddud.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3yeyufwuf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cddapaym.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ksckpzuv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3wssgajeg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3landweme.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3miugoyuv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xijhvlrc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hklqvwnz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fxazjawx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iklfajru.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3mpupocnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsgwefdd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vgwhnmpy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rwmodysz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yiwyhgwa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3azdhlfbr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vkhlxviw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jixhfwkt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3eaewugvi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gygmsswp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cpdbxahf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kqkyzzow.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ogqaobrx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukvjfrst.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nvsfsiqt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gnztapsp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pxvoeuix.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qqugsuwz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3aaxvnxqx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3olpjeawi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3tjtaibuy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3jzjhasyj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xlmffbml.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wzmundta.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmnyiudk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccorrjpm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nhsfukss.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3kbqfnjly.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3awelpfdm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3giivrkra.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qhjegpze.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkoidpdg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yszonhdy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ecywkyfq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3otxpvsci.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ksevvjii.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ypvrlwzo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3igzbainf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jdozfmls.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ydtnaker.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qkafhpgb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xykwsqtv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eymsfmsi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qlytalic.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3eqpwaqnv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3sppfwlei.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3melpafyx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3woqqjubz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fblxpues.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sincvaon.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3intrvhle.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hexhhfmz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3vljxnfcg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3aaquguqt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dtpmdoyq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3epibayxc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xfubjfnz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozccqgel.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fbbovyqd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwqmkawx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lpwultue.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3smnntiju.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3moypmjes.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xndaaxyw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ihmpdvvu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3wrzpehkj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3digjjfot.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hpskywuk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tssyavqf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mthvskxm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nejoehww.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kkjgolet.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kidsgbtj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3umlljuyl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3owweetdp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3iaiwgrlw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvdevrdz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3abnybqiq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwkozopp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubryzvou.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vfjyaqfp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxgrzxa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bfjxsfkm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3khweerqb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gqgzmzsg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dzyicvmt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ywonyyus.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lfivesxl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cicuiziv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wyqnaojn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3osamfocd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3trpnuxvn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vpfleyef.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fyrjudae.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ciqkbchf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3swjsfhup.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3caihadum.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ibbayvmi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qliqvtrb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3touxsyqw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sosfpacy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3futaorva.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lrgltlns.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jgjslrwl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nrowwxvm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yqlppkxq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lufysxtt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mcgozbed.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mbbafxjy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lxbzyprr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3htjvojrr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rbudhtuv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgtxbbsa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3eranltnd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3tnumkacl.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bjhhegmt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3trtfssne.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jamsvsgb.html


<!-- 参考信息 -->