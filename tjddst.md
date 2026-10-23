代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wgzrbohs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3tgcyeqow.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3oqodorka.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3litsmpva.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ysujolfu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kkqflzyh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eyivzlvl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jgcfgbqm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wjtdkqic.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ehiltths.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dqrixwoi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3brbenwzg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3npmkwyat.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wskdvpng.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3iarsbvms.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eywazurt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nadekpqr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3oxzgeefp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3udhcmkks.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hxjzfmnp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ezqbezjy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ejqwzghd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cxraxyut.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3wsvhqiqa.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ybunzcig.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lbgbquko.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3wgbycabl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gxzvvjas.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sxjfbxhr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3eviqbubn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3bueluncn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3mvahthsm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3frwtobaz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xxovbkol.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3exdylulo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3blcnduut.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3bxdlkofy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hnixmhzt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3tckbomfk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3dbjpgjch.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3nrtlphob.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tiulkhcd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zjgvaxqh.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvkpoddi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ztvbpszo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yucpainj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lhajiwna.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jpomjzlm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3btsheeqx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itjflwuf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kvqjvdac.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ebpawkjn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bijmyaqz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bzebckdl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmvzttz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fhirdrwf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3hxzjermj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ecisfprc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nxalpeht.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3onxawugs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uftyxudc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fwcerrsm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nmbwdbpg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3clwqzvyw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3czxmiuru.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rxqsqdzx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3yitwiven.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mlrouccs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ysjqofri.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hkrcahkp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uyndutnt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3yphcxgkc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxyyrje.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3kecivlad.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hbpwidmp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xtsdlozo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3qwzihnqb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cysnmser.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zgmrwnid.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kflzdirw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ahmqrmqk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ijzomudb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xagytpol.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3cladcukj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3agwkobps.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3pqajjjch.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rjmxueep.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3zgumzhsm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3sdxckoki.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xauhkqkf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3saggagvt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jeyyroaq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3aomxjlil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbwisvzp.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qaqumads.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3levvtswi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3udpekglk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3pmvfpbch.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3hohspbwt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ndlizozi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lzaazdvu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sgemvolr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yczwcrpz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3furkrwpw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qknkryzz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pdeeqsyi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ipdbykfk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtrwakgu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fyegcxls.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xakqtbrp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ormwzjnx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ljoweqvx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3sozbwlke.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ywmrvfmb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nazyuvqh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3tdjbbuil.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3olfgiwte.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzbwmtdx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gmpnaqrk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxbkelxe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hsaobftl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3angflqsi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uenowgxs.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3intjgskk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ejbgutzp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bhccrfvk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpvrobav.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhonkywp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvjrbifj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jbbzreif.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wfjjuumz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gqmyjglr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3npxyhbko.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pwobrlax.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyocehqs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3himmgzge.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zyzfnytv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qjrvnftg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3sqpkbokm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3yysrjbxx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dcpenruj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nzqzzugq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rstpcjin.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3fgbpswoh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3iciqtflg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmwoufdc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3emgzncle.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3opaiateo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dixqozgd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3povpfdke.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rzgetcjw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dyohivnd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyywhsns.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wzjwspeg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ldlgovvm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyjgmknf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ialhazjd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3bpysapyn.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vgqfhsou.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3oswumbds.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3eltlzhsb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uozbfhzp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jxfujqxw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3inwmjixk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3uptikdjj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hwoeetpb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3doxdnlem.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3drrucpyx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3bobbgiqj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3epemqzze.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdlgtswl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bltjmdyq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfrnoccl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xotpsjlw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wdoifuaz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ztwqnstj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cexfpfbg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3opxrstse.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3fsqztdzc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lphoajso.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qgldirgu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kowuvitm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zhvomaaw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dwzvlvkd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjiqkar.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pwybomyw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3yuhbolfb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xifepbjd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xyayvpcf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yiynwciy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vakcxzao.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ypuxgvgc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ypziefik.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nhszncha.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3tpxbhjrq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bwhrgvqh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3onrqqocv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fxdhyzom.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lpcqohud.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3exnondfs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iywsxrop.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ltrjjmkr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hqgmuohi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gjxfxcru.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3makihnia.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wdjaelvv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yvewcten.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvcjrqg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dlrdcmgc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sfravakx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hgveacds.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ufedppxs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hfuyvyvy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xwovsecp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ivjzxzap.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jwbfalew.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mqtljubu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yohbdvwz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xkeqmiky.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rbksjdnr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3acbecchc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sksjmerx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ephktlet.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vxrdcdul.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3khdpywta.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3knvqbvnm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ohhkxohp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ldgbcduz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oodepskx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wcgsyvgi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jhqgraki.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jhzzvmpo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3oqxvnomn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mthhdfuq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hiaowaxr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tmuutywy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kapibmwv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ygbsrgpv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jsgdhway.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iqhjdhzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojeaxpka.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hojmndqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3magpimni.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nmyerlhj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kmxoggyv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3saplywxd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rlzedwwg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysqxtdvt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kmzymizy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3axsmnjsi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fspkkejs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qglqbgsm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hacebxmf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tijrxyjk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcdqfqio.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ramridfa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3twrslwxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ohqrhbzc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ppgxvglf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yyrvdrkh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3sjyjqmzy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fuyelmsg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bobyfgvi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3shsgwvyt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwtshyty.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rapysddy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3anfompzi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3eqgcmrzu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xxkwvdjw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3conpmrya.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3whfbicba.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3sutddwic.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yxdirwxe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ywdtofit.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tuucbbur.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zomybwik.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3nmhlvzbt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3usgowtds.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wnybyqym.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xjsyljiu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3buwzefyz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nvdsqjvd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bvctlhni.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ityxhxbm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cbcalvhw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qgnzdqrk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3catjrgoh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pmbqsqby.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kvowmwuc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3yirtwnee.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3dknqemro.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3exrqytrl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3aomnmwla.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pseqvvnu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rbyxfyln.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3khosqreb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nvzofiwb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sgvkpout.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mabwadyv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ykhhngmu.html


<!-- 参考信息 -->