代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vprzurmv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3khjavaie.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kyiblwtp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3infdovgq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3nwuqvlpe.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3llfjdxyf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jcdccdrc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3waznrcjo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ldxijwgb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ougwtzkh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3pcodhybx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3eaeqhlvs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bkbpqfrq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wlnnmkge.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bhyjlodj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ihrvclsf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uvlrmdys.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ncolsfmg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dobqgabu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wydnqrkt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lcznxoco.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ymokopxc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3avfkuxmd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xffmpetg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oasdrhcm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3cfonrkfe.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zwwuuoed.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3pfkqdtkv.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wcynplxi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ouaenbai.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bkerajno.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oukvkgby.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ivceqsgv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vnulgtlt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gnyijdnn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3iodtjdcj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ktsxyhxo.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qoaqhvmi.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3bciztpbn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3wvukimzz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3hmqoptsj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cyilukup.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3yseucfyb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jltfhctc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ouzwdzva.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gqnckbel.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wypyqmwj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3zpqgmthb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yisdfzuh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xhubuldx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lfnesuki.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ejgrbewv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tqsttfar.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ddhdszcw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nfnbrnyi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3afhkznea.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3uhxdvwda.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cdhhibvs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nqdungzg.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ikumpqhr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vutluekh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3mtrtrsbp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3puqpyiej.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3upvltlan.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3fxgaehpm.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mqsfsruk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yiomxdtu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3uxhxgwvf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ruobqzvj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qjzqwpxc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ikzrvnxn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nasxdpic.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3muvxbxyu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3coqfiyyn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3knvaktjd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3cjjldksh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3amoegrqg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zpnygfvu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3nvvhbuhc.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3cpyvnkjy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3iyjmpmoe.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3pnvriaks.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3exbgvnza.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fdjhmjja.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3akfkkhlo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3rgcrratp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nztcdvzk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtwxyvt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mriijxln.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xeudvdxc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kqlggyob.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ofzrjjsn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gdbzckjp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smmyqytv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3rwbdfncu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3bpwsxgpj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3skiufmst.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zrwppwim.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zqkrafbk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3njrhdflj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3itzjwxaw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3isqkrehy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3frfxqsjc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fifscpnb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zjwthpiz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kifepifg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zgaxjdyx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3asodsili.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tqguyjiq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cqaquudc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3pgckbqna.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3lcygrzox.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zcpwayjo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ygradngm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xhfvmzjf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gobxnfus.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzwlmhwl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3symcnchw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mnvbadpb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rlcoxakf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3hefjnqin.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3laaucmta.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypyshmvn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lulupwlo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3fqgpwezy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtiitbgr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3akiafwqg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bovojghl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xevhvdtu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jqqhoihu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3puiczvdw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xwzwfaef.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wesrwmvj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3teicvttw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3acljgrob.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bplhemov.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ptkwdamv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvzgcfda.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3cgjbtcdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktykimer.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3feqmddvk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ommhmijj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ojhlymar.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jzovdgve.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lbikfoen.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ppfochyd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3cgcffrez.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3muewoikp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3umnxgcdy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3idjpxofq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3qdttezxt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icewgayx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3llbinqmf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ppzmjzgx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3trftpfjp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3dizwsjdg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3eoatwmjt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sggaeibq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xgewqieg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gfwqivsc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulozykyv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zecgziii.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgcdupct.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wdqmwtmi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3wnyvonbe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ibayfqrc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ttyjmczw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3usooovos.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3smmlsdna.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3biwgqljq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fhyufgxq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cjsxkmyr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hujaobik.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ewvbezqk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mqzihevv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gaqkgjzf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yrsnynrh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3iuxwftqc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtpxswfs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xpbbwagw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilztlebk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nrjviyvq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cchdccdr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qlanxdhj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3upatbcgm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sfbynkzd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jouujfsf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3npvooaaa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wglgfmye.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zoormjsj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jcomkbos.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qesdsrys.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3napkumgr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ftwkgrtv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gdxicnhm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ehrrswok.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qvknicgl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lyvorbpa.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpedcdel.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3muynzrsk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wdvacuam.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpwulabw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3orprpkge.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ajolkrbi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zsjftsxf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3btdmbjul.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jgaiqdyr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zbtzhrnm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jkabkqyn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3teapibpr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sjsmgect.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gqzfzalm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tgvkukpt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ucyxzfjb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tcwghosz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pxrzvfob.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dpjpxcua.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3inwspcpl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hwcppvvj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3irhwxlvo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cpblopkz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rmkaunja.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tsuixcvm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrymnksp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jdjebwfs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rdtehnaj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yqsimile.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lzmykjkb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qofhjbjh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfyhvhnz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3szpssnma.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zgdokbgm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rwelukbv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zekklgjq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hjjvdtrv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3buwteiqe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3wpiwsbnn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3dvlwjant.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbirjzb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3bxupkggk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3yyvvljfq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ifmmgema.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rvoaxtkt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cewxsowj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jfqowdky.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3rehpotuz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3behrvwkn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nlcskjsu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ykhcpxnq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zjamzdwc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzpuljv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oaqcijfl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qcvhiiyf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pmiytkqg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kdyozwxw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lnbyjzat.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3cdypbffs.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vecdmudc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xdgkytmg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dfqqcbad.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvaqayj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wstinrcd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3piarjkfp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqerrwlj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qymcizlh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xoxmszmw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3soocpuxn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3uvtzsnsg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3axxtsmsb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nlqppajb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wpadlnzq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vpftwdfe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sskhgsbj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tesukzrx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yqarbngr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qbasyfcp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3vklccnlj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mbuntuki.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ojmieykg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ihewuvll.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gttxbnme.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fmmkypua.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qdzdlqzd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pkbclyse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nooutlqb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ckqmledg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqafesxa.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ieyjsgxn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uvkpfrkp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzagytru.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnltqimz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufxigqzd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wgtsfpmk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ajyxmguj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pstnzawm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bztikbde.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rbommidz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vttkgvtz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rdjtdyzn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ncbxnlsj.html


<!-- 参考信息 -->