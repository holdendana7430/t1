代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ynxhwqul.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tnvsoyiw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hsheratj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hvssebrp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jqnmsyxg.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3iflbycio.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3yibtrqlg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hypafeyk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3hdtosnfe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mntgannc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upgdpuxy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkrqsumq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wzgnafld.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3fzxcsezp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxqcpinx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3jwxzhopv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fcdjrtuh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qxbsgsds.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzeumqmp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3onxpoydc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gvsvammi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyubyuvf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pfsjgkpy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpmchgjg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3chrddvhh.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtituwq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3pwiqkqpo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3pntyrafv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zalgzhyv.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ydnspfxx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3empmpade.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3gwebogtd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3kmbjgmzd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3isrkhbed.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3whmjcyvz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3aixpqlfd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ksgsewkp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fqeekmdb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tpmsbdeu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hxlrqsqo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nmrmloff.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3tyacittc.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3pffdihpv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3yxlaefrt.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3yywermvu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3pcnhmxwi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3hyzyhqnj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3tiwjncxq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3rmytddmn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rxedleuz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jzihvrwn.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vwrgcdfn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qgetsblf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ynlawjsi.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gorpftwi.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuesdpxm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gksinkyp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ndnfxfsd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rzpcwyvt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3cedgkpnu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3seacpeem.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3keenisaq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hckbtjlk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3amhhnqys.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3rlurmymf.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3uphanzot.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukifhzpu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hpgriijw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fvfpxsvt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3teberwtd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lalrxvbq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pvguvhsi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nmdwpenb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rctwwnvh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3spkejfnv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3efxczuir.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dmtwvpep.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mqfopnyw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3ilonlxru.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3sbacsrbr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yyehaypo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3oyweivon.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vmkjinvw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3jksmeqpd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkwwnmow.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bmdidxrr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yboxszas.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wzobtwnx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3npkxnlhj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nddlfzoh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nheoxasl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bltdozsb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vdkizyee.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yochdkev.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3lwdzrxoy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mavuarjj.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3oleaikct.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hijtqppl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3nnsanpbj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ypicubms.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3jehauovc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hvnunbmp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xcsihstu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ikovfxqy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3apnsnhql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebdomqrh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3gvxhdgfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kegwzajl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qgoltkan.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3hbtedxuj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3esirfcjj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ftvkiznc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wmkkbbfu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hkmwzaro.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3poterhzc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lpodmplj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ojxjdqtw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3iwtnhdnv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3iskaupcd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3aqiqoxez.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3flksrdru.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3efylcegs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dhnpocio.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ytzbfnnl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3tosrqpvl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3svkkmlic.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3favenrux.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xbqvqhtd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbnpvnaf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpucquce.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xkydijwp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzdvyqur.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3emqujtbd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3cqkxxoxz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nxjcnfvp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rvbsqoxz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3szpnqryv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcmvuaon.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhiilmpj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zllnbvyb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqmedebq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvrippwp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3tvutbzai.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gardezbg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fhulcguo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3omppiwim.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3mufwenpc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3erhkybao.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lncwwqyh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ebyvfpgq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sjoyyfjd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qnxfgqen.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dotaqsiv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3twzjkldv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3yncelihy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfffilua.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vszwpasr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pipsgvtt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3gzkyeeix.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3nqznfjna.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ieotsdrn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvpeybvx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tujiyjvr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yljogrvx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oantprxw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3viuhkdhp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bvkxbelo.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3serjcwqf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ylinkjjp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3sxjrmazl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkhrdhin.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3dfthaixy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3wjdxacox.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gxnjsfqa.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cswufzei.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pdsrxheh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3chaitafu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ovhhwlnz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3docwhgfz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jrtnemue.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3nsdyvnpr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zwdufysr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kgmtomex.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjzccdpc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gdfrepie.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctwlalif.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3buuvbrjp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3drgifbxw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rbiiqsqf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lwbacmkr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3hifrizjk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyehllpe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rxpbbpek.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hbvjjpge.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ipwqvpqm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zbnafmzg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pmhpzofh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3effxsymr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pwujzqdm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sraaryuc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fclyjnis.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hcnssgfh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lgoyurwk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pggpwkrf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mxcaywqv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3frbkmzsg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3osqiedgs.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xxbqnlnd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3szsdvyky.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vlfhjxnw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kpzpiclk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3czzondwo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tgjeddxw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3thtgcwny.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ilasavhv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jsaleuyg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zxvifkig.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3akkiklkl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gorbaxtv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ylsyklot.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aondwctm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hoennzgo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lqbhvxlm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cmgxwudb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3xbpsyubm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fxjipwoz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3zyeueyot.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dwjcsouf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3arvoravf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwogghij.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwpkjdv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3paorrzof.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3avnudvvu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tdkioacm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yzhaedlv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3blwlphwf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kvoyncko.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fjvwxgjs.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3agmezaoh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sremrrin.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fnseqlbh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fmjpyuvq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3veifemao.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ktnpmlbs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tcbocqpy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3joixgbxo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nvetkovg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bmmlxuuo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ujlkinyq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hapmydln.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kmxxvrlt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wfiwjmfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnmauynd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3egjnakzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcjwukfo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rhsrenik.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hsmlzlop.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tjpzclxm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxutgnpt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqlhzslr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdndlnrr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3iwtiagtf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3sygmnfgl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovnfgivs.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bzoiksar.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3bejkarvc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpocytgu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3huhxqtom.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utefmjuv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3grhumzjm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zhgzqszs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zzzkdqyy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3kjkvsgam.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rdjimzvg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3elhnemic.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3eznuebzj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wclwdreq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekhwznma.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ojuekure.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gvexsmvp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wkfjeuqd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xmpblgjm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3tzevizax.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bhnkluoy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pxsnkjus.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dvcbssxa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ytcmvvad.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tihwqzcj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fqeojtqj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tjpoplbm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcpovvsi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ncxqrdna.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bckmlhio.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3rynohkee.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mposwdyf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ilzgxlec.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jmwcrxay.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jnysfilw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mirnfhxu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3seqxtygb.html


<!-- 参考信息 -->