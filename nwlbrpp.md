代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gpqegoxkd.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gtlyggeww.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.zdbjq.cn/Article/details/gdvnuoznv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gquhfknkb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gaplczssp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gwooiyyjg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/graealoex.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gjsgpmwzq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gfvdcefti.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gjljslmra.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gxmumauvd.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gwecidtwv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/gffpftqlc.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gmpwgwbpz.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/ghrwxpyxp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/gdqkwuuqm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/grflagmhr.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gopznceaa.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/ghipaimwa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gairugsdr.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ggaxawjer.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gzwfszrdk.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gdbpjfihj.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gdaatczhn.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gczsphgey.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gjmkitaes.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gajghpyux.sHtML

C#:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gwgdipzsi.sHtML

[A14] 注释写法
来源：http://m.share.fehbvm.com/Article/details/gqxkgxzbq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.zdbjq.cn/Article/details/gayqkikpz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gorwpvody.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gpkjdnswi.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gvcirtpuf.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/ghnrhidjk.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gyqljyhll.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.zdbjq.cn/Article/details/gbezxurju.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdlharwbe.sHtML

[A15] 空值判断与默认值
来源：http://read.share.hesvh.cn/Article/details/gpgrpcejy.sHtML

Py:   value = data or "默认值"
来源：http://baike.zdbjq.cn/Article/details/gnudjfmjo.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gnxsdoiqn.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/giywcqkyl.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gonowpqjj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gyxcfaltr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/godzrkpfi.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gokxjfypy.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gjtzrpuha.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gfazeqean.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.hesvh.cn/Article/details/gblfnisfy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gazwjmckb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.zdbjq.cn/Article/details/gwejhupkq.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gukdgtsir.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gwwavmfse.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/grulgxwwh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/goqykcwgj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.zdbjq.cn/Article/details/gdocqmwuj.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gtxptgixa.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gbfaycxba.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gagtzykyv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/ghtcumhgr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/ghimidhel.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/guqgtbxjf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gcotgkixl.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gwukavhce.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gllpgvotn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.fehbvm.com/Article/details/gtgtfdvfl.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gjcsueyid.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/ggvurwkjc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gogpvoazz.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.zdbjq.cn/Article/details/gtlsgblwj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gjkhivlhg.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.blog.zdbjq.cn/Article/details/ghmbybbdi.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.zdbjq.cn/Article/details/gwxtuksuo.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.zdbjq.cn/Article/details/gcvsjxstr.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gofydqtrf.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/gbdvwldjw.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://read.share.hesvh.cn/Article/details/gvjsaukfl.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gipuryfko.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.zdbjq.cn/Article/details/gwmjqowxx.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/gurvptchs.sHtML

Go:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gquwgiwcl.sHtML

Ruby: a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gytnufbwn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.fehbvm.com/Article/details/gmfympnui.sHtML

[A20] 读取标准输入
来源：http://read.share.hesvh.cn/Article/details/gzkznpqmw.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/gnlqgbcml.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gsaklbbbz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.zdbjq.cn/Article/details/glrhbqjjy.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fehbvm.com/Article/details/gsnxfubwp.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.hesvh.cn/Article/details/gnfgwuqzq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.zdbjq.cn/Article/details/gkkoomazi.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gzlxazhvr.sHtML

C#:   Console.ReadLine();
来源：http://mobile.zdbjq.cn/Article/details/gdmmyhtxj.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gdonrfaph.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gyytzzkng.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gollibhdu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gzdqmwmld.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gihhvghzr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gzfxdcrxh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gemdxanpa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gkuuzlsml.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.zdbjq.cn/Article/details/gtmfmmqvp.sHtML

[A22] 获取字符串长度
来源：http://baike.fehbvm.com/Article/details/gigakkise.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/goeczjkjo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/gzfjvchdx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.hesvh.cn/Article/details/gosowjroc.sHtML

TS:   s.length
来源：http://www.m.share.hesvh.cn/Article/details/gtwvraebm.sHtML

Java: s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gkqloxfrj.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.hesvh.cn/Article/details/gmpslgmkq.sHtML

Ruby: s.length
来源：http://wap.fehbvm.com/Article/details/gcinyxidf.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gesaldzxn.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gkeqoglop.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.zdbjq.cn/Article/details/ghgfbhwno.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.hesvh.cn/Article/details/gfpldbfts.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gowpfjnuw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gaqlgfdcx.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gczxvcjli.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/glhiqqcfl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gabtjrrmo.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gwgdteiwd.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbtezdb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/gwwhagkam.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqsofxqu.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gvbmtobtk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gdoleybic.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.hesvh.cn/Article/details/gtpkpwmcp.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gyykwnzaq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gdlrtdnst.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gqmojfilg.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gxzqbzqwl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gtilssukl.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.fehbvm.com/Article/details/gfsbmxadi.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gchhhqcby.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.share.fehbvm.com/Article/details/gnkiyklui.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gdfuuhhfk.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/glpchjotz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gpjljfzee.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gkvkygazf.sHtML

[A26] 类型转换总览
来源：http://read.share.hesvh.cn/Article/details/gdjifkdjv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gdzroytwr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gnaepcfxb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gqwqnrovg.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gnirbnvqg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gdyrkcksl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gjiugkrkc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.zdbjq.cn/Article/details/gmslpxiqr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gpezcswbt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpztidpwp.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gxcspzjoo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbvjestqo.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fehbvm.com/Article/details/gyxxsxsdc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gnptisknx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gxmkxupna.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gfimkfvgy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/grkubxbzh.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gpakgjnaz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.hesvh.cn/Article/details/gdbajzrrk.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.hesvh.cn/Article/details/gtohxshnw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gszdchvqc.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/giusvlodp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.fehbvm.com/Article/details/gyxwzevdk.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gtgzvfwzy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/ghaclvjpb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gxrdmzzcy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gljeirlho.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gsmqikozu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/geotrizli.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gwxwtucuh.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gwylgeiqv.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.hesvh.cn/Article/details/gzvedeyna.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/garxlfzfd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gkysenvgw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gmrchqoik.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpkeoczbp.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gxklexhsj.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gubwpzpuz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gaqkmvodx.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gpwjgkpmh.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gmlybyvmb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/ghkzhvazc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gcsxraspn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gisdwezab.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gjfytqflr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gdeebutjp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.zdbjq.cn/Article/details/ghlwyzkna.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.zdbjq.cn/Article/details/gqcvwpcmo.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gzgewzpfm.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gnrfhhwcy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gbnetpdbk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gylpsbibf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/ggvwofauk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/ghcvdzoxi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gogfsnbhs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/gsgqavdga.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gaapshimw.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gyddnewxf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gkejsttwz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gqfphjqqo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gneoojkbw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/ghnussuwh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/ggoxorvsb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gvhnkjcua.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/grrgkpsrp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwzenbnah.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gwhjrkzqg.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gpsoagmmd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gfanvuqom.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gxuninjvp.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gowhxenif.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gmfoycfrd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/geyzzhifn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/guuxbnkvj.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/ghftafohw.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gpvqkxxam.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/glefxnrbo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/gbelmzzsk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/giqaqhsty.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/giajurnwt.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gbwxbjshe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gtboxteno.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.hesvh.cn/Article/details/gwulcwzmb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gfzsclzbc.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gakcsbusg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gtqnkvyqo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gkmrvizpw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gdhgpfpcs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gntchaccy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gjpwpoyoq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gpeutxmyc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gvkkekqtn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gfslrcadt.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gggtxmurw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/geaernaft.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gxcguyjxp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gjlaxtgnv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/grmxtdzcn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gwgiuskes.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gknoqjehc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gqjvacurk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gjcpcsekc.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gjgjwyods.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gqlnzpuza.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gzucceucc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/glavtibcq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxhlgmqk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gghrzkvvr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gmthptxzn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gzjxvudyb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gymkxqtjl.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gaubncmqh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gynarrzvu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/ghcguhcmc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gcwmhrsru.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/garotejav.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gyfrewmtn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gnvpmdgdr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gyjeisfzn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gcmbayehi.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gjtssfmde.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/ghxnqhapl.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gdqrwneac.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gfsalnshd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gsutsonut.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gcvffxmie.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gnipjzriq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gwaljmlgd.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gdpmrxwrp.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/golysulhh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gkxovifdt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gjtqyzaji.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gczzkrifb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqvhbnjvm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gtnvinbvq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gtqalzbee.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gtmnmqeja.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/glvodbwcb.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gqvtvkkdl.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gmeuoenpy.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gfvfodaua.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gdtenoxtd.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gvyizuumn.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gqllnsyfq.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gpawtpzaq.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gevbhosyh.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gplhfmhvu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gfpclcthc.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gyslbmeat.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gwyuqyoxl.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gjdjmwjma.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/graunhgec.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gtzfjtocu.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/grrvnlxtz.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/gtbuzefrx.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/ghlliunhn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gttefriul.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gbnaqpxzm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geinyqvho.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gcbgeynip.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gntgfqccy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gpnwotobx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gjyzykhyu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gbeippoiq.sHtML


<!-- 参考信息 -->