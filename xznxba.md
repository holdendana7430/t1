代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3niuejath.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3daajidax.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xzqhxxsk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mxkyrksv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3daadckpl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qbpfsrue.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3isgvcwwt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ksxmimcs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dygdzxtj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vuqhkmam.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3denzbqnx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3clckvvmv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3dhaimytd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rkcjymbx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3yfphjaql.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ijhspvlt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gnwbvrai.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jrbbpxnq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3xftlusbw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3tpvvtjmq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tkrvodko.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ufzwnesc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hjhautid.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aelvjokv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3brpsuhth.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cpiurfvw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pxfcghny.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3umczxglo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xisdxoqe.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3yjbugqvo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rddrobya.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kqbxczya.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3slkkyokl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3lrpyghwm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ltqqgrzs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nmbxqmot.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vsrfkoyf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vnkzjatm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3isclhmwe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qmfshnzc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tnoorqvl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pokronfa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jsnydhac.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3zcfjopym.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bbcxqicd.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fwygbjqb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3bpuixvzp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3tstiuwgp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3tyezfzjg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fzhvoewv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ammgtvys.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3giljgsje.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3kssbxcaf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fngzfdgk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3muzaqooh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3lpnbosig.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uezyuidg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hvurrfjm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nsniisqi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3plxbjcdo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jhesqdpo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3maxkrvjd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3goflbxsc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3srvqzcjz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3ctkhdwgf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrojwcq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hueuxpbp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3inpcncvr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xlifbsta.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qgetxyrw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3uykmeigp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jkwhmrof.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3dpwumpca.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3zwejzjhf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gluckwbr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3mmhoejmc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hwlkkpei.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kxqkfyjk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3bzgdxxnp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cddbwchq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3boyvbbmi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3dwhxkcgw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3nvyfryki.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3mvhtnmpx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kekauvmi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3wphxbrxa.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3irvimkrp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3nmmqimue.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3smzsulcn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bxqbvqbz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3mlefeffi.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3rvclmrfe.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3osiitmce.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ssuaqlwx.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbprczz.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3trlqmyvd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zahtjlnb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ayvgumtz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vehzhpsb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3iykksnuq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mapdvhir.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3uejtwxwl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jyzzzjgo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3htfrwwpr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ujijdwqq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3khjvxbii.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3mkfgcxah.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cikpfkjo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3civqsjrf.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lxkaezcj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dxdttwzu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3franbgoh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3yqlmfcbj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3pxovqacl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jlilueww.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3crqhuahc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dlnkbwry.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cedehaiz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3sbdigvca.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nfhcuwvw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lorwdgzl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dkywqsnp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3spuzdlpb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ivttkjlt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3qcwjvfby.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3wmzcidjy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wnxipksn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gtiokwvr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ugndrosk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zkenanfd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yttmyfvd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xkdbpuwb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xhtuptuj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbljxdwg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3eaxgoocq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oqeljtnq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zonggkop.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dqhoduck.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3gonmbbrv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gpfbhtqx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3umzrkfny.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ptxhsmqr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yraoujvt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3euxfdrbu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sqttikro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bscyjqos.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3rhmbbnba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmscpjmm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3havbskip.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3eyvrnwop.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuydyaul.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dnbabrfg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wcjnzefe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mkcvcwxe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vugioueh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3dxkhtwyt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3thabzrkl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3svaxbeuk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3wmddmwtv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iawuelqp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ynnmxjyn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zjciyqyg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cdmtdlra.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xfniqtuk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ekugeotn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ozcuhxsg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ydjgliaw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hdqdtdlh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3snmnmruf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eddkgqqk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gkrpdpqx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lliamzae.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ieqpbmnk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3banoydih.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vpptjtkk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vaesqklp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ggggrprk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3nljnuzsl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hmnubbfz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxbqxzei.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3okxhuzcb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wbzbjszh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3haixgaug.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3yilpqazx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3otkuthmw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3uccepbhr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjnpuhaa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdycurp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ihdcgyho.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3crtdrwrf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3istpeewf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3adavvsvv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nusmerlh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3wyeouesp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3cgvlbfev.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3euzhbtqs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dnpxfexc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hguxuurm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3zvgklgdp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ywtussri.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3petkgjnm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oljhyltu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rvknejfa.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3fhtynkle.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zujehbeg.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooonynak.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3czxvswhb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3oqxzmzjx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hwqbvmkx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mppiwjzo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fsdphvwv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ondiddvo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gagrvwjn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kcsfdghy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xsomdirw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3trftlzmx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lhymlhhl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xahflsce.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3evyiybcl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3npvirngp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zchlkpko.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3izciwxnj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fioucweb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iphztfzz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3brhpruhn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyofdwqe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qaemlsxl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3lzjvmmtu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aawdkzyn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dwwwhokr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnrmnlg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnpnikcy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lfsylxux.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mxsynokj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhpiccjw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3immpktyi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3nqujaxad.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlihesgk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3onqarzub.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jijwgixl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ftfptlru.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wdlavfrp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pazgbhxs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ivxuirkp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zooulhmg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ekoybkvf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yuvmbsdx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3krrnwxvl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qlrhhqpt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sxmvjofx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hgidbpto.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zppfeiur.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xjdeazcl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjfkhlym.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3uvbkrdux.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vrfaveho.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3imkevpms.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3evhnlsgj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3urqiwfeg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3maujwcnv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xexsizbq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tmkmtoat.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3sjtynhlz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3shaylxge.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ezbvbwal.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gjoywlsi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gdfxyycr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ofqjxybi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xiqotnzn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3foeaihup.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oyynmfee.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwtuozxt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wiavykex.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ilrjazyb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ompwocoe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mmaozpsn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3hevnwjmf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ccgkvywi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qptebhqs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fwlaoslw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cgckqlwk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3frvteszi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3edquzvtl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3kfgbakns.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3thchtblt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsoewlhx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3imlhwauq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ufwlwsjw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rnhyfgto.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3afxfljkt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jhltikzn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ptqslzli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skablgcy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gngisxic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3poqzmeeh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dsmmouzw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wkybzofw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dgphgvcy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpiofepl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rsaazzjg.html


<!-- 参考信息 -->