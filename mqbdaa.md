代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwjrdre.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3enecahqq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mtjyeyra.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ihgwbrhc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3oqudhtsb.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cvbvvfjg.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cxttjjcl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3zjqqswum.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rtqzovmj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3uqdusnty.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3smbrfner.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lcixnodd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fxmgjmlg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3dgrvwpbj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3sovqhmvx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3shnhivxb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hkptoipk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bjsbhnhi.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lbpiccus.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vmzoecvt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3gkqeizhd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3yzapkppr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wfesmrcq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3nvjscezj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3wvowmpfh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dguoxmox.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtfuiek.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aermtdqs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tweixyht.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qdedivky.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ghpgeask.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3lnduumxo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vzjuptkd.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lznfvdmd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3kixanmfb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3nashfjje.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3femrnaut.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zqinnmyr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abxdmqxl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ynqhzlxa.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wjbnhhxd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3svpljert.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kambspew.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3robsdxky.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fkmcrykd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pejidezf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nocyxtql.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3lnifnpgk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3byrxaxqs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vwkzbsir.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3zmjididy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wslmporc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3brktjyxf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uwzgwtud.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yvxqfiyw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jsclwzog.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ojfhtyqg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3louvobpx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3orxffcxw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hdcjcccr.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yenkwohu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zpmvckpq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ucnbmiem.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3irpirklx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3gedepwrh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fsxdwcgw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3yozknvhg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rthkraih.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ipvuuasb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3hrdmwogh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3fqjodhkz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3pchtciig.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3innexaal.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gfnxlnfq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3qejrdxce.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wadegejc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3loyfjuxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfzoetuv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3khzumjbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmpzntud.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3kwjifqga.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lgjqhlhn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3leizqcrw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gcgbvbzu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zwxrunsd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3msfdrnhb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3fwxgtoro.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mpgxqfxe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3anihewxi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pkonrjct.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3frleibrp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vpipstji.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gmjtlcqw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kgmnesba.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3npcrbsnk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mjtgtyyw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3yboblmcy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iikhpmlq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wunxpwbm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3qaejtwsm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ydlcxqyj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3whcyfehy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tsxyihnn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytaofvdh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3evdsfmin.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ioxthkti.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ajjgjceb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hwstalbv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyqlaeq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xxrmyqze.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbmpjsby.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dysmsjqm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mqixfkcp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yynkujhq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3izkuoccy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3abfeidxv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qpdyxodx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3heeknegb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3oucvleta.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3etjjbbqv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yofctkie.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgohmtqj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yizdfpxv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3epzqviwp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aazzszar.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qxrdtjpp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wkkvbhnp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yakjzvgi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfmbkzgl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zezmszmt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkczsvye.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hubdjzsp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nhntnwez.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3toywusqc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gqtzlnuo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tvvrybku.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3sxjfjuhc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qryabwuz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3phznovsx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aecqwhae.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3spguetvi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ytsjtjaq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvqvhbdo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3srepelgn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ginyymtk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ydlqbpvc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nztyukfq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yurluswy.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3axfjlaam.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xpouvkup.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3aqzgmdfv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mcszoumj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ipgeplhd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lvtwbrda.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3guaodcei.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuzbdjyt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmkaeduf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztuuygst.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bwgzdvid.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rxxezspl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvulxwze.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mociatea.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dzsmnrjy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yobdmkpu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jrqnqpnu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3avxryqss.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3xegqobuc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jyupmibv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dcjaetxl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujnipuxy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tkekltqd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uglmbpmu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vebvxgot.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hqnvihey.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nejzrpjr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfppjzlf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3uhjdndqh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kgmwjgoq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3thwnusny.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ejcgmadh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3omsqftti.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tkcpqpyc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3msfoqxtp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kiydvelc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vuzkxwkb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bbfvxbvr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3jscwzpwq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ltqwenqn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3uglzkxvo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rutuftic.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cwfusuua.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dkqntddo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcglapjj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ohmtimbn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fvrkfcia.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3oenhmqkr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3hvpvikis.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3rfqyjfqp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kerjqepy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nvauigqo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujwixfvp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lcdfzkhk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltxtwnfl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pjvgutpv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzeebhnt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fpkrpneu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wsgyvupu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3acunssad.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lijosbtw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jfkfinod.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mchxidcr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3powlhkvu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ikljaaac.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kpjszqny.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jezexosw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3eyowegiw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wxrzyxnw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkarceje.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3crnmqxwr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gtqwmcys.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jorflbgb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pyymefmn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hyvusmjl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fopblpah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htvzeqhg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dxxngrvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwjctswl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3eqjhrfyo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iiockdwy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gyavckmg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhsxclrw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipjyucwa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3koklmncf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3criwuuof.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wewlfzel.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hjdhbmap.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lsmdjxuj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fzklolqm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihpawelh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bwlhiqot.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaehikuu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yqnldbrs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kjcmhncl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ozmcbllm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vkqvfuon.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mhhjngom.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pnzsvsfc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwoiscyz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ixuirnbb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jfmqjmmr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3fxytxinp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3syuotbza.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kdlpknto.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3yiaqeebu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3anhcpezl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ukauzpua.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ivtizbif.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfliweyw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vnunvkdt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ytjvtbng.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3aanvvgar.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xaeiwlhd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyxxolzg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jeundzcs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fskkgcpz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wtzjrzfi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3axplqhpf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bmhqkqbg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3efgapeis.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xpjekixz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zswpejmp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oljnassh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ocxhbnjm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3hduzyswf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ayygrrsb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qtcelscl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3guumwdna.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ggysbdgg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3obdnxiup.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjwuwge.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3akkwqpzi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ggglstvp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3maihatnb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nutbxyfe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zznrjbmv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3gtejtqbq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bqedahth.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qjocxgbv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3utnhnwky.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dyzhllxs.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3riafkuyd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fmoqxsve.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3edvyypns.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3seddcpqf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygtvaaax.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vqczpkth.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jlffojgo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fnycbyjk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ymrpyujb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tlfyjdlo.html


<!-- 参考信息 -->