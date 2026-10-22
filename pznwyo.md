代发 wailian999

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hwoytbcn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rdzjdhmp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hglsilvj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2whaetfdm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2dvbtcxso.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kxqvmjoa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xowchuye.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2egcqoteu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jhybzrga.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rcpcwaaa.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wirmzmvi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kxpuxqpv.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gpddriys.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jseqaqee.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2nevgycow.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xtragchp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aeqxbowb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vllwmygs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wptoszls.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rawexsbw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2obinkvws.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ilfftfoo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2hxrpgyem.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2wgkawiza.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ptcqllrj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bagnofmc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ygslxkoh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ukqrtmrp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2sibthymu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yxlvwvgy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2xmvtqlnv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ncputvfz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bwfjucys.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nqeaosnt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dynjhnpr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nndynrir.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2azzeydan.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jolsvbyi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tvblxyjy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2btgaxgso.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2myfkzsvq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ojbgdorc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mwbekonh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fdknfaen.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tajacwmp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gykwtbmr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hgmwfrtd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2jqideyrr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2grnsbbeu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2oqyqtrjz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gskftvct.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2njzermdw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xmfzywhs.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dlzkfsyf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2cmyvqksq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lhmofmlr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hswhftoi.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hkwtrawz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gxfilcrz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2kksdpnin.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2pglfkrvc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ouwxobjx.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gmksediy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2mqejpoea.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wteazxsb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2npzkfnbu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2odojnnrx.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2uotxnpwv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwkuenve.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zcpovyrw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tirhrbil.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ywftndbr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2codwsxmu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bwhloqgl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iesseshb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hrkxlnqz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fdshfdqt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eaafcesg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jmuhppwh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2huwusomi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bgginzkf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kwndaqmx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqhzmoou.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xvlzcdlt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cvlaqyjd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qdbfmdcw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ctoqbimf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwnbngdy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nmqmipnq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mxxbihrw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xnjobfde.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bqvmhyig.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rgmfkeiq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2jfsaipsv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hduvbfgt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2coxoqyms.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ylrlxlbt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xqtsftvl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ajigahnr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cmwxthwg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2jwxfzehg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lyswkhfr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ldewdnot.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2thyteduq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ngavygcl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2flrsvdew.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzyfxvle.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jqtnpydq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2wnldvaqj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bckmghhp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dnddalcq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ncmemfby.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nvugqxzi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2botonmar.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2roxexssn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ksatbusw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rwhxvtwl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jiitooho.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2oazwobqv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jlisxqla.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2syornkih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ffisisrd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2zrgzeozz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crlqpuaq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hztnzjkl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2uyulqvmp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bcgcbkit.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zhryltdw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xbbtbdsy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2higxxffi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ygimrwof.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2rdmyehem.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pbfrcgph.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2yialqqrx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2akfvabzx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gytnopqk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mlpfwixm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nsqyusid.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qowcjjjj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dqhgrunj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ngzrquyj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2diwswoes.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jbvhflml.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nyceorqt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pxmxstvf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gylwiprl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkdqqaax.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpzxmevg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wxvasbfa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2jmadpymn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mzfltncn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2crqrziuz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bvhejwao.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jnauuhyj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2peekjxlt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fgrtsjxh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2bgctxmwm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vreujzcl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2oohkqott.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cwwneqym.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uliandqj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2oclazbje.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2txphfnlc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bgairuej.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ocrxhmfp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkwoynob.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xlbgbelx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jireicsa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wywrvjoh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ksisxnho.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vlgmlple.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zeubnfon.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rehiqibn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnqerlwm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejispccz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2hkrdpjgq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gcvzgnsh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2iimgsbfm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hzjaszlz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uonvkcyf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2kvnfcutq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zfzqrbyl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzsfgusm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejpdjtgx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ncnreofz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ceioxqry.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxifbeqw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zurpziuk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vheedgip.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lqdbfebx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uawnzwlv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2unvgefuj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hcpysipm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zquwadez.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lneyfrcb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2takggocb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2memqvaln.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2yvtslddf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cnezwush.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yfyvjfhk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyiqhmlz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uleudgxs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fvpezgao.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sfhjixqd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nfcorpay.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ifxrtjej.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2enrrktzw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtxgbhxs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2csjjrrek.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qnzuapav.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2blmosfci.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2otkcgqha.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2lpyxykyg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2pyemhpov.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2tihdcunu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mzofkdcr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hijwjcfr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2senpsnud.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dlvqxoxn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2urouhohq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2mqivkczk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vkngvegj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lysvdzhy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wlknzkkx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hgarnwzi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rxybuiyq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2djknohsg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dakozoib.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mshybpjb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2buvrsdil.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kiatkqar.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wrnrqznc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2cnfnsepu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2safxuzif.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xacubpzy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kajaqwrw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xiyllhgc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2blaplnpt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ceftbagy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2zoaviomd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2voemuozq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wbffqfyc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jjouyrxk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2xotxypgk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmrnbex.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oaetqdxp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nheugqar.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjnzwvaf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2enijjbig.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rydsxgfh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2uyaxslrj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2frkwalgh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2sspazryu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wigmhxzr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ozyluhbj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2abhiwpdc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qzxnzyhn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2czcxcqil.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wgqknckb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2egkuayfe.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2aswxslov.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuznelek.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jicunlef.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xepxfomr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fodkndxf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wjpombju.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2svdqsfoc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dpmnonut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cwlxgman.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2poirseto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fktwnwho.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fbqtnhvt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kgktbyrs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wfbswubg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhrjugjx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnwzhyp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvirfick.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xmuqwuzs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mjgwtlbv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fvojehnc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qdzritor.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2icxtdtdj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ypoqurji.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zybfkjgq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tlejhgld.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pwytjfbp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2pmdczgkw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ibcvzqav.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2obokhqup.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2wzwzjqab.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2pdaikelk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2omprlhqp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yeucjqqm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgnyvrqn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmlzqrqt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xchobauy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2nhrhckmh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xzhbjyrv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2umkusqfe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2aslcaoge.html


<!-- 参考信息 -->