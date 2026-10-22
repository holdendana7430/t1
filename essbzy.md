代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xmrmygst.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2konekixk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ymcdhrsg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oeigjjnj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dhbyndio.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nbgyycrk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ktewvbjj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkewtofl.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cgpgtglf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ermmvczm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ljjfrxem.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ltvmbqfm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2gbratjho.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gsukrets.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2iojfclxu.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xlckmige.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2afrwmpes.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2dxzvoriq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dbmwgwxe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2aznfqkqw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vogceltk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jpucorrq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fqfacape.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wikyuyin.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rsfejhgz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2jlnorzwl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2cjkealzv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2qymrkgur.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2kdgcfulk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tuouwnwg.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ahcpdfnh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2abtrxfap.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2omudeqxt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2tatcttdl.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2cyuxhujr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2trttdbaw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ginmpupe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mwbikhpi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmqxqoqo.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ukuejatj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gzxiqtjx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gzeothyd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oyfekmkd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2joaxdmcs.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2girdhezc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvdhcyxo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jfakyfkt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jdkcmcuk.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2tleuzrpw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zepiqhkt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2amwcushk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2cmcabysv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2vshdmgkk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vwzyjrvk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2adommhox.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjrjlnn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ojhuoorm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mzjrnnoi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zthplpdd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2uyhyoqxu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kxwrufyb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2nuboiahn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2sfmahjow.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2kxuduhzf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zwvxuatk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kanoqrgv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2fjepimjm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xihpctrj.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjqrruxv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2hwbladoy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kupfbcum.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ujhyokdz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2szsidypn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lqhjlymj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yywwjdzo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wquzlyak.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmoipnnt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2nxatirpb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xstnrcvl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cbudqaon.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2jeipxhlb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2qnqfajby.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2aurztoji.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2jthclczj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2baboqehl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kgjdfbwc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kfvwrqas.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jivnpbho.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vaaqspsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvfiwtkr.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ehyitkyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zaiznmfa.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lorhfcwp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2pujefkee.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2fwyrcnko.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dfrflyek.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qwkqhnog.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2upkzwwqm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2egpifgek.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2niygzfci.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rckwvify.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2mvmqxmvd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2huqoqlfp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nztgrqao.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kxlinbob.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yfihfsvj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dozzfqpu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2aeiscwbw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2eaiqohpe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qgdauzpz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2vafukmxb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2nuzapcsp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmjgackw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yiikqycc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bvmmcqdv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmduxjca.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bgdkxksu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ianvtyxs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zqyfjxmh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bhkrvdvt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tfeltthw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yffaslnu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lsehpbqg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nrwsdrxb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qcchlyvv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mcgzkxab.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2olktuhts.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2atuzykwu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2hxyczpfs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrrblge.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmagomxz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhrbtjbq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xjdowmsz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vauwoorl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ptbwxgcg.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2dblzbqpf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2epxozdhm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rckecivg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kazpmnsl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bswnhybt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sljucluc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sxlrxwww.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qisyofma.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yxqhodjn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vxaxrziy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehiukwog.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vjfqycee.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lktuxnnz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cmcfiewf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xyquhhjp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fmkwdnoh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsfwhnrk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2myfokfro.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2exdpukvm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2haqgvalb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ogodqmxs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2mluftroi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gswbxmxr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2usyjdjxs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kgvunjca.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zgrlfjcf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndnceiyj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2umiqpdmc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kilmxupf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2xpnlonrx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijbphgmd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2atjjiemc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vyzquylf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjcyazic.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hhaunkyx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uctoimsw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfslompz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2diqzwsue.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2tfsbypxy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2flgwbsih.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2leizbapf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pbmnpoqg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jrwvcwsj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ntahzuky.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rqrixyrb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2irtblxbj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fupzytrz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2mbpedjqr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2phbnsrjj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xekagyro.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2crmidett.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kbansjsh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ubzsrwtl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2smktyodd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qcspycan.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sfmiksuk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2orxhpgbp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2plwfafrb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pndimdey.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ryodnsly.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qzkvrdxn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rmcoazan.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rcudrstk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ozztcpga.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ctgoqmeu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2tpzemoif.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2osqenkyg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2myqflmfd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybheulbs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2efhssncd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dfhnczjx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2atqgflaf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wamykrfb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cfvdvktp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2pgeducnt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2oboaikov.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lrssqdhe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vbvjzpza.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2usvpwbju.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oomsqwjt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ccopbqko.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mjjanbsk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tcvalpxk.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pqregjhm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dxmfofrk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gamxzuoq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ygruyqfz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jykfolyf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nzvlghpv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jmkrwson.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xdeviyzx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2doukprzy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nuopzwza.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ervuqlmr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2imhqzyve.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iewxbuon.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zjkkxavy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kywccvpm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2whqgezis.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kqgmdaoc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rpzssarn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twdodbvf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2toaszrux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xsbemyci.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fsdkgswg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eifecffw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aigbtnzt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2psoomtpm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lilxdzde.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ajmqbeia.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2adeumqzs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2akupewik.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qfqtlnrt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pxrsbcfi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jxqspavw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oouehwri.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jcnujvnp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nnqwyerx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nuepdnao.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2enbvhjxf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pdziwdgm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2dofrazuq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2eoxyasfq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2krnywmzl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nphuodxv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2taqnjsoa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzvwypmh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jeaqizlj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fompdozi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yzfjmncl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qgpwieeo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2gabpeznz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxcauovg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwjfgiun.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpenrkab.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cduotcsh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rgimbulz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2aqwyixzr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhtqjomk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkjditvm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2elilzesp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gtzivqdr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2buhtzmdv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vukrlhwj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2thperasz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ezocgkji.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mpidgkzi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fssxsfew.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qnnvxgcl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xzeukyut.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xwbbcktz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qtafxjdg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rldoizss.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mgsodlrt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2snucjolw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qrtgfjtn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bywemijn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bhzpmzzo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lsihtudz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2phyhiadl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kczmhjqb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2evfllmpp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gjfqyqjp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rkybgrzd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2nettkdwr.html


<!-- 参考信息 -->