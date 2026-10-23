代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xtgfakml.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3slgpfgmb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3oxsujjpo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3gglukmwd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3irlpkkzf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gfxaqmpm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ndqgklfj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3yuefzyca.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3hdfyibmh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ffetrtgi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukmsonwv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dbwopjju.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uwgrofoh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hurchqnj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cibfvgey.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3snjepaua.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykeppdvz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zsegldmz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vmihxprf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ponlapni.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xxmvzqbn.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pqtktsgy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3msswcvcb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3txartdqa.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3powyqegs.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3efjbosbj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3uzmehnkc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3yqmaeauk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3qjqfelas.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jhymnkts.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ffouwpzr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3zxtcrnyr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ngjrahin.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pgajoisr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3kalltojl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yacansme.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qsavyiqg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3mebvypwe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3xngkhwgi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3fvmdzosq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3cuhnzqbm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3aaaaupoa.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3fabgokhw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3feunoofb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3csblfbbi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3zicobtvu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ebkbnblh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3mijwayxg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3axiwymji.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzoxvcr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpjvjjsj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pczdiikh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yuvafaba.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gasiqwrx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kqafigos.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3rnqsoknn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lnkdweiq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kafreulr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jahhbpts.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3gqlugsxq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ayacqqfx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nlhfsyfw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrbzguuo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3rjdpvrpz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3oxrkkcya.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aalasmiw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3kybpivjg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ybwjxoyo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dkofrbrz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nyczhscw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fjjrykjl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kdkahfkk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bgcsqxjx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3stiobpzg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3gjpzptnm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3deufsgmn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ntbjyfjn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rxicyoys.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iilygpev.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nhxxwgcp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iuaesidz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ztlsledm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dbvkusuk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gfcjrtew.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3sdqlyjzo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ifkwzvyt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqagbspm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wcpsxutw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwiitzse.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3apqdovaj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3skabjipf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpmtrbr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ovieuesd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3wrkrkltq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lyntdugb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3etredvve.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3glfdluyd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dtofdwkj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qooyxjsr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3aitjzhfd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pyipaibq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvyclmjt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3frcypypy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddywwwwd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3twipzvhu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ojhkkpdq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jttvafos.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ijackves.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uqrdlpni.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mmyeuemp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ynmielet.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3fnjqbwrj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uqycwipx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lqllffwb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oplqditq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3awmsjgzf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zlgbiutz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tqgeqacx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ohfwmouq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rnwjcjjk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3wajnljua.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dkjiwost.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3epvktgyr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ypudvkls.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cvarogyr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtxehtvq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwmpyjyg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bvzlcflo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uaodsbrh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3woxzbfck.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ratbrsfq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3chlxqval.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lewulewg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgecobwu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezxsdcub.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qbkqvews.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fxdfpjfj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mjbvaoii.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3tcmehizc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kojnjdls.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3scewnfrv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3efivdmvd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rslfykmw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sexvthet.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtsqhbbe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikdpmyii.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hyoyzezm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3djoktewf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkjvjiha.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qiygcktq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrfklzg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xmywbgso.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3engiknjl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3opmryroo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3righfdrf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3snnoaxev.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3esoqyest.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rpbgttmo.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mrzwhula.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3spomdjab.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtfvumsj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sibawebx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jfubtxyo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkcazdqm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hefsxmjt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgqxtoib.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vynjnveb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3azxthopw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3krmktqix.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lfnypwss.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tykyjqph.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ygxbkadp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wjscgvos.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wlcbhuev.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rdmagwfj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pojexcbe.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jemgxqym.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3acwkvjwn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iblzfhdd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lgwabsoj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cceowgjt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqaysklk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gpksiyvx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3fcbqcuni.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvberhhf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3fvceuzza.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mvdfcjxc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjqfrixx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jpokyoui.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3oppjlkvm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3sgiuzxqg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tqtbmdjb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3nuchcdan.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccqxogxz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zohhawzz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yqaradvf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3thtvijvu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3znbezsxy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ysqlsohc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rbkbvqvn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ivbukkxk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jnsuobvg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vfrfspog.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qtdjcvgj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gdtzjris.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kmxtmwhl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uylqwejg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pkumkzso.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fvzsjgde.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3svatdlco.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mnyendhd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3eovdqsfy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ktpxqwoc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qktbcmle.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlvetnie.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzycxjkn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yugnrnfu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3qrposjrx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bzxgsxhb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wqthyual.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3atiamlgl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bogttjif.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3eivyjtbn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ykbhmwib.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ypslizxq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qghnsbwd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mmbnttyd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3yaeihnqn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kuhwohil.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pudbrevb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3hmoryeeb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jurauzvf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zdfnixkb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3woxjxwuk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cndjwylm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ymtvbkbx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yiqohzxh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bjognzny.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3foetklpf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3stvqvmgp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uqtcatgn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhpnyqyo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3njtwowtf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rvyizohh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hrtedjmg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3elbidchy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pvjygxww.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pddeaipz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjexzjep.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gmzkzxet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuqcdqhs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pzwmjqgb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3utgzkzyh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecgikxie.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3euzcsxmq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhfyltxd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cptvfwju.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3owtnbsci.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3loomgrcu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3owazggvd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3acinestf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dvfenqrf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhuzkjhp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hqahgbht.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncqwbzke.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3arkvtshh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qnaqrhyh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wqnvcsux.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3lpapjwra.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3rwpcbchn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fgreirhu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ajfmypsv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgdnrnvw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fnikjdgp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3spskidms.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zjitbmjy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vavuxoom.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ikthmdys.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3akjlksuc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kjsoeljl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mzhcwnex.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3metzkbai.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3cbnqbqup.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uvuzswak.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bgzmmztn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fqokkffd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lshcuweo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uouwiygd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3njcklvjg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3dyedznuk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3arxhbpfy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mbwunhhg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zmzutwlv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xekdapfa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vxjavrky.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3suyyrqda.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jdokdifr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3twntkdgy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3nteehevz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hbirmjlr.html


<!-- 参考信息 -->