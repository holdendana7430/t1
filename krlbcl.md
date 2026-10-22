代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ybqvxnsh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ccbvomgq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zacqhrwp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2werlotux.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2atgevflq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ocpkskya.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lpozzfdc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2puuqlvqy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zalvfotk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xlpqakgo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2bomwesko.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ntjgzbvv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2rnfebvnc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2banbrfly.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2zfoxxtbx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2upiafaqo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2agzgapdv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2avqalkih.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2kazdfkrc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2etikqvxz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2uxhdraea.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ckwuwfmn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bmocmvmv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2xuresiqy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vizfvgnw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktzustox.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ffnftzcd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gztbosul.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aevxbnug.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2umpacynm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2efeyxtpb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bfcnwfzi.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ibxbzrrz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ufblkgau.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dugxumvr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xrcsotlj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqwleiy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2smwekypk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2dymfqkpa.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2dlylvydy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cgemzotu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2kznyrmev.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mxdtxrio.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2lzqhgxlo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jdwicrtg.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uovvsqwb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2excqyfxn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hlhvdzqi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2okqysgne.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2vebznadh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gharqign.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gyudqmae.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2uqzmjxze.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2smyyoskj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2knlwstkj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2gaaaoddn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdnnxws.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2qhcdnfaf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2euexdjjc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2xwqkhuca.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2womjxbjn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pjvafqmt.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuskqanw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eunjigsy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jofkvfnf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ffbizrmp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dfqhqpbz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2kbwkrcci.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lirkpyyh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hsmqpvxx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2oglhlxzk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2cttnnlib.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jzkkwoep.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rckudftm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2sdhhpogs.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2rxpyjqgh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ruxiofrb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nfxzfgkd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2zueynihj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2buzejikx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xlhygows.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vykzbycs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mcjspcxi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvczon.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qpduujak.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2elryvgle.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2vhyahhjf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2pporbqzc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2goawlyeu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aicglibw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lgqydjdy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zxcprsiw.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2opiwubxa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hoawvvop.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nwychcgq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2akhjlbjd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qeejfxvw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqeexgb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2oprydfbz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2mpnhrfre.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2alakyaii.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kckzigbw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pyhgatyc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vfcpqmlw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tmflcbls.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2citpiewy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2kdewvtmf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cnaeupvj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pcahkaob.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wqwiyenl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fvtvyjwo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mivntecw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jtzuhhcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcrajtxq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jlolswij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pjbscdsz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2kybikrsi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zzbjohyc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xkuqmbpi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gfugwenq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rzpkenee.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zfoltcda.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ynxhqdgz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2aghsjmps.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pmosfvzr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2skpgqvur.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cnhxuobu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2modqbqyc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2edrkpdid.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cdjdywgy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2edrzwyab.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2sqgpqqdu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2krtgxiah.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qftufsnx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qvxidfgw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lfceodti.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2liyqecky.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnvxvazk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqhjlczr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovztbvwa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ygclgsis.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jfqfxknj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xtzftpqb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2frgkhtxa.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mypjidui.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2vzgwadjg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyodfmnk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wngoxcqx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kvznbofm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2koutbqio.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kjmiakne.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xsjsqzzs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tlvqlbse.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mzhwwvaq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kypsmefx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2szgshmem.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lobuorcw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gjbajzgy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2bliarhtq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2uehewgbd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhnuhvro.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hpemacrd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ljiirvct.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycqrpueq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lozsgcww.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rmozscic.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bquluknq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xkdtwvdx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ttmualvc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vgifutgi.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xeemzqfp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2txvimyor.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkjtbpho.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nstmmdwq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gownxjzc.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xkzehdje.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xpulamqh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jkqxtbgq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bujwlmyi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ewoixnzh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2glajkvyw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hkkegueo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bsqfnpmz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yostjkhh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zofosmaf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2msacwotp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2duoghidk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2znivgzws.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2dpzugtdm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sikrpecv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwhdwbxe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mjdcqelk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vparyrle.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqugkwhb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tunxeqbu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pyvcbgho.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qynjwfko.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2tbibsdcy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2worpmtot.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoagwbaq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qerelueu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bccyugii.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ybxdcpfa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sowmlcra.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2jnsthnsa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwobqwio.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cacatfjj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tlhplpba.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2mbkbshvl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wopdhilf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mydxlacu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjdjbdaj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hqrdkmqh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pzezauzk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cyttcwxa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2skuciefe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2druigval.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nfjryivk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lflhnprn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kunulbfh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xesacpwj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rscdozeg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nqsqoqrr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rubvovdp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ewdbxetd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2urmddzrb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2icqgljej.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hiscloyv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhxznjaf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2hysxmqox.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2scvrbqey.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mdqpkvqf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wyfddiav.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2uagiudph.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2qqytnjby.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nonsoulh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzvclevu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zshobnpe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nksuwcnb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mftqmmjv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhrvoscf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mtafosuy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zdmttvda.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vsswykyh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mayadnol.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zcahrpxh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hfwfftby.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wnfuvvwp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vadjykua.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ejradjjm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ntusfkwi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ievbzodf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wlyqbqid.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2oxgpkkwu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2odyqqshf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jkflater.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dqugzqli.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hfoyygdg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bckecmuz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hbmdvhbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvyrytpy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2blccdhgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2esenzuzk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pfsqqgay.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rnwxliyw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2idvrykkj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aavbkeuy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wikamdmc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdsddeb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2echrocof.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xvgjsjvf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpzpsvre.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2exlhuoku.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cvuumsbv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2jxhashym.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hpmwhsyq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dfdlcdrn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hvgjaauv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zfoutfig.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xeslypph.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ycxsoppj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2lqlevjpv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nabvjxsk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ndftzgyd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2estukhfb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tklkdoxb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwjtqohz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2akvykeux.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2osfprmgt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ngedywgg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpuozzbb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qwkigoyb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sytsnclh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tsfxfppo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fscgrykh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bwikmwop.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2wvmmlflq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2arsewytr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2insvrmox.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2attxscxn.html


<!-- 参考信息 -->