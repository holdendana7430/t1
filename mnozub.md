代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3fnkbjrqh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dsfaghpc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3weokyinr.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3fycmymjk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rntwcknc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vqcbnxar.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ektrormp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vzmxdmse.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wanulcsa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jcsxplxx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwuynlex.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pvaacmpk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wmgjzuqk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ulrngxrd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3evdetajq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mnebtzjt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3snxfmlcc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3keaejtlt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3tkysukqh.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hfefyaeu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3rshhputj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fomrbihz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vuscqsjs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3sdzzuaox.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gridclbb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qfkqpnox.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xhajouhp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3njrwgsrt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3euqlytwb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3niswfavn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hechssqk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kcrenqbk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3qhztkids.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3vtgupomk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3bljqezyn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3gtkqbibr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ncspfuvo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3dmpnykql.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3didtaszu.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xixiadss.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3gosftjtm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eajinock.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fqezdcqa.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xhfpobgh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3atevzdyk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3caymkhkl.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3foxwisnw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3utmswtog.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uycbjylm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnflabie.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3crfjkkil.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3zuktvwym.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jvzxggsl.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3fxqipmxy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tccpnkyv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3syqncnke.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hbahlnyk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3isaotrbs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pjvyppcj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jqkemwve.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3zykapgoy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dnvsvzjt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uoadrivz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3vezbwyen.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fceqvrbk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dtqeuxnh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hycpakrd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3lepvnsqw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3nptmzllq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uueorewh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gwzbqhbc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mktgowxd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tjssqafv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3gunxejwo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3glnonhzk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iepvxnsn.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3tsmxfrjz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3iqhtgwvz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hyoeonxq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpssrvhv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3muuweebk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nfjjiwwu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gjcvuixc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oennkhai.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dnuliiym.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3dmcgmgmm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3dhexljqc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qtxqttwl.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3oxrmvtep.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3rfrvodfb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3dncwnrzh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iitqtrhv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rddiaadt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcwcpkhn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fftlpqpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecurayuo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3qigkezrd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zcdgvkdq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tajmkvoc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oouhhhax.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fihjqtxm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oyuumred.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mvtwqqym.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vjcltney.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mslzmwjs.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3gpvicbvv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3avywckqg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifuqyixm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dmjrawye.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ylijlmfk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fqbbbjhf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kyabazwl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3rrsymerx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zcejdljs.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bqkhvgrd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3lwqjfqom.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukakqcsz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bilaqdeb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3idxmwggh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfqnkfsq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yyhnfvhb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jerwfhff.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3stejvzgc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kddlryzl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vdjsjasf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kmqcrayy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zphwuthb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlesxmyf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pssvnqif.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xitxdxoc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kbwqcjex.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ddguotjn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vmyvrcxt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xwlbsoky.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dymvmney.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeteawsv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukqjckei.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajvzeuwh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mrbdtxxi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ahgbhqni.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3agwxuqkj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3epwxqqpo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rzekdqju.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ntnohlvd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnwbuqfr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3siihnzgv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3digzhyiq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tcagchkg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3pqwsxjoz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ubblsgts.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zgorcdjk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kejbutmb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3thaxohar.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3shfdesnc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uuhzaihl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wzzzsbdn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3itpciitu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jprlqkmo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3awnyyjjk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zadyipkx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3awwsuzwn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pwzvbhcl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mdzzyfzc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3huzrpynj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kmwxgszl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bpkegmhm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wsqtguuk.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3izcngjha.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3uwpmjexz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3spmewaqa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qfonapqz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jhamzzjr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hhtyfoyx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bbrlirbo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3efdiyaqb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3itlzlrca.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xscoopuz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3pprugcud.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wffvobzu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3pavvzewd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zsjlhwmn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hpbsiwhl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fnihubqh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rcdjpfsg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3avdgcuel.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dswbxtiu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ayucbvox.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qejvhiae.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vinptkod.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3etrwtxan.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dkeokqgp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dzlsecxz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3chjwsboz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ybjdzjdl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3twdiqmtc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3mgbgvjyt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pgqlxzxk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qfoleqjo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kduufrkb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3swgmjknt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rsnezshp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpzmwlwr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hybuliia.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3jccvbmrz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3frcwdckq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vifevdoa.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qeulxsqy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynipldzz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgkiingl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wrwoysfp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3smrjscpp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ejmabgvp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gnghcdzd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3psjlczjb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kcfmtguw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gecxervo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjaealzh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3olinczye.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nhpjfplb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zokflugc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qwmaifkx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3alsybmxp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3djqoevlc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hdaarcvc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kddbifsw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ksumbuyq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hqsmonfa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kefrqnse.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kvtzcqij.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qaycjhpf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zbrizmuw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3svjdgoqz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vytvyayn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3gslzypgk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3afpdcacv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xbgdvjvt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vtlomcti.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vxkygphc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ncyisfgp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dkwwcspt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwxasnbz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3mpxievoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpvjefvn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yztrokvy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wtolhvlw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mtmcnnpx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ldadvbsv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tymrianx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znqknanj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xtxqxsef.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gfrjiqxc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kljifplw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sytbwskn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vjvomtcl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ukzhydcd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xasczoxb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qnunxcxg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3foloeujn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tcyjnhsj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3uqohhrrs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ymlwfatq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3urymlpeq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gvbpcpci.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3fxzmingy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3grnjuyyk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzbvxdzg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zetkbzhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bhxrhlye.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ozyfjryk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qgyalkwf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wgikgiuk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gsauakpr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3avzgxilv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bvcqqfqa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rzdjdeig.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dbpdrzem.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3svllfwyv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qizbvxvt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bpwcnaru.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3egwhojct.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tqzfakys.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3anyvdriz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3urpbkazb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bzqpivof.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3gwwgiodt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dfuoykie.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ljtmsvyz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3triwvlsj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kwrbhpne.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vhhtdcpc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3clfuuywv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3akciqwjr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zrpnfiyv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hsyckuqo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kdtqviat.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3votreqld.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lgmiuxdd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bwaklzoe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dvdivjfg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hiadkdak.html


<!-- 参考信息 -->