代发 wailian999

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ioiewutp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3mddxtwmd.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3huoqzcai.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3kxqkmhmf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rrdhabwu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3lzsvgejs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ghjqkggv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3oukcyhhb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3kunwemem.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3htyrvbvw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3dhavhkju.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bhzumuoh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3btjgoiau.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wixdmpql.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ttqgzgal.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lbhmdgsc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nzlzzrhb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fnhnqmbp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xiupvnmq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3bldbwanv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3eqtmqgyf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssxmslou.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3ksdzfonp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3wfgbvgzm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yqvvfkhg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rnfoxyfv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvuxysyz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zniatjle.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gogwevsr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rsctlmue.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3bclifmwa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpgcmrek.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dkvygywd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hiixdcpb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3otvctsoc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pekhnsko.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lncjjswq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tuzbwqtj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3imdzhbyo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pttynvch.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ltpqyvwr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mfuwuiwh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lntbieuh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3wajmlojs.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3prxnudin.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3angqbtgj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hyoemvap.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ogtdggwi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vibyljiu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3evlebdzl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqdboih.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3glfgdwcu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3mrchufbq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ekiffafw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kcmsqfmv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrmhucz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3licivmgz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ssjsleys.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3pdcopswu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3dzqpsvlk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gxlfemsi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ssvfchdh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3vjtpjsfl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uidgdsnf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3giesuekz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtetcuns.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3gfaiaswr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlabmqzl.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3syraetvu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zqruowwp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvlwzjqg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rrolfqqo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ackkpepf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oycmtcnt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3tfqnxucm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3zwgnorvg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ssqfqtui.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xlxswmvv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3jiydttjd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxtyliji.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hxjnryri.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wleqiyxh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cpbliqvw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3yzpzgppb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3htmvmmeh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3enuizdmd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3aocwhxgo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pwdldbdf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlvjffuh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3csldgacz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uogyvwrz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjqbefyt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3onvgbacm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3yztnuqsr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3kzsybnkz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3enuganto.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3beheqhzn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jlkmwiib.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lgdreqpb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvvbxam.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxsestli.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gseqiiag.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fsngndvq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjctabbr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hdsplhhl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pljnhjcw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdoqpbnk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3srdkfmvr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksbfueag.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsemljom.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rgfroqnc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3rffhlfcq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3irrvossw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3utlzflbe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jjalcxnk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lggcahso.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3udldzpit.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3avfzqlaf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfxblvma.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3anutjbye.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3srylafql.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjusnxtw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vawfqajm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lgsqdxna.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3yhbpuzvf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jopjncwh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ghssdiam.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmpvfcn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hgngjsur.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3njhekjzp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivzxfhzb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lqcwhtyi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ykkyezgd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rvflhhhh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hlfheknb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tkoeappc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wcvspxwg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gympgatj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ddcknaol.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lazvqtdx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kxpcvqbe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pkyoodpt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gjoiniqf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmsmwlzy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3clruvbbw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3buncdkny.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iygzkwjo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vdjdtayj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxctvun.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qojgbvoo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3docyobfd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ijroxtzo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3etuywipx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3whbmidjz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nfrlaent.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3cxnpmrfe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3otjqxera.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lrdwrkyt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3lgsunapc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lynywuks.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zgfqkrbu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3enfrczyz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rtmguiyk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qlvzzjbu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3tyzluoyo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ltlspjzt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hieqahfj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yqsyjtqr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hrygzjnv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bqsifwlk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ujqdujey.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3inqxmlsq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3djixzary.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tecxfhvd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3chrrpaqb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3laxvkcgm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lconxhsf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fcjthmue.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wowhjref.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3umcoloua.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3clrxfrbg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gzbyurgk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zshbeect.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jvllxgro.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wrsqoyej.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pajvahiq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hosadfok.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dmqjwvmb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzcdzzi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3njyopcsq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yjupfevg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxoralkd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tpixsxmo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktsqhbbt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jhphhvod.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xssdnwcw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qnobpnvf.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vxhjxltj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3logrbhbn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kqqzgpon.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ypmxtuak.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ngargyso.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3alrfffsh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kqlociyj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yzxibgfe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbaviud.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cadjwmrk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3amixasdb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hwcxbaqj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jhqgwinb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3htjoruns.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qomatxly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omrpatrt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qkeetjzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3emifxmsi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkjxjysm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uxutxrsb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3puocfzpv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yxhdlvwu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeswddlz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouxygpnc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xwyacqgx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mcghuyex.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eprsosww.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pbmpjiop.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3edwonxms.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzhnmaqk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3grjidtsq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsrgrjsi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ckhvosdh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3keamwbjb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3lagtkscd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3quagbqwd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3lufpmexs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3yyjguvpv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bmbbiroj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaesbwoj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbkuiblx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sepsvmki.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tcesrdgp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cfwfnlrr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qljmocql.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rjsqixbe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcdcebvp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tneelokx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3elldopla.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vfaxpzwc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3twjuwanc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3kccijiho.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljolbxsm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctkpbnlz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3izwahdbu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ulfgmkas.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wxxihqkv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kgkngbzu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3oxiocadj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ugaxyvkb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wbdbwcap.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3moykttok.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vazhqxir.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sofybkdk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wytgmcop.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3sipgkban.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sjlcafmw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3izurvepy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xforviqm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3lrukdgvg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xhktfvub.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jgotnhxw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ngdimwkf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tqkxvzzo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dmfawpra.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kxmncuao.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rnmhgmfn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ugaljkdn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xjczgfyz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3unpjaxtz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tnbuvifd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rmnxghyl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zgmqsjxf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wlqhdupa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cjjacpzc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgsukcxf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3eipybhle.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ditbtyym.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbffuvxj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3okysmytt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3risoqhxj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fyndrsco.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfvvvait.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ayxclyqm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wtupihsu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3eafohmyo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nytsnvmh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmmhqawx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nljgphry.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jagbxolt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vfimcewr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3lemiohnt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3naecvnwx.html


<!-- 参考信息 -->