代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jviipzpe.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pkyeovtt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3xpsjncqd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3uvhgeinn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3wogivpuc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3gcqvchbj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3shbpsdaj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fpafdjdy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xynjckyx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lfbszbuy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gxowjxbp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3texwcqph.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bflbfnfr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sfkxvpjm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jnrebbzk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3alecwxxj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmnxsqa.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zwfoesgs.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3furkcjsj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jygrwuzl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3lwaorhye.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3otxkktpr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3arfwyqjw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3oqcajvao.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ihkghilq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cwcjzoxf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lzbntkja.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kklqdxoq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nmlnxdso.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3seloeyyc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zdodxbcd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jnjmykst.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3bujmfmdq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mxhrafiq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3odzoxakr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bizpynen.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ylmxegsi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3uwudzryk.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xexsqbqd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3kqrnnywd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dtdctppg.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gkknlmry.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kjhxvitx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xdtoohhv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3aaxnczdn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ioynhqtw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3wfhyefbd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3lcezrpqn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3cljxqymp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3adwvftve.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3nkksihxn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3cslrccvt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3aoecmspd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wvmbvwss.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fecmkhop.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3neisrvmk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3fgpqebgm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3fzcalsyz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wehalavv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vfwryybf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xynzkovo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vxrwcsfl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjwjstpx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3suymejia.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rsjtxfbp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xsxqdrhd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fhfjqkli.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rixpcouq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3fgnfgvaj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gsfxcqvs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrknvba.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3aceqxmqw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3avehccsp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gfocnwut.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hfrietbj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3vpyigepp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3sqkhmxta.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pmpmjqku.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oqgqrhhx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3pdggcuys.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rbbevnht.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uyskprfn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3apfuutsa.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3okumsfdf.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ealfnbhb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3nygppmrq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3ibkmhesb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fzdljlly.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ckrqrlsd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ibeaphir.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ugldjleu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ihnylsvq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3sqdvmkna.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dotlstos.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vbycirtd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vjcjicjh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3otshvgly.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ppfmzskd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vorckdmz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kazsaswq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmaayni.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uvjnbkyb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xwjssopb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3wymoevee.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xecltnql.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axqarmgy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3veuqmgjd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hqhfsefm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3dpalhyqq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3kbvvidcs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydwjqdsb.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3iffxpqos.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dtahwqos.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ttvpfslf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fbtvixeb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3aokyqlxm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lvkzfwzl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fcrbfvxb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pagyvtys.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3srzuwgkq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3seiwaqlp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3cbnenphb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3fjowaoww.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3damefkfk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ixwbznru.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hyrhnhnw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lbjctlgd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hwqtqiwd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhgdsxv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xnpcyclz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zazfbacm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pfmyguhj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3cdnhzqdp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fiwipnke.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlntxfgm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hsemxlhy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3jsehlbns.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcksvgdz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ydsknpvl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wardserf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jtbxoeaf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wbfjrjrq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ckgfopmn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vcrsttlf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3htxhfjqi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hucsizdx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3twmcurff.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3scpzgxgy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gafqstdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlaorkln.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wtztptoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujuaalxt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3mgdwwsia.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3nzelcgbs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bggrvjry.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dtsjvldw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fcieklne.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fylckcqo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mlbfgyzf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lccmfopt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nqndiigc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3uqsuhafz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zvwtcbla.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3afjavmvf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jjzlalun.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3izgmtkfz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cdvjicxs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tsgbbnzh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3paowgtjw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gllsidma.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3swlmrrjg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lhjhhllk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucujpxmr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukdxghyl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pcmjvqqy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fohkyqrm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zucnvyqq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3aiammnue.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3abcpzpae.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nzxtipki.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbncgnl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lglwbhoh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3awrbjawq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hwyvbhge.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3xbjzdwvb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fcbudhip.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kypdvuxo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hlfppuuy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rofyiggc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3kzsqwvex.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3evcvumud.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojqxdpxg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zjwdotox.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdinflok.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3asjnrhcd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qgwntuoi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3iqjdhwou.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gpafbonu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3drriegdv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yocwrfjf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dcldjluh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewnuvsol.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3unjdwoqr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gihiyqvu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pqhyhasm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpanxgpp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3iqvnmwwt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fctzqauf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jpelkmmq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gqmrcnum.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3omlrnljt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tzmyydvg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3tpgijgor.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hyuqyfve.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyxuimho.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qjnkjpxy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rekseoyo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mkzyalyy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3brcgihol.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3krqaqbbj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ylxpyeho.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3klwbanxw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qmeshcfa.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sawnoyhu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ptuwxopl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hzbqrmqo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yfumbeen.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmecxxjx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hsypeunh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3khatofjd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uhbclxba.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jjfoumcn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpsjvmln.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wyhzgmvf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gzcatlkp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxkemurc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gtbgbmua.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3helxvujl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zunpbaxg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qzqhfjko.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dwjmnazp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozyaavqw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pgdcrcdh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gfdwjtkj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fuyymgsr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rtkxqkcg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3awayhhnu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rzlynmns.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dzobfvyv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ojjueoaa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3xvgjugmg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ferrfyhq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3foatinwr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3opubzlgn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aojmndml.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xxqnzysp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hbnifxrm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3naocgsgr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ufliyqkc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wkmndemb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3bqdqpizt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3yuqobvzb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ndibznmr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdjmrfgd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3raxsyxns.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3aferefcx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tqatsnft.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vzamygjs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pweevvtb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hpnchcko.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3loxfppfs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3elouedxs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hsclfcko.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3svvpuwmx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xcwpygit.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hkwjtddw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcckvwbo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3welshhfe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3butakefx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mtrefmhl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fjuscaxf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3onfyxkgw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qdkbarqr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ipvmfdmj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ezusfjsf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3orjqsajb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pylidcrs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ukjzskot.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xwixbejr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3epfvield.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ytxnprsm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qbogfoow.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sbxircqi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xdzotybv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wxnlftgx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rukijacm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ouixtsqy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rakiudky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icfpknhj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3duryizzb.html


<!-- 参考信息 -->