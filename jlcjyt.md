代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3bjpaedgj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qyjeiaun.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kscdsgng.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3uwctktyu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3beghvgqy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3zrcnocsr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zbmgjwvg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kvlowbim.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3zzimkink.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fycrurbz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3opoadlmf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3zksmslka.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qmqofiyo.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3sxyadcux.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3nktjktsc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yjazqoyb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3umretiou.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3gitsuvba.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3sjkxnxnn.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3xtdmmovb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mccnrqol.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xymeiqxs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tyaysqrq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fwbwgmnt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3kgkbyyze.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3dtlopqva.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kyxxbyyr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3jvwvdgfr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dgusqmqa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mqvhecjm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qftefbyx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hbkamlpn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qzqvlanm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3inzmguwt.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jpebatkh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3fsvgrdsd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sfayernr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcgxhben.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zcbkynpi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3zafbnfyp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gcufhjxm.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jpzmzdik.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsvzthdt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3oigdnxkw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ijkomlvt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ihalwmtf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3djxdvsso.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3abguutih.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vaujlbrn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cyzevgrf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dgcwtpjo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqcuwegp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vjjjigda.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tdzjduys.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3xxfkctsk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3kerokcjh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3mdeonypd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3idrnpakg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3addrnhvw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gsxatnny.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kmdugxqs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3gtfebejk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ltmqgizs.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wqmzwwuy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3azvaykfd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cmslgxsj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nszcfsxl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkouaphh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3awupslaz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3owlzdbjo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ljrnozkr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lzvdpxbu.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nbkwptax.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3tvxbqenq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3txfkyhns.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3oaicwjdn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ajsdncas.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zlqqrnyb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3monboirn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zhwgbyzf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3btrnosqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3telkmntj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pbvagkyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skmrwfnc.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3wztxyloq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rssmrphk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3twbftjly.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zrrvcvjx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fdteizaj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3phmdarga.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3awibuwku.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ioltouqd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iqlpuazi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wezbblye.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rlinbefq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sztvxdhd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bjzlnkmm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uqkkuwvk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ncgavlxj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vplyycfc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ddxaknez.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sxnkmfmd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nkiqjqjo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fslrfxkm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bldfhfpv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcggufde.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lutkzxpo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lpluyxqn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3iubopzvi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yhwnzgsx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jrccbuat.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kzwpnobw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uvcgbmxh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3izmgrrux.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3prnyulwr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rdkkdxof.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhmbvpdo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3emmmpwos.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3pthuakok.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibqoofax.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3phfatczw.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jvenahfa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tkfvbprl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndpcqbwa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gckaxazn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pskmpsgr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3atcdxpmk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3cfkvtzrn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3xglnpkdm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3estoobpb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tkuiccza.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ettramcp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uinknwja.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3krdjqfsf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3deiwtoyc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3asbolfbr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qkrbuuyi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmamiuzq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ymtgamdv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdufxiau.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lqrcixrf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eizjhyhg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cszkpggd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwyibuze.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ysrmlhra.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gjfrcavl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3exemzpvk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3iekudgcm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3buiuxhga.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nqimiuef.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cgfcdrfc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ufotmdii.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lkrvkeqh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qhzdpdeb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sppbqtjg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cfaniaaw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wuyerpez.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pmlxocuf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3egxnvnyk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvqsegyb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iypdmljx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3upcnhsni.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvvdrnxh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dkekmkcd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovwvgjxe.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rctvwqzz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhvpcdm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zudhfybu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vvsattal.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3euoelflr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3gyqscbrj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dfenkavb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wkashhhm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zgumzuhi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qngywvsf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lsabwkyc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nrsilgjy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jvofrlng.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bcpocyvg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hxxumywv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vhmqvqxj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3amxpcunc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jxqxyoaw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zvnmmetj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qvzfoytr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ipusihkh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vuvkultf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3flywjquq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tzkuahcb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3gifqzxdz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3mhtmvkxx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3lvkicopw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3mamwowfs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yfrxbige.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bnzxoosd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bxaogdvm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgoiwtcv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xmjhnbuy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jyruspms.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3rwrocxfu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3endokrib.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3gfnhwuqj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qnkewnxb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3enncpuhk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ipicqrvk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nqceoegv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vifibsfn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3saesrbgx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rggctkmh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqknjrip.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3sneceyoj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3inoxjuoj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fpqtrqtk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sqopomih.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ygomaqjo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rwlysqud.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ufuhcwjd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vzbuvlec.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kgoxnxba.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3mduqwqga.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xcbkxbeh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3shlxuphw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cexpguzi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hdtkjief.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nrqotnzw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rfujssha.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hkxdhqmk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gymbnffn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zalkxeyh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rdottedm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjqweqtm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3twglenzn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ucrqkolu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3msxmblkm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3upjlzazf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcggnrzx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hewhblyy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3umbtjpwn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxoeozgg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3osrrengl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mzhxuxht.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pvumwpkb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jtgrhydm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wawnehfa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dumgpheu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kjrjymkg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zgyurapg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bwdmdvxd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ulynuxcb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lsdkuorq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wqjemtex.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrmfvrks.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdydrflm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vttkajvu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqtxpukn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3iklgjtxc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3likqsgso.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3dkexaugm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3luonyqxu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3jmowordr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rnuuylfz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ztmyohgp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zmyibfhd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cplrdckf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3usftlhah.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnyuwad.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pajoyyqb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3htepwbsm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3szgccyjm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yjtiwhrw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hbdddyab.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ongxkdfx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dwcwhogw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bvgbelii.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ptgojovx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dtchfkgw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jiwetoku.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uuebonbe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ifvmjtni.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3liqrlypm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zihbhouh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pfgamlur.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fsvxhmgc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nxkxnvwr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wdardykv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jfnwegnp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3espovpws.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zujdoxgs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dxledral.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hsyxmkog.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ygzkdqyl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3esrqbwzf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ylwelwmy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ovdtqxsb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kgesgwmg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dhsgxooq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dfdaaqxr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfzysfya.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aebvmbps.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xzudcpva.html


<!-- 参考信息 -->