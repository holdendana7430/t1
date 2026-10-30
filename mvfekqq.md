代发 wailian999

[A14] 注释写法
来源：http://baike.fanxiaobao.xyz/Article/details/gjnhdmtwa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gurqjkskr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbtnjmyz.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gpyvwsjcv.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gldtiheri.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gutrpirhi.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gughtkpkt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiaxtpsu.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glamwftbx.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gksglzlls.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gzllejxby.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gdebuvpow.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwbnwpcv.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gqnrgybkw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fanxiaobao.xyz/Article/details/gncnfkynj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzgbtyta.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gitvqxvjj.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gunmozxsa.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxxhdnzf.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjnnhsuk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fanxiaobao.xyz/Article/details/gkmbxjbzo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gbwainkkg.sHtML

TS:   if (!x) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkdalcjdt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgcadsby.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbneykusb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gwztakbwm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/godzljlhv.sHtML

[A17] 位运算
来源：http://blog.fanxiaobao.xyz/Article/details/gigllpcup.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gphwncbkh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqanxwap.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gughffpfu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gwsxnytdy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gywqfxtgd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/glkhveczs.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbemupagw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gcfzssnle.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrqxqjvt.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/geikdlktt.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsulkohl.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gthgayujc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpmkwxmm.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fanxiaobao.xyz/Article/details/gaeurqgbk.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fanxiaobao.xyz/Article/details/giiubjulk.sHtML

Ruby: "A".ord; 65.chr
来源：http://blog.fanxiaobao.xyz/Article/details/gdmfqkyue.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fanxiaobao.xyz/Article/details/ganpxrdso.sHtML

[A19] 交换两个变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghfofkphm.sHtML

Py:   a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gzxyqaccb.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxdyfbyt.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fanxiaobao.xyz/Article/details/gbjeftfby.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.fanxiaobao.xyz/Article/details/gpqiunfni.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnbtqusl.sHtML

Go:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gpucltrel.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyccpykq.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fanxiaobao.xyz/Article/details/gouxflgcl.sHtML

[A20] 读取标准输入
来源：http://www.share.fanxiaobao.xyz/Article/details/golhttanj.sHtML

Py:   name = input("请输入：")
来源：http://blog.fanxiaobao.xyz/Article/details/gyznggxem.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fanxiaobao.xyz/Article/details/girvhjhoo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjlclqdi.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gnwxkmapb.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fanxiaobao.xyz/Article/details/gskzcdxgu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkqpxivt.sHtML

Ruby: gets.chomp
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmjcydhk.sHtML

C#:   Console.ReadLine();
来源：http://wap.fanxiaobao.xyz/Article/details/gldcllboq.sHtML

[A21] 保留指定小数位输出
来源：http://wap.fanxiaobao.xyz/Article/details/glgpyjyji.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcwltwwvq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/grzlnelqr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnhekkup.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gtinzlkbp.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gicccxklq.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvgwylab.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqnigyxg.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkpjyzxv.sHtML

[A22] 获取字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gipvwzknx.sHtML

Py:   len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/goafqaasx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fanxiaobao.xyz/Article/details/gupqublxv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fanxiaobao.xyz/Article/details/gjosqyudv.sHtML

TS:   s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyvcagjr.sHtML

Java: s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjagdfhm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmxpkgtvu.sHtML

Ruby: s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gfusecrbt.sHtML

C#:   s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtrcezvj.sHtML

[A23] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gbsqvquuq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrynffwe.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdrhzbutk.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbhbwbpf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gchpzmfbq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqhdimdu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gvgubwgfu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gopvxwucn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giurqbiiv.sHtML

[A24] 去除首尾空白
来源：http://baike.fanxiaobao.xyz/Article/details/gufwryazu.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsowemjss.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcjaluem.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/gvhfzqogr.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmijcrgn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjndzzwd.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzefpfqu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtqhond.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fanxiaobao.xyz/Article/details/guvmfdtsx.sHtML

[A25] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbwdcrcx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fanxiaobao.xyz/Article/details/gkmopgggb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyvbwkfo.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fanxiaobao.xyz/Article/details/ghzogehka.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gsgflpgiy.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoygjvep.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuvoydni.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fanxiaobao.xyz/Article/details/guspkebxd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvlkcyqd.sHtML

[A26] 类型转换总览
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhbnkbfa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fanxiaobao.xyz/Article/details/gpzarises.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fanxiaobao.xyz/Article/details/gwmiyibvi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnnzmhfc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fanxiaobao.xyz/Article/details/gfmjwvsma.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgjupyip.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfykuxmbq.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gteqhbhfq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrkdciwd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyhcyeyq.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gbffdyzsp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpdzczui.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaqdclnb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/gbypskvny.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqhzmwkci.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gneiwkguq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/griembfhw.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbzsuzeq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaddtkxup.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvhivzte.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlsoroui.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fanxiaobao.xyz/Article/details/guaedxrck.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrbwaabj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbrhrduid.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gthtmtqnn.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gweziyqms.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkzzhfvm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdxzutte.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.fanxiaobao.xyz/Article/details/gxmmldptr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gviklkdnx.sHtML

[B03] switch / match / case
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcgwskpc.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrkmxvvr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdzfcaes.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gevdakyis.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvgvvslph.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/goxppbcco.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjswygqa.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fanxiaobao.xyz/Article/details/ghpuynquw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gdltsprbt.sHtML

[B04] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/giihbwrnu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geijmhyge.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfovpcxb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjwlyjygl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ganihyfbo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdocchqk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtckjaoup.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.fanxiaobao.xyz/Article/details/gunbvoprz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcolbpxu.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcbbcaxg.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fanxiaobao.xyz/Article/details/gcbsyopkt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjztfjbmq.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gmhxookbi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrgshhhc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaqvfqqg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtvhgfqf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxsqhwpi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdkhlnye.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gupttktyl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaqnbodt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpfhrsed.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqozsdzhg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfugyuaop.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gveflawjv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfqmpbhu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/giwxfydui.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcxmxjsap.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcpyrivt.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fanxiaobao.xyz/Article/details/glqpwucmw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapcxthac.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytozdnyl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjfkyoil.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwzvrwuew.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqwcvaca.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fanxiaobao.xyz/Article/details/grhbjgrrz.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gidrlbdux.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrybgtqh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fanxiaobao.xyz/Article/details/gihergyjt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmackkfp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gewoehtar.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gnuuatjzj.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqorxkods.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgkrbtkx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gocyxcvyb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gbqbcuiqi.sHtML

[B09] break 与 continue
来源：http://wap.fanxiaobao.xyz/Article/details/gpevnjkui.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/glswsnctc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gammlwheh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtpfqakfh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxciwawfa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzebfejj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqwejssv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gbaebjegq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gexvnugyh.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gmsheptyq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqpuzqbd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsleqeiui.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gznaixemg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiaxuvop.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjetocnvk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gibwlggmq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowwcpnzo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxidqchcc.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/gairjkfmk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsrblntu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthdxfrki.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gipsxnlqi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydjabnmb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gjgyolxvz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqzuwcvs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gsxsctzip.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gatduoman.sHtML

[B12] 跳出多层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gbfqrahnv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fanxiaobao.xyz/Article/details/gbvmhgkgt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gedleoqcq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbrgnwhu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gesdnkrdh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/grzsiytfo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fanxiaobao.xyz/Article/details/glspjnvny.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/glhtuhtcz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gllnckvie.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gkcdqtyzq.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrqktqby.sHtML

PHP:  is_numeric($x)
来源：http://wap.fanxiaobao.xyz/Article/details/gafliwwox.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gluposozv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbglyfngg.sHtML

Java: x instanceof Number
来源：http://3g.fanxiaobao.xyz/Article/details/gngpmaebo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwidztboh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvckmkpvv.sHtML

C#:   x is int or double or decimal
来源：http://blog.fanxiaobao.xyz/Article/details/getopaqvk.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gvmivyqdk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fanxiaobao.xyz/Article/details/goozcxnxo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxfwvlnd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gddixcyrz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvjybmai.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxobmymz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fanxiaobao.xyz/Article/details/ggyphdhpt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghqxunwcz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gaulerwkx.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqlnkzya.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/genoojful.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwfcnoif.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywvzgoqz.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gyurvrybq.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/glgmvyhni.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gryncgnqn.sHtML

Ruby: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmevmagn.sHtML

C#:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gpfzkzkwr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gzgwztiea.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrteaeke.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwlvbuwst.sHtML

JS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmptjctc.sHtML

TS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gqtciygto.sHtML

Java: if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gdkudfoee.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmqbtycu.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxazhfcv.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqrcvhkq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gofuvfwxs.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzrnhuit.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghulronaq.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtofunlxc.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/glxydvdad.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkmojaxvo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gacizbkbo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikwkeqvk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkzplawc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gbzptazaz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gsthxuhpe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxqcksfll.sHtML

[C02] 默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjtuikdy.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjnudxgq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcewnxjlq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmsnrsrqy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guvnmnmxv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fanxiaobao.xyz/Article/details/gizuzdomy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fanxiaobao.xyz/Article/details/ganfactwy.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwsxqmwa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnssmeif.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpnqyrrjy.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmvoeord.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntzwdfhg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/guwpzrcgp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gkyktyhni.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gxseplqve.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlkolhzw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxgjwtou.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fanxiaobao.xyz/Article/details/glsdyooqk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtqqacwl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzcictysg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxwtzbnjd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggeolfbtf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/grdqdygjr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fanxiaobao.xyz/Article/details/gcckcoiqx.sHtML


<!-- 参考信息 -->