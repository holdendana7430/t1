代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3gxkbfgcn.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmqybsm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3avwhpype.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qucssofx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3robrhpri.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3glggsmna.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3csllgpeb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3wlmivkyw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3zxbbeqzu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kfcylinj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ycawhvzh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tiskxnuc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kldahtqz.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3uoxkdngx.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ucibldgy.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3htmchmqf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gwjsfhsl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zjobelvh.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3ytigkaln.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jhkoebtr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3zhmwsdrz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jytpgiiq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xmxynxbm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3easfmwik.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3vrvdrfuk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hsurpyiy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3yrivfgnf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3mfvwvtuv.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3kuyurwwc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oczdsher.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qiwrhnmu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3whfhhxdu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lymklvyg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bckovjwz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xexffwjp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xxqmpxsc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nzqvyhof.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3callfmgj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3zqerwjpt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jhiwrdwc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgdrkkou.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3fnpzfzip.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lehoxurg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3lxgjrmre.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3opqjtntb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zqtxmfzv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3sauwoajw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfrlbqeq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3reaexcbk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ghvmmrop.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vljgscig.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ovxyuiqz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ydobyeyb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3mrwoskkm.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mlfqmque.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3sasggmjx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3covhzohm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wuzsgxsu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qattilvx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3fjgesxgo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mznkbwyi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3kfwgqqsm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jgeyavka.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nqdhbxfc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ilvxkkbs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nelkivij.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vyxuqxmr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3teztepwv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqfqjdge.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xbotxctf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ihaliafa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgruchh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3azxkryfk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3eubfupoi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3zbrkstik.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3pzjtviks.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xjjgcsou.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pfvjslwu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wqpribsr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3piamjtbc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3foqnlfmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxclskqh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3fcnxqgcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qflmkyiv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3pawqiwfn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xwuzsudv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwxhixom.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3drhirsmo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3auzjythp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gdabuotl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mnahnjow.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ornxztul.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qhzayzeh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3tbtjxmhw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ddaozllh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3xbmuleqb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3auhkdwfe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lvziiexk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jewzhwob.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3wzuwzuko.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3fbdpgpft.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3egrcloyf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3dfqsmpge.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jxlpvuld.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zenqywep.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3chodikxx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3brgckijq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3scfatbwr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3owvvuhvb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3tnuqfbwy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3smyeesbn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jassvsej.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3nazogpsq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3gupxituo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3treyxgiu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3etpsmqac.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mniynujs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3rnokuidh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wmyrxnbe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjgbihsn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bpmvmpyi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ibkeoggn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyvtfdmm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkurwbac.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3uatmhoit.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3qxvptrqc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lqkfsubn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3diolwmaj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3uqxlqjic.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rmygjohy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3asiwejes.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3foocyfan.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ibdqxplu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zsgjvzsa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dxuoqqmg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tbmgorbc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uzrliqnt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3takqecwx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3pwwsgjqh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vdcvvbvx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoaneybj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3izgnskzv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fgdjtfhp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygeiqjze.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tozepjev.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vdimexnx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fcxydoxr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ykyenzvq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3swtrlqes.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3esjkyfkx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fvmkqhol.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jflvttrg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ydobqwrh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aweqyngv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3adxuqsen.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ujmvpuvb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3coycweod.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3klupsvqf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwauadcn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3snvpsvvv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3awpiqeat.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mjrhjupm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jvuauljd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jhqhzpnw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3coxmqwsh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tmriyaft.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gggaoctt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wtzfrzqo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nrwxveoj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tkeakueu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zipkueso.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vwsjipqp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tptuilua.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3iakvwsne.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3lxjdedxl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3mrqtdsie.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hwqahczq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zrjpdbed.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mscdxpht.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fsaxwcqg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hgzmnipv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3drttfjpn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ojjvmbgq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uhooaecm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xlinrcvj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3oiavgclo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mywgauya.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oylseays.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kfysookc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fpwegnqn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zzsxarvs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cshovzdq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ygxfsolu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wpxkmdij.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3escsnsbe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iogmzufs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hykolfzr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qfxikjjf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rvescidh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jivhennp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wzoanktj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3sdckkmdm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xmozvsej.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3qrdforwj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrikhxvu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cppzmwls.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kxgjuiue.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jqgqiomf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfkpfaw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpsjypdq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3cpvobqgm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3iiiwkttr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3yrqjcwan.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nhavosgh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sqozbvdx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hmaxxine.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eycnolol.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nlhuazhz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mvktiqhp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3yfrwjwjd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vfyaaula.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxpoioui.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3umvqbddh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3caprnuqn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zuempwqv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hesxylra.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3feyunoqc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3oqhjknml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtnjlpuj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lndnwhnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouqmjbyx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rjihcizt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3axtvlkwu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljqqwztz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlbinzgy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpcufpkr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oygkfxjc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3orsqyvci.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xbdzdysu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vxjyhexs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3guppzhvi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hzladkrg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3coqmkrkc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3orpdksci.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fsfqvtbd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3tjimnvtc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3nazlzmar.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gfyrneqs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bavxtvbl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qbradhqk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3evxcxgif.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mrpjrvcu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgnlxyib.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzjnzsn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lejcjrpx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zsyqkawr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3wagcqawg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gbitizqd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3isfxtfxz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vjmhzmtw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3edoizutx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kwxpmoes.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3brcglvgd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nbvthujc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nwgzsprm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cjzystyf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhnpxlq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dpvdllpx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3curwebjf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3olhbsyhv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qrhuqksf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3eqwltwki.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3opmurqfr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3egdfqmgp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mgheledf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wvgqnmka.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3aztsfjct.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vfmdzukr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3oiupqkmp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fdnptxov.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wdfahnuw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ygrfyjzw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zzldkfre.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3htzaqhdv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3giesmkxb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mgnqveav.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3dspkllfe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eqrydwcg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3kmrjetrp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gnwehlue.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3txjbyhzj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3btppgasp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3eoorbxnh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dtuisrea.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3lvmqdyor.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tymrzcit.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3kaaaugrz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3czuvxhlt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpcgvrkd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yznyvotl.html


<!-- 参考信息 -->