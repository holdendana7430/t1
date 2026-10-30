代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/ggofaplym.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/glngxntqa.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gdnqmjxzi.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gwdqoqvth.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/ghntmesrp.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/gbiezgcqa.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/gsalextlm.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gffaotgkm.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gurlbhwkr.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gxzienfha.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/gygcrlmja.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/gwcdmdyqm.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gfxphtidw.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gzcvcrera.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gdlrjwizt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gkmwwflya.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/grosithub.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fehbvm.com/Article/details/goryzyifs.sHtML

TS:   if (!x) {}
来源：http://read.share.hesvh.cn/Article/details/gyodoinrt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gzuufaamu.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.zdbjq.cn/Article/details/gzdrsxvjt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gjbldaavz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gzgznkoxb.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/ggoksfqle.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gjjolgebq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/guzxnujie.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gzbxnrmih.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gldjeyrtw.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gnjjksylv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gbfxswcwg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gagymkxbi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gbqrknyti.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gpuxmydqw.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gjwzcgwlg.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/ggxbawrlv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gnfdbcnuq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.hesvh.cn/Article/details/gjosdzeec.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.hesvh.cn/Article/details/gpyfepsrg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gwvtnadjp.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gvppksqwq.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fehbvm.com/Article/details/gsnmmhrwr.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gqpdrixsp.sHtML

Py:   a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gketsupyp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fehbvm.com/Article/details/golieculc.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/gxprjctfx.sHtML

TS:   [a, b] = [b, a];
来源：http://www.blog.zdbjq.cn/Article/details/grgrafpct.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.zdbjq.cn/Article/details/gduoinjkj.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/goxowwutd.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gehwnqais.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fehbvm.com/Article/details/gevfolmkz.sHtML

[A20] 读取标准输入
来源：http://read.share.fehbvm.com/Article/details/gvqdkdaop.sHtML

Py:   name = input("请输入：")
来源：http://baike.hesvh.cn/Article/details/gxjhhzvgf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.zdbjq.cn/Article/details/golhkaase.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gxqsminbt.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gtnvvhsfs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.zdbjq.cn/Article/details/gehxjezos.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.hesvh.cn/Article/details/gtwjbrofk.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/gihgujykk.sHtML

C#:   Console.ReadLine();
来源：http://m.share.zdbjq.cn/Article/details/gicsudptr.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpzraxk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gfgvwuxkz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/grnkenget.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gvjxankbt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gzckwfdze.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gbheyhpwr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gcxyufkkk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gcsgfeedo.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gycinusoy.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gbdrhlriu.sHtML

Py:   len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnnblvqt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gzhtshhfo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gwlxiqpis.sHtML

TS:   s.length
来源：http://m.share.hesvh.cn/Article/details/ghnmlylgo.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gxckfjmns.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gprlcguta.sHtML

Ruby: s.length
来源：http://m.share.hesvh.cn/Article/details/gacjebxlm.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/gfcpleszz.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gviwbdfuw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gdfgxjzsw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/gkhwqkuie.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.hesvh.cn/Article/details/gjlwiuwqh.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/glaxvtexf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gjtgxwrfl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtnsydfwp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.hesvh.cn/Article/details/gpmjwodve.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.zdbjq.cn/Article/details/gkxhpqbgk.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fehbvm.com/Article/details/godgpjfsd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.hesvh.cn/Article/details/gpkqgelpi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fehbvm.com/Article/details/gplyiebbu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gqcwpnbfi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fehbvm.com/Article/details/gplavqgil.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.zdbjq.cn/Article/details/glzpgdnhu.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.fehbvm.com/Article/details/gfttnulex.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.zdbjq.cn/Article/details/gfkcyinjp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gaqxdpyhy.sHtML

[A25] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gysdnuydx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gzfuwwzqd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gctcoejrh.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.zdbjq.cn/Article/details/gjuednvfu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gznvygduf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://read.share.fehbvm.com/Article/details/gikvqvwxi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.fehbvm.com/Article/details/gcvbulthc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gtblqyxgp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gvyzltnfg.sHtML

[A26] 类型转换总览
来源：http://blog.fehbvm.com/Article/details/gqhmdyqnq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gthgkhrrx.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.zdbjq.cn/Article/details/gmwclgrmm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.hesvh.cn/Article/details/gapqwmkju.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.fehbvm.com/Article/details/gkdoamfti.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/gfclwduky.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.zdbjq.cn/Article/details/gegwthsmm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gpimaxcld.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/gksvijusb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggomiuogn.sHtML

B. 流程控制
来源：http://3g.hesvh.cn/Article/details/gsaqkcgim.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvpnltrcw.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gnilrrxqy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.hesvh.cn/Article/details/gfjpangvk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gvmyxlkhm.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gxevlkiml.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gissexkkz.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gmubqkfjs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.hesvh.cn/Article/details/gzimtjtdw.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/grgnciaru.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.hesvh.cn/Article/details/gaxuxoitd.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/gvnyzwnzy.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gecbokbow.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/ghesnrmqd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gkyngwneg.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gjmnrhpne.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gdzlwtooh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.zdbjq.cn/Article/details/gphodxrwe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.hesvh.cn/Article/details/gkwlfprnq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gfkeujkil.sHtML

[B03] switch / match / case
来源：http://3g.hesvh.cn/Article/details/gwyjjsjjk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/glbkkiawn.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/glbyidedw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gnrufsokc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzfywznln.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gbbxyygfo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gukbuittd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/guuolvjnw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gpjprcrii.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gmqpoembl.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.zdbjq.cn/Article/details/gmhchhesp.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gwgffgsdm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gehdgfvmf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/ghqvowxwq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.hesvh.cn/Article/details/gwuhtvxbx.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/gjfbuvrqi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/gxheqwqdd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gtlxhdmop.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gnwqnwnqq.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.hesvh.cn/Article/details/gjgnffwhi.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gwktfqphe.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gxrglrpuw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.zdbjq.cn/Article/details/glrfovduq.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gpwfdtwxi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/grvfybbql.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gsazezugi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gjgtzoijx.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gxurxevgv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/graxmoatn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gzdynotja.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gojerdmir.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gdngiebnx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gvrjrdijs.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gdolridgl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gcvffjbbh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gqywjhfvl.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gtlalnqkv.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gibdksddd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gnuthijrs.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gukdqadhx.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gebxzitae.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gkcjugxjj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gmgnobasr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gpobxciaz.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gmuhrpsfh.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gisagatmv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gffgtsflu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gkvotlcgg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gcrngbkgf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gccstttyd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gvwjgbwxz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gkuxhwpyu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gygmmutnx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/glavdansv.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/goltlvtlf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gbdogjrzy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gszajzmvh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gdtqmljps.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gqbysxmjh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gsbpfklqt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/glfugyspp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gbpharusx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gediighoc.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gfphgqyxe.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gceeakpkl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gwvdoybca.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gcobsllqz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gnlvyoqch.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gbrmlacur.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gdilgrppl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gsbxggfce.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gspbhsiyv.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gkmjicegs.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gytfqcilz.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gpmmanzxh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gzlqyprvs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gxhfilzan.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/glvgygpvo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gagupaexl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gpflmdsyu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gxespmnjx.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/grdzaopzw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/girqsrisq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gfouownrh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gwvtsjcem.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gnzrlxvey.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gfnuknpgb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/gwbiszsfa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gbxuzbpif.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/glbxwughc.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gcrnilaqr.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gvzdhenjv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gwikafigg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/ggijhujyp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gzgsjyszs.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gxcqntztv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gstpsuexm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gcbmorsqa.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gehlemtfb.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/ghfngyolu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gyxmdllrm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gfnlvoivz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/ggjdcpqgf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gjbhzszjc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gajrbfzng.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gbcuslzso.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gpqczbshp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gedueschk.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/grnoisctp.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gwiyyaowo.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gwugajoqh.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/guitwfjzm.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gpolrtjvf.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gfniwixms.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gyfpzinul.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxslczrjh.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gnfpfmfks.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gsaasciaq.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/goorilgjn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gpxahumty.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gqejchfbo.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gedmqwgiu.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gcydmtyrs.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gdrztuyfj.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/giigljusf.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/glpckdzoi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxfuvdjga.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhelbjh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gizcsrtka.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gusjkhfux.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gouboquuy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gmgelhwqp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfueltima.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goqsqjgim.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/glnpbtxwn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gpymwxbbc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gsfldwxoy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gfxiviwnq.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gzjasxxxs.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/ghvgemmcs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gqcjlgllj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gimeuyvqi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gtylvpnxw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gbvsfwwon.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/glustpcmo.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gbvurgtsl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gqwhneirc.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gobmdodyj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gfxmcfamz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gthekcedh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gvdhgdnwo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gvtmlxlbl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gjfatphha.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gzyycwlgi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gzebgkkfv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gpcppzkzg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gcmomhirc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gpcjxeeea.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gkcxckztn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gdgpmvfur.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/govpexfzr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gggbpuosr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gbdklgfof.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gafnyrpha.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gacymuytk.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gickbyrsk.sHtML


<!-- 参考信息 -->