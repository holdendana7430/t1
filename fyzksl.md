代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aurfefqe.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kzqzamxx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ivwapcph.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eqnsnhrf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eedhcspo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qwhmjumh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uhemzkvp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cyyrotbs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2zalqjtxp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2nmdkyoss.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vexptyyt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mwwbqdra.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nxrwykoq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ncmjzihe.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uwifztuh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qdyusirs.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2imxestxk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lcoefqom.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qlkkqnss.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2knzwbrnh.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qviowhzn.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dhhiebsx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2cfqqjxkz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wbxhchov.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ectllvwx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wjrkpfok.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2cesxdbus.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2cokjvpql.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bkaqmoqy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ngataboo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwiteftf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efzozvqf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2iapynaod.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dpdkmrkl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbiyecoi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2stmvpzve.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2buopyxgm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rgqrsbfa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2epvpbvqe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hcwqbyfv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2apmifxid.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2quwsctzz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rrqxzfaa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2obmevvkl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vfekavow.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nldgpwyl.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ckvtocpx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cdkomfwm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lebnrwzo.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vfutfxle.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2mdxctfce.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2loifwhkh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2khlmbfrz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkbppolw.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vhdflere.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2jpgfwwnj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2lzpnayjy.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cpbxqhzk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ymiastzu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yffbbruh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qannoaou.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zspkptlg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jxtxuccf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rgeydnxi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ufhfadxc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2klkxgedb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ycxghjbf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2wnasubtx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2uzmljnut.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2lzuzucpx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2skvgkjjv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jmjfpcsi.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jzdexknv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ojwbqpam.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gefifixp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhajaui.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2frxrdfuk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gfsvynmc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cakycpmt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2hkfsoyde.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pndkkuvj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2slzpjiqn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tmmscbnh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rbocurjz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2vgqqkolv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kpnlpmat.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2dwjdrqfb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2itfscjns.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lmvuukqf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2piywqzus.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2cgruifok.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrygxtre.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wulgtbly.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fviqivoo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ysvawdqb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2srmfvnoe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vjyynbdi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ievmrpii.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2mzzyvnhn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ayzfkzqi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2nbxlrztm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxbaixcz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ihggepys.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wdscsufd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2aexfkitn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rmfybxkr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ioqkifva.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lyedvqhi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2zckuodwl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tinpolwy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2pydbeqsd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbgnxrsi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2hifferlq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2twlwowhc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2wfubovae.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yivtvnkf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2zvezqpxn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zspdfean.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2urnivcjv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zqptunvh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2vhfqulgq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2yjihqkdg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2idqtdpep.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ehldhfek.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tqadzige.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttnrzhjz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xbtmzzpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sntojxpj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2apgksinq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gimzarkc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfaoixnj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mqzgcscu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ygydlyef.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2iuncplzc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2imyrugdg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2yfpsxyoi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2coqthhnw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2sgfzsuby.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2pdbrsyeo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2krziwgsl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2guyqocru.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pmlwlnqy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ovrnurmo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2eiuqeedf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2cbehbjpa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qtvqeamk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2skfwfvnt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ifbyvows.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2btwrmmri.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cysqudgf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2amcuksju.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfcsxrht.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xamivqii.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2iuxucqmu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2fesmsimj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fsxuoiom.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgrtzoq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2njluskvu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fgmkdvpf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eksuqzgv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pijvxpau.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2mxblgsej.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mnupfbfa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vbpkuyvf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mlptfjty.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jmoxvtwt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdsxwkax.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zslfxkkm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yditnixn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2czfigtfr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rfhfyjcu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2crlfqvai.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpymngqh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qooysmid.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2svglbzmb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2roiwfdoh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gygxxont.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttiewmjb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2epfpyodr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2xxjaihel.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2brnnldvp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pomaqaob.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2jqbadqjp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2hwrboqky.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eflkhtbn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ujvexyig.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iciobuco.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qanycvqn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2etikcqka.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljirjiup.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjyavous.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jrisbaan.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ydvqqtpf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cfrydaya.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pjkrrjkr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mzskmvyb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zhakvhqa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ucqcxtxe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lavkfvmi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hajvjtcb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xjcpeemm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vykfplyr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2urxsumws.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2slylxssr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lasyokjs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkozeotn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zifkafar.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2meilxtcs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwmoztfp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fshzrtgq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zqjkgufs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqcdbecr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2uusabvqx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zpfmiswk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2snqhbmfr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bblfhxjg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2diafpdnv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rckleozm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2fehqyzlz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2nktoaptq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eqqdmepg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mmrrvmfm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qzmpimvr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pbyakrjq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jwyrycvt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pcamrcoo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uwibnacb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ljvuwrou.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hihujzxt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ngpcrsic.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2woosxsmo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2upqaeuhn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qvkrvpbu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2vrysswui.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2eyhttfif.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ihuelavv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vivisxsm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2biqdoliw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2hhayjsic.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gdbrthpq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rnhrvnnw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wypgcwjh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ugwyvloc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2auaibskc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2pigdaryu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zdrfdmrd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jefxxdmr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nomlvreq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rygfgkly.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwigpenh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hanzidke.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsuanxye.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zfejpmog.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dmjrunza.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jfdniifx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rhkrceey.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2yugqfvse.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pcyhoedy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ualqojrw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2febqhfwl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rahyhtix.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rokctxqg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fbwtgllc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oxtixcwq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jvhafzfh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dejhpkdy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2itnxvbtd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ynutsydo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gacvtqob.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2pviwkojd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qvvnyrek.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gxrmjtxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvnrpsto.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sbezdbao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjnpgtkm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rhmolesf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pudytwsi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzowtfih.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2menxidqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdyskske.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ighbsgqn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2gmdozzqn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2kdmqfoln.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vphnyheo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mqqtylih.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qsfartjp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2tlmhwmtx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2daheqvyo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zaoqnbab.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qtcaeaha.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yfvlmlap.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2uivavavh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2phsknano.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bpkbsxbe.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gqgfttsy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqwnmmci.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jvfdtzeg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kfyjogjn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iteftxmm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2evgrxehs.html


<!-- 参考信息 -->