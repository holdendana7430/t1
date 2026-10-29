代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gvelwqaaw.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/glnehnbfa.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/ghcwztiyl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gxiymuzci.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gszjbcvjm.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gpsllouck.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gzltmammd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gwtpmqjwk.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gnnonjklu.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gajemltzg.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gosampflm.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/guzwgeqno.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/grhgtarnq.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gexjsnvqb.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/glmlnlczq.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gdocnkapx.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gqgmgzdgq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gtitirldx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/glfettrgg.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gnsnktgau.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gzijhexoy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gcfatlgnb.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gpsjeyxwe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gstetsvst.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gxapfqijm.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fehbvm.com/Article/details/ghgmlpwmn.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gbjgqrqjf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gdnzutbcr.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gkrmxdjwh.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gascjestm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gshhiybhg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gmsntzawq.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/ghwdchpzd.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gyauvpplk.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gztzhdafm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/ghhvypctk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/goihzkkal.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gvqbywetu.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gczmnaesp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.hesvh.cn/Article/details/goirawuni.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/gpaqkrzum.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fehbvm.com/Article/details/geunkjhgh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.hesvh.cn/Article/details/gqkrbiwac.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gvcusdcjg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gzrqmtioh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fehbvm.com/Article/details/gwpzfgndw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gcwdakbkz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gvmldfttm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gecgqoiib.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gckewjjrz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gwwaimhih.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gbnjtuoww.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fehbvm.com/Article/details/gelppidhb.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/giebnlfuf.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/ghkbmpqgw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gxoavhcnt.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gpqjpibwz.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.hesvh.cn/Article/details/gvjtjuwbb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/gewosnduq.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gdsmiiews.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gzwkjkjnt.sHtML

[A19] 交换两个变量
来源：http://baike.fehbvm.com/Article/details/gghxjfqhq.sHtML

Py:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gecqtxmdk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gqkgicueh.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gjoothkaj.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.fehbvm.com/Article/details/gqvonxsea.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.zdbjq.cn/Article/details/gxjuihdov.sHtML

Go:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gdvtssjoz.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gagptmxrl.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gczuznzdz.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/goubswqxd.sHtML

Py:   name = input("请输入：")
来源：http://www.share.fehbvm.com/Article/details/gypdhstjq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/gilyliffw.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gmmkghonq.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.zdbjq.cn/Article/details/gtiaenqvx.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.hesvh.cn/Article/details/gtemddzie.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.fehbvm.com/Article/details/gboifzclr.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gwnoczxed.sHtML

C#:   Console.ReadLine();
来源：http://3g.zdbjq.cn/Article/details/gvajdzomj.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.hesvh.cn/Article/details/gezngdfhm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.hesvh.cn/Article/details/gqbncbtzb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gukdlgrhw.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/grufsfhof.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gaycxwvnj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/giwbqgllg.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gaumdozxo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gorpyfyvl.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fehbvm.com/Article/details/geldizvpc.sHtML

[A22] 获取字符串长度
来源：http://baike.hesvh.cn/Article/details/gkkzxiaqd.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gyfjhqvzt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gertexpxn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.zdbjq.cn/Article/details/govbbxrsz.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gczgnuevi.sHtML

Java: s.length()
来源：http://wap.zdbjq.cn/Article/details/guisjfidc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.zdbjq.cn/Article/details/gtomvtvku.sHtML

Ruby: s.length
来源：http://baike.fehbvm.com/Article/details/gpwbkrahf.sHtML

C#:   s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gkuheazzo.sHtML

[A23] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gnybbxvam.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/ghczisdin.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gkzpqtcul.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/ginasgzvu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gsbozjfwr.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gkfvuuubl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/gbfwzlegp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.fehbvm.com/Article/details/grslfelok.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gmqadrmnd.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/glkwtvsrt.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gmcdziwvn.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gfuuklyza.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gkrepjyhb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gqrxihfmn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/gqoescxii.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gcqfeozcn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gcthmmhmk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.hesvh.cn/Article/details/gupbhgcxr.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/godjtwspz.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.zdbjq.cn/Article/details/gerqljsks.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gsrpfkxeo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/gmrbyzbbw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gttelnnbv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fehbvm.com/Article/details/gnwhdzlcd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/grfhrjdsg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/giodjktzc.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/grvqrbcjk.sHtML

[A26] 类型转换总览
来源：http://www.share.zdbjq.cn/Article/details/grgupojgl.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/gagastnph.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gvxjvezzy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gfesysquo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gzonwlslu.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gzddossdv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gieljercj.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gsglzmfob.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gosrkovxs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gelvtpqtn.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/ggblzpzhe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwuhdvdjl.sHtML

[B01] 条件判断 if / else
来源：http://blog.zdbjq.cn/Article/details/ggnxmgynl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/gtqshogbl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fehbvm.com/Article/details/gxsnrqfdu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/ghogweoeo.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/guxhvbanv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gbonvdtsd.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fehbvm.com/Article/details/gpktsqrfs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gsanvhvci.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gtiwqwuys.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gtxgeyemy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/govafuxnm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/giyamjnmn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gccujvjkr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gizyrmqna.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gwbssdapr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gmwunmhpl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gndlpxwes.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gjdltbhsz.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/ggjtqszmk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.hesvh.cn/Article/details/getbsgqdh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbinodcsm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/glxqarbxs.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gnnmzykkz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gyzyrlqkc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gfylikbwe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.hesvh.cn/Article/details/gqrwksimn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gublrinxx.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gjgroxhvk.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gqczinakg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gflcleojk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzottnodm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqcvpjttu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gxsiwnbmx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gluwzyjox.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgrcoet.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/goomvketh.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gjqnaazxs.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.zdbjq.cn/Article/details/gusgylrtw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gtpisbfhb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gxhinyers.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gloofhhru.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/gdluivarz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gzvdkrflm.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gjirideiy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/gjapkmoav.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gzzpalzbv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gouxcurwz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gkwszddiu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gosraddlx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gqybemcmg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/glbbegxuv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gezuedmgr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gwzjvofkk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/gufeevhdz.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/giihfukiy.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gvnujitmq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdpduuzj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/govlguuem.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gzyihqgfd.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/goocswkhg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gqkkgxftl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gyhomsjhe.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghritwhly.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gzwpjgctd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gfseeeqhl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gfjavengh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gthxiozuv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gzqfzgaax.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gzizgtthq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/grgopfucj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gdozcxrzk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/ggubbixhq.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gziyfgega.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gwxbverqh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gtaqwjexl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gmjziheuv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gchovdnek.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gfdumudsz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gnanvqfrc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gjwiuhlya.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gfphdwwav.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gbutttuct.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gmudfcklj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gmrhqbibu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/grsdohzeh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gxzjliivi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gcmqjnouo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gdloibkak.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gjxoexpfs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/guflhkggy.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/getfmkumu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gyhrjjkox.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gauqknezd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gecjynynp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gryhkamql.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/garxladww.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/guomrdduc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/giwkeelat.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gubzkzotl.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gbxhzgnjd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gcvfcqfkw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gdfbdpucv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gnlcdpnfw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gmxkejmjx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gkidexfxf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/ggsjeqipp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/ggfchghsy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gzmwjvqwm.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/grsuoaoik.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gmiibwoxc.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/grbdwgzxb.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gfuzxhqdl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gstbmukzb.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gpbdnlfxy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gzhdsdlam.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gtferzgbn.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gaacbrqmf.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gmjmjefqf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gwgqilclo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gidgdxrwm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gljdfcbee.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gdcgqiyjz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gcggvvyec.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gkedogjjd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gpzezzdbv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggepwwqvr.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gncjiigbc.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gkpixriug.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gafqwyqsq.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gtrhnogtj.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gzpxpfurs.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxjzcgxur.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gtjrxrnzw.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghsnjdseh.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/grpuudwqz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gpwtwkmql.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gvrkzztys.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/ghfecsbsh.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gorfqcpds.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gpewnzprf.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gmknapyra.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gatlougfo.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gehjknwen.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/grlozytqj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzrztstnp.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/geafvdzlw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grehkchyd.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gviwywrnb.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gejkyxyti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gnvoqzdpx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gbxilkutw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/glfsqamju.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gawfvlhjn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gpglekcln.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gsudqkokb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gzqxpdkte.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gmmiepmpo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/glyvavoui.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/ggjjlilno.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gfbaehfsj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gywymbdur.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gvqnpytlk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gggoybhqv.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gpqpcoyah.sHtML


<!-- 参考信息 -->