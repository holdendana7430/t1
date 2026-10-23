代发 wailian999

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3pzmvxoef.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3rtilcugz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ocfsxzos.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bwdkueip.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rohhzpln.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3yvbuopuu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zsygcxcr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3bjtwzski.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vqzdwgib.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3caehbgrv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qcwegjim.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lzrlrnau.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qgxqygko.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3trmqabas.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3hzedkstx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zrzpaseq.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3pyqtzcdn.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3shtvapzd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3omolnejv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xqjyteln.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3joslnrdm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3anczolii.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqbwvdxr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3aeijhncq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3njptxnzn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mezkivrz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohlflcat.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3fyuzuzvi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3auubigho.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yunjwgbl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kvmhkssu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3blbowufi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wljngirz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oftnaouf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3meabmhog.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ixmdotzr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3zpgddffl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3uhduxjdl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tookhmss.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3eyiumocl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xsixnect.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3iqvfvvwz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wcfcnkro.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tqlhebcc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yovzqmgm.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3uoidsllt.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3urloxrhs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3gmortdmh.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nchkwtjb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3tlyftucy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3psvgqfdi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ruvfqqna.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lvqhgilx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3zmjrmrid.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3mezkuldh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3boeqfvrc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3qgxffakn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ubfommsm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3diupexom.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3pkrjmqsh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3guzbtxlb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3leaubosx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fgkicfzm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3zvqvuztz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3wpesmyjz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mrmdriea.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xgomejdt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nyhbxnyz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qicrrnsq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3izdfmqmt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwzabac.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3izumvzhm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mbwnupbz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kcwhnadn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fbfzamgl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ilnkevih.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ngsojktj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qwmhqxlt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bbezovxa.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cxishmza.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3mejxhojm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3okhimijm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nfdzfeyk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ilrlwvul.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kxdzypid.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cdwmyykb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wnaguukl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzuguwke.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gcmckuyz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3teksvfed.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jhebrqyb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3zitajezf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3xsjatmuv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rymoeddv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ijjzqbve.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3yrznpfrm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zevpbbpl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3czgbowzn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3knxshbmj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3qrdjeema.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3kzyuqgfl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3klglkday.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvonqukn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3gopywkjc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3zmdlckkd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xuvcckqt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3crqwdshg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtzkajnk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3lridihna.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hsnrrdys.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kzpbyweu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ogredscg.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qbrexnyd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rlfjrhdf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ekhtwkez.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ecvkuxup.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xxhlcvnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlngottv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3wdbzpavq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzaqfkau.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3aykteckv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3donsgler.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqnlbeph.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zenodoxp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gwryopor.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bfjhwflv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rrrbixre.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kddkgsyn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ecaauypq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wxlhtgvu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gdadspnn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3nzhqjbtx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fhqwhdme.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vbbzjheq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rxqavzns.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ocnrutur.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ntpjjedq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jdoufpjz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ezjzbrpa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3byhxxxvi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rvbufioc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gygmttmw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jqikgzfx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yobngkuk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bwcwrcve.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zkvzcnel.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qiwypzvx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tixuxaec.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3chheoqxw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3iniwwvun.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtgcdbrv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3clahviid.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hukppdlq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yheksrbb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tevkcgsf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmyfikhj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zyfusokx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zxwkicyg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3omxagfxq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3udosqpkj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kirvtlmi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pzdbokbw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3evfbzfib.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3swukmdkg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpyykixh.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wpizllad.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lmyxsnov.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yxupiqpq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wacezozt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ryyzvpvz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3udyuqjhx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pqfjpwnx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jjdjehju.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3psuzynwg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3peotursj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lztoessh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3symaeagb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mzbfoqia.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3youekbub.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqbiarbi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fdlrlmbt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcfrnfmi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdmrwxec.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tlrzwjdx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ueytewww.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ftjurzdv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3livurmyf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jlzpwtpy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dutqdpxf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pzvthwyq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zdrzuzjf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mcksxiwv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3sxthdgxw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ibfcsusa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cjhgdpan.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wylgcxfx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mazogwjl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcafsnqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qsfnrzae.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fycmntpp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3quukuhxa.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3lmxswvuo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wktvqych.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzdemppa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3brcykhsy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hzhacgae.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ymmpaudq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3elfibvjg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gufutncj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eksrfrex.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eddjfadj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3tcfoybgl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bbacgufa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qozljdrx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bhgykenr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jehpziui.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kawgdnog.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xqzoliqz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3isbalrcp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3mzbctigb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3btckkqlk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3swvqvkvz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3amwafrml.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ssvkqmgf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nzeqgcps.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dblenanc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fuygncvh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xfjzaxtl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3bdzujorz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3yocrnanq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3faqfrwkm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxtsgqjf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iazvitrf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rdsennlk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yqbtcqaq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dlioryej.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cwrzlgir.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3tnmighgd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tcluoqfa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3soazgqty.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujzcdvcv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzbbnmp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ukccauwg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujzjansh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rrgtjxja.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qusfamka.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3iphcotlm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3sedcqyim.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pdaxwfsm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hcjrfxfn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3obzrwgmr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ppsmgmjh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oskrlqhh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wkefrbcz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ajkotizp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3twasjcup.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dvuekqqn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmvlurol.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xswlskrf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bbcebglc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jykcqbfx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3uoqerrtc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mcukfxle.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cjhkavrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozdhpjaq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fljdkwej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iufntowe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bdxssezg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pamqwtex.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtdxormx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofmbucyp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljqcbcgt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pexvqufz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zlaphrum.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cyuxwfms.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsxdhegt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vcualipn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fbngyvft.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3txafjjua.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nabhhqry.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rabeidfe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dxnuogdu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnljckpu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ahroyptj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mlgsbwjs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ovhlwhjs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jruvlnwx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvryghgy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dtcnhzwy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngfnpwko.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3fygajbaf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ruyvphdp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ehnueqnf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xhsxnmxm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3forxuhjy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3akvhkvpz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pvbhygkl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3abvkmbdx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gzpodacb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3zidykaka.html


<!-- 参考信息 -->