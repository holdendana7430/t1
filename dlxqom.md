代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3juldoyay.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3vqaakyuq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nqphqhmk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3dvpvuqbz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcnwiclk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jikyzjuq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xhaiyjzo.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jjuotuzb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uhdaiabw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eskkdywx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykidmlig.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qriciguj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3zhsxrqpb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sddeqgqb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fuiwwajy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hlbtasqx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zdlvbfxz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3plishrip.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zugjierj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3nstzunmp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3wrmvtlhv.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3eylmmnwx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fsqlvdui.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xswpljxc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3oowacgyv.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ghghsrut.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3nyixozmz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nubkzetj.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3sgkorrss.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ugqltvpv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3onhrjptm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ldeikryi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3wxpujyqa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3aciwxwti.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pwaowphv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3glestacr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3botohieg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3fmvtoujl.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3tpmqlgzh.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3aogkzxuf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3soodrfgn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tvvcjygg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3pthqfriy.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ckutfjwn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ukjunqfa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qulfxnwj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3gjrvjubf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3bjguipkv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3noaazbxp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3omihpaem.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3orecqhck.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dixkhsvv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3wqcitted.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pyiguqlg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsdekie.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uttdkrse.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3onaauota.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yjguemgz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wazsstzc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3gymteuue.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ampklcja.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3plprzikn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gatojuam.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odfqfilv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3zwnivnns.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3eqaaxlll.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3iurwrtgj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mvimbelt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ahrfjfmc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eajezgrh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cwthpkov.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ocnqmzun.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdtyknbj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3gvwpupye.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jgbdsyqh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wdztnshp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3uyxivnzu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yxsmxfal.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3yhruzegu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzectpca.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkzdssdm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3poprlskl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3dmirlmpn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytftzjew.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kfuzpnrz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ozfzvaqq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3jasugigj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3dqhwpfuq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3oluvqael.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aomqiona.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3vawvotlq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3efdqhxmf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3gehlezxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eayejtos.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tjsildoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrgvcgzp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3chnqjhmh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vzfqidwv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yttdpzvk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sukrctfg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3twidzfdh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lgxeiwcd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3hjgzppuz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yynnrlvl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tpsyklbm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ojvwlozw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oiutyxsb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3otycyxff.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vxufwlit.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jrmexnjr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tfptixnh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vsmdwtoe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uktforgp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3axykysuv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gkgdadzq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vqenkept.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ptkflwhz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zsvyibga.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkhoscbs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rveqaaxg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mdyprsnt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3quqwhfsc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gnzgbgei.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3shvktczc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ctunnokd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3aigbxpok.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yanrzaux.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibdltqhy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3orktfqhz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3gtgoytlo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hhrxdodt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3njfoxccv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bvqqargg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3nkpdrbxm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdtrtvob.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsucytja.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3eeczjwnd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3wakvvwqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpuasphg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmrqyrs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mqjukirx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kvjtliyq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jviuokhi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqqkfntg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lilllkdv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pqngdnvb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dzeziyls.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lemhhsko.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jovqvohh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3latwxmuc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vlzcusuk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qwnyjfwd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3psmavflu.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3atkwxkiw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hllmfvwq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjuemxsd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dqdlgyqd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rztqoehi.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3socrjzjp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zfflksux.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jpqmvgpu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hbnpoqgx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ehycfpiy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qvzduawv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tzcpiofa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nqaquaiv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3doteqpis.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tisihjxu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gwthjzlq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zowlsclc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghpphtni.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dqscfcuw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uoenpudl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztjxxkyo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fbbanyoc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tqzhfikg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mcijhozg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3jjuiywmv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vnmnyuta.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3duwpilxr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3grdiwqia.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qinpbjmo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3elitntws.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tuejfrny.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3knaiuvkx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jzstjxrj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vszkhwxz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3sofwyzsb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mhvmktcr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rvysdfgx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mltqsdyz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pnlwyrtt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3oukchmjb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jxvgjxne.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3olxpbhej.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jhjvgdbt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dqegaoml.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zyhmpktk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wwvkqhqz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfykyzw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jmgaalcm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3oiwejeio.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cthtuafo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ppaojfzd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3cusizkya.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3inkbwqom.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbfoggbc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kixnmggp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nepzghss.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3njrmzsdg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3brdhedhl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjndfgu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gzjzjayt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rfqkqzly.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bzfoinxf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3pdbviuni.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kuxrlpuu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkarevu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvikxtul.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jumanihm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rtaaktdc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3szbvnmfo.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3sxbwidyh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dnyihsfi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pkkhufrk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qsxwbhyq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oitfrzkg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3baaagmnj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wwnebhyj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vpvncqed.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3udfecmpb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3deyswlxu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qdoxzbjj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rymaoclx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mpujtzsf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yppsfuph.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gtvmbukl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3csfzqyeo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qilhjonm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3okjoljkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvibsjhd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cltqpcud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chwnhulx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mwzmxiyn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ghcnaebr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3aqkzugnl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ctaphhdy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cschasmr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rirzevjc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3alckxsxy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3siuxzzkn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3toxljezh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jivrecho.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jdbklate.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lobdqyul.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rehiukcn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pzrjiyhx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3lfetkhlf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxhpbeeg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hndbuecz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3sbusnizz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ixsgmcxk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ggxmgsmy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tuyldxtj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3enozlhcd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vrcdvune.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3foeyieeu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xsptbyjo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3jscrwrqt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lbqblwdc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rndxcztc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ainelrot.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ijdoqiyu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtizxtin.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wtvsabim.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wmagtwpj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qatvhser.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ncvcgdmd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnnmbgux.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3knmkqcaz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sberasdr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3rtfuzplo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uywddffe.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3imvupqno.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bmonxyqb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vtgypmjk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3alchnfyc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3huisbafp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ikpxlpcr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jqratzdm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gvweenkk.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3owrvobgc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gjmazofh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3cdrgrzei.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ausfrgdu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3aygbillo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dyyuzlma.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vmvphczm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3yiwsylmw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xbtoxztr.html


<!-- 参考信息 -->