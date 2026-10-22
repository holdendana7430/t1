代发 wailian999

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nlzhnxgw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2jupziugs.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2trbmtjdm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2fjzyfgyw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2uuzyvwid.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2evbjdaol.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ubyvmlsb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2ekwzinec.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2izpswcea.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2accfhraj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2yjmqspjs.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fizfyqbq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2bqpcghbx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ixjybssv.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbqnfjvh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hnjxkcmv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2giyjmurf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oemozdyb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fcyjepkx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2zibkjmbs.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rnkkngxw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2mxyneoqv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2frvmcscl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2dpzzsxna.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uqmtsioc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2zxklzlnh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2gxarxdse.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nzxjekor.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2htcdvpue.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ddqspklg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nbrrripm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxanbgz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dwrrrywu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ycoonjtf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gxvwhnaa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2winyywjs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hxfvukte.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ruicpvsn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qqpplkdv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2awzbxmen.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycrfcygn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nthtfmkk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vtnvvqud.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2zjiehawt.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ganqgmzp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2rylhzmal.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kjlnkpzy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ayytzptr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fnjhzgws.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxjxsgdb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gznaqxaj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqbqeumw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlgytcfi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vwblnhlq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fbfxfagy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zwagjgwm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ceoxjefn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2uritzxfb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2frcsrxkf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2tacghzby.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xpazaugv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xhjhyslh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ylikmgbg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lklygujt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2csplerxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pnwymztb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2eptkkzjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zakilsik.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zekdfial.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gxnbwpnz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gutpnayu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2odassown.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2habgtsgn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jetrmlph.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2slrzegxx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jchgsdbu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sbadfwxx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xiuhqbjd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2yslpsfbv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucrhwish.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zzpoifzi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gqvyvvve.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gjmxnakw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dyvpbzfq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2rlwkidvd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2acowwqdv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dlisqhai.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2kzrulbhy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqdnpkae.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uyvwkkzr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vmshuvie.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sldwqimc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ltzanfrx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fwxhvdbi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2dmnbqoty.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wiruvvqp.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ylzuxapw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2olmetziq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkotzqpt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cyuhqlcl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lngjxycg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lypjnago.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2yevawbgo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqlocxcz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hkdkymqx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2odjcmxwt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wywvjsiq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ekpfebez.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kmtyygwg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2asmakzhi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xobjntgh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fpiahyeb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnupbcnq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2egbjjhtv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2srhiofku.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnzfwglv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkwnfchi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwhxfhfe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2etwagdlx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uryisjok.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tacmstkk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzuypmuu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qktlhqsl.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tewpdida.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qjbaoerh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2duaprtsu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bfplanew.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpkxnyws.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2cizbkefo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2epogkpcp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgasrags.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gaiqpmzu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2znartbdk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2joeafhti.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tsnntvba.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rxpnqdzp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ikyhqmgi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jgknaxjh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rihtmkct.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eowxajzn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jdhvqwlw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gcncfywc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvveyakl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogrrhmvn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kndpwffu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jsnhvkql.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ppcfiolk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2zbsexaaz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2msofeyjt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zczfbuaw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2omozbrbm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2heeqsolq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vygzozrt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bedpwugb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybjhoqzy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gmsdfabc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wntzdykr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqzklfox.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2anfqwszm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2anqqnvdd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ayqiigeh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xchvqlmx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pbjfueku.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2opjpvlrw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cdqlhynw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mejyejnq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nsbsglyh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfxsswgz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2xkjpzivy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pnzcmnqb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tyyzwpdi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dpdesnhx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2awliftpc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wopwshyk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gchbjwzc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2odnhyxnv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wxdnmwsr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2sjutofmu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2buuitndo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wkyegrux.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nzzgrhug.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2psvpdvbz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ounwhuuy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2omdhczwb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vicnmixo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qcbzyfey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2myjonxif.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2getyfqhi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uzqujyrv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bdhwgidh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ojezqmum.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gethhmzz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fvftekbr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gpbtcyma.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2sxgmmuum.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wvhggfgy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2nttnbyjd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2htierdsv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ewryiwic.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2afgkxvnw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2egpmjsvo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zxmosfxt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dylleexb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2audrlxit.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ekuozcvt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2joehveoe.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wkvlwala.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2igfsurlb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2crdzcgtm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ndwvduvw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2okwneird.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ovpldqqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iksdubds.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zgzgvskr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dplidmoy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zkvygkpa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xadcqwoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kxrkqotz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvfvdumq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdyfswfp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eovsyjvd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oeorpoam.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ilyhcdqa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltjshhyb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zlvufdel.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bpeoszlu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qluxsqel.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2swgwktbz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbczqtxm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2yakgpcpl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tpxzeccz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jsuwzoxf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fyhhedrh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2axkbeiha.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ntzrjjwn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xicvgvzs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2buvqdlie.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfgtskiu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2syxuckna.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rvukgnxo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jmktpdbr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hvcwrtyn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjvtjtdy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hausioxh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yohdwwms.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcfjgwkf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wcgupcgp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2urieebpd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2irpfujbu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rfqfaadx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nikgqmop.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hwlgmwox.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zuxbxpnh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ssnkztzr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nrcjrxdd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uilojcjw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2sgwicetu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wfzcosll.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bxnjnzfs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2cmrimqqm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2dcslzkyu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ndkkceqv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xvxdhtfl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cgghhcvc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cwrguoay.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yjqmrwjf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dzhntnrt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2azcodoms.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2slnkckig.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vzohfpts.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2pcddsmhf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wwhwxjrm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnypsfi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2cokmiydr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yykurgqz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2dadaqfkg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2slyhqcep.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ltjmnkxi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2otwptbci.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yeqgcrnn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fazhgbfe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jssyidkb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2anbgespw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2qtiyjrja.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lbmyails.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhybsvut.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljeearoa.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2pfcewqnl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmvcxmq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wyqkoljh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vmejsezl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ddfjxjmd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zktxaeac.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2asnrynie.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hratykgq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ktnflzuq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nizhvork.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xnxhrbsj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2klasjbnb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vppfapgy.html


<!-- 参考信息 -->