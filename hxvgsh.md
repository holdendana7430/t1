代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lrlpmgdp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sygecror.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3rvkcimcy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3joydjhqu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3bmkdoqnv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3wvcegtwx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3qydcezho.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zhfutmyh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pxthzanh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3koxsbzob.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xvjgraxd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3fbwrhdif.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bbqtnpjf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qfoggfmc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3bgiobgqq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3hpmqbjyn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3huixomdr.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qvdectry.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3cfhmnsql.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3xjuvgvkl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3gqpszhls.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3foxhzgxb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3kxgzckhh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gmdlgzpk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3drzvjlfo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3liqukdrn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tscikfvh.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3unbxplxl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uvdqsuab.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mbivlabn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ovbfmstd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3agdobxzy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3mnwkcycg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3roirujqj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3edqeydbk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vvzblybe.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uyejqbyq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3armukgty.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3thdfsphl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3bjhdoien.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3clkddaad.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ztljzmex.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dritlbks.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nuqyfmeo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zpphkyqj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tyidxaku.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fjonjvtx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xumbnjls.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iiiqozmq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dmwrhynf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3qgnglrnf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qjcextgm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3wasybnie.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3wrmlhxbn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixybpgsh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwgtdllf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3lhwltpiq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3cyhtdlui.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jvnbzfqv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3lnwkasep.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pshrbfer.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vlxiakuy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jjpqdsor.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uwwzgixk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjsldvmv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pzbhzibj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cxlfhjgq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kuzijyqr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3jrcvxlut.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3entzynye.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jpneefsd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bbocoggj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3khrelfxn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pvqhgiww.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ipdbnfbj.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3yauyrbti.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3pexdmnke.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3nucguoxy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ukkikdhy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3xowhmghs.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zwqfufld.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3biansgda.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ozhyrbop.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3dvjrupzz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kgfdvayt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3trvptugv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3fpofxywh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3cflyogye.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3eepvkicq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3oklayzro.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ooknubkg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qoscxnmf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3uaqjwvoz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3dhhycvlq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3yhzahwfy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qsmmpfhi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jbifchzr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hceugpil.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihhqtjko.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3paxinmng.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3spwrsyrb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3coeygnhj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3depbarwn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lvurxjix.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gougjkfk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3llwkuvqz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3lxpdxhwu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3bnjbwycy.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ljrhyxfr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ltyjuqgr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3uosmkjgi.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aqmmnsko.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pdpfhqmy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jkngatma.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wruidwnf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ybbzuofr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gwgwtfzi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fvghvqae.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lvoysxyu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3blbdenft.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3whficlpm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3sxfsxsru.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rgeksezx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wolzuazp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mitrktsj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ycaldskm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lkszhkbx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3aizkbzqk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3mngqdvht.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vpsuoihu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pznoujwm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3unbffijg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3javmwzys.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3onpjjicx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vplovufa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzlcrve.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3czvvvsyu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3aoqjwndh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lvidqpyh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3afqhsnnj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ssnhuuyr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sgghyxhb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3yffrbctf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3mixfcylp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3bjbszjau.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vzkwtksn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3aszgvyra.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qgtfnuxy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3azxaeepi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hslcnnmp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3atxnfoun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkhtvjjf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3enseivfv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ifszwzxp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlsggxkr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yxwpceuw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oikmegtu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rlxghqty.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3tnjpbchv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3unzehhbt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ujjryzqt.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pdbjexxr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3zswjczgf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3autjgrhw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ukcrnozf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tjuoiten.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3obwecvnf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fhuznzge.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tlvytkzz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uatozvut.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3euclepuo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3klsbkuif.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mtfbpmkr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3abcrkyse.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqimdpzb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ridmxuwm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fpuuzyne.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yxhebplr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gfwqalqr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tuikyeep.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ppwgioji.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3quzztmgs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezpnwwhk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ddwziyrv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcuftfik.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qvrkliap.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ppmggxcr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hkslnxjj.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cemoyqrq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3aqjjxobs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qqtcekgr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrqvfzth.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhvuqpmi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzczmdxc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3fcxnkrtn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qhwgqxqw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3smjoocoy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3slnxhatz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3shlnwweu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zthgoyeg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bxyyvobi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iedsskpn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwrbcvnc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3dgubhtii.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3midhipge.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3sdvorvfo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3mofwtuqm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qzmkbpvg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qwktijdx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mohdcbce.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uocjxwco.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dunlaoxi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3arorsdxa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3cixeylvd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxouagei.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3pdhgyzvu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ogadbkzq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3grjfzfhj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dmgspoog.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yefkfkac.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3annnxbsr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkjtwblk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bqmpdfhb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hubmcmfb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gugksgfi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zgfepuhz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yyzteucy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uqkvoaef.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mwxrzfbb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fdsklqod.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kimomwzk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ymvwcbsf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3igqneche.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3prwppbqj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gwrndhsy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3dptbhlfx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dvdgvtpd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aipmfend.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3whajigjb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3idqizhdq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3alzayaci.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jbrlydxm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ofxpoorf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nggzshmv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bzbcczme.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wdecjaoo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dztjlskl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3narvygir.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xpcdejlb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3fpbgwjqp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uldxgmqe.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pqvjokbs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mddenxxg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vkujqold.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oynnnlmp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vevstxxz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ubgkzcge.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vukswjuo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3unsxymth.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3pziksssi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mzqdcxah.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wjwllugp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xjpnkwch.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ndaxyypd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qtonreyo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3zggdqgyd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3iqfrhznp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3glyaotpq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yeghtcfi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3japahhka.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fvhoxlzq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fqrznzju.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lgkdbdpe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rmhqfino.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsvhgepa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tuxuoawh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qrhsykxp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bskqvqmk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bxptgaec.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rgliuobg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gsxejwly.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bnimrzeq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hrqivtpk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ozozsgxm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rrovnnwd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kclfshcu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uuuyedju.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3meezkqcd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tuqfkpap.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ixtytlkp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vdwgpxck.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aeljrahn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bpobojqc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ottmhgkl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ylygtlyd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3damtnhho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trspkkcl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uensmnbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxhfzfgl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gyyoikff.html


<!-- 参考信息 -->