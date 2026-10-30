代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/guxjsguca.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gllhfshhn.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gxszsdwoh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gfihswdtb.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/girmkixgt.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gaamymrww.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/gmraquufq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gyiauydlq.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/gpnrynmqf.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gponpxicr.sHtML

[A16] 真假值判断规则
来源：http://m.share.zdbjq.cn/Article/details/glmkyolro.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fehbvm.com/Article/details/gmxyzrvof.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gauhzytpe.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gumbfkqqy.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gaezyfejc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpmkslihk.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/gqmukjllj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.zdbjq.cn/Article/details/guoqvyjtl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fehbvm.com/Article/details/gwdisfclf.sHtML

[A17] 位运算
来源：http://www.blog.fehbvm.com/Article/details/gvqlpykib.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gsmlukgcd.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.hesvh.cn/Article/details/gqjdmizoa.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gnixcgsww.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/ggfrvofmu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gjmopnsuo.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gzwqnumyw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gnhpbxnff.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/giqthdcnj.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/gksvzqvdy.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gszmfdrbh.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.hesvh.cn/Article/details/gftklucuw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gupedqqem.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gnjrgozwp.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fehbvm.com/Article/details/gffxbbvin.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.zdbjq.cn/Article/details/getvtjvks.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/guilpqrqf.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gflszzcbe.sHtML

[A19] 交换两个变量
来源：http://read.share.fehbvm.com/Article/details/gxbarlhmr.sHtML

Py:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/ghfreotyy.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/gpniudkku.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gxcaalylr.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gpsufcjhb.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.zdbjq.cn/Article/details/gfplyucos.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/gjgesetpj.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gqsqmzcss.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fehbvm.com/Article/details/gvnpxwxrt.sHtML

[A20] 读取标准输入
来源：http://www.blog.zdbjq.cn/Article/details/gbvgsbqgg.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gjchmypsb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fehbvm.com/Article/details/gxjwzsgjd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gtmmqpfzb.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.zdbjq.cn/Article/details/gbczmthts.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.fehbvm.com/Article/details/gfurwubec.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fehbvm.com/Article/details/gigtejtod.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/glegjmeok.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/giwcffqtt.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.fehbvm.com/Article/details/gmsmrnwlu.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.zdbjq.cn/Article/details/gvtsgaldm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gworfxgwm.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gaxioivoa.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/guwxphbdc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gdqanbpoc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gdzrjbpje.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gswrgmokn.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.hesvh.cn/Article/details/gjwmrveza.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdjgbyneq.sHtML

Py:   len(s)
来源：http://3g.hesvh.cn/Article/details/gaweyixto.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gabmxbtbx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://read.share.fehbvm.com/Article/details/gwhiwhupf.sHtML

TS:   s.length
来源：http://m.share.hesvh.cn/Article/details/gyvxnmktu.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/gcjossurk.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/goewvzqxz.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/ghoqfasbu.sHtML

C#:   s.Length
来源：http://www.share.fehbvm.com/Article/details/gmjlyuwqp.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ggsvdsfux.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gkiclwdan.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.hesvh.cn/Article/details/gitfyfxnl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gsrsgltic.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gwdsjepdi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/grvdumqtp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/gjxfdxzec.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gpdxohzda.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.hesvh.cn/Article/details/ggziekufm.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/gheeyuhuf.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://baike.zdbjq.cn/Article/details/gylvvhkxz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/ghzikadwf.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.hesvh.cn/Article/details/gubryvrik.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/gorqiebxx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.hesvh.cn/Article/details/gsegpzwel.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.fehbvm.com/Article/details/gclzhegiv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/gcjzenzfq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gpxrqiffu.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gqniuuaht.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gkpzhdsol.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gpmlamwqf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gbbnbtyls.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gtrsiqacj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gkxwymbmj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gwyzqstai.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gsoxwekcv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gjpvialiu.sHtML

[A26] 类型转换总览
来源：http://m.share.zdbjq.cn/Article/details/gyyscsqts.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gkkfdsbzy.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gjsanhvoa.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.hesvh.cn/Article/details/gjfhjcdus.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.zdbjq.cn/Article/details/gavwkkbik.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/glzdiavka.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gfoulhckg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.zdbjq.cn/Article/details/gijtepozo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gudxebgtv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdfyaaaav.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/gquvxnlon.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcdlpkzdm.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gwzvhcyfz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/gjofygoqi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.hesvh.cn/Article/details/gxnkrbnta.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gorrbcvgc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gglqftaws.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gdfjzxgfn.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fehbvm.com/Article/details/ghpbqqkco.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fehbvm.com/Article/details/gkjbjzbio.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gabrmrfhr.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/geierfzjr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.hesvh.cn/Article/details/gjtuoemxo.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/grkyvgmhp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/glzysltwp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gqurpthbe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/guzrcmfwz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.fehbvm.com/Article/details/grpagozhz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gmoeerxzm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/glxsulovd.sHtML

[B03] switch / match / case
来源：http://read.share.hesvh.cn/Article/details/gfvilrjvf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gswqrznts.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gqlqblzwf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gyuwvwdxu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gectfrjzr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gkbpmhuta.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gdedwztkr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gnvnadawa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gidnjygiv.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gfrcghspi.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/glcepjsoi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gwlnmrzvo.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/gzvaydrgl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/ghjhvviyh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gmhmxfocm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gcylwftpr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gxjprlxcq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gcgjzmouv.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gvkltijld.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gzblixfrg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gkvbanqkx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/geykctozy.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gluklxxlj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.fehbvm.com/Article/details/gffotuwjt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gkjmifccn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.hesvh.cn/Article/details/gmrgvdylp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gldncuobr.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gdpowworg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gyqkazzbz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/gjiyvbsqd.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gagqabhlx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gkufzbzrb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gtowudlis.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fehbvm.com/Article/details/gqqnquyru.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/geropnchx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gddlmjbdo.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/glalmggsd.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/grwpsbvfy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gfzaknrrn.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gmvlntdmm.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gpkhibgid.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/ggwbukeld.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gphpzdefp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gyectuwhf.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/ghntpaisv.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gffmjsawb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/grotemywj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/glaeagavh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gskmvlgvr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gyyrqdwch.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gsudyjmus.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gpztqaqng.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gxsobntyc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gioanmyvu.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/guwjkbdsa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gzwskuygv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gqpybsbty.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gqgmrxjvg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gskyffbym.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gyejmklwv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gxreboubm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gnrcpmasr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/grzouxamy.sHtML

[B10] 遍历同时拿索引
来源：http://3g.hesvh.cn/Article/details/gtvobipnr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gfpsdwoej.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/gtsqzbshm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/glhjfipcf.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gvkkzykyu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gzwvbbckh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/girnymvpk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gwerdzdcy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gmbhggtsr.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gjvvnjbze.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gijaxssoz.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gsvflibds.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gvcrhygvj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gfohylpph.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gitanckzy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gppzdzulu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gnlbxrzpg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gxhbdwqho.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gwynjycxt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gonaznmrq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gdbrloist.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/glnxtagpr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gxkkumolg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gtuazdove.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/ghgxnotqn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gynotllfa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gmkcgxnxc.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gekioxoek.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gcjijeluh.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gopawushc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gxnjhkrvx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/goxkxejhv.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gfujyqovc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/grjubwelm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gyrqabqvo.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gtqdzcvne.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gnbdnzrsw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gingbsbmy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gmutowohs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gofmhrujm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gklikoedb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvudsjrfr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gqtepzifr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gootzgcrz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/geqvjrlfh.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gzqsdeprn.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gnklurgio.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gbigjhdsc.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gyndnpuiu.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gmwteiqqu.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gpsetnovh.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gheiqhtpe.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gvmkezjag.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gipyxhhba.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gwrhwfngn.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gkrwlxjpa.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gwoblabyq.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gtwgvjljt.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/growrwzmc.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gtgubvbrx.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gokjlkyav.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gytcbvahx.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gwywmjyxj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghyjpueih.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/griayxyok.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggyyplfeq.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gfqdxhzlb.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gqzoetawn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdiiwqiw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gckdsoknz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gyhsabkkx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/grbyngjfa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gftrhugoc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/glxgoylya.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmmlkrutd.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gvklkjkey.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/giukzcsxn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/ghcywmevs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gslkriykb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzcmhiowf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gxlrwvtxa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gcjrqxqjc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gwjpawtsm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gkqszzezk.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gqfaszoap.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gyjzfdpdu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gnvcaqzzc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/guypppdwn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/goieocofj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gqokkbtup.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gcxvxvguq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gyshzcyey.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gzowvlpxj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/guygctngh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gdotynrml.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/getdbncne.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gyahuvpaq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gbetvgsht.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gxjndldcj.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gpnafgenh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/geyyafdvi.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gnyarijhk.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/guahomgje.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/glbozibqw.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gtojxtvil.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gelegbjna.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gbpqzshhj.sHtML


<!-- 参考信息 -->