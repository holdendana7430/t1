代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uylcphbw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hshwkrqo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xmaqxkfr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ptnegjhf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vwkchjqm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ijxifboo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ifkmqqpu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vmgwujil.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3iatlbjss.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hkojqjnv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sygeptxq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vqksuyac.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3apgkybqr.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vuzfajdq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rvrcapbx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3obokooju.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3vughadjc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3wkhtlxgc.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qxjzhsta.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3qysbbjxi.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jmdxwmky.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rygjragc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3vaejxsxq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yaoiqppy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mbylvhos.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3uluvbong.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3atzifvzl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3csyczmnn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3oqdmddxb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xxrzbfve.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3cvguleuy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3tuorzkpy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3prvmgekb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ilerlhok.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3pdqipehl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3inyitday.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3wdhtanpx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3thbvhqwr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfghegst.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ccesyvzf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xmvmfxzt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qdgdsoat.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wnbwvxsi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3wfbdivvh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wsekerrz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pqjotphn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lzddcnkn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3etwpcewt.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jnbjzgdc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ggsjzqlf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mcgjybky.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qvhywcly.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bsghpsjc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eqguvcqm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3kevqmptb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3vhrukhul.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hwsfzpji.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ubgppyhk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dqxavneo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3jyzzovga.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3laialboy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rmbjbbyi.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3iqlvgqtg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3avpdluvc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ssvvduqz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lilksbco.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3njdeyvok.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3qwqndcob.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3euuuhccx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3gwhpmxpw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dsrapxpa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3unllxbio.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3rdtlumsv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibmqvlzu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbqgbxn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yiswwntm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vxnctfpz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwhkqxad.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kcepoczm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gcdcsxhf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cduzxjec.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nbmvynha.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wdvhoowq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ifmvdrie.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dijwrwem.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tebuqbbi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3laznaxzy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zxxlmhro.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tcsnlwpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsqrfikc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3tlaqcgvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xnxuarhm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vlneydtm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3olyvvlpp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3iwsceump.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kzmjmmnr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3etizkkbp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sbndgjra.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lqggzhqn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3rwawnvac.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qxochtjd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xkfqrziq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hviwoghl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wowtgzhx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wtrjgyhr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ufeyaimv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jfdcpsrx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xawfifmp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3eqgotdjf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xknazbnm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jaztgklj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xscofkmf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxjingtr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qryfifuu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fktjfwcg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jusdqwjv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3besrvqkf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ljzyxavg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hgwbmmbu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3pwzbvazu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vrutydlq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dssoecrb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qhjtkuma.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kkqbeofn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyfbittu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3lnqfqwnl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3xymamvew.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iumjvhmn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ddiyptip.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3silkcveq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3nkyslopi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3koxohhfj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pcqzeizv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3jexggigb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gqmuddci.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xoynjffc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmnjyjeu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3cdjlgvgo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hhvbzvir.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vvcnovyd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3agcakmdy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zlutisrn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hbglrnol.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3iczmjjjj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yqgufmsa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmeayfnl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pwzovryu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hhjwkdcw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xrgwfbws.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vlmxbqlz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhvtzvbc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oankepcr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hvnzfjni.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vgkovxqe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjyyaasl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3vzqrfvku.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xvntnkdk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sccubkhp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tvrtwjzq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tjlcxwiq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3axgotzge.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3maxkphbi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ecwzbjmf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bnsqdjtr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fgenkott.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajuzknwd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ksaseshk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3puameqal.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pluroabi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hnbfojmk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yaiszzey.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvcskdt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qwelmflk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hnbzzrub.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cdmbjkjb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrsogigb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3udptpfgk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ncapcepg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3aciwymvu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tvzqzhau.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gpyypfqg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3udzfikms.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3puojyxib.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3clqrswhp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3mkotbsjt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3weuogdst.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uveleffx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ctbcnknz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xaxqgfup.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zrieanss.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kecrrfdm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pmezaszk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cfoaqoov.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3kumvjyim.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yzbebdum.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ahkkunrs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dgtvyozz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ioadadmk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ivsxymxe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3uutsllsu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ympeqsbv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ekblevny.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xkpqoiba.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmzjahg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hlzxxegh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jamavmxd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3oawsbyay.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ehibrwew.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xwqrqajo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3piwfxvey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bvrkkdsx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3myabqhmy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fjjutaro.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ialzjonn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3evfdazvq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcsgymyd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tredqqsj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gkrxpytz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3flaggguh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ankafumc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cczaavqd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rocscdoo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bjqadqed.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rcxzhaxf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jqefueqs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zuutehtj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ueeqzraf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mtwuygju.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qbqlcedf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bwvwhfbn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ckfttbcc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lwsnjeqe.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nyboswus.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3osbidjyg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kmgaignm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dcfzhjbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmulnslq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uluamugu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzthffxe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yaidzeyg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ctxgqkso.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rvebzyiz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfncikvf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jptvibqp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aixkgcbm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gthtggns.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hadttgsl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ijqupunm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zdximret.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3lalqoqlx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wpkagrja.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbndeaai.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3slxevcfq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3zfokpsfp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ovjjinvq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cmgcrqlx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ainfdrlx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ylzxkvjh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pujzwnni.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbqmujdt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdzqwfzl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jcoafebn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xlbmbgxg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3cttvizjt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3dgytxnjr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3klmzfkkf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vrkikzol.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ugfnniox.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3whgqplku.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yixmorqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nqgdzkji.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ljhcsmwt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yxjtfwxr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ilxhpzrp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ffgcbafp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rglxaasq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jhdnuljb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3estbmdsp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mgkwydxv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xvljbxuw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3lpvyxbas.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dbyfrcnp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jpsdtoml.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kzvgspui.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jaycuzwz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zmarpxaz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nuqyncdh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uuhyxiot.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vmskptye.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vguwdyby.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ecajxesx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3znjavqkt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tjqwoqxk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ufumnebw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3lqyrftwt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pdpairws.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kaijormx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3olgxowjd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jyusulss.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3luruzbzv.html


<!-- 参考信息 -->