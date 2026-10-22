代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2adcotepl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kgsxnszn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2zjuxnrlz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fexkqfkr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hqjuvuud.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2ehhwxehy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2kktqbgvu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2imrpvitu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2znbvyftw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2txxrzkkk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ltjapnez.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2mnihqgcg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zepcfeut.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2shfooxir.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2cthypkoo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oywdtvpx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qohclpom.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pusmmbpl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2chohwdkr.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2xxyoxmoh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2zjvsfndc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2jiskltvb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cfmjeolo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2qywckvrq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2tdpkgzsw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2bpcdapqr.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ltxjteqk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ffhbwgpo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gbreevqw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2anxnmmts.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2htbjfczm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2orzixofh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2blnewcda.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2udlpnxhr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kfoitwym.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2pqlpjoig.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ghwmolzj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xukiwwyc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqgxjh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zktawtff.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2pvzbsfwq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bfbhktve.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvaifxxe.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2hbkplwbl.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2svdbkdjr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kcjnzlsb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ezmtlrze.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2omnfdqgj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cylmyoga.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cdlhzbky.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2evrlfqyz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rvydkdvv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mlmqobzz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2uulswxen.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2mtwiuksz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nixignvb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtdozfqm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ocjfmxgy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tvhpgrtf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2xcolmyzf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ijsxytpl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ezljjnvo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wjvunrij.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yoiyexzg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qlfkslxl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wajvzllw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwzgrnhd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2opnbjjxf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2kofekkih.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ogwtgfpa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dzqgrhrf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhjbawxg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xwkarrvf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2nesuelfr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2bfpfkzoi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2cjalyvlx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yghaefvs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2weiaoaoo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2yjpcgdlc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dvushqjb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hkooudxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huewgboi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hlmvwscx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rajdunfs.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xgkakvuy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ldnpwqbk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2toliuwja.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lmvklnie.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nqxsfyyr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mldyjzih.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2nhbxnbnw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nuedvuci.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nqjlfqry.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hmpjdfwz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cbyiisuo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohhbqefe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kaltanax.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nbctxjzv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jojxttim.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pybzberw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2bjxyquiq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ebjoyabl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2lzctagqf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dwgwetii.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mhvprupz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nahcdlga.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvrdvpyj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pauprzcr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rhxxyzqw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2evpvtycy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jizjacyu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rhbodevx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2msxwteiq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pobvlfge.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2hbffhmzl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2syisrlmm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2nsxirhoh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2wmfxjizh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2pxnjrsvn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2civpgocp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dumovbjc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2hztawpef.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lypyeaey.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2loqazoov.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzbavwzd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvnttqnl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2okqxizri.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zrzajqgm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mnfqgdnl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2nldnryqn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pdixecmr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpwzgole.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xetywitc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqczjtyl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2uosajbbv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ktiiiqre.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2klymugcp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rlehowbm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bykugcjs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tosqkzac.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2korffuwj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxxikcsk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2robteaig.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2japrsyyo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dpiofroi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivhtsglp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zbvoykwm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rvccneac.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wdnqepvr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qaifvdxz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bivtdana.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2djcxwjtv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jyodcqyv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2etyhewoe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ooesqwpw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lffpcgaw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zmhxhadk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sqfnnfcj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuyyirdf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oxxbtyzx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rpeamxdo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwxxhhpe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ztwwtncc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fruucprh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ecgudblg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ujclwlfj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2kgjloqps.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lwppkrkn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xmdmipda.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qplsmsle.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhxkkjaa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2calgzucn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2smsmrlpw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hqxdmndf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jusajvtw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ytgookva.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2arcmynvo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hgstyhia.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ahuboqpy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kilghcey.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2psfqtcik.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2otpjwvvd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ymllsklj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vqfkmnzg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ccxnswvx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rxdmhbup.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yihqyzqt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ltzeldnt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qnchkznm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qremlnmn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hrazyftn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2egyxvlhh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hovbqibl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fhxshuxz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2upudxeex.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsmfqtbr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xocntyab.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ppoxdjqj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2djnjvfob.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2efqceudg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2clfimjvc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gsmleoja.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mhppjgxe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gtniakfx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ihoyfpdl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tmuiqsvc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkgxorm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgahnezk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mclovdnf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zzgzwfzk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2aborspde.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2aghmnylx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2liwuixma.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cbmbvsyx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2szholbay.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pwuuwkql.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wtucfgxq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hjofsndj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2msnizbdo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fnxqyhal.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tjkecxam.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnywhxnd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ufkgrpgj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dtvgrayj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xugipqtt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ongrbfhl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2sbuedhzb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2inrxxtxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulukyxgd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jmmiguuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzuvtidf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bcevykom.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iovvpgah.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2aaetgsjz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvyybwil.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhukcwbv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2loedglxu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2svdllncg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2krbqmjui.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2skkelqeb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2dokiapbf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mygzjlvi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhrrutsl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amjobggl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ubjkwjch.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vwxphobh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zubcfafm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2skbhdqjg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pogpneml.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fevedeaz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2csqrdiri.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtgkodht.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxbunmur.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vkmnavia.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qioxxded.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2srmpetbr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ppkmvixp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zucmnnzd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfuclavk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yumbpzog.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pszuaexr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiprvyiz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ulbevyfo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bacxfoiu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gnfbvecz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zaeiwsei.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zqyqrbwb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gbpxykcp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pezeguix.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ikwwtapi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tulefjik.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vdemxjeo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jfbktfft.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dzjesnix.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2etiuvuev.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vackahut.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2eklmzyfr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2etvgydfu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rjzdxovn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wvcnamkk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qphpputk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jilxrayg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2aznzpeab.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zhtesvqk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qdblhrdx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rujytknw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bltpaaci.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2eatyztyv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mgndfxad.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rrgwrlzw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2exjbbhbm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ezwirxjz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2iobfrqni.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mhttkryz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pcgiimsg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2iikcfoib.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2rhybcscp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bztfeygo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2foycxmkf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2sigmaxje.html


<!-- 参考信息 -->