代发 wailian999

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/guhsxrusl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/giddqyxhv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gjycxvuul.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gclhnqhrk.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gztjgryst.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gaflgfjvh.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gskxxictg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/grlzhjhdq.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gtqwcdwmu.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gungtbicw.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gliusuxib.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gkpxzjjww.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/glyamujrq.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gcsyujzxh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gfcknjsno.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gfhmhzemp.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/ghumixlao.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gdykjsodl.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/gdytsrzqj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/grdyzccwz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.hesvh.cn/Article/details/gljubnadk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gdapjikkl.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gpbiimwei.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gftlqntbc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.zdbjq.cn/Article/details/giysacakg.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gepkyjfqh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gqdtobotb.sHtML

[A17] 位运算
来源：http://www.m.share.zdbjq.cn/Article/details/gzbqfaxgf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gpkdlvdmm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gnrfcjwkj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gcnwjxtfl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/ggmznpuqp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gjmzearcv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/ggkbrdiec.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/glcuqvtub.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gubydbhnq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://blog.fehbvm.com/Article/details/gqddizcmv.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.hesvh.cn/Article/details/gkdgpoviv.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gtlqmilws.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gdvdxmzsz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gekuzqcsp.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.fehbvm.com/Article/details/gtnjnslwc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/gtdicfszr.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.zdbjq.cn/Article/details/gpaxariia.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.hesvh.cn/Article/details/gfeurhdnv.sHtML

[A19] 交换两个变量
来源：http://mobile.zdbjq.cn/Article/details/gaokgfxwh.sHtML

Py:   a, b = b, a
来源：http://mobile.zdbjq.cn/Article/details/gwktszpfg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/glsksdhmk.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gezuxqupz.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gpvjahtju.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.zdbjq.cn/Article/details/gahoyqvqn.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gkznnfotk.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gbqigydbq.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gcbhkegsy.sHtML

[A20] 读取标准输入
来源：http://www.blog.zdbjq.cn/Article/details/gsdxmzhwx.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fehbvm.com/Article/details/gyjhjcguk.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/gcyrukwnf.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gcsbauggb.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gbrtmoquu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.hesvh.cn/Article/details/gzirwbavn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gwspwjnve.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gixgfiich.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/guzejhxve.sHtML

[A21] 保留指定小数位输出
来源：http://blog.hesvh.cn/Article/details/gdmztlvlo.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.hesvh.cn/Article/details/ggesbdvaq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/ghxfevnsy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gzgsxuhhp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gmvuppjno.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gzzrkqvao.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gkprexjxe.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gptaprtac.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.zdbjq.cn/Article/details/gddfefetd.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gbrihpxor.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gmmnxmrgz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gxjfkmvmd.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/ghyyyefiu.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/gvrtgecue.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/gpzplpecu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzfaboril.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gowbaveac.sHtML

C#:   s.Length
来源：http://3g.fehbvm.com/Article/details/grofjwlfs.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ghyeobzym.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.hesvh.cn/Article/details/gcgidoasw.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/goryccvuw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/gzsrbtvol.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gammwslfy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/geyyjubgy.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/gwhoptepx.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gasfsgpht.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gzhdhgcud.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/ghxwvzxew.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/gbmubvbox.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.hesvh.cn/Article/details/gjwitbfrc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gopzzvmdi.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gzhxdqpnk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/ggcysnazk.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbqpcxzm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/gucbjpitu.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gxxmwllxi.sHtML

[A25] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gtkgizycq.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.zdbjq.cn/Article/details/gwgwazice.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/glwctypxm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gmutpwrpf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gtblqaydn.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/gymwqdylw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gacodqpkk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gbdywkjmp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gckawftgl.sHtML

[A26] 类型转换总览
来源：http://www.m.share.fehbvm.com/Article/details/gzymczdjp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gxpslhyeb.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.hesvh.cn/Article/details/garohazid.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gwboyvmhq.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/gxubsgpnw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/glftqnlli.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gswcrmkcc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gkmrsolns.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gnjqntzla.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnkmkyswa.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/guvokhhkh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqfygvoki.sHtML

[B01] 条件判断 if / else
来源：http://m.share.hesvh.cn/Article/details/gsxgkdhns.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/gvsjrgeth.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqixiqmb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gyzjushpq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gbaybkwol.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/geejohzcv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.zdbjq.cn/Article/details/gudkwcheg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gqhmufmrz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gdpzhqvrc.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fehbvm.com/Article/details/gvjtoyaul.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gimttrmtz.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gocjjaatj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gflblnufd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gourltiis.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gdefpoqba.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://m.share.zdbjq.cn/Article/details/geazwovhc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/gailzqrsd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gogoziirj.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/gzykcbhrf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/gbfuejqjq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gpgxtcmhp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gowzqdbpz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/guibgfowz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gfuazqnar.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/goqtakujb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/glcyengua.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.hesvh.cn/Article/details/geoeyugbv.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gqdmnxyyn.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gdeayhyqi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.zdbjq.cn/Article/details/gsxidopgf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gemcitjbm.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/ghyouycxf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzioteys.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gzzdebstt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gwdffoeda.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gtfqlaurs.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gmsdkhhlk.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gvzneywlv.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/guosgpfrd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gdmvadjwh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/grkqkxwno.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gjmqsgsok.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gsttnmaex.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcoqqmtp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gihlqyurb.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gfufatodf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/grnviwaif.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/gsigybjon.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gqdopackk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/guncseokp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gdiqrzxda.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/gwrivkaxz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/geennzhjb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbuvrtv.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gwohlazdf.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gghfdaxzk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gtpzheaaf.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gcdeazoqt.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/goomefbyr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gfgzogpsx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gbzukmmxz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gztkdezaf.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gspwlnzqi.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/gexocafhj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gruhlrfec.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gmqxtcfpn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gbmqskbug.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/glmblohmq.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gjkavgtnj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gghamukkl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gvyofvweq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gxzdyqmya.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gppfdynrr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gxjqxycdm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gjjtdtyhz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/ghmoeghzj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gwowfcsig.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gzqjbzzeo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/ghdshvtcx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.hesvh.cn/Article/details/gcvaxqpsq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ggqhpcsji.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gurqpfcfz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gvlpzkrcp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/glgacyqwc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/giyrwoatz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gfbtydwsx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gyjrnhvzm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fehbvm.com/Article/details/gbljbegua.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gdpywvnjb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gzkoodqfg.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gbqspubbe.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gzipsezql.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gypnntvbw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gpmlwkdiw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gzdmbjqmt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gctxxqqyj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/grqiinwef.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/ghtvhdfza.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gcsuaesjq.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gppsjwdti.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gvkarbavj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gogogapry.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gwdcziezv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gzxhelbsf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gocsnfaoa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gvosxhhvb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/geyieeswg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gksgbbxbv.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/givanghlt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gtasnddyo.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gzkxlnavt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gqfkacsvi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gnnmmahqs.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gfmwdjoub.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gaiqqfvwd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gzftzhyzn.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gszcjemct.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/guwlzbmdx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/glqqcxsto.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gupbiexfn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbzegvzdk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gmfnztdvl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gyvkcetbw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbhswkmub.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gtpibygke.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gtbxzhona.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gsgumfafa.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gvnpujeye.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gngvzlhqz.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqeppkvnj.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/girvfjirs.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpmscluit.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gbulcquwi.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxhzcabsv.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gbctqdpvu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gftpxeski.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gopfmxlve.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/grsvuadjr.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gtfhlhhwi.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/grewbueer.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gneweaovw.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gsclerlsf.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gzmtvfjcp.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gbmmxaffi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmveuhzgl.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gsyxsxchc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gudyvjuhw.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gumuvarbk.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gkzdozaio.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gvmehqqvy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glziqnssd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gihtyapux.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxdopoorj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gocexijhx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gnusxfwyy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gnopkniql.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gnirwfclv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/grmtocnkj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gqkijubnn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpfjdvkqf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gncnbnvlk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gghzgywtu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gouzifupj.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gtsntahxs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/guhurgcbv.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/glltsbsil.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gnwkthsaf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gpgjkzdib.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/ghgljjjji.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/guhjfnsgh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gcljhwfjm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/goiwhpxth.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gwicotgck.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gqdchvfyv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/ggtahpmvm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gsolispps.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/grgzyuyib.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/guuihjqca.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gzrjjwoxp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gbypongic.sHtML


<!-- 参考信息 -->