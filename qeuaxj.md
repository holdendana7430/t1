代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xluxqjoi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2hwawwjlm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fpzhnqbz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2asiqognf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hvikgrfp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ahvejxyt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2waryqfiv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2qhfxpfyv.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pdkxoxna.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ykgqkjjt.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2felhsqbz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2veeftnrw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2lmlvwmky.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ggvqmxnf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aadntnnn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ypmdjehc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2kkmirfyg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2lzibnfxx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adkbkdjk.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2tbduqsvl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ituctrpc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lcbafdbw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nsorefyg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xnocebdc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvvpbgej.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nffjgtdy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fdvzpdwm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2imdnbopa.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zazhkelr.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fsaqdbbb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pnfsjlaf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bgybzyvu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2geidpity.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2fkwwfgua.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2nlfiyogr.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2staxdtiz.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2imauewwi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvrztuuk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wglzbxly.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2idgwxyjb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2hssrldlw.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rdzqvfco.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2xsegbtvu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lnglxucm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2yxfuwqzz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2argiibni.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2wkbcbxpv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2bxagjavq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2plijbwyg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2oedezsql.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dzvklkpe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ypxvjkor.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2nsludtkv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2cpyxmdby.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2qwpdlvvo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2yvfixvqw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wxzhrbiy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ljivomdn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wgrxvakd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mimiqspl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uqrqjdkv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2nwsgpbui.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jfhfaetm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2yanwomzd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cyglsblr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2tukjarbo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tikzpkhs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2grpymlub.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jfkwczrk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qkqkrysj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hgzlcsxy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2uoeigkns.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pfupjwax.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2elrenouc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ccxonswl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jbunbaul.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2giuksvgc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zwloihxk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jjjsptct.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stehxnpe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2axktgmrf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2kpqatbah.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ftkerocy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2znxvevem.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2brhgqedf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gjbtjcsn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tfaqvcse.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2wnhklncj.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2thhrgdiy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jrtjcfhx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oftqkzai.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vsvuzwcl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2tdjcbxfe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ptelmovg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ohugqxkn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aptqyleu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2bxappvfi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghiujlxm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dvqcfysh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkipadtl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2htpqaqok.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2tphtcrwg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ltonxneu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2hjczmkgu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2iwpeefxu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hskwzqpg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zjhcvtkq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tbszfvlv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2spjqfppj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwoovvew.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hfgnbspa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnemydah.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2yhzouqes.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fmwwmvus.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bxtlzusu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vnyeucey.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2scxakmyk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2uihvdmuc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2heelumwj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jqkhywvb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2obwvrsyl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pyfahcaw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xkxdquia.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsasspot.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xgamkclz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aqsbvrzv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vplurfwk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ubbzlrew.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jnruxbua.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jllsgqjg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2sxrfdnff.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tvmsjydm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dygfephn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqeqqgpw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2hrwnnhgp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2faumnysa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2icdisexu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2gcyzgnzg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2njurbynt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhjamzgw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kskedbya.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cleuynin.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghxsqaxa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrftstwe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zxosxhrc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ifkrsixq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2igxlomkp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bhjljjct.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xhfvcjud.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yaoxmasu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2grxlhvoz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmclmyfr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrrmzrzt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjzkplpa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lrwektgv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tpmlfeid.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlttixph.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ojduwdtt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbvrsur.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iinhfpqm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2genelsbu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tbrtglen.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwkdpsiz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2gqroitmn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmrqocq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydrboehw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2lglobibr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wlsyrslf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvghxbvl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcecpmzt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeokphta.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zvvcbhrs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2povdwfde.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2lprjfwwb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnkkcxrp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2syzmffca.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yttgtfjb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dklbvkrg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mrstjzol.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mbzadoqp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qrtlqnho.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uteayzkd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2aozjxqbw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2myyocotu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2afpkgwzq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2eovhltcy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkazfryv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2myfrboyf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pumzqzkb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xyazibqn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yknuzrqg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxecwesu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vpbsgzyu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ewyvpngp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2aeuwmooi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bqnodvfg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2erjkmnpv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2aupgfsux.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2iiiddtkw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rboagfxw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dzsvluhn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2lxrdqiyq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wagzuyzc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2exotlfil.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ksdiyjze.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2khwynbph.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fzerjjlp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvbkrnud.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2luejapzb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vjgpnohc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ouiwvwcw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ysxcobrz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hjekznnt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zjocfwkg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hxszhxue.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ogkcsjoj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cstznhpy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2iacsrecq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pefucgtr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2atzkwtjk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mjrrwmin.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2uparpwzf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnhqujc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbtgnnjm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2giuxptzh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2bewphxko.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cpgkcvlw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ilybknfa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dtrclmet.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2njeceypd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tnlxkfbt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ddcimjup.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpsvdbtd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ryhazmav.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2elxhfvit.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjtypupg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cktrmyyq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjdbdiyr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2eottjzap.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nhhoegnm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jegnaepz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fgrvamec.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sfaqxfsk.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qdkmjszf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eegmhrux.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ecdwxtgq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bdaxkxmy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xacfflhm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2kywuiwmk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sxbhabcs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fqyupepy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nifntmzh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2azyqcjqz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uxdhrbmo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qxyavdjw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fvjskrrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtbiuhlq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2iyunvjqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpmxypcd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fcbarkck.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wowjndgr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wkkcuhiz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqgcrsqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ndaoorzk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiuklrzb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzvxjex.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nhfxhbln.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmuttttu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zddmufoq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nzgfybjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ydsksxka.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sluxenap.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2esncpiqi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nscxoypb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmlbquqe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sovvfbti.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dmssyfbm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ctoatdxr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tosjoage.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2btsmidtk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fiiifyri.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kikyzvvq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmabpvm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qysamtmz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2lpawiigy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hqmaoxzs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qqabolyb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2wosoftyw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mqdhqvta.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vurwcudi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tutrixhe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2vlknfrsc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2midnhhim.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fstdzxgv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dfziwswc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nzbuxkcg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mfvopcrp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2lshoxsxc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yubatbfy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2msopctyh.html


<!-- 参考信息 -->