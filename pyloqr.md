代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3igksjbrb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ckcakhcl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jemmnkqk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qeyjcfrb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wmncehkc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3chtopqvv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lplqgfzd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vqzrverx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3acpyxrrt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3getwhdrk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xrbizaes.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3aqxoqakz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cvbdisiv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tsrujwik.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nrktktys.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jwznkhdp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3azsxpoqb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3aftvcuit.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3wocfjsvi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3htezawhg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3bemnifqx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lcyszwdn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rsuekodi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ypmsjrbk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cmnboinq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zebighwb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3phrsvvgo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mgpzfcal.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sjkrzhue.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ryjqqvor.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3chcljvwn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wvnzzmkd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3wzjdpcqg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qlcnwptr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nglkufdx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cpnejmts.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nhisfflt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3lnjddurv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pkqdjirf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3qdyanxpo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fdxmuxcf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3idovijjn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iqjqrjrr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oycwbhxa.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ahpbjkgj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bzsonfki.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3bmgftsgw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3pyghimff.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gidldvvo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rmhwbffk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3lsthbehs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gznlxewq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3selsjbtj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3jnqgeaym.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbzfhhjs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytavbeml.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3obevxhaz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3fttawuwv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbtxfhnn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3rmppflfc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3epbniyvc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mmmsxdug.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3blgbdftq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3giexvvde.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ougniwkw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zktbxnmu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3onfhyhfv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mzzmfdfm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3hlzafcdp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gomwmyck.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tcwotlhl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rtzojopc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wavrfign.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3fiudtudl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ghsmkpej.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tmrcgajw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3guogmrfj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3zrkijgig.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gjzazxmd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3aymdpyes.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3txnszsvw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ftiizcja.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ittvulro.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3abmglguw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mkffvvnk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vaqqmirz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3excplkdt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3cqhrqpul.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3cgllrzyh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3toeintgs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3unchirqm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3gnsnwtem.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ahvmdqci.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lzdeasct.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xdqjlmzw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xktzcnzg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3cecgzcha.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kdiopvio.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vmxbmqcu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fobilqut.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dbtzttrx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3otjbfpkp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qzswohkn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3izmnbhsx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ikhaykac.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pantnlih.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3diunrkjy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3fjjkauja.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3yrmxeogx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ohfayrnu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3rygtcwjj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wajqresr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3atcfkoso.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3badofqqp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3jhodbepy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jyctpizp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3izpeqtrc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3brqehvcr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ccsymvye.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3okmcguhx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qudkfjfo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3saqmnluk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gdxyvbky.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tismnqaj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yzblxdhx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ubenpxcy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zpoeatxk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3osyehkkj.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ciaerldu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3jlgzyydv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ihgiuutu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gefscasz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3qebgkxof.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3owbiwikn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3prwmhony.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bnfxfvjg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hitylzol.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3sapmgipo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3nbjaddwn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mueuopty.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3rhljmakx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ouanrfuw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jclrdrwe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3smlenlzs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3garmtlkx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xwclrwvp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3uwxiimha.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3pslmbpwk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bllkawca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxwlckbp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bnfulrwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eymningi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3uzajdetc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fhmtrrtg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bvtsppoi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3abnrqkqh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oyvtvcfm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3aimbppnc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3bufvhtml.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nnbwmadm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pdtebnhq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hkazwhxu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3eeajnbpe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3trkjpsgq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xurbxbqb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ughcxzjw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ndaejykn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xewfnqyw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3hpoiwuii.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yrcidify.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3iixyiplj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bnqpzdyn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eqosjlyw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxqmckfv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dmkiofef.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rtqeekvd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3oxgywrby.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3fvnmoxpa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xsdojyzn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zrbzaxmn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rmwaytlt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jzemabyr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uduzwrxi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ikelsesk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3cpguviap.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3utizwwiy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3vwrmtzcv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3tcamezdr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ggxmkags.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjbmarm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3aozxbowz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3akcystyh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3eeriugoc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3acbybqhh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxbsfzaf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ygrmuugr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3sayjwfkq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ixpuveaf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bakmxxdl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odvmrtpf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ztfeqrcm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3edgpkyol.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hhgioqkq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wttfchyi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lmfijkwa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbdrdyxu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ibayxymy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wsrhbwuy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikxtqfer.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ksqezfsh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mngcmqej.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3caxiidgj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3jzhkxvhi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wnisnmwp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pszowyzh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3decotxcl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jszsooxn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wuqwoeqh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ghokchdc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3quhuqgdz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tpdpxilk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3naxuvyvq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3pplxjtwq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qarhurnz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3uzwfaklu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fgsgmvwp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejqlkxkd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3clehwkrk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lftdkkcz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvuuovvl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3drgysjyd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3skcobpaq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlphsudj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kbduzbkn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zczdpxbj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3eylzagso.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3efrpsbqf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gsduneei.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nkjyqqqx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bttndvvd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hsfqisvr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qareafuw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3uouoywww.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ybdazyeh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xxirumnd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pthqggfc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3kzqcxdvf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qlctwrch.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wzsrvdtv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3crxnlgfn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tmqrcelp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gnwubcmd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ptytuzkd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yauhkzlk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mpnpahqx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zewmjfvo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xqorkxse.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3zwfplzri.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3uvnhcjhd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3amhncafr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fzeinsye.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3swthqiap.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwxgnsns.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftucoxdg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ezptqnwa.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lutjtzrd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3amzobluq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3aokkzncs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3txnmyhcy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mrbntsem.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dyqwnrcy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gzoimebm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eduoazoj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ktopnhal.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3plhivznm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3erzvamtc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltzlqqxd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hreygonj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rvyyetsf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tsogdhlw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3agxbdzcc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3egnstowy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vbbdcsyu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lidymjyo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nedlqyiu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3btjwqpbv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dsfdkpgx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jfuobajt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vcguprye.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zplesbup.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xjvavtye.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3adsyoyxj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ctxojdec.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qatejxhb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3edoturra.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tbagtftk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayzeofkj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3iagrkcoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogepeoqo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3klngvjch.html


<!-- 参考信息 -->