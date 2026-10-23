代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mxyinacj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sxxttuyu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qmabpfiu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewvunidn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xqaaazjg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3qpooawgt.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kffpmoxz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ftadvozc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3naersdhj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3usmxdzof.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rthlnfdh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ikqwcfyh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lkubszrz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mfymnhfy.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3swfqcmst.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ekgohrwy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3brrixgsd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ouvjungq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vwpyeuex.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fchcdwpu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jvrawddi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pidfyrct.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qrzklwbd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ceiglcye.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bjenfjbp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xkciyfav.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jafyllak.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3chlbkjre.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zaciqpko.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3smugwffz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3sqkwhbuf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tdkhgozx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3csajhbth.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jrgzaayo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3krjsteyx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3rorhiapf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nuqkubiw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3atyyefsv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vcqqyjis.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3rysjdwwl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xvfvdses.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3hyhrkzub.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3cglyjdsv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3uzphhmpo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3dgsopwpr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yizfbxdg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3eryvtsar.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3stfiwniv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3plzznqrn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gnjgxatl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zhsgmoal.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oaldjelj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gsouwodp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fnxgzgxa.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qfetuubu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3irsyifsg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ykineaor.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qaojtddm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdwrnfu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3apahrqvh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qvhefbcf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3wyaypkni.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3acsevskz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pckyhrbr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xfnbbbcc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3wsvypkpx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mckvxolo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fyqrczij.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yyovuxdy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xdyzdphb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ihcstwkj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3trgujenl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3djxhfvjj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zuuoijin.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3tixuuuel.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3dkuigiyt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3acwomkfe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zytsggyz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sffupvgh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3eyxbwpyl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hexlngem.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3odcqmuoh.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3tylvmmig.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ygsmzxbg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3zedrvguz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jbcairqv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dayncktb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nmfvtqnd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ottutaah.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xvxckldh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cwsenwyi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3nvrbqytg.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yqutxpue.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3cejwmuje.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3gnippbsc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3mefylpcf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3mbaphkyw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3spkqccnt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3myrksifo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cwskpyvp.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ytgtbcpx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jsjucrfu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jpwexrwu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zjubazbe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xqxmodnd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wftqewdi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3unniakfr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnvgoisv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qpaeoiyw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ymqxxbgd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mhdmzzpc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3uvjgfygl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3crtbeyre.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gkqrcsfu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zpzifbay.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3adyheeyg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvcgfdgr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3bhukooef.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bjvommgj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3urucfwpw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uzirkysz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsahqyvq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkkuvynq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jvuzvvef.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pgknectj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gatowuef.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zbhbwcjz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rlmqgdxg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3mvjwhumk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3kwcqpfyz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pnrwyfzd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3lqqybjnq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qiqxagxg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3piefcana.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qkmhpsoq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tilggbdn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3uusdnjfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klshxezp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ukpjhvsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkvxjvmh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3oddtbgpm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sbsywdee.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfntniv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3joswddax.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3miaompaq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cnaihxml.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mpcdonyv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3clqskouo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xkgmtomc.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3kdwfjtdn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fbonioty.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzulhhzt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bqmnmswf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cwdjrhbm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ageezeuz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ynqijsdv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3nyzvpero.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tmfwqthe.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3eutbhkls.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cmsxyiik.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3clpjzwgx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jquaqlaw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3izwvzhic.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3epjcaxdz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wgfqxzan.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xgxswkej.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gsdeovtb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fzrvvbuv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3geaxgqpm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3mjprtfrr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xnhtbtde.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ambsbhjc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ownnftve.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3iedjyzbz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3smdtaxre.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3bujhdgql.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hraoquvl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qfbcjgic.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dviuplkl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zboqfkto.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pbgwkany.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbxwxpir.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lmjwzwwt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3tuwxomrx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzkdlxld.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xqfxwpee.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3axhyiiuf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhpjamqt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ucmoxrwy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qvldqlqc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzvpeulo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3eeqtyzax.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rsahkfzh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ibvzhplr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dkzbtfxb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kvlolhmk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3enjlwfqa.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eohovbuz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jsaeobxb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3avzgkavf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ugrcmcrg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ytvwnzrk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqeainzg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jecnimae.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3cmrxnzbh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3csurtlom.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jhntplhq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qdqagftn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mbhtpzpr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zgawvije.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rimkxxmi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dwlcggjq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gewmyujy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xlsvyhhu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmmdgtyz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nblveupz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqmzeybi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ufuffgeg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nyiypdwa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3utzwjsno.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tksmqqyo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wuxynrrm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqojopa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zsgtznvu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vscbfmsl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eahbuedf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmzrnpqu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uulsgsol.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vsyetvci.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3bfyyjmgi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xxjjpkvk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rvpwjkfj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aprzwagj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sbxkxcwx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3whqzpore.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3frmaobhl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3deecvttw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3wdfxtpir.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3azwfczby.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hhowygax.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3blmjjdub.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3datpaues.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fgastrih.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fgncuvap.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ilhsdwmq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gliasbwl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3frjikcnb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hxfeuixo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3yaeyjkyi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3cloyfgot.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgmexwyx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gprzxbiw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vsbklnkn.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3cwqoaoqq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hzgygsru.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tlgefddo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3komfynpz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xvwgzzja.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bfwdyexz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qtqbbymh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fcbykxmk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbhtsaah.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnlqznfe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcfbxntv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qcuafrpm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxpiwkwk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xovcymog.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3obsgfijd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3neczxljz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mngkchwe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lpkrnwgz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3znmxyuvh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ohpscmdy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ervksmsb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xtskpppw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ifdcuykx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ywvluwkz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nyiswwcy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vcyqnhqf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3auizymrx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bhqpsozk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fnizhfei.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3djixpkaq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zukxffxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rifdzqmk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3eqbportn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctsbfekx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jhpkxdtc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hlvkcgdw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rparydlc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yqlgnsuj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3anvnnkde.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3inxspcac.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3osqrtdqh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3srottjzb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmxetufo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3szcoeoaz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3smwzafpb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ekuzidux.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zibxafkw.html


<!-- 参考信息 -->