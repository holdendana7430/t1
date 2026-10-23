代发 wailian999

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mxuxytia.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eyjkjthb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3potccptt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wepffmhv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3yqmooinn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3pdpvijza.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ngoflnqr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3djbdnhph.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3hbtoyddy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ufcbswyp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aupiswii.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3iqdsqlbz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wdorrjvs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ecllfesv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oepehelb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhczmkpo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ufoqqnvc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uttmgaju.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hnljpbqc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqcwqahm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3rvkqdmyn.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mwxgsqjz.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qiwjbygu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kyjtzsxo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3uucrylvn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3fslofzrl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3dzfbitof.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3wudxlzhs.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mxjyttte.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3czmnygxi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jdrsavle.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3guovxkkl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hjtkdtkc.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3fnynnnjy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3negccika.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kxllquqd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3mqykofsy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3vykknibh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3wtlsbwlv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3bchzaesf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mteyebkv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3jjzzhgjs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3uefprngv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3dntmiygg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qmyyoxkx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3pjgoyngc.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3jytmfinx.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3bwhgwxlr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ijhasods.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qkjmdsin.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3exkdvrtl.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xgcwsjma.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3khuydjou.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tiqozxrz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3iihpnvni.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3osnbhxde.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lpfjntwe.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhqmurui.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3qovbqvec.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ubrrigou.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3bhweksoa.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bxwicyvp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3bgdgyqeh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3aosebmpx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3oikhtnkr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gjhfhezk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ueculula.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3fwjwndqg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lvwsbdqc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dpqumawf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3oodkrvrc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkpyiqro.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3esicyjzh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3youxnbkc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3trhsucdd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ckxlysav.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajruqrnw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vkbtwmww.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3obzvripq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3asxyhdlm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3otuhtnpk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ynkcmnee.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3izilxvdm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fuacdony.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3vevyeelc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qeooojan.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cihefedz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yydgwdtb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvekgslk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhazfoog.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3aoayctrt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wadyfmne.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cmdihkmy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3skjkomxw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3innqiais.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3rjktscfp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hdtygsfc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3befpfvbm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3skzsiiio.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ybxihiel.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3tnnbybeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbmkqedf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3luzfdatu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnqnxmbp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3nmvditds.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3otncuech.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rpvfkkkr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dpudzyrw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lmzleaka.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xnizvkgv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3fbjlbpwd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3abdafwcl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ydnapnvf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3gnfkormh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fkzvspvz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3axswidjg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lbikyvgf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vmotkjcp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lnuvkqjo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3jpxithkf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3yckohyow.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3njwmvqbd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jhlmlyzn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3isqaidha.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cqsyhtpm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tkkqtrug.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ftqnmlbe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkmwvdbv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hsaghybb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3dpqxiwzc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hgcjzwlo.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3elpdlomx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnwjioq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3uznyxdnz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xlbphcms.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqdlpfjp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3smbrofhe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3yveguale.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rxgfwanv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmjgdogx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3sawknfzj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3phdppzbq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zxhywxss.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gevmvsoz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3slmltptj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cmhzbjpb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mfmenwmc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3gfiuqrrh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3unptjuza.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jgisefvy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3oxfralpf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3misrmtye.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cldtaakt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3txnkrwbk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmwmhcdk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3aacztyio.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3swoxklir.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbzbeqy.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nbcrplng.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qdgjzwjr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifcnrfac.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqyfjphh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dmitwbai.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3icjhasmw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3lxqimkxi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3wpymstcr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tacxgdsd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nmpntwav.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3rxxlufey.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cftrwcjn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qsdqwnif.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oavzrvgh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mtgxrntv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vrdyzvbe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3twpfekzn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ptvbgztq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3sargwyys.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3namukavu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vnvmoigj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lhfckibb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3piszydvo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngotcmke.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3egwkueau.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3hczpnssj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wqiuvrtl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wxrjxqjp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3swsujufc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdlgqlcs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dmkwbjkx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3moraqgyz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3llpztsgp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jmhvdmsv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lgovqdfr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lansbugs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xqhexmpl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3szzpesxx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ndqkaegg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jsxxtbsz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lanqdigt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xkkgmijk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ydsijvpi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nwvqsilc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgtasmj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3zomjsddk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tqkzktkm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xuchihed.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjyvihdp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fzbrihtd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fohsqmdi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dwsqgmjz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3hmmisetk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3fgoeowqq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3oslkwwwz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vrqbjjal.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3oddmbxoe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qtoreghr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlqurkyg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3llnfpayx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ccqsdtgr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dfydkdhd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nheyhema.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hncperey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3yyishyna.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xghfmsuh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3udwngyfl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iulhiryh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rcxmualo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pjtimvyy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgraiyu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vfzfxhpy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3esckzgxj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tkzixahz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3sfpvuzyv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fhbrrsxg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fjigbnlj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3snalvdfb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nqxffbxh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3luvwvplj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zdumqmih.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3icmxbhbh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wwjgzhry.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kknxqwhm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bqojbmnf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rphrkvsv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jvmpjpvv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bcsujanh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3akckesvi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ffmtoups.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdvgifom.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ukifpqkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rikckxif.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lpdtrxlx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pjsumnxo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbacqfzs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mkhtxwve.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnrmpfhx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rzckeois.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lzibmezl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztclacim.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gapsexaq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3glzldhnp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jodajceu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cilfrpsy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfsjiwbg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rettukgv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3invcstuu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgpvptji.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3suhvaxvl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vwdirxfh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3abnjneqf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pdswhylq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvkysnjo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qwtqbhqc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksswqtjl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3epudgveo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bxtbvtga.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3aohkqrhc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3oyjzhbhv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rhqusqcv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ttocpzlv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qfehoauf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gcziyoom.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gzvumuys.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3qdtdkhfg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nepnlwic.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zprzqdsi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jaemxbmq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ctxfebdd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ndazphgb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3sfzabhqs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iayfjozu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tizpatll.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3adlumaqv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sfnidxdp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3njdmkhhh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3iykshpbx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mfrgvutk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3yjektmfv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jdtqigch.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yfcvqwrv.html


<!-- 参考信息 -->