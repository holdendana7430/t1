代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zipnfieb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2aqvaxyvg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2foongzzo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2resvogta.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tpzfjxye.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mmidtdbq.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kkkfbtwq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dsjlrcnc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2agtbromw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oaippjky.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wjgxmyfo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tyqatqls.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2hndytams.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vhjoxlkq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yxgbfwfx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hbgoooev.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gkpnqcxq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2znyswzbp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yywylkga.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2isvbroop.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nwcxcxzd.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wzjdbwln.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tyroqecm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bydjzqmr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jodpqcxr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ybycllhs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qtyxacvp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dklncdxx.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jjzrcvxq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fshlgfuc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2yfcdsduq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zmgwkzqm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ywcbkuwr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2kwyecedy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldenbthq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2avksgbth.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2njlwopok.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ibsvoabq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nymhbkdc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ppgbsqmw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrluubac.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dasfaltm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2muezmsxz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2psboddai.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2waknjreu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuujlizl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lgbnhiqf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gzsmebzz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vscxysqx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jwpkepox.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pnwkevvt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qxpbqaiu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2uheppidn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2kkxwoxtt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2eqlxusiy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2kmalbvrp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2pfzaxcge.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ygajrtts.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uzccyzkd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mgdbaoog.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dzitbahh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jazxmyge.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2gacjxfid.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eqbkwjwi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2eozofper.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2zzxsscqr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mxwxwqxm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ucsgldmh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2lnvcpbpo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tzzdnlio.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qufsxokg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2qumxffds.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dzebpegi.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qswnhuin.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2naebayey.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ztmllzsy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2gckjbndo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lvqxzuws.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ozfpcnqp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ucyelzzc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zwcrfsyr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmoebii.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sqeouavi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2npbfcjlf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ozhgvmzm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqxzpxe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2xqylcxew.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2napxieyu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fzwwgouw.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2iblnhsue.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbadhupc.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aiuemdey.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sbpcdhul.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hbaooqqe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jpqcplhv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kefphkhh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iynsfzhk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2angvzbac.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gzxvzowg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xzpwwfas.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2idcbostf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mevdlpik.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2thaonzqp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2popwkggm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmqdxenq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2piyuutyv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2citxvjhv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mmrgtani.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2oevzvhsn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2brmkkkxz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pabyaogi.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dpvspuoz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2pvbslvil.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ipxqsngi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bdxwojpm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pncysvkt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2kmmwbqqq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxzpdtjq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xibkjzjd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2clvyojdw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2kawjcyor.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2csodmlvj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vhankhij.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ontihqof.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2esblodzp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2snkpcwfb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ucfntzbh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2njdduiyq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iaoibnkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dthaaowv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2nvknjrfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixijefxc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tlvjndtw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2txeknjqw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2uoqgcsmg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tcisckhs.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pcrhekrv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pyzcwpcq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2iywxaokl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ythnjrga.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2eyeyrgld.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rpklxmys.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2zllwwaeh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2hwqcanmq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hxdniifz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yrerjauq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cvldmjno.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2nlurtrmx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2aojqurrj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pewhbhzg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ohhqxtlq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bjifpuyy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lijqcidb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fynhaerh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ijqywjar.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxhbupie.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ngppbpcw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2qvgbqerk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lrjrpllj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fsfotqfj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qzzjkpby.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bozzuudc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2utcazanx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2apoiahfa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2yepnorwl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2yfwnfxif.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2acdgqxjs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rhyxbnrq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hofjyryx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bitthooc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysbazbbm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bttqfand.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2sehbjqmy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gbhfdbix.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gktpefdj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2jhnttjss.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2izsbzkoi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lbmbyxtd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ysyyazzm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xmruvphj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lswxospd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bxuzikku.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zinkgpeq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2oyumhlhk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sqvofbry.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dojrubfy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2cunsskcd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2urulipyf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwvfndjb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cajdbzij.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dijaiwzs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iozrzgvk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2pqnphyhi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jkyfmokb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjruozhx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2oiyonleq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tshyvknh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eaxeomat.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kqihoepd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wmoxzacu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uxyqltgk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2stgvoghv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2shwhnrco.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wxvqekvu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hfewthkf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wviuzzig.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jfyoozrt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2btiakitx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pzokjknj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uxwqlfxz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2onvwaito.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pqqxrchx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqwackdc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gsfdxbxe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pwklhlzl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wfufvjem.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ysurkeug.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wheltptr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2azfnvzdn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ldkhxzzu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ghvpeexy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qikltbfd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2lovtjdjm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mrivtbda.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hammrlcn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vjjpdcge.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2duxclsts.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ygqodcna.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2qxvhrzos.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qedlepvf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ntunqseq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tssdebzy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2elbikjbe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ikpsorqk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iquvvkwe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fmeqkkqb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tmhheojv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2uxehwela.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2tzqgmlir.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lqqaamlo.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hujjshuz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qfovbadi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdrmrwwo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2utwkiyrr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bjclusoj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2drpnrxsu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zphwghku.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2kjnjtwbs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tvevgpud.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qvwxtbby.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ucvtgrhf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rfvpdzmo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2stbfjgdp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhilkzvq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2apihoxil.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aakyuqtg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yrtxwnpm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fuuceotl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wzkcpjwd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cuvvzqhe.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wvykcwle.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hacsxguj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2acwuvxpr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uwmhyuko.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tyxdnuov.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mfiactpl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2laqjnova.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2swyskvob.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mzgblzhc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpigthfo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tulqfmip.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2phdeiwlj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aoxagmuw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mybnycee.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wpbgnxuy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zwyoiyev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfdvoeuz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2iusfmbgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhlfolqh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2evlbnotn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nmxfldue.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uffcypto.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hhspqibu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2azlawcil.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pmvldvbe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ajhpqxqb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2plikcjum.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pepmzyhk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2aprasegd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nmacpowt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxsegirm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvdbtjcg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vpmslahf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2nxxxxkpl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jrhnlaui.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2aukwvtur.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zqmcrprt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jmojuhyu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2inljtemz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pwfwbsxz.html


<!-- 参考信息 -->