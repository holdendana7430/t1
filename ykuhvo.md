代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sqyequcp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wzzocwib.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vdgcsmbh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zpeivqiu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3hpssywbm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jxkttves.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twgajwvx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3bweughbo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3kbskktvn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3oajjbbgc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3zmjcpiwt.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3xtrqqobn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tqyopyhb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3plnblwxo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dejtjgpb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3utnxmnrb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3slartqmn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3khcwpjby.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nywnewqq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3enyeihbp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3exuasyub.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mdgralyu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vpcoxplt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzbkjbv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jdzkdjio.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3upyseyiy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3eszmeybu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3awxxvtvq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ukpccjxh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3otmwgwdi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3btwogzjn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fcebnhqw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3egwzulrp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qoskabzq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3javgyjtw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3glomfrwo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ouojgtch.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3spvasnfq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wqllsmbp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qqsyonkb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3sbeuiaga.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3yjiojyvv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ksnmuymo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zlscacon.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcuvpfd.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qgtjwxzs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3noumqkze.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zxvtyvwa.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dzuwlvqw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wtgyxvld.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fiehgwbu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wvngfumk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zrxkmaqj.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dplsejzt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tzoubywa.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ovwusahy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qsenjuht.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfgvqfgs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3qdhldskf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3thzttpxn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3kutogdeu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3fbudorpg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldgxtowh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lgwpqzte.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3muhwmjpo.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mazxqhnp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3fsvzdtdx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3seoyugvy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3idlaqbaj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3sprzljhl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ooxvirey.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3unsqkkil.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xcylvmba.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qfolcpwb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3upeovptp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ezyqjzmf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcdxcoup.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jyxphpsx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fwwitnuc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3pomlpybo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jknymrvj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jpembwwt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ecarwihn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nsbbropr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3vhxwzycu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hfmqbmbf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3szluisgc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3inykpygz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mjvfmnot.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3atffuxin.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3cieaaabx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mscpiydh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ojloczng.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ttcwuvxt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3nolunbxo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qsgpcwrh.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fqcjuuxi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tifxkhhh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ohioalwk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ntxadbgt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3keovayqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imgciuts.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ftazumpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wznmhetm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ucznbpgj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uaxbxegs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgusbaoo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3geeodqup.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qcpkycca.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uuyqwwpz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3irazvftf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3bbdndfzf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uftbarfk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3xnzcslhz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3vvfnlfof.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vkkbiohb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zfkxwrvr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lgwgxxlt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hpmoyxoc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3porlsvbz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qhcvjgkx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dvptbjty.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ronawivb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pgjzmnoe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjpcsgco.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsqxyrpt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oawvudlx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qgzqiido.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fxzbcpvt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rxjvgxxw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tzgjhbpv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wqcqgfrt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bkapdunb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3fndoolep.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vllxblsz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzfnochs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vyblhqwr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3xiyyuvnq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qlcmsvfo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmxpjeby.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3orcxfkoz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mqecthsj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ittavnuv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugjnfnmx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pxojczqq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujhnlozz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ncspzoef.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3rsftywht.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3orovflzp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lhldvcjn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3bzdithfr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ztgozqvn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqxiqniw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdohpuzq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgakiiea.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3cbvftnrr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3iqfwsmbd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yhxokqze.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3lheggmfw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3phcqcuec.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3sriuahfx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tluewzzt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ujznsceb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3etydsogk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3nuvedbzb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qshlvyof.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3loandkgu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3emaozvrc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wpgtbhqn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cwdoezif.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eneshpek.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wnmccagh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bpydpiei.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sbjamuuf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rkeqhvev.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sbdnncvm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cyfiaerw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3adkcfeky.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjdtnymb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hshjapha.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qwoonsvq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3beoboxza.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rdilxbsy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3bljbpzrg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybwdmdtb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3punnzwhc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nazfpurq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oqmetnby.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kpwvpfds.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xqugvmdd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3idlgamya.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3elxlrtoi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uxureqkx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3iwdxbirs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lnlrnhmc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hsmncwnu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3cgkzmylv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rtuvoabi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3imgnctbf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3tyiwhtrt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nnbpiukr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3aqpdiijq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kzzvvyqc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lrldmulr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cjkvxeta.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qoyqyeoy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mneishpv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kqgcviit.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vnarxpxq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3aedfmnii.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kozujufm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kdqdvuke.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ktscukts.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3rqpjcjfn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yjdxhzcw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sovbmzhn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3kjikkfmz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mzhnvjvx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3opdzaftr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mdrhrkhu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rpzeojjv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mpzsjqmv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ukgqvtyp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wfaydfdd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxjvzfoc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iftpokhi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbvobzeb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hcdfracl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fghqqejb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jlbwcekq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rmuhnchc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3todapqcs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fkfzzogo.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fkiosltf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3twkilcbo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nvnahvpw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ruawkvsj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nwwfdwwk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oievxwov.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xoxdlezl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cetdgtkz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3utxynhpj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vopucscq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lfxjgcgj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nufaizke.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zoljybxb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ctxltbnl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dsakqkrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkwevngf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zizdujon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvctkbeh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bheyfjkv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3edvmlptr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzzsushq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcjtsutw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yvletbtp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oanwncxl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3puwkjtnx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oncfxsvw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jlrwbdrr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbnnwamz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jgxbwslt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iweupvca.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzrqrrc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aljgrsrs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3icaabdbl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ovaxteiu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qnegwalc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jqgcvysz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jynimiva.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hmkozzte.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3biocenfl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmstswwh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dktovwqq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nvyuivcf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvrruum.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xonxtlvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yzayowoy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejlrqdrk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lasnbcda.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lrgjlnfw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymbxftqz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3lgqzndbn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3edzmvhgr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ptdmojqa.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbgwxhfh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xmqudway.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3yucfntif.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ulodaefv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wfyrgqbm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xeheeuzz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jtcelsra.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vrhwnbiw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kacnypma.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fskzrtso.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gpqzqqgg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xbktynrv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qndeeiul.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xhjvdtvs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nylzvpcw.html


<!-- 参考信息 -->