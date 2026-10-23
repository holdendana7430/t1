代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3oopjmcnf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zkdxfjvt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3doudbwed.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3gjhkuixr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3fxbiuguj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vheqtkxe.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3hqhlzrib.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gyfdwxjh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rnlpsyho.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bwowpuzj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gnxudhsw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cmzcxkuy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ltfgmupf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tdoqzcyc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zhkxdqgq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lbgfdcoc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xaycdxpt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3rainqpgt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ndklcpqb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3padbwzsg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rdbttbcg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3egqaanub.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mwbhrvhb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3taoxwkef.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rpqvgdnm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kpzrsjwv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3dhrsvima.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mannegfr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3obwdolhj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wypgtnbl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hsnovjpo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hmmjqtqu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ybobatpa.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3llpdsywj.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3qxvreede.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bmmcbcsf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3mruqdged.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3jpyysxwy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruozimwn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3zfbtksyf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3dtrqwegx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ueoaxora.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmmymhiv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3xmkxxbeu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxvnhyhj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3omxyrnzp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3alytijjq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oqjiabmo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oitpqort.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bubtsxlv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wlswrnum.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3luhogbrr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3boqayddm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmggiru.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iijhmirm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tzjjrlml.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3egtiqgax.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3opqusyvb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3hxczdzww.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3aqulmjpy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qkyruhac.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3xzvwivec.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wtkuyvjo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3bicjtiqr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3opczzywn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vzjbnwac.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3bzeibizx.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hwrvckjs.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mrbmjyab.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3aorfhhwk.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3cnbzlppl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3vmoctdqu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ovaflfsz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3imspiyqu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3utqxbpob.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3tvjstsnf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3uoupvdfc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bqpissda.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3egcdwfft.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vjaoqquu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3srzdckyp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nmcftobm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xqtgbszt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qdnbprye.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtejbpk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fcjwwflc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3amwwmlfb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ylcuqsdg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3scfzsiat.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prdqrdwk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3sztpwdka.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3orfqiqol.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sxofbrpm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lzssghdh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3niagjeyq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ysbdihxz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pvsegfqq.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bcezyryf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3glmzzgni.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvfqqxgf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ruslvcin.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rygmlgsy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xohoqcas.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbonlbmm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zbrhgjmt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3sjmrvnuv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3xkkxcbjv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qzqllsng.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjommvjk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sdovnelb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kfuywglr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3emrrfzjz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qlpyfkbk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3uvpkbjul.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pmacgauj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pdqeugdo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3kiunfnxc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3eejbkikp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ejgzadic.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyfhyedf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xctymzbl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpuwdrry.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3aygtxvws.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jufptnlh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wolfwvha.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rgmxblfb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3poutbtlz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3tmaeylfk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3zvqfxxly.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3szcafioe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3zoiawbsn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uxhnthlq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3qjjqzjbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aavkgcwx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bawkyftu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkisrljs.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3bakxmydc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vyaqitfl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lszdvrrw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yzmvwzmb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nowzkdfe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ddwlomjk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3qnpdczqb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xpylxyuv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fgzshoti.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lncueswr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vdthxtqf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gucchdgf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qzeizmeh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ivpdnflb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ohgvhunr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ixtapycn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3aabvghvr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3honixfkm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3akkcyqbs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3wzxvzqdx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwaiywjg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycasfwjf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tqfdojzc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hvhxozuo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lnnhxccz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3znhnocja.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3twfxstcx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xaihemgv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wlczdsoy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fbgvmuub.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cowcheca.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfioikpd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nonsiwum.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3urxynnys.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ziayepge.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nprdufeh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lxjfskaw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xudrdvgd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3otwctnrd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uawrprrk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tssjpzhr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwdyxilz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qlmbkmna.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3amxkirqt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3qhstpsgv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zkdlxrdv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3bntlxkgc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rvgrydlp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rbmbpudk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3klisuksh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3eavtirdc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3dtgppznk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nusqgakh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfmpogah.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xxiftrhh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3tfaqegka.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3amrkcxcl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yerrprxi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eenkovqe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lzncaiqr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nqewkaoy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwmchjlt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uuqlehga.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jlhbbnxp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jzqrmpnj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hhlfagom.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hyofokde.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uobmupfa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ehlrankx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gdewshbw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wiaemqsn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nrvcwixe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vsggmrhc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3onfmirod.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3opncikbw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhyaqtoc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gwfzgglb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qogrwshz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mndozavb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3skupouvd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fjokgyuk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3qjayiztt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dpbxaerq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ncvgaupm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xxwzwniq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dbvrzzvw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cszyoijt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ssqkwrzk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tgvmawot.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hywoswkv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3kzryvkfz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qshgworm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zgfzkdrh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ryglbpty.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wbulifpp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mmtvfdhp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ihateoyi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3cfsxayde.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ybqdsqmj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cwrcryko.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3aklmkaom.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aedxbyxt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iznzmljz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tyifmfrh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ctxtsfcw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bgqxnnsq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kjsxdcuy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3quuwfujl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ptmrxczt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ttkvgkjg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcryniai.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmlntfcf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3brglxvtw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bkxzkepa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jjtulbsl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3kjbvvwiu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gprdliis.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3nzpvmcrm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ciivcuog.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3rbdcomcc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjtgajl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3geexatud.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mjsqfvvo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tojfkmeh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jywdhucp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yywlgbtp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3kxwsmuil.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ocebtkvl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hixjyzpr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3myvjofgz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qgzjknnt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uxhgxnxw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eygdxejn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bbmrcqxd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nojldxma.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mohbvtjb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3owakrzsi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdjzupfm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3imfbunrb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nucanqpe.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3difrcpjy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rmqlguha.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3puhteubc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kuvbdzmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvplkpzf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xomcnipa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pesrbwqy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3shdetqbg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yytkzjbh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdqwowof.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fjpdkfeu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3foztmtxv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3deopgazt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rlujeylq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3psmxryiy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3exhhaamh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbkredcp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jwqitvvy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvujnplz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fbmxtijx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fhzauugk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3sshujdnt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnhwwfjl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wdgfysfi.html


<!-- 参考信息 -->