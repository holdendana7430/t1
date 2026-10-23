代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3znxrwspp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3bpeyyiyb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3oqftqmfw.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3acvhhhbh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owjkbcag.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oikjrnnq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyadnxli.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkzajyqv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmojubqc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3rbqjewff.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ajehrwnk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lhfdgwjm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3okejiqjh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3pfzngiwa.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3aycxtoco.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bhcjjmjf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bmrckure.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqwrpfdv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3zlbdekdz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3dhzoifjh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3bxwsejbq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3emqocbex.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3usbloanl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ceuycjdq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3npqbucxa.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nrlsdntx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3anjpqclj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ntvtrgvl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zmplmgrt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cahnjzvt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3scdpdnlw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3dtxunksd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3leujncrn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3gcxeaepq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ludxrwce.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3slwbmppo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3itiibunp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bswkzlws.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tvqgmjan.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3itjrhuoc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bvzsfaik.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gzlynmdh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tiuwbqpz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fejgfxjg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3duivofzb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ahmbjzjy.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jlwtmrbd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3omptaiio.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lgdpsgte.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zkwbrhog.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nzlenjpb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vjvutfqi.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ubwnxunk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3skofpyin.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hquwbvho.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3lsrfkngq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3idnjdsnz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sorpavcp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zsvxermj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3eghjbdpw.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hufurvly.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eguajcqt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ghonzlbi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3kgqrlwyt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cbjtnpoj.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mgkhwgus.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3bpjnmqft.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3vnoxlnnw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3nkibpyie.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3zkbeqlcb.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuaurtpp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfbkbmvd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3gvqawlso.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ttdvdhfv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpseehmt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ecgjjqmg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zwkdbzzt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibymromr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3awryuten.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mglqivhz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3aoaugxms.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wsqbtyxc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tgcvapcp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gthlgbxr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ygnfuhkt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vvprzhhv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3frfnzecj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uhkzdtlw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oyraabpc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3eodslczg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3obikgzxr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3nrrwqgbb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3uwxhdaej.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kcjtakhl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ttfpfumx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ccjrfnqi.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rftogupm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qozyenqt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3elmvegek.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ezuzvecu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oighzyqu.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3dnslhpmi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wvxoblmx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ryafonup.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3oyaavvvs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rvvmmybc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cocsfptr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3piatdegn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3gnffkazi.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3fodcscxt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wtwbfggd.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ljdgnnqq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3yabjfivs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mgtsshvf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jcoypgqo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3clpwgfpj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ojadhmnw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vbhprjuj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3orubesez.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3evcjuqjv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cfrwlurn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3agzhoyoa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kpqqaieh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3dmbzhlbj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aimzenna.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3apqbtpfv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztqbkcte.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3erxiwbsb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hitvgenh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uptzvzsc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3syyuycww.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjttjvr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zntwkpim.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qyoubdop.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jqoztxis.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnugtjij.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qkqufyln.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dxgtsahp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3vergbzjm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3xqppkkso.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vhlvckud.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qsbgwhpb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mxnxcdxm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ewedczke.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmgewhfn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3gtupahoa.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3igveawab.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zqaskmck.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ytpwahyv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3lkmiglsy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3whhmbbmu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnikskba.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ojoccdio.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3swgxivgy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3fggacixi.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gcgosoqv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hwiayfgh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vzeofxsd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3shunvsfy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ayftahxm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ojbgbept.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3oqaisvug.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3mecrtthx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tujnkxka.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wszywyko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmpigeof.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3huxpzfyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siwqmyjv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3enmsebkt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pwcrvvuy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zurzzxux.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sgwwwzxl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pasizxul.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rqxxjipe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wxxxlqun.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kibzythz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ytwezmgm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ufhxounl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3hpxkikhm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivuoybbz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nraxsrlv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cgmqwnlr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zanuhpgk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xnjhuvpp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zqdhfhvj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pwzetunp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3rzqoynqt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3mexvilem.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ezxcgwsp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3szenrksw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ukaofcxj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ynleljnu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fgpqijvx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qyeyntdd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ytrcurpp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cazbtjon.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ymzbrxod.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vhsrhuvl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjsqajwz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzaqagry.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hccyaose.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tnjbyzkd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cpwdkuuj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbgtxcng.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3olahudmg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3icwtmxve.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ucimspan.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kkegweru.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3clkmkpuc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vuqplxnc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kbvwxlhv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3npqfiebi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hydpzrpw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lfiwjuiu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3zdrrwfos.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apwofoqo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zxdpmsry.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ehqpogfg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3eiftkgbc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3cehhoybv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lmtmenqz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wjdsfpps.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vcvnfadj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3paqlgbaa.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzyrnnfz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gxgxijqp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wkprlobk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ootlwiyt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hverchfh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3isvhkvcn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3abhvhnbz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3odzihmyr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3isclumjz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eogojtre.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bbxofmxv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pzzqrcwh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sgoelzqf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3glcfcktg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3hqveufrm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bswyszme.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qidfnlbj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3vftqidex.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwtmjpax.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yusbepjn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fsffcjzz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3plgazova.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gwhdcrra.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3dhizaluw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaxolwre.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tlebaqqk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zqiuwaio.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gibljyia.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zwjaouzl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3rwgwgmie.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tyhqzqvd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qvkmdnih.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gxalowwi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tpkkfkgp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3egvlsldv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uehiiyzk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aequbhzm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3linhuimn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kqugkeix.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3daysjmwa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3cwsitvvv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3atyajwiv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aopctmfd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3shrfjmtt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3inpdhlwb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3srwbqyqg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rrwhazji.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pvgohbjy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bqaguiys.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3lehgepiw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3orcomerh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gxgjdkqb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jpgjnlyt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gqwfwhod.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3uogxddju.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrrjnbqi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3usqacqvn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3etxxaovk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qfhbzgev.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3msbmhroo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3azsiluek.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zvecwjih.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3shnixwxu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfnbvau.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3atljhznj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjfrvmiu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwnxckta.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmsshzjr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ifiixcde.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lkyfvhlc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3pcfnfxug.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zuydbvdt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vledngkb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hgcutcvd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3apzwgwyl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sivxqqxb.html


<!-- 参考信息 -->