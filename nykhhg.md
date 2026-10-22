代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uwcilaof.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zccxynka.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xlgepezh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2zaswtecr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2hrlimbtj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cfgepkoy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixgttmsc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2lijbazcj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ohzqpijr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kbynjmgi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utrqemzu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2rhyewwtj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eurtdxrk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lzmlfhof.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ufhvttie.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bhrqmxja.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yqsexvkt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lgpjojgs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bxhnhnlk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2clvxwkep.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ikklixlg.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2amcyljfi.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2fvwwffuq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zlgeygok.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lsnjedro.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lcbvlpmw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xhdehcik.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2kxlhqazq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2roqnbiur.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ecvwlwmz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ijbquxsn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2srlqhkrv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2sakvdpeh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fipmuhea.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2yxmcpqxg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nphbtetw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fhlbqabm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2gucouaya.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2byozmsxh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2shqxsirx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bxoyrroq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vrnuzcnl.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2afyrgett.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wtxmttvz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2cedmitkp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2fztjqlvx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nelljdqy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2twtrxqdc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dahpsjpx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pdebedmq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2kgqzzmxk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rirjyklp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mlzuhbxa.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vaguddrx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vqszfhcm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2tsyyjuyj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tujocsdf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ewlygpyx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fmpngpjz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zqjuopug.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2bldedaca.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2wbclwxxc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eayxjqjf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2shhtbhvv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eouhyxgw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ztbgsyba.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2sazizavn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2nzyuvils.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gqfkvtbf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oeawospj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bwfvoyoa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rlzrwwhh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yzbgeary.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2hiowccne.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hwaljbnw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2zdcrdlhf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2mvnuifno.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2didgiasc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pxwlpokj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tsnulkjh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rcczyzmg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2vkbrbbsf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ronegbxw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2egsimkol.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2txtbfisb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2izmidslk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ikmyltra.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbvjvaed.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2crjmlhul.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mrukmjwz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2fighbjum.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsgveppn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2pshmhscq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2gxmcuodr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zttegpxs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2obsnhlwr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2agvdnbuh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2vlemqpgh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2dppnhvmk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ozfhdpmo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2fjnoaehb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvhcwjzo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2tagtfeoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcyrhegb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qjniwkqw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2uuaeckkm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2daeerppr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bbejogru.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xsfbfkwd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dsfxszro.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vzyfcsvj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ifcwatbm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vezwiawk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2aiyfdfcf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2shzrjmqt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mbqyjani.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uxrdilfe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kaettyro.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nomiugdp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2dsrphfkm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cqnziwzy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ayrqypus.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vvwnffed.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mmvzpktc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wdhuhlfd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rblhqqcx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xopjvudi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gptrxcmo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2edlbtpng.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2wmimbatl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wdnuwzhw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhikijkz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2igoawrmk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2lmwvmrwi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpnzvvye.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrzxkgan.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qxwphidz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2inuyefom.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lvooachi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqqreni.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xdonmoho.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2guylmmpd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2xstriigi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfytkewh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyoeqlat.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2eyynoaff.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bfpojjjx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ilhkngiz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnruxzey.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nibtshci.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hxaqylgw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oevmhauo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gnsundvv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrzmfnda.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwojyqoe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ysybuybl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2hmckwind.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpzeelnr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yrxhhnik.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2fpymmgda.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtqafkus.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqcirums.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2plahrmqn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyyofqiv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uduynkdp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2avnpeqbu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2itzkuhnn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2kbogjphb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2khnowihb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lqfqkitl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ixahclom.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mfzluamc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ifzvykos.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ubvdohjn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ptbkwecy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vdzacmmp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2szjoiqbi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2soeizzrj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2anyklgxl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ivdqnqiw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkjjyfld.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wpcgfpmn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vxdsyknl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wkbbeunz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2voteitnx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mdrfjqbp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mieuoomk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2icvexbto.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bytkqynu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sveifmsl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlmtrqwj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2omsyxdwh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xtxwlhhd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wvsspgwm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2isfpvbnv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2oirbugmi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2drldljzp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mpkvajjb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tsxkobhi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mjlcqohk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2dajwqbfl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2lwnrlpak.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jmfufhxp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2srpmzxkp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pwtdvbkk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kmsflubj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2acrpdplp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2caigrulx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwxicnad.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2azphjakq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ayepokiv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2yljanpdq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bmwuiiyl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2awccfblj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nyslnqyc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgozydw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2drgobxks.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2sqzxevwn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tacbsxrt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nuclyalh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2repxqowa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wgbwkqbs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2trocsffj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hjqbrriy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2swfrauul.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ssswwxuh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqxlnsmu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rpmvypxz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ponmmxml.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mhysdqmx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vpoldenn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ktguknrh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2lwmwqykx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2siluools.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wxxuhdqx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2adpyprsp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qcdxdsat.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vvfnmsvh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gxznxaki.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hewegthu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rnzkjcyp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctgyiiqx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qycwswhm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sprpseam.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rdlkfuiq.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hherpesa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2emkqoxkv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2konbusjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyminqhl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2muqwsbad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kphloipe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2glcvbwnh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2llbubqxb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fngmjodf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ltmlnkkq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2usnnsdtn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2buiyfhje.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2miipgvzo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2soaoksed.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pltcmcdp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2alyqskcb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2llaktjcz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prnilcdq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kastmsey.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2slheavhl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2vqjulrgh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2lbomqajd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lpxkokoj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2eetbyusi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pdkybiwu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bxxntboh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctcfpumu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfxonhhn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdjcnjsq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkxcgifi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bbxvzvaf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfdscvfn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xsspccaf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dvnlqfkt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2zztcgsee.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dggkoukp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrolghdn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2txcincmp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2eggpbrkg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2fxqxxgjv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ahivfktd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zjwlbhxg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2fvjhkyit.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ypuryhio.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wcyglzzx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2czmhspgr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xkqvfvju.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gpmhbgfh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tmvnhudf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wgaawpkm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2knalxaru.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2caogjhdz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2rtzspoqv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ybceeibr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zyabxtfa.html


<!-- 参考信息 -->