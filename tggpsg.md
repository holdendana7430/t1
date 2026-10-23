代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dgbpazmu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3apbzwjob.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3upcfolvz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jrlaqwlc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bokjtuic.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3abiagvct.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zjtkxiaj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wxtsyqrz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3rjecfvnw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mktdepml.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mtrriook.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rmqeecib.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3elwjmnkg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jzkpfrxj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3phcvrimn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3gaybtviw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zaywusao.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3qsxtufeq.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ezwgcifv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ihubtvoh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3iveiotmo.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kjhlhghn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3khrolxwd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eauincml.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gxinjqqy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3igwhrenh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3usmfjurp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tawpyhgc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3agieogpp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3yaorkska.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3nwvhzxda.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3tgcfsxef.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3xniavymv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tiqehuhr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cnnizfdy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3aenmfcbq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3bzvwcjgm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xjxqiikz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtqbtgr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iatrlhpq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xmlltkig.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lvtkdrnp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3obwccolf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lxjqepol.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ixlcrjmh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tscbnteb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ycilmxnq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ujvckftk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sjjyhvyu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wauhntsl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xjgwtbzk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hltybiwv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bxpdwaok.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tduuolnc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3yrxtewtt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hftstffe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ughzufky.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jqwtvyow.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lnyquuvl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3egpsctsb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mhqcwmqk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ebfqxxim.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3lxvhvgpq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3lflmnopx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3pdqxdgdd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kwmzkbkc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jyadcvac.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bfehkyky.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3jwcvrlhu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3maxiqmph.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3bgxcfcpt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kbyvidfz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jaczvkxd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3silkprbg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mcgyfpqd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyxmvakz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3brrnixus.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jihbrshq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kmygeptu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pcsowvnb.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3omtufzhy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3bqokjapz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3krpcvjcv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3jybqznkq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3cnqfnmyg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ismvqvvv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3eiqusruv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ndgrnexj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vaztxejw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ungvoytn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yjtftxsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okmnnevl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jfdxiesu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hsdimubk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vklrxtwi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cdukxbqh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fmbswqrj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lolxzbsc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3iesrgekv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rlgbhxww.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3baliqhdh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3zwhyvdcm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3gcvykqbf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3iefluxpm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nmtegvfs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rubzorwb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ayfvbghx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3tforocwy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3pimfuedi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rjtgpcsa.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qwfdajjk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3lusfeswc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tculgudy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbduahxg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwopgnam.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3altlqmaj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3fkcgzxbb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3avpyhfix.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rmrjuhqz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ensoczyr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hhzhnwlc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xtcftghd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3forihqti.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mdgilevz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jajwobpl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ydatxhsz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lbnxqaqk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lczzhtzb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3spibcdqk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wmkijgvi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqxzuhul.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmdlrfbw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3agiiwtzv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfipvfib.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3jzeqcdfe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vwckmwzi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jxrdemwc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3biuucyks.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kkcwdmti.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ummieudd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmvkgtjm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxksknvj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvwqbqrb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3fnlzvsfv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pddzpapx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3smaqeyoa.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vewsallv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pxwmohws.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rsmgahqt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tbpvbjei.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wbxaibqj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ubswebot.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wqfkpoox.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mtsfvete.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mlprrftu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3czoyfglr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3sgtzmjms.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ewwegibm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xguyktii.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3diyazvym.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pnqmeeed.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ecnybjap.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3elbathjy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sqwhwsgx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jokimbqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3oosucerz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3niqfbxzw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ihemxqho.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3maacbadt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ionvzzyx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3icgslans.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3luukxcfv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqwwyagi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3suxnyjfg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3rydjuxsb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpukqnjq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ivpgqtzc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xqisexnl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tsvwxofw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jzctteeo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3axatleeq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ccjpjwzc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3eacetmdi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3atmqyeza.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cwxuafec.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3apopdcva.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xdjjroik.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3btynbecm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zfuneeod.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3kqtuwdeh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ryqttdzk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nuacwtib.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nxpjuwxh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xbpdyyug.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jtvbelzl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hvvrlgxv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sboqvvla.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ymdebcww.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cnhivfje.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gpluqdvb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cqvcckct.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3bssvtcgk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ddtxvxuf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzfaaso.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vbvfypge.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3brutwfgj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wizphtfc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ssuxlrkg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dgljnnsj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kqrtjcyw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3woazwivz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nakbjlwa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbkfquth.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pvlwiqxv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zmbnuwxu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bmrdpkvh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpfgzfkv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3drakizig.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wathcgdl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3frqsnmlb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rtqoaqnq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3papkssag.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pjqhcvas.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rgkjbzuc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kjgvkkrq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3diotpzya.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gnpprrwr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3oabohhqx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wtuxpofx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdjnjkqi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rpkrxbsn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xboslcpr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kmdjzwwm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3uihbcsjv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kchtpsvt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3flnirksb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xutqienl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ejvxhfij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugnvbbux.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pqkanuhx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3khosbycn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutrjzas.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3twjqxgqk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3syhywptz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzrhyhur.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gekzteab.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dkckwwzs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xajmziat.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqgibgpq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3yxhwwuxw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3eezprqrb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gbidzabn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uinlyusd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rprcnidf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrmeqogi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vjtpyimr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wuvzamiu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bxniubvm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3foddwmge.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhsrplnf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fesrjetr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nswcxuct.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcgqktap.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fyhcxalh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3upitcejk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dhxfojiw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ehzgmrpn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tdnwolih.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fpmhnbbp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ppgicktr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jyqdcika.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bxhulgqk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ifeobfbm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kqqeeigz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vlotjruh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pysobyfl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fvqllbsc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3cfafugko.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rgoisizf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gutsgayt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3gbsrqzmj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pheyrrzo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ztluvsmn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rwdjgcjk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sxzbelqc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cuvdvvxc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3sltsdnlt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xaycoqva.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dqbdodzn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3adnzsivz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kvqbuckc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yonadbwh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cfbnoull.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lvfmotvj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bmkdovno.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yvegyzmk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvyfeiw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fhvgivcd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rpousbmz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3erjdwqzs.html


<!-- 参考信息 -->