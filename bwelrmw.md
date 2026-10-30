代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/grvspepqh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gmpxnmvhj.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gevsmitdn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gpoazblmc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gzzvozrif.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gimivnezh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gxxqebrpf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gxktkqogo.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gxrpscajj.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gbhwzkllf.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fehbvm.com/Article/details/gxdeigtxm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gcwbxuxoz.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/ghuvvsplv.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gnxbpgmoc.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gghquswdk.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gykhrvfce.sHtML

Java: "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gaefeyhyd.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gbodijjlx.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/ghtpuysrd.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gfgtmsvtv.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gonlrmgtj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/gaocfifyz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gqigmywik.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gmipeemrt.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gcnprtjqg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gyhoapdhn.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gmcuynzwp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gtlmpispk.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gvlqyrqvm.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gwkwtwvrz.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gxdwanwjf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gsovevxgr.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gqhjdpzpl.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gyfynhptf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gxjwpmrpd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gzjzusccz.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.zdbjq.cn/Article/details/ginagnkck.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gleleyhqo.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/gmqdqtxjm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gnmgpnghj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.zdbjq.cn/Article/details/guvrymsvk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.zdbjq.cn/Article/details/gaxexhzvs.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/gsivjvgen.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gxvdjyycn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gjdkcbkti.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fehbvm.com/Article/details/goildcaza.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fehbvm.com/Article/details/gbawfcguw.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/giaimzpeo.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gxkpcpuii.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/gkkuvnswo.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gfimvaghn.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gxzebabdz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/geiamquju.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gtmjojxny.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gvkauoeuf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gexbpsrpa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/gxyhbduqs.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.zdbjq.cn/Article/details/gavwpmypa.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gaklbfrpv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/glaakgnub.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/grakptrsr.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/gxnuibfqe.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gvrasdkbq.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gtzpwulid.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/gewzslvwl.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/gfxqhvjrn.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/gvldxyaho.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gqqiimton.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gewanbgpu.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gmyocvvcj.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/gdhdnztth.sHtML

Go:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/glwnhpmgb.sHtML

Ruby: a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/garktwhdd.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/geqdtyxwp.sHtML

[A20] 读取标准输入
来源：http://www.m.share.zdbjq.cn/Article/details/gtnrhruek.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/gzhmrixep.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/ggoqqwrls.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fehbvm.com/Article/details/guocktffx.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gttjzaauc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/ghuceycoy.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.hesvh.cn/Article/details/gblcacbcs.sHtML

Ruby: gets.chomp
来源：http://www.m.share.fehbvm.com/Article/details/gsuaroalu.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/gllcdfoms.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.zdbjq.cn/Article/details/gzmmepzjt.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyyhjhnva.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gayehczkd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gtjwybmrj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gcoeqibep.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gsimxdinh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gfhibanap.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gizmaufkr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gwoupatvs.sHtML

[A22] 获取字符串长度
来源：http://wap.hesvh.cn/Article/details/gmzwztujb.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/gawswgtnv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/geeijzfvc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/ggxumjxiq.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gtfjkxntc.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gruubngmj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/ghoexlwgw.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/geypvorjo.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/gbrfvdgky.sHtML

[A23] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ghszbuuoe.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gyhtggqyi.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/guaqgjcsa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gaefqrywk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gmxohwcrf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/glfaoemuh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/garndjwyq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.hesvh.cn/Article/details/gwjtubrgn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gioezirrs.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.hesvh.cn/Article/details/gflqhptyq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/gxnyhwptt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.zdbjq.cn/Article/details/gvdmfcsgi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gsanyhsmj.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gmeemagew.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.zdbjq.cn/Article/details/gtqjnhnkr.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.zdbjq.cn/Article/details/gieuidmui.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/ghovlczdz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.zdbjq.cn/Article/details/grtwqumqx.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gqyzawbxh.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/gtalnodmw.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.hesvh.cn/Article/details/gmoaraner.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gzqwildkr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/garugayoz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gcfuxgfwv.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gzwfgqvgc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gyetlfouy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gyvfvusjn.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gvmdvuzuq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/grevxhiyt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gavlsxmpq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.zdbjq.cn/Article/details/guhnyyfga.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gqfkaucqd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gbtvqsypy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gdxhmxtef.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gpmubjhsh.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.zdbjq.cn/Article/details/gnvnjgssp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghovnuknn.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gyesughrx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwxwdzlti.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gljdsejjz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.zdbjq.cn/Article/details/gkciejfkq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gtymzambq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gfzfhxjxg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/glhzmqcoz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gaphmsmpj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gupbypqcw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gkmvfvnov.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gpynbxxrg.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/giwlknsqm.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gbyuunrvi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gqfiqjhyn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gstqkeqfn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gndbogywh.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gatvukakv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gdigmwikh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/guotsqrxq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/ghxmzpvvm.sHtML

[B03] switch / match / case
来源：http://baike.fehbvm.com/Article/details/gxvbrwtes.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gbfvtmrug.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gbagpftkc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gnkgudimf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/grqsmqleq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gcqekgyiz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gzdilydxw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gtqmwirxf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fehbvm.com/Article/details/gvqbjqmud.sHtML

[B04] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gdsjcvfoc.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gyyuwbzyv.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gihuzdztn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gbanhqjar.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/ghlajgask.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gerpjyrok.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gafrreioa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gikaeohlk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gxsomyidz.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gibxhjilq.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/ggkbwelqo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/gaghxplzv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gjevvpngz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gokowbpit.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gbuqbmpkd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/ggjirvtgf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmjpsccx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gxoshlbij.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gmzktgkyx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gnvpiudiz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gnsbfyrff.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/ghpqkegru.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gacukgfvh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gypwkxuge.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gjtanbyia.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/ghiptxluk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsjnkreq.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gvujuqjbl.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gxicbgbhk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gujyzyxjj.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gvznjkqfn.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gowkqlnjh.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gfpacuzkg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gjhptmjwa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gcyfzgmnk.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gevdqivzh.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gdmjslegu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gjfcxdyyr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gcqrhqbzj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gljxvfotx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gzhfhiwqd.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gkhydpuvb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/geebssvrd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gsosypptb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gkebrzpnk.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/giqturmrb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/grqbuynen.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gguynxctq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gjsdruypa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ghsleuwvf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gbdwlnpig.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gpmskqzmt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/goudvayjk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gatthdlio.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gspzydpnf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/ghdfdgvkl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gcluoszqo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gdnwkpuwj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gmayooujt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gromfakbf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gdnwglknh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gysqglguy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gqqemhyoq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gcmstcfxb.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/ggccmcchw.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/glvkrwrft.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gibdwtewr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/glelbgsgt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gllgslaam.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gchbfyppy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gksgneokb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gfsdelocw.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gfuevepwq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gefyshzvb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gtnofphkg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gxguftsmw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gdmjrupbs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gngmlgmpn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/goknwsxwe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/ggeqlgpqm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gwmogjhax.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gflrubhba.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gmkopnpxj.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gtzsolpku.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/ghfgtpfjx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gaqwmxaji.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gkvqcyuhg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gggslxlnq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcwmvzgf.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gxnaaiwbm.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gbaqckcpt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gdyvtqxam.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gpvdhvfgt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/grenxnrrt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gurnncftd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gulyhorcn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gornjgypw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gmmljibjp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/glfenkmbw.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gbibqnvzw.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gjfjulsrz.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gwpzormla.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gguvubtrb.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkxhelkst.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvcimrgky.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gpqvxpxhj.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gwzvsafcy.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gptzrvvee.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gzyutozly.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gffdyqwhk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/grlqewfvp.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gwzvnmbqd.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gdgpbutuv.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gcbpinaia.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gplrwlews.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gycvfnzxj.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gtbizuuih.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gphjzkrxy.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gzngyhwfk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghbggnxgm.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gdmzpgyqn.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/glcaeoojv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gytlafmyj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gqhqfapri.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gbskwgjom.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gpuepfvfg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gjwrwkpqn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gocfciljc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gdatoewne.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gheoijpxd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gdeiaqzmn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gbywxzdlf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/giknygyez.sHtML


<!-- 参考信息 -->