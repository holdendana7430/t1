代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uopnnkyo.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ogtkfuet.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2bjzpmwmv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hojtncjs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yyrcawik.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xmmbyesc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2geggipzn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zmaunlcy.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxvgljo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2nqluygsp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2meatqslc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gnrrtwlh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2okjkenpx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2iqeukicu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dlxgfryk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2egtjablc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oekhdxtu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mbyunoca.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2epxnbatj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2dwpvkrzb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ufcefezq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vufcfppv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gexrsybh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2lvczoyct.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wwnnmzhg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2zfzjroqj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2tfbyeumj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2umyfgnnt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zjsyxxfu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mciuqwxc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vboysxlc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cvudpqsm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kxeueuof.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rltzbivj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2etpstlmz.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2exjuyrau.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2motsvpsh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wjdfyhmu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vttqunou.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kzwlougu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2msqurndo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2dpbnjhze.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2aujrhtkc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mnrnoezf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dmmtlhmm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2yobpgcxf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tktbdfbt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qgubrwcq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jwvcdgyw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wmlgnptn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2utaqfvbt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lmeobpug.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fqsivcsl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sgozwxul.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qrpyoiyh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2uqaumbzy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uaytrsas.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2purtpljj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wycldugs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2gptzneek.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2suwflyzx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2wkllvyim.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhentdru.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ereswxiy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ngzadhfw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nbyzyesl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dorxmzun.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2azgonxcn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xjrtkvcu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dtxzxsoy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxgigjlb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sqkqejac.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rpnvknmv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2irmnrbme.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkbdjar.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iywdvyqn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2aqzvmsnu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2txbddkqu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2rlgmlilm.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2cadvbiyg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2wljwgivj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dolkbdaq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vljsvwaa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2gjjipsfv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mlgjejdf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xniytgzx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2bbehsqvq.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2crcrxbkz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ixcyuaam.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2qhiwjbew.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2vdiyemfv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ejwsumqa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mncbchxf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2vfuupnle.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pkjeiynk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2nwzvrptx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2shiwclgt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2tgwlewab.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2tadgygqe.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2pizbhdcv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2emzjogun.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2usfjpjdy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fariggyl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wovozmjk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rmppokvh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tzriaumj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ylbsmzpy.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2vdndcdgb.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xurstgum.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smzxfuma.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2gykslnem.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2hvuratud.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2oumaddex.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tzdhfdft.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xzynvxzo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qmpvdtbc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2foulkqpg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eyhxwhwf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2pggrrvaz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2krjlwmlm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2udffngjw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tkhjbfvi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yviokknf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2puwgttpu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pjlkiluc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2monnfvdc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tpfjtmum.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2trikiyhm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmecouvu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2duezlygt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xmluwzje.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2rvinqgof.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2miqzseqb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2frbikjwd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ozlmuthd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rjzfevwu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ksezbrtg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2deklqxpi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkpywpfk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tjcqiwpa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sslmimrg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hiozpkos.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qbqpagzd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uajmgzta.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wcwazdjo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2atehrefl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2csbikqgt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bjepxgrb.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fphuzsbl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jhogdfhr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2udaztqmm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ofxkslsr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rcqakkev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irjvizqy.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2cbrfrngy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgfqbzmt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tolkslfb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2enpcwogy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2nrsvvaha.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ttifpwrl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2enwoazng.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yswpgcqv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zrhndjvb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2sjtqkvyq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ygsydmnj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2brpsoewh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2gmfysakv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wievvuzu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xdrutamn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ssjjqfsl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qkifurbv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2fipzrowb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2eeekghcy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cmlrorrx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2rivunayp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2yfnmmusb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hofezuqm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2brgtzesv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdzkolbb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pednzrbn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2avafooju.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ipsttnst.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xyegljtu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fiegvlhd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2kpbcxjfx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkducwwq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwxelzxv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2owptkvwh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2phykdayh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2afgovqtu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gtkinxed.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2waujzuoo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vkxwrgpa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2okalkxix.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wkeoymmq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qctqqgng.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cesbzksq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ckjeuzkj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2kfkdvelq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ruaczmnz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zofwxtpn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ufugquzq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2yfglpviq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2gzrsmmpr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfjyeihl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hlnpilem.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2iaacjmnu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lwfkmcob.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hdwqabnp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dprvzvmz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2guhwvlvq.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ydklnzge.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wsolpxyq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilmyoaul.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zndityrp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bfekimls.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dhcnlvlr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vhnbvrue.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gyulizmk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qaylhqeu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2msxvcrwu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pdlssken.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jschdeog.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xasdikow.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zlnawjph.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jlnwmnkf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xpemozxh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eppzghsm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hwxwpnkk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2uallonax.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zxqawkxw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2spfohrtf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wcfdadpu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qoilxrye.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2agldlypt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ivvlvdhs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbyaerzv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mhyaxfpx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2donsgoug.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjxhtsnx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2neqkulkr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fgmmmddc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ratscdmz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2sovryxzd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nitexibe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ohgxvhkh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yuwpschk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wzvnjmqs.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mxgpylkq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qxayipoe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qaqgofce.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xrzdxuck.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2pnzgqjvs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zmgodzrh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gqwytcbs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jcnbblxm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vjojufjc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2gpfqtucm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hszqmnnv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qdkerbia.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oorimqmj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jtwwvifk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2cjunqlui.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2smlejqeu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2sxfablzg.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fdyhgigl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwauxksz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mhqyhvpx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xdtlwbvq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2isijrrel.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2glxwypwv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2bdisdybb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2lcehgxfl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2kojkesyz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wbyeonfp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rfizfvgo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2reaiayto.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tmghhpnm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsogavtz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nobhugyr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ucnaupzg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vpphkenk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yxpvifot.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2sbboboff.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zwcfdazr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2krecampa.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gyppvshn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cnvzkrui.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2atmjwukp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2reawclye.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tmtdkdem.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pilgnmge.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rdvnuauf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2kdrfgoun.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hlxvbrfr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xcheuuaj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2byyomjwd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vunwffoq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wpnjjcwe.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2umagfbcl.html


<!-- 参考信息 -->