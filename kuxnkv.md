代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2pjdcardt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zniltdgk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nyrjhfem.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2dejapshc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kxxbqriv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2uiwflavn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wtwbzsza.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2itxbnrwm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ccptssyp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ifsshegx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2orkikork.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2mmzweuzc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqzhbesq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2olnrlnpz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nuplprug.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vtvyvotq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohactact.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sxqlsysh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxvkttjf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hpqgokoi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rmpkgsdc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vekorlhs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qbqpaykw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rmamhtwg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zytgswck.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2osgbnwqz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2syicnrhg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2gshctgur.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2pkwrxqxk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2vqmrwuyv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2giqjeakl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2zblmivac.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fhernfis.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rptqwegm.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pwgotser.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aiisthgi.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bzyqkjvw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2mlxdglns.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2nhwyzzyd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tiubqtxu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xbhjxlug.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2tffjxlsh.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2hlqyqhbs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ptnqjwvm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2pujflzpa.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2sjutaxhr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2wjjrxvlr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2hacmqeec.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2prjykgdt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcnjlgo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hvwmsubd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahdnzgie.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zhpftrcr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pxhzyscq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2iefoqmlj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2vvkpxtvx.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pgpeanjr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbqybbiw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2btppssus.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2covnhlzs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hbyulaje.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rjnhgqzl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2tcgtqkfn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xqphurbc.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iuiueprz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vjdckbuo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2trxkftgx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzenqron.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2yswftuwc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ziskdiss.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ewixceme.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjpccsce.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cltnbmmm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2mdaizyxk.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ubdjqgue.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2rnjhdcpl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2stehsfaw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tlibdpra.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zbbuhoas.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2cbjsgtiq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fugxnheq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mtrycbgt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hrpcaopo.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2hjaddfqh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2agdbazrb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nenfqced.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bodzscwa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2funmsedn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2utkqecka.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bskanana.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2cufdwgrw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2igrqhtjn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zeuhfmou.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2suntkrjx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2fdxxtipy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bqwkrwec.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2bwkgyfdb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzdlmcd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2szriysun.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dyigknns.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nlfjjtyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtimfkln.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2cgxgncxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdudwjhv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uqiqbpap.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ruwgcrpu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2pzfjvrjc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ndnullua.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jihavexn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cmbrthzs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bzekjsix.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bvlrqgow.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vhfwotlu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2sairebwl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mxwevbwf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gtzdqyof.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rpdcrwsr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2izszsfbq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ulajzgnd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rfmmyopa.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2tygoeaxg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nntaevwq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zrfkfold.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lvdhwnae.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjysyeiz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndxvhfvl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rfbkkmyb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hessbzsl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqfopgkb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ozqbjwid.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zpjrclpv.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvgthizq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sdrnpaek.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkbacuyz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fbnambdl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjavnion.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2exyjbehe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bzknezhk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2puwyiwja.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwrqgwha.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zbevnqyk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2humpimeq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvywfgml.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2nnnrgvzv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2abpiylgg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdgiosje.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gqbgmcdb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ujbehtpa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uptwhbme.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hwluhsbh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zgzxsgsd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ohnnmkol.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bvtnqeqh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijvfovul.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pgsyhxqc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ktjjhpzl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rrwplutp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2zremjeyq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ajgnzyyj.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wfitjjmo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2osbdmlrr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sjaalyfn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mtvwysrm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fazzyzdi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2oddskekb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qqxyrvsm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jxhowbdn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hoeyhsaa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ksubnjxz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uhpzigpl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xecwtnfv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xlefpmcu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dhbphzsw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vojumeel.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2nlbbhhgu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sglscydn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2dokdqtib.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2eegiwtca.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrqsslal.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2geexleel.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wbcnznch.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rbawwwvj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pdiqegtl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2dtsfwjeg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvkzclt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2inccktvp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tutnnfcq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjhoctdx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rmqkgxfb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cjjejybf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zygvjdqm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tjuykufm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vsxtuwvt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2knpcwqcd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2uaxcdprg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kgomccnn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jbnvgdim.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ajkkltgx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rokwkxtp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hrxkfqma.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2hkgovdmz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fkwlchwz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sehetwdm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nbgfhfmp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vztlwvat.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pblvnuwn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hycqbwrr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rvhxsvcm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wxjfdtjk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hxgjisvn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hvrnsfnf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hafefnij.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fmilrmtu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2eqjkmuah.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2rjnvdwsj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rofxadpu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fnzzpkry.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qhderfzk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cappqxhd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2shlweely.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lxuxbnrm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gtbvyojt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2vhpnxxgk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2humcrqje.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mphdyczn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxtdoly.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zzgmgnlb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2sdashfil.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjjcbae.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vefybxtp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ragwhugv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wjthwxha.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gcpqpebx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rgttyzfq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kpmkdxsa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mcxdyiii.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ajgafzyh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dovmacts.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fjzowefy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2etkgxcfw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rpzhpqpm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzbzqlcj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fopezscq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fvxxawmx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ninqzmig.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tnwkrzmy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ymcsbjxw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kppzdkxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqwbqzih.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uokgjaqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwtttdwf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tashxsrl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2slnlpvkr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mpgtmuhs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zaqdzdbk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxvchheu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2inktidef.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2urgoewlp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2itnxjtrb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2njiygyjn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kpqwstmd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2yjxxfphc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uejzetci.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcrvdxqu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grlrhnsn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ghrnrfzv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2sumfcuef.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sanzanlz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2udhekzeg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uzoachlf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfkvjdp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2miwivhct.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkuuzglt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvhbthqh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwurdisv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2btrtcbfk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2uoaoxgsf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2lgyobkvy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xmjwqxnt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ffsiaclg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dvgvlyrv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2villvwab.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ttvpkjjc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bmrwoula.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2lvcotfrr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgqqbofh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oukmpaiz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cjoosbam.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vlwdulqy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zonbcpru.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bgfydyee.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zjcrjtzl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dftxccos.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fuqtzkxs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hsyatrwv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dsjkjtqh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2duypzgbx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2elljqyoh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qijdrsjf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zezgyivh.html


<!-- 参考信息 -->