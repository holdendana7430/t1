代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vynkusay.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2agiiwcwv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sobdavlg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qmwbwuoe.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2oqgyfjmv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kxhqqgyr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zbqrqyga.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2byjdzigf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2aovapssj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ylzpxwis.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dpasxucv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mxjhvace.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fftlkoxz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qluxopna.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gjjkwubs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yboeifjg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fwxbkwtz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yaepwuvl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2kiybhnng.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2azzupaif.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2sxsqnlov.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qdqjiqti.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nceajvft.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fjdfbjjw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qlghnbfo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jklndamg.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjikxklq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2nqweywhn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2kgpeutep.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hzntdkpb.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hghupzwo.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2rajgybjl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2awaxctty.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fkytambb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdnkccit.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hcbhthsf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eiiewcmt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bsysqhyu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2awtpuwkl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2koznebmr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ireussoz.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hdzfslnl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2piyuyjku.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wwagnmib.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2sytnmaok.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ykgwzxar.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jytxmcba.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2jymcmqmb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ndzufxpd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2amincter.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2nutnbjvi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2wqsarubu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2hoifaofa.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2eicpcuyf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2nxesunyx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2olujddnc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kicvvvzs.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2qpxufvlk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lmvsadwb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2tqwqtroz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gmqiqgag.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wuwfnacw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2agwivxwg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2jzshjloj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2zbkhgoxi.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zrpvtcdi.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2uffedstp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2jyclymhm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2sdekljyu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vvitvwqw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwzqclkz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvwtcxpe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ovheywnc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zczzzxpv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lolveprr.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2titjxcpq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2szutlenr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2naulmoya.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2bwlbkhdc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2wccrzguw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2bjcylsvy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2njzzoely.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ezhxczxg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tqlavtte.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2tnkucdoh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lfbqdoma.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vpzyqnzz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahgmjaoh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2scrfvicm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2wxzpaywy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tkajojhs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2oizhpevq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xxntfbzp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ioivwqrn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2oruuodmp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2cdnlmzhh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfvgxjrg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rgmavbbh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rycyazhn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2isfryifn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nujzisro.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vgwmvdbe.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vumpprml.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bqwxoftc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ujxnzpyy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2irdygfzo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtmvvvkx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2khtfmbxk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2bhwvkufq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2aiuyaxqj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2dqovizfy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bntghhnq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2svareaeh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2dkcqebhx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fqfzbwpe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ldzpjkkq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2frkdafco.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wusttwki.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vpywfxyq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2xfbxwjyd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hvdkcaid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztoicuee.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ukotbnzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wegttzmt.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xmritjcb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qnlemvhf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiilgeoy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2srefllhy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ugztsllj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bmhdfwsd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmarumk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2kdsvlnwk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2anbcxvus.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ndwworwo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2agiywpmw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ctwlzavl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qflopnqf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jdkrfgfw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hicbsusw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pggxyopu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2sgoibien.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2gdabmqrg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ivwdknph.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2geondjio.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gpqcsdhn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpigtgge.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yratjrrp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xiyyrufo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2resyjvmu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2riqtowwc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xosdpyyl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bunmcoua.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zunwdcxv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mnahntmk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2whjlahyi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogcnkphp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pdbhmoyw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qwntfyxy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qztbnbpn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfihvlhv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bvfesttz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ovaiqyyw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2drsroqgq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycvznkrn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uoiwsgoo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2whsueqyp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvbqzxkn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rdgofyau.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dawtbvyj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gtgjzpgw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lhriccgw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2tgwvermk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhohnazn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqxfvrql.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xqyxammf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkoycimv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lsyrreaw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2apwpbplm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ozsmikyd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bnymigwf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdpgglmf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aclrywnl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ktvkomwj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ktnkehdy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rcdgrper.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2krmatfdo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xcujaoxn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2hymeibwc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lgcgqxua.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lehyhqqz.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tzgefyef.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qgabnnll.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xinbdaxh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qrfoxrnn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xjomdmhc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kqfmscej.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2omypyqsv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2nyigfwnh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2reyvaylw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2socjctip.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlutmcqz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eempjsey.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gkxunuya.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2yolpkrgr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fwtfvyyu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yaycrxap.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bxqdikrn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwegdpbq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bwpayvou.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nfwdlofl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rplodhby.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wmpzegdd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2larzgtxc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbhuzytr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2lipzgkqa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2nfqbibyi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dmbclrwn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wfcqtows.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qrnfckhd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jhrbvowf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ulwabfhn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dyzmuehd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2uqpevjpr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2znnzvuws.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ufqvjndj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2krgizaur.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jkdiqmxw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jfefdnjl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2llgigrrb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmxrvcpo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2sidazjgk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zpicjfqw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mymurzus.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2tpekback.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2aebhwyai.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qketuetc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kupbvyin.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nvvsmtus.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rgdutgwj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cwifoahb.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bwymvxpt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qfrkuqpj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2unwjyohx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2cqkqgvem.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwhiqfft.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdcijlh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uekwqjha.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xlmfddcr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mmkdmgbx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2klvavgzs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dkwpweja.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2arzxwgte.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xpptrmcv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jcnnbhyy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2enqdqjfc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dsfztglm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lxuoyxtd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kagohyvz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2huiwfcox.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mftpfugr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hxiilcpn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2aslerkso.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dxaglsok.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2twqsehnb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cjrlwhpn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cibqziwx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2yxeyvfiv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xzgnhahu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sckuzsxy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ibxqecsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpxfkcpu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ucorqgko.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tabcgeqy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cxxjikbc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukxxetix.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fgekgobo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dnnnhxlz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kldstyyo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2iputzprq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gosifriw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2khhadfrg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2iakhmbck.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kbtmnnbn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eurzdqqa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgolpjfa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2clyazhcc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ekvmgpnv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2mqsypihz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cavxtumg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pguodkmh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2xxrvizmy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpoodemi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cibtadbh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mzytnhvb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lykrsyla.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ajayxpko.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fwtdgkxz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2dsjfnlip.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pbfqzixe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xbtloikl.html


<!-- 参考信息 -->