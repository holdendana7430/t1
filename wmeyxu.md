代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3modhksql.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3snqvzhuy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3scepwuwi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwifrnnb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3qtsfrxgl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3buvquuck.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoxequfq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3mjjhzpdb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qawoxmme.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tanpfcti.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kayuewqw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hgpiwelh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ivxizphr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3folkiqex.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekprwocd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gwwlkqei.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3yvzfeksq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3owghijfx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mhwphgtk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sphdyoft.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3yoltfuaz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3ykuywtbv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3fkqwtxkc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3tkmokjbj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3knkyxmex.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3izmoproz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kstgrbdk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kepgnzrx.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eyfqcdzt.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3bqkwdvkt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3kbexedqb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nipkykmr.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tjtfampe.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3cgniegjs.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hunnvtsd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3aenhupyq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3zbqihuwp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3feioxvfo.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rzfwbspf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vpailnjj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3rvfqnclc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3toxvtyni.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3taudlyzq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3pawowzjm.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3aibdckss.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ljknxhtt.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxwgnag.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvmaikl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vplkvlkq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jxwnghrc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jelnzfut.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jhxbcyyf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cuobttmr.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pkvylyyl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yplmpdwf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3gerjfsgr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3rgogvrms.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bvkcphhl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vbjkponl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wmiwgtyc.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3stowqojo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gmmkryaw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3yadpxoxz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3iyymdnya.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3bexgsjgw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ouolicjq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3arzzpsda.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewpnrmtv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ldseyllk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3daysuzxh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ginrdvij.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3cyucqybx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdogqclp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pksjzpdk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yozafxxl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fwdxubqa.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ldnclwcn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ybxbzqay.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hvnzuwaa.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vzbtnzhb.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3gfbuwgxm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lyonqprg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xooibauj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytnbldqq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzbahexs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnbrtcbh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3llhuptxf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mpncbzms.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3uxsxwjpa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ylfoqbxv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3vzjlikcx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3oejdpzdd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nsqhwkdl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nngqiwdj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xgjdszkx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zxfcxgou.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3etctvyhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfaonpyw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3fmbhpmuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blslvldc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ufeduuvj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3zunvznns.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrvetbxp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rsufdieh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hcpdouuy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uxtvvzik.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3acpugxfv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qiloebpo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cpuantau.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3corjwwcj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3fzaeklnl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3acodnela.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ckrgwskj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lcczhsaq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uoumbrsv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3oexznmmv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3afbrsipx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uynmtdlr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wqaspnal.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ksitctns.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kdvdpxvn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wzkqujhr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fafawmwd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mzsimehz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xahnuvty.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3qyadqblj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3lirswooy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zyxjenfg.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zhrvbajc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3liyttehd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnayqesg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3addcoemf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnnysams.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3aldncomg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ztlataxi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wpdctmuw.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dfzfmhir.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3datlasim.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cphamwrn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzwgtpcd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3usabqyod.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zwdyzrqc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zrtsnftx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3eyeealze.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3qmyevxkl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3cslfywhz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfulqcy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfjlsuyc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kqjkycar.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fanwyzqi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nqwkukle.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gscngesi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kgogmoqp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3deonyllm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wnlevyev.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtkhnoml.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ssgplsbv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dmkoxdzc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xqmmdmhy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iwzgwosu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xgfagrig.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3jjxfcmcs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3onomtfbg.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ahhbadho.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3piscbkfa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lbmacilx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cilwugbf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qzejnyyu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rpgcfdfw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tkllilcc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3imfuvavm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vmmhydmr.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ntaiauhx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3sjwftcfz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zqnltdfb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3htiskjdk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3crtywnak.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tzotzxtf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aloiaaam.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3anefniij.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dyoqnpnp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3mabtpaho.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3bahaulzl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnrirvsw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cpmkvdhc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ytikthzr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkgarirw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mzqypndq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ijmmpbyk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hszuncgn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3spdmrgyy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3kptqfggl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yzodndyb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ffdqvldz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3amzccyzd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3rwptvpbh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nypftcip.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qdgnstaf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3dywnwqog.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jvomsrqv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zauxmvfa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3fdyaoypm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ebrwfsof.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gozshqst.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tccrfkis.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vakeoktr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rujjpqbi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rubsfwqc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3eqpogswh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3umhuzgsd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrhymgk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmnpkgop.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqzfthru.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3goicnisa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3qcroaium.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzxsocl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ksxrubpf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xepqrxru.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hnlcjyol.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xlcyxmvy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3djzwjwbm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hghfslsv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3joylesbo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3iwyqynfs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxdpjoz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ugzkpbnj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gembfrgh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dipldqqj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mipieqho.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vbnuydci.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wvigfedd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xesccmbc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3naczjfgk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xegljvfm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pxfvmayp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nwzigwdt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3lcjlvqre.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ddxkping.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gnbmkekc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ipbdinxs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rdvychde.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ujtkolsu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3nhrgsfce.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wxehclnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmovkpcy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wvrhvmav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znrpjzyp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3grlhyxgk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3gcxhzmeo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxsfzvra.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpvohqhn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xxnyjldm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jhdzknwk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dokwapxm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wnzydokf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3irpfzluh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zxxahnxk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3afdylijz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lhtjzbuq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvyvqhta.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqxdzsa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qbrjktpg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3csyuenek.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kfmvcrau.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hfohqvek.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ddldotxj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3eqmtbbfy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qgkiegae.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eghitodl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3czvdovsy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mohllwwc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3doaekiyz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nkfdkags.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3wfcirsrg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rfnawyhm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvspzpcx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jqcrgywo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdjmzarf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3auxptqay.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fcgreuuf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3woyzxqky.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvcrnydb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wmljpyza.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kmsskros.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ebtpfvtz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3obgcyril.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3phtfrqgz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fnjjacbf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rzvfxhew.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uzbylmbm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3wreyhzsp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3medccysj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qnriicux.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3zccfufgw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rnjulvox.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kezpxqpq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3shzmkhdj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xkgbyvpj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zmtskqis.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lmpnkzdu.html


<!-- 参考信息 -->