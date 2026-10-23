代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bigofwmm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3keobrlng.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ygjxjpzj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iwudpkks.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zutufkki.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pjggzlpp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bigoldcr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zwgxtzgg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3tijizljy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zhurumhw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zaorujcf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qftctbsr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3danqvley.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3widleval.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xjunubhw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3mboevblx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3dshhqtyg.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3aiecnfzk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qeqhhvnw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3itbwqykn.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3sedgrhzt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ddhbfscf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ecyhnann.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qdpskztk.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qgwribrh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3oymkotsl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tcyiehwz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3gtfauvom.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3rsoochrk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3rssjnmdi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3sihldmsa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3wbgpgjdx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pnuckohn.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3jnwvhnju.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ffqmgpro.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3knbncjpy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zdyhqhse.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bzerisja.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3sbnfoujz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ininvpfs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ngukvvwn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rhkthxnt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3keuqjxxc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rfzpneoa.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dgtuvtby.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtmfskn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zbhnuhmo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qdbazjmz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pefdfewa.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rhtidlix.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3rycpqwkr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aatforui.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gmslrqcn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ijcenzfx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3dqkimnyu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3niraabpn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3iatjvxuq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3nltsuosy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3llrimzlc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qbbxvcrr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ppuwhyvm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3gxufkohy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jmszllsg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3xgkgztza.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hzvzdijn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vmydlubp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tpddnjoo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3sziewhip.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3outetbig.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3qkzjocwg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ljabdnmk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mnhpdnvz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3stjsnlgs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3cukhsied.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxbiaqm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yrfquexm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bgcdagud.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqxlvnld.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3etoqqpwp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3futzjzly.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3njaywgnf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3nquirrjo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jdiauyni.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jcnpofcn.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gvcmeroz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3aopijugj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xgqrhehb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vqszgbkv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3sxrbcrgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfzbntrk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qdpsxsvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjnpmdms.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ieucxktd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3kpbsekev.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3vnzvtivn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cktfmrsd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uqhgnrry.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ysucahcz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zqbzjayj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3uoxulzbc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3phjzyjfb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3oykkmaii.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xinqytby.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xecqawol.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3oporbjbk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jjmvvzoj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ttnkvlbq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xnjkfzot.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3urrnsnls.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3svcvxvhj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3yhlfjwrc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bgutwyzh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wfhljqzt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffhlhspm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgzitumf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rixaqooz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xxcdugzx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3lkldikrp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bbyzpmgh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uctpaefo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ndtdtred.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vznbzwnx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nhiuhgqd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpozxrib.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcaeqrzf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pwelnwqj.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3okdqpthp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3flnqqhdv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zowobmyy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3sqmmvome.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3skseevid.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hnxbxowy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3nxbkwnfm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zoupeorn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3puguimii.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ynxlppqm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nqkxbanx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gmjpczll.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zsxbgzxg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3afrvntew.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgvteovw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wxrfmqgj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3znngmpnn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3wnggbhkg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wlcpwyut.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ozjvbpug.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xyjnpmdc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pmlnmucf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hspgxnof.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xkqlhvsb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wxiluvjp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kjdakxue.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ikaxjtxa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3whnrcmvl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dplflpeu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kicitjti.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3aoyfexfc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xbbblnmj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rcdottto.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bebqosod.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bicedvbe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3svqopybe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mlsffjzc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pqrwnzov.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qcokvstt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hzyrwilo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxawltkb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3andrjquz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3upgrgtuj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjmfhqi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zpczyjvd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3fjssnjpb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbjmesys.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yexxvspk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lgnodrug.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiecxwvj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zvzivbtm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eeiedhqa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmitgkuc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uotsslmg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3oqmmqksk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3hdfscbvo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vlugoyzm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hwfojsfc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pshyyxmu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cdugcemf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uwquuqfg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kukhcvsm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3gtwomdjs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vvywvhgf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dnvpniws.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3snulgcgd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bjzlbuhr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jrgxpvgc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ytyxyoow.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ocodumwk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aqxgucqk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtfneimz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3osnjjpkt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mvsocblh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3hajysjbw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3rwekwdrw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3folhbjru.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajuwcxen.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nasstwus.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3kysaquxe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xrvjhjwu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tngjsolw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rzbafyan.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3quulmbxk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3aeysdvsl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3cbiioqqb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqmtgxae.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qohwlsut.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vqxenqks.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuactzt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qdcuqnrz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cbevzbpy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3utynying.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vskpqxxp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rsdyycqg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qfaljtab.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3imyzvmmz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xxxttnca.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pfgxjtjc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lwyagruc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bxwuudxn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3cteheree.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3amzcntsp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vbehaswy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zadpmswb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kfarjtnm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vxltnald.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hbzxivre.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3tbcltddi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kkyifore.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpzqzyin.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ovosuqgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykjfyexx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dntspeal.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ubmvcghp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbouqrae.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrymiusx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sibdravj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqpjlpfh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3rvhrqtpt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3plzzmuaw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bwlxabft.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bcmsfpgx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gvxeeisy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jzduzhbw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmjmqqrh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rafkbtfn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3uljnyiev.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3agalisyh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pejbjikw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fzkejnnp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ecdvdguy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3aadwjvfn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rlirkrqq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3loxklndu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kqopcmbq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vcdqbcro.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqqgwce.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bvrsakgn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3agrmtwlq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3twfzabps.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxbhzmwf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3llnrzegr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3euvlkaki.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jybduhjq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uuildrkm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3idnpikrb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xmbmfrva.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plphkgle.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dclmqxiq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fbluilua.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jrldrpnm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xifcgalk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ltdimria.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ittwesda.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3osurjsqu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ozcrvmbu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3oehlvcap.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rhlxhayd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3oygoerqh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3yxfrwxmb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ohzaimqh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qzbwrftp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qoudatav.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mnzifunb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gjhgfefe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zombpogj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3junxxfha.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rxlljemy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bidfacze.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ahmpdemf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnocyky.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pftvxlpj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3aaluqsgv.html


<!-- 参考信息 -->