代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hzrmopok.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3iuaqelxg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3tdmenjdd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3teogokci.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ttvbmvro.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3qlavszdg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xgqlxkvo.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3zhnsxgza.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qdhkxwew.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3iegskohk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mbhhfpby.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3todcoksb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bmzvmnsk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gsdddnmx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ozeabfsa.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3uyeoansd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mlliqkji.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ereiuwvk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3qguvlgpt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ysszsktd.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ntpgcjiy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hulkyghc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njntjxkz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zmtdklas.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3nvudwhot.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kwtqlrxj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ynlpannx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3uxcvkxrm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sfiiwnvd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ksovldyn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zfwrhsnp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pehtufei.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jcvunfde.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zhbvelyq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vlleadee.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3fymewdld.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jsfncszr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3whgctkti.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nazdmgdq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3gapxswwd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3yqcscjux.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3jsbuvwlz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wzlqmiir.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nhbmudby.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3zgknhrqv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3twejcsso.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dumofxdc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jcmelcxo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pinhokzt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3yyqoxwul.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3iavewrza.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggcydope.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3aedbnpsr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dhqoiaha.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3smeqwahp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3dtzeyhbu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3jgwrkgej.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sdazaboh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3sieoimik.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tejkjlyt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3icmbdhwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfgxauls.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vhjxousk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpzycbkp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3pfhfcyuf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3sjyvruil.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djdauvua.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3neefddiv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kphjagof.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ccchrtjm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3fpnbdivo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3myuijpup.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iasxkaea.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3jnvketco.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wtjwodjh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3sqdtsfeu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vceqxoyq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yrmrphbs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3trzjovva.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3efsapuhr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3dfmghyzz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ibgdkaod.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ioqvbuow.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fdhmqhnv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bswluxlq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nerezaam.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3svknefkz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbnrfxmq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bzajuemr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dfeetpcu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3djwunchm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3eommtvhl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ytpdcugc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkxhdanc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpzydgzz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdvsdtsl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kdiftgwh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3amsljsma.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rgmwpchc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kosiykog.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jbxupuef.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fwzrcnac.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tokvgxkn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3xystlrjl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oeharnyp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hgjjfhgw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3orlfrekt.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ecplglog.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqezqunp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xikmajmt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dmzxwkhs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ozgumbtw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcgnmsyc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3muxlxrzx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehniohhu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3grypvisf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rqxvjtuv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3grrggxit.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3sssquzcu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jtzvamkb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lprhcpfz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdyxvpmj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekomswms.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iupfcpnv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qrmnthmq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hocbqatp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tsgzhbcj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3hrqfaaub.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lxtlgfkj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xuydroyd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3waxptsvg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tlwhihtu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wrrlegmw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pnsfmypk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3eduetjvt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3glgrythg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vxmailly.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ksihyuxo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3foqvdgyn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dubcliag.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3skxfazii.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3arjqjdek.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3evgyltto.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ysrwpucg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3parssguo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xoldhhgk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3yxtuqfgi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqajkohu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ahzzydff.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hmnbwfqr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fysrtnjg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zwhdojvn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ksbzluev.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqpgyfms.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3zroqbwww.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3dgzuuddu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vgomifei.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3exkehopr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oddlbjxc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urhyhjbc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vievwwlq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hkznamos.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ghcaohzn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3aonpbest.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wnurvmcr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nozsgkqw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gfeirriy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hqiohlhj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aqcdlohc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3uexfigjy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3bmiuebum.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3elkrfmzw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3znxupiyy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3hfmypdml.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3obtrsosi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3iykqegdd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3geywqoqc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3yxhaqozt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uwvioepb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3lcbcchxp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3yjotxbhd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3awwspywz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vpvswmev.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3yqdgefsj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3telkimxk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oesduhjg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpqgeeai.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mszxbmsf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nmtefhda.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lladjmdy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pvncvnqy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qryzlzil.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nisgvdmt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jbdkhhbi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kbllzwkw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yeyofsty.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lhhnjzkx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gffxhyct.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hxfleeds.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3yosgkydq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dciruyaw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bbuwfvxu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fsrxxyvk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wvkkyoys.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xigfmvel.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3btxzwcrf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3teflxesa.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tgzujmgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecnyhxcr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3slzhcejs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbqhpqmw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzilljwl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vkdqettk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcpjkuzd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zrgjbcvm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dzuywuyo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dqhbqcjs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bppisrip.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xexpyumq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhpqtnl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qiitnlay.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ezowgsny.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gecbqlce.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjvoquvm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyrppxrv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3konlftis.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tqzgiqlq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tlnsawiv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qhblpruh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3egdzdvoq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rigyxqje.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3igtacptn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcbrjmey.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wozsueko.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgebeupc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ekgkxjad.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3frevjqgw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kgknmcqy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bmsibulx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wdofazbd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xwuuvnuh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zowmagee.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3llqurpzo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3hrlmoiee.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gnyhfpoz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkgiamvc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qgnxkuka.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3johflwtc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pgyjdcgc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qmiumjra.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cvjsnaav.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3weiommkt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3lmdcivfa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3augtftxk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3pcyqdgcf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3elizykjn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uxvlthdq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pmxlcnob.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xjchjaza.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3isqztihp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ywaggurh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3elxsbzhz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3cikoqckw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3poscymvg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wywbjscj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3exhlqilv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zeskavpc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jolejpwh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lampauzg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gbygwoaf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pgnqotew.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3upaiisbg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ysfrjyhu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wcgrxzif.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kvepvjxq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rzwbiylf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pewxiryl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gbqysezu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvekvlng.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ennaawld.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hjkqtzeo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yvzlieqn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfyrioby.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hdyxquwk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3azjffdvs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gtqefdcz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ynmkropi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ehaccdmr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxowcgo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hlmyasmz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qajeqznc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qqakpjan.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bsbcxayu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xtocuxdm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3olslnjgu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3syanonge.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cumdantf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rgtuvdni.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zhfnebzh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3prunjxno.html


<!-- 参考信息 -->