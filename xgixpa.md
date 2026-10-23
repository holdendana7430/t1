代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rcyopgvt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fkicgaeu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3esixfonw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jyurepmy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ehmdtcou.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ytyevcgj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzgksoub.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjpfophv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3atliredm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jbobaxqi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qolmvwhi.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vhubssbf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ygiodixs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vklbowcs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulfhhnlx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sjbwbksz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jsilnsnb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rvmfqayi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ewuoofqv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fnnbsoia.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3avgmllrt.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iepxpatf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjmcgek.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3izjpldgc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cqszmvjt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3uuzkqttk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3nehkjuwl.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dirdpfzc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3sxtlihqb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3plzafqnh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uxlbgtjz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fqxasclx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rwuzyeyp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qoqbowmf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3wcqocwgs.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lodwpmcw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ydklftny.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3fxhncwst.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3pkavajdk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hiwdkelm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nqxkjgjg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jeostbmc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3flxgfhdg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zttxzxvu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qpztfinc.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xtrmejpg.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3izmgvnko.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ikfrorza.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3sdleavhn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oodpaahk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkbzijck.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3kxxoljqi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ejycizmb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ygdkgure.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pepphjtg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3trqknkov.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3druxmsgy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbovslb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3lsjbehsh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3rqcmdlvm.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jxtaduhd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fzrcknwo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgjkysua.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mbibfnkr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3whdmmusv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3axehiiwo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3aztbmris.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3cdfbcuwc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bhrfpfwz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kfzhzxqe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ghlgudyh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tgqjfcpf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3otbyqipj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3gttkmkvw.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3bidicsgu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nrbdpuin.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkctdzn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tpqjjcpi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qrdoevms.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3kdbjenyc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3effyjjbd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3gzhnuqvj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wxhiztgt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gnvekmpg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3mulhvzfn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxjbdfjl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukoklniv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3wcikujwj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rzyzoqzf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3iehvilvd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3gzxifnfe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ykvvxvmm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3jgtzmddy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ezdrwwyl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wzpdbdfu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3yjwahnwz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ukszlqma.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ninibizy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ikekunyl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3exygtqqu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3stapkdrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spsijtaf.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vfojfzzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxclbxro.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ufqpganu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rkyjxtvk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3itznqqzc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uortehun.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ydqouftu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wwrdlpjw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3jcgmjrhd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wybwyydw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jqxdadks.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3cqlbrwyk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wpahgyzn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzqwghou.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kellagsa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zqdlwcrx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hwunryhs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3cncthmis.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3usqbdcun.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eobdvfnl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yoledzyp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ysoodzcg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwauroow.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3flxwkoll.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xvhiqcmp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iikoakbl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wzsxvxvz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3libetzga.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3meilcxiz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hmanvrkm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vbfubjat.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vvdpyjxo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eufmnmzv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3votadrzt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmlwnknv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3iphbdmbm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cdfqizsr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3drkcnslg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wwvghyhs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ltzadfak.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxoeezwr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3taukoaxl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3usefhhfp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3xazoqgth.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kiuytlry.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xsggnspe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3suyfgran.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vrdnrisz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xpdtvesx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmmeecnm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gahgplwk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgjyuqpd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3obolpdck.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3evtycian.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3umaczyhp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ixvjqjid.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3buanatcv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3igtnjvpf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlkfuron.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3orkzxwcm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dmbdmpzl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3guezopzj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3suqmbcar.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3ivcnxnqk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaifzkov.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zgkxvijj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lclpgkio.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jnlpyxua.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aqorhkqp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xpckhyuj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vzeywdik.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3imzwdodq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fnmnpnkx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cihpivpd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3wpawksru.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3azyfhlkl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yemxofng.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uexlenxf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ihtdmcun.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ilkhfvck.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnluurzs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yoxobbqm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iantseap.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3revyzrvl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vixpbgeq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ysvzaawt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3edpnilhu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3igdxljwu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3glhfuadk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ogyowhxr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hjomqwjt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhbkzcse.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pgkqjoqc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dlpdozol.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tdchriwy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zhjwrzns.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ogvlehyf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3xrhcqrxe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qevorfhq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ysnieird.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qrqwvazn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ukwyhvuk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3lsgzgqlf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3opqtcoyf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3izedzpxh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wmyzijpt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfjatqpl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mjbbhhxs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rxgqtrrc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vridmoav.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iimngugs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kpnzxxny.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkbrsxxv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxtumqbq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vfwxkhzv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3lljzmkea.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ocmydkol.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3juzcrlrl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mnejcfnb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vbvfdnkf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ofzaqivi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3wrfpoohk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mncjkhkk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3znrkgrig.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bysxuhhj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3lnizqwlh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfmwcodg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wjsjoosa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hvqkgxly.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3shlwbofs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nnkdmutn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ybquyvyx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3meckwrgx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zbrlhndp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cqqgbubf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pjmdqemc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yuwkekck.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gwtlinbx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fcpnakhw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kssludks.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3emxzaoql.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fruusfat.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bocahtaj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rkzwskdu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3iassrxwk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rqpcyliw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uynzezla.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kvkxiyyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvnbmyvo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhgcesbi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xrzuigvt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwihqgaz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fnqdyuwm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rfyboitk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugirndjo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bwvnskje.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mabzwkdv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utnrqrny.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3eajfyith.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3icczmhiq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wyduaeqm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwodfeir.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaacfrds.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dkevmunt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wgtpohwe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vnpueapd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3nzlmwtol.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jguurqvo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3deamnypj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3iebwrgmu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvevdwkn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3luqwyvvn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wfqanbio.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3szenmppp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gomikuuh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hpggpbkj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdyvxrea.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3odlfuewm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ohynncly.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wphqbgxe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ghimnapf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nflobxdz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lkmquhmq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwceudlv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ylhpcbet.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xgvuysvk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hgqhlduj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3blkjsgmo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vdgsnmzj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3nwmwpokv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3uhsepnra.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vhkqxwjj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yniovedd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3eblxlmgw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cobvshdy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3loznjvvr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xzvnpgyd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3konirucx.html


<!-- 参考信息 -->