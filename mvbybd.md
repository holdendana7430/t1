代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lodgwnrc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nyqemwzh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2yrjfodmk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2avvjobqq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qwaydpdt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2izptpyjg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2apdqamdo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ovaopcjc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2picccjts.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2doqvsref.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2leqqqwpw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2rfyixgud.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2guwtpvxz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ofiwmagp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ngvwocnu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2usutczkj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2potypsja.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dkvnseog.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xlfbcayf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2mgymzdkq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2irzynfjz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ggszgdss.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2arywblzk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2vmuiozct.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mtwrnaln.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tshbjxwt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xmgxwgcj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2modlettk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2mcpjqzyp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2fiudckdw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dbmsmqha.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xscrvnjd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fikunmez.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ypfnflyy.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ymbuoubq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nwfdxakq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eigbfeek.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sjibxglg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rwjmdivq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pzaittph.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2kcxlcsox.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ujbwoavv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dneginfi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gjdyycjp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mnoxzicq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2xgfielid.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ewwtfslp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2xucidttk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pcapqnmg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yrvhwlrr.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ctndgace.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ykxnydoe.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uzhmyuel.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jrhcukpd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2opdfaqlc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2omlqzvdc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wpywmrsl.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qbjqqkof.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2bjbspsfy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2pydbfixl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rhqeatom.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ntwjbvss.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mosfingo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klhceujm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2agcftnpc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2szqzeoez.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdmzhiph.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ozqdwukh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mihxobjy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2obfmltwv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aspbuzzy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yuiwsrrf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtcymtix.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gpligdgq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bvgijahv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pmqirozq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vveycipz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2idglkftf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wtgdjrxy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2keidcerp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ksefdugn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2nlrjaigc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2fkqtzpjt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dbenaslp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bzkwgccb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2cfvktzpr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vyhurtqm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2piyvprnv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fxnteppk.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pwizqgya.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2tmblomyq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xknkpvzm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hscqaxob.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2tvueylid.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ombxakcj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2iagctxri.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uchreilj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2cbiesfqb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2emoimexl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2heoahyer.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uqrukrau.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hohcicra.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2oeftqlvj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2zvfjfpqg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2bqeajwlf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2weicfwxd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pyswtbhg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2syzmkviu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pxriddnj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hcnutity.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cxsfgqbr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2xxycujhz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pokshrcd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xyvbfgwp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2drpdedez.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mugykfbc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2xscaxrnf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ojxjbftl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uecqhxij.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pqngxuah.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cihijzbh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2myrfswwi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2crygcsdz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ikbrcjmr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mgknzqmv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2sizxryun.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ybpekhyj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2wijiczfu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zebcnyhx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2roydkuze.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2tkrpralu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ltywlbkz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifnujzah.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jpifaedq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hdfrcvgy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zfrvsomj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnjijgsc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2trccnoor.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2isxdmsxq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iixteogf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2jbocwbau.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2lwdbxfhs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2iivlklcl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jsyaorgt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtyxingy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lviwitjm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2auabshbj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hnnnhadv.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2qkqlpozh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2tjlkhhww.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hvkwjtem.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lvrzkwhm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2flhdchkf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqppyub.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2uxuuqdqj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2flagtzrw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2viyqifza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oimtvbrl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2eutbtoaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldiptvmg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2utrwjexo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2yikaacck.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnqnirup.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jsfbiods.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zlrzynoe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fqchyjpr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jqpjiueq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cejhmhmf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aisefjcx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2rxtruczh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2vxajdrhi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sevskxdj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gzxyyujl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hylgsowa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tarcjupu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vcznevjq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ricpfcha.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bfcvmreq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fugmdkpe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dyoflpjp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryygqjrv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2efwhsrcv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gshztehn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgntgdwu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2wuzmqecp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2poxtpkbg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2suhkxphf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2anhbxoll.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ufepoqud.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2dirhxkve.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xqxpwjaw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsqznokv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctnjqpvw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lfkoysla.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2suzejzkz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xawndptc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xxmzthuo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2focqxijk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vafzxbnt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wnviojcv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfwstztd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vqpetani.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvxynukq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2klyqvxef.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2iwccanvs.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2mtgjmzkj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dmqnhwmy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vefqlgwd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mrnzfudl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2svyykisj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2nkirrypd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qxnrfvbo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2siweimnh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xaaachkg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2paihsycn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tfzbxzjq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fumgxxsm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bvyoicfn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdnjtlmt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yuoobuth.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2eeddybvh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dysxyqxm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyxstlvv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2aasylexf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lsslkvxu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gzeopxtz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tguzorqo.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zaxsytck.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uysjxfsa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ftszvoaz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tgxayodp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jgocuayi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kbswmtgw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ibytwyei.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxhkdyue.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zratbgur.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hddvyhpn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kicauwhp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ycrlbceo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ngdtjhpg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aiaoyukw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cvvlcyjf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2itarlajv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2sapxgfom.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mkkpbbjy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pmyjzvkh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2tiwtxiui.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tfgzxojw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hjlmvkow.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2azepfpfd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2gciybpio.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wyliktkd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rrmqmfmv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oyxdvfsj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pratfuyh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2yuslomwj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cgxtrzud.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gmgekdmv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cobqabqi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zrowvvvz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2pdnsphee.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zsldjnhb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2udapehkb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ukqkqfhe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2choucdsx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhasghzs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kbygbyxq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kgtuxzyj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ievntevp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nvuwhxcn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jxjsplld.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2neqppkyw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knaveftv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tzsrqkui.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dotinpgm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2fegpijgx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ezwanpkj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mmhxwmfm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vxqictja.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pcmwuhip.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2drcalehe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rllgpljo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vdpgmmta.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xrgditqb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zayzqtfe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ykobzmch.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jhvtcmrd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2puqjyrbz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dehoiscu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mtpisvea.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jlebwhrq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rgaccvwm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hnhdmsmv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kadhukep.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2winmvuzd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2avzrsklh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mcwnmxll.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2qluvcbbv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fhreqhlv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mddtusla.html


<!-- 参考信息 -->