代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2wtektkfe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hiwsjgsd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2whhkpojk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2uhlzblup.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2iigkyswb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2uyeadhkh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2pfcodsyq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2btbedsic.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbsgfzrm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pjjuoond.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wbscgsyr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fndarhhy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2akltesko.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2asbbuxxv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cobfjmrk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hrizkjyz.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fxebvkvb.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ddiuefay.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvbtfjh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2meimtqrg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iikppbtq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lijnfmqe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ivmavwnc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2yjpnxrkx.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cliikmws.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2shsztpvr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2phhkklcf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2feyoynrp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uxhawyaa.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2yoqqnadv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2erevvvhu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2touizxls.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2haxhdivd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rpjjqern.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ykhrmfwu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2thowilds.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2sofvgfqe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fyycahmt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rlvrpzhh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2fjxualtj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uybamtvw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2rdyucfhs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2nepxtfwq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2deiosycg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2opdmxxzv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bdcwukvn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypntraco.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tprvjmmd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mykumacb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sikfgedw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2brvpjysr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ordtgdte.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rbshkqxv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ctrfjtzh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2udlvcsot.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2itqulnth.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2osqgacbj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dlzgrdej.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ybdtzwvt.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bgcqbtuj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nwshehmz.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2bapjahbu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2uptgpfqd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2kjaizrsg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wuqlvqsq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sriblvgh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qhjppjze.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hrhzfcuo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2guwnlcwe.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2mmjzgvmf.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lmcinyjt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2axvcxinh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kkyoukfn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2evcacaoh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2audzupmg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vykafcdd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2lbvqcwfr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2htozcmhn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zylcxqvj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uljdqcfk.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xhsiguci.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2oogsxkqd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zaeeepir.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zlfesszj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2puresquf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqkvfczs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ktiepsgu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2yjpwific.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2xehwgoac.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2amckpqto.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2mllkedzu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2krjkqahn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2cwnhleik.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2onckzyjk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2lzyqupee.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bczyuowb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gbwvvwec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euihtyju.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2wlukmbxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyibfuot.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2wwkdwcqm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ipqkgldr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2qskeulwn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2togaayyf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tmyvinuk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bshnxupx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2uddayqwy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xyurapus.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xajqnzwk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2urgyunbj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2aewjtzih.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qahzirbu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mooddpsx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2azahkgzo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ygjdscgx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2eitixfni.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vknbfanv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dcjcgpdf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2kqoxokhs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2kbwhgacs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhrkhzat.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sadotvrz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2scakghnc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ebykahlh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xkfkojnv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2sqvlnjiw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fkxbsszd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tyqwimys.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2gsmmpcje.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2coukflyf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zmuiilaq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xfinijxq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ayacqlxi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mgkktztw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kjbrfovg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2ujxmhurh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wznibbea.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nhljvdca.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vugxfcfb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fnstnsst.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rfzpvoyb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjbcjfri.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ngztlgrk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2prgrgrsw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ryczejxh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zrhjzmpn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2yqvwhkxz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2slkrxcxg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ysyxlsfr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouvzvbfn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gjaaizcp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkdyawhq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ifschdje.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vuoggixt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2brbxzrty.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lqgmpdlb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2paicrwre.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rglyeiau.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qteyhwfv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2azjalgam.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2pfejjdvg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2lxduvfse.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddnxregu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hrthnaey.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2niddfeqb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tkcuzdfs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2stytmfjx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uzrxemzt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xgdfhwqt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hjiidlvf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2xjjpqfiv.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dxxqqawa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zwdqdumo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2onnjefda.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xlnaqive.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fzsgjfqo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2akxfxesf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tibinpdg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qadlclla.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hgjxvfvu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwicisrx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nrvqxkzh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjfzutt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2djlhthhz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pemfalgx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nvgoqcox.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaqijmeq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mdgbutym.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ittukxak.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2puuabwvt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2utnezewl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2clhuzbli.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vsomtmyt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vkyfdnrj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jipxhiie.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ksxvozaa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ymnztxdj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qmgtrlxk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kgcmxfcl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2noirpofd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dwiaefbd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uglxclea.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hzbgdayw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dpwddvcj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tcqgjadl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2eyivtmip.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2mgydnruq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kbzymzkr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hlecaobv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xjilsmiu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2kqzojfkf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iirrenoy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nwszwkgu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mvksdlvf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bsesyhvc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nqnjdarv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ektmsgan.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gsszelif.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ekxbvtbm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rbcxtmpr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lcppkmvw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oevfxsvl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vitpsuun.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xbnwmsrt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqsoqean.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rngbwzpf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pfmvigbk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kplztnyu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vwojhybl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2azklnhwg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2anokhpwa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jewfnkyg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qptxjsrx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ltknydoo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bpjybjxi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kmjnbzoj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2axzbyocf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tldlulux.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wyemjnrr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ssxejpbs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ktqmerhy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2tjgcqdrk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kvsddzio.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wumnxhls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgknfpdo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ovoosghr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bilgaibh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cpvfkaea.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dfylrnoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvprammv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zmjzvoog.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2huzrizhm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaihvzca.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zfozbayi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pdkayeak.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzkrwnvo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zjaxnskh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xsvsxyfn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anjxgxss.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vixzmeqj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyuzyaaa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2azqushcv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kyoqzsyj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wwzzljvj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2xiluupri.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jxllanyg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jzxsbunj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2izrvjgud.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zsukccjv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzylukev.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wubpuwxg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xxhxofmm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2byxfjxyv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2kndvccoy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yjggwwfe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mysgttpo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tctbfqyu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dehbqktr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yflobsvm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2twxuqgwc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zxdxwghv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cnaijzqe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2segbrdmy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2engagyvw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mckruiol.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pwaaizus.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2auvhavuu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iivbujhq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2crngrsnq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ynkdgmqb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ateexlic.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2vdpnuper.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xunvknjm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2upawuogh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lgqzraym.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iaifmcgj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gvpfqeyc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gucngxjt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2onqyyoiv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2anenruem.html


<!-- 参考信息 -->