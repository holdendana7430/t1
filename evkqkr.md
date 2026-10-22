代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2animlemw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gambibkk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lofekmij.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hcryezpk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qrthocoy.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nobkqyld.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2eqdmyhuy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2bfylgkmu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iactdxvx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2czytmgce.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2apfbqkss.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2zwbdyxmm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kprxzdkm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ohgoawyl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ecempeft.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ldrqbmto.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2zcskscji.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jtlwjlbu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulmnwmyu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2kwzjmeft.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lfkujeql.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dyywiivy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gzvgdrkg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xpctsoay.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jhtvvfah.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zbefzbxo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wyqivbgn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tldysnvq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fgbwaawz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hvnseews.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2xtqkqubf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2eatdkeox.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lnzlsfvg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2tyjozgqs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vmiaywbd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2pbyqzlfr.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2mxastdiy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2wqfzovqr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2byjuzdft.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2zomkcuxg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rwoufnax.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fndnnxvx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2rsvpvtpe.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ntfkyfjz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ysvtgvcj.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2lgsaspeg.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2erstwdva.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2mqsyjsjp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxnand.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2yjdxosei.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fhgajixb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2xgcduyeu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjjodol.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2pmhitgtr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2feocwqjh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2iuaoxjiq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2haedikcr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vxptefeu.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sahlmewx.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mksmrdgb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2omltcbma.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qcljkmor.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2swzukvbs.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2raeuuikh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bjlgedds.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2dnbjdhlm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qpahhjsu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2wyilnsgo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qdpuomxo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ianztqaz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbtkccxp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ywrqftab.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vhrgeuvz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ykkyelyd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2mnptthtc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjmyvna.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rzydvxal.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2utlauyco.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ytniopai.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2zubvmnqa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qozzznry.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2owhpkerg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2cyicharj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ababgdoy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjuixtkk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ikjnokaf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ihfazaoi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kgmepktq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ucudlyud.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2wragaqpi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2urignhir.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dgqpfczx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qohwqijw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdsdyoay.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hixovifk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2silxcvbz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2kcjybawz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2byfyjxzt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2hipsxizd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qpwcqnyi.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2rcilzyav.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2szkexmol.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2aphqdley.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2sskfwzmk.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gzwqpieo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ywhuceml.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rpipionz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mkgbeomb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hrjsrbia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hujqebzj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2idexvefb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofqdhuvd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2olnnfltu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2tkmkgrkf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvkcivbc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zxxhhjne.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sovzyjtq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dkncvogl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2xdxjqxyi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pbwutsva.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jvyaggab.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2cagsnbfc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2usyqdwqk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmdnsvjb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rfkrpgcf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pynvvttv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hyhturbh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlsqhbf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2eamwllhm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2twflsihd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2sfjjltpn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2qhaixahh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2avmyuubr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xrzwdttl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ofcrjfuw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pyefozet.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fxtpdgay.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ojhzjdrc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2scsniwjj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hflqebiw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2uqxwyfor.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2csmrhkyu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxktwypn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dtxlahrk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xrkuphff.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2trfpydug.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mkkxbjlt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nejodhva.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wceufqpc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2fgdttbhl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2shdtoaex.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqkfkdzu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2trthkjmm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbkhhmqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tyvygfec.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xrfcriwt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oomcedke.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2mjndmwrp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vlethloh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2klpyktrq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qqnhgpdy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sphowttz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2bkttwmff.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnfubyt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2yqmsuibg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ifopdzxo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnysjfps.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jefoztos.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2gvhlmqux.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzwfdwgw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbimmjoj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nidsyirb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hdyfzbsb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xqantevh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tpvczxon.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2caamavyh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2gqnbxwnt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nebwtvfz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qajpnclu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rqacbxrc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pitpcast.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cjhvnslr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fltkbnjj.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lbvewvre.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wayqppqz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mojebvfe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2desfsbyg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bhtwclpk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzejuzpv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vkfvbepj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vqchltja.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gqqmouxf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2smbjehlb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2jqnuyszu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ebwxvvye.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2voifgsvi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2exrxteyu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nqkldcke.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvkhqsqw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2lgngqiar.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wmwjwipq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vggzegcw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vajeoedz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rfumezkh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2iqaurfvs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2psfehqdu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mhfwmvze.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2dphjgrwz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2psbflasb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bkwdlnqe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ckmmpgna.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tbwgikwh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ozvgmgrx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2semtfdme.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mhsfaxko.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wilsdmly.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxotintg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yzkafefd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mslqpppw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2flwrtfmz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xdzdwiwh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2thymabnv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jscciqle.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nbldivjo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zhjhjrql.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ubuqpqmp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bsmlcobn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jdjjcjqq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rzjtunrk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2tbwxlxad.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ytsjathm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2onugjgdd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxubeni.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fcscebxi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2danhbclv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gtxvssfr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2luiyvrwf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zthdscti.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2expbtwpt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xwgzbuyj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jnatpryv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2revwuahq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xofdjvub.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nhepclmo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xlxecpge.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vsaoxbuv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ustmujut.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rigdrftr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2oiifppzt.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2syqllcgj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sqvqbojy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2filenvlk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bedhgwbg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qnxdisxp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pjozzczw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jbpamirl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rczmlxac.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2zwbflprh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwojemhj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iiknosko.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vpmlbbwq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgmwgsgv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qqytwdwo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xafrgqma.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbdvfsen.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kbuekemy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fltamfzt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nynnwzpe.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzvalbhd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2eqqfjhnq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nzhkqckn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bknbelqx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ihjbfixg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xcbqiqgt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kgnkuexs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tdqigbon.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2frmagvue.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zgshjyqn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2msmbeprp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lsrcpecg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmxxmavz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2chcyowfi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aphlccng.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2acntjokg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xknzwxyb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2soxmagij.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tpnfwdye.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xqcaugvm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pwuuzqsb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqrsnwoh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2arwwwzev.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rrbauken.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hvfhiqzy.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmqvibuc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rdjniigu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2efmnvlws.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yrdenexm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kjowruel.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kkijpdwk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vsyrwopv.html


<!-- 参考信息 -->