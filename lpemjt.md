代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2adztfosv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ufqayolm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ztrwqifl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pmmvvsbr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zoueafta.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sxbwlxbn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2bquljevb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2sgttzdlb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kicfaubl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mwwtppni.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2yknguwjy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ussgmhmg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xqtlgwou.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lxtydqtf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2uvhremvy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfjwsyjg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2yleqnbwt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sqqmpyyv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uglqnmim.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2qmaptkud.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxjvzvbu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qdyjsipp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mesxvspc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2azsvmkwb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wholetmn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rlbalvjj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eowksqru.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2huahitlr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2gmygbcdn.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fmfsgpks.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nmqfxwle.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2szheinrr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2gyytjzxf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2mziefdqr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xogdgznv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mqoklhmb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ggfswhkt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2tgqebcqp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uwcygktt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zkfveoiz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pibvurvl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ibklsvgn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2qcaqqqzu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2giqyzign.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2glsamfbl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hwtfgvgj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qsekvbmf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2arzliiri.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2enjgpdga.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ewxmtvnt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bzyzfcfz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xjrlvkyr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vfudvtgh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bhqkedfx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2jejixaeu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ezdfjtoj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2llwbwgmh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fcnmcnlz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2itgynyli.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zkqgmwoh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hafhulvv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tzxznjgi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xozwqvnr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ydwpfwqy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cggukdme.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qygvojju.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ysemaykb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2hhpueosq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2owvbkzwc.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2melbailj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umdvdmsu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxhbquhi.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2oofgppsy.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2khcxufrq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wjfwaocz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2swvkmzkw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vmwiulzp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ckroyxmr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ihidtsfu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vcxydiaj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ejgzsimq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jaldcwjj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2seiaovdk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2uksltxti.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2fgvdjceq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vuujnxcn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fvsimqec.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2jaoqehjk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubvhbpsl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jylmeyga.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2slujjdoz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tvromzyp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wcuhwaxi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2cmetjncv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hjoaqwez.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nvtfmrfu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2onuozare.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kyuqxhck.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2rhecomzu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vwclveba.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2fbblawcs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2rapafiid.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2msbwlpyt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2eezgonhc.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2frmkjnqc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2afllolnr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2baimatls.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dqhllpor.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jsizzztb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljunpzct.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qadbjbyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oapypggb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qyciovko.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lwprvriu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ynbobikq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hhvqmcpg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jdqiggln.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kfbpqpqf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2iwwrdkpn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2eimlijcx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eyzcrqnr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mbgvbhis.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2iwjquooc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zguaobga.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lcdpbtoz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hwnlsyok.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ovogncsp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2aagyllyl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2owztebxt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2poqetdfm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2rhldaxng.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nkqilqdr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2esagzeiq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uhkjqugu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2eecuscwy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzvuvblu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqmehfb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2drgbvyng.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lixvswyn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fpfvqwqv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2srxsfjei.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppojynta.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jvzqkqcc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dslbjkcm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jhrhxdkh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2asclxexw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kxctaicn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2utavezgu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rlmvezny.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ttxspqjq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hhpxrzks.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kubtsmgy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rxndrqgy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssqsjqdo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hllcrwos.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2lrpnkjzj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxgpfhjc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2opwobekw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2eknycppd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vrlzhztn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwyiuakl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vargxzom.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wmkndorh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2dfdmvcco.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bvbmvsih.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2lfuvqicw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rnxmdarp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jzhgapcb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivpmrhzx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fotlwkbt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpvjqwti.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zcivftxi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2snledjuz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2dnonocev.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2weaefoym.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kuvuvzpb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pliqhhsh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2itnybgoe.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hpzrujww.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lboastsx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jfavdlml.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hyopgqqa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vgkabvdu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2houolvus.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zigelimh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2xxzmkbdg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ktslhcxh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2swrsskqe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oryjlmlt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2testhvoo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfquxev.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ttbnzqsc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyimtxxr.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hquioywf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fkdfixqt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvehojhf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2odbnhowj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2exprodcb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikwrpnmt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oscpyrul.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qvktamac.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkhardpl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ieqfwiyg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2aafhsbdx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yaomezuc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dnkhlvmp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kwxnpkwh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2wnoazkta.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2twpzcrqc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yyldrprs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2grxpvips.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2eqkqprrb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zxqpdkke.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2wrpcfejd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fqyygvjb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dojwjvpz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gjtbqsau.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kbvaranh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bdofzvfa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ojdhouis.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2edtfszpa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zgsnejit.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rtuhztsp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2byipqora.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tudeapef.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vbsjprly.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2utbjqvsv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qugmybsn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ypwimqhe.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fhtewenj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gdobjyns.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hdmpekuq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kyngzkkb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pmkssoxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzgzcksv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2byndtcau.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yjojwogg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yfztfezi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ogobjbru.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lbwqnrct.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2snzhippm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2igzegtjs.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2chnkpxsm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2znbvgxrm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vlmcruwa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wbrioytx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gqmytnur.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2skmyehjd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wukpkpgb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yzgyxswc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fhsrxpvt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ppytcfiy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lkeuixgc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vuilpjor.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nksnlxvf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pjyhxlvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elpnagwc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ezxhzaeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owfpgnbd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qpcfynej.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fwqlsygv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2earhqpjs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2spaelkam.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lfcgjbqi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2alvagvpc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2inmjdqvo.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipixigpa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yleekhnc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2jocwwxvq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lwmdteug.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2edccebzm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kstwicwu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmhpfbyo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rmryukcu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2tjqwavsi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zyvkfqqw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nviykcct.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xhifqjxj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2uukbvshr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2voabhzhi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxgzfpqf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jquxysyq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hebfpehy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2upwzvpwl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fnhtcect.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nvlqfozb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ossmtjcz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jylsefrk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mrvbysmd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyognqua.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2emlffewd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ovzwaomw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gsjhwbhn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jbmtxquo.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fpvjniiy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2djiqpjos.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ugktfcjv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2smbcjldr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zasnuimt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fwotjlsi.html


<!-- 参考信息 -->