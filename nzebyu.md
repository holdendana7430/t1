代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2dxjyldyd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2eqelnkrq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bftzaurn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqddiogf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2saxhnszr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xdzuzysu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kexbqdrb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2dsqnbuio.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ehjasiub.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jygkynza.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ftvnpuqk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eryylhdm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjjmyfhy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zerczlia.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ccwrraha.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ajtriahm.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2sxgcfedw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2evckcjvu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hveonzrb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2cvwugbve.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2djficmke.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2yhgpdynx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2wsiofotd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2itlifhbo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2vsrjphiv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2risrcovr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2glemxfph.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2vpeqnvky.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2sjedkshz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2xvmexzpu.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2pbzxuqlt.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ghnyiwss.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zryilipy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2sztpibau.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mndstaxh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2eabtrqnz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jrujezcu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2cnayfhcn.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gffoqmxf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2gvlshdne.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2fozrcqce.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2iezyuvpq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zaeyhxjd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2glejfubq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2emsuhvjr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sxjqvyra.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dilvuglw.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pnesotrk.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ufjqyafh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2repxvojy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2klwbrafk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jhrfbpuf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qqesvgfe.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ryitubpg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2kmhfpoum.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zoedmqpo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2lmkferkp.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fkrrspfa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2zkysbxpf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2jjxfsygr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ayzbepnu.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fhgvwmnn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kjbpcaij.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2pdtkgtzo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tvypzzby.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nmbiaoob.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bmfzcund.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2phpvakki.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xwuqdiez.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mdjulnhk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2aptfogkr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2flseblog.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ceojvakt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vowxcsos.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nzrlssce.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2qofpzmeg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2lwdskkro.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hezathga.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ztpquvoi.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yvobqczs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vnsoxubv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2aqeaqrgm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tkqsupxw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kmuyjmsp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yuugurtm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvkeloez.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2masvwmeb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2evgdyoek.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ztzcclpg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2cnghorcz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2qkvasist.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2wpydrlbw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ygtgteem.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mgkhtdxz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jeidcvgg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gcdksruq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hroquglz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxlqbvaw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2rlxtkfhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyetvrjv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jqhczsmz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lnynetdr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kywefbhz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2heshsrtn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2folczpxx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ltzwesvb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2naccrtxk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wwcpfsya.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qivrqxmn.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ursdyedt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2kuzoskuy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uskzoejj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ditvrrmt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2malzgxcb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2awfvdlsl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xlecsixm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ffumapnq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2msqsbjqs.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ssrnfuho.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2wxxberpe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jxwmrjcb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2khibxcwi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ccrynnsh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhkshayo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2pqyidery.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2zqvwuvld.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ognstzmi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hqbcugjc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zqmyucyh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cunzimwa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbourbuq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubgweamx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mylnueqb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xsxhmuws.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2hhrjgzdu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cveonhwp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xclnvsiz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nbbgwjcv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2ewiheceg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rccauhwd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vskcxcir.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgxguobx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rseuckvw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kyvupzuj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xratniqi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zpxskmmr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bwduqtty.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bnmlwhft.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2elujtzgz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wwesaosf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2etwnlzvq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pzdjpxxo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2faqpboui.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqyvmhmo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mdeloued.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ndcwnzho.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nkmuoxnj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztqwgftg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gceznqnx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxnjoez.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rwmnhihd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ksoltyhg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqvhuhny.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2tixrrmrj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zntvhejl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2shwkyrdj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vymzccus.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2spxlygsy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wslkysac.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wgothkzs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tcdnrwnu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rzjgfsmx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kyhrdutf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2svsvfjcq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmdmuyen.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gubfskhu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgmuxizh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bdpsjomp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zungdose.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fzllsvow.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cmsuvuxv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2yurszqtv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2eldlmlls.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2mhtpugcp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lkdzalol.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2faxyxxtw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2juwsnpaw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vwjudybk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kxtwceok.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfcljjiv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ghpnbhqu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2adtbnijv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2najtbmpo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xfhfudiw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2diphambd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tzyvlevk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tflbnwua.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ppycpwfh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bmxxdmxb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dgsqoetc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nsjqmtcu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kroivprp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2exeawppw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qrjkjlwa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2anqeqvad.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ctkzkiem.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rziwvwce.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zlpmilip.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2itxvzipm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vgzijotw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zccrzlgp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dahqiazb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2atzftbzj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qowkaehd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nfzqahze.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gfvhgwjc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2mzdsefbp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2madigmod.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rjqqatxs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mpueybqo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ppfirsqi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uapvmaxr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fgehlkqh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2otxgpwng.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ruurctct.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2btgafkfy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dhnlwzys.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2grcanieh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vkkctrfi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2undkmews.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2htvifcsv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fflpzzzc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hcogghrj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yvhjaggz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ouqektcs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2scvvicsq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dgjxdgig.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2iooqiscc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jvbhcldi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2toyjcvkv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pgdleqzi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fyqydrwl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2lruqrzwh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jwoujbzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxgqtlkb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nbjqobjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycsthuor.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2znyqnjhu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2khueazhx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2axiwpejp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aysqjkps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wmyyffgr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yuxqfwef.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ogmkycjz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2metsikua.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2byaaufcl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jzbatjmc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zligoevt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wumejdqz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxafqdqx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ezffvvuw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2pgdgkumk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zcivukpm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bwkrduld.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vwiqgjla.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pphfhgzf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qzruuytm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcwvoxvr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uoxzommt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgxhleqw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnakvbfp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2tawbfxnr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bafzjqbt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2diazanfy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2eereduqa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hfrcngip.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dpekvsra.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dvderpwc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bbgosjil.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xupbdcmv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mertjteh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vqedfrvi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aynvhnlb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ocxycppk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2eglxddsc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2cyxizkso.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rcibhzmw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ntfzecih.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2feudgzrq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pspitmho.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fdcnrham.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2reflarcu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wgwverpj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2mynfspyn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2antugucj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lolbkqik.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lojqwfpa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2icrdwgeh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zurbphad.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bsnngmgn.html


<!-- 参考信息 -->