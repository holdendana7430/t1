代发 wailian999

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tczlolxq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2plzztygw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uxpsyocn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ilcmvdel.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xhvvplnx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2jxsetscs.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rnjagzby.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wjaobjnb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hpninyae.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lvrjfhpg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nksagirt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pnqqxfgs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ydvhldyv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pesjzqlj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xnoxaqlo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2otowlegb.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ioejsocf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qdqzxuiu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2igrasaog.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2iugnlhzl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uvshcnaq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nbgjlube.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xopnworx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlifuvfd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2qyzsmpcf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tjfdxdle.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxdddlke.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nvmnlnfn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xpybwwpv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zgppbczq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oethajjk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vvurzqrv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pvvxaire.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yqypozvt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ccacpidc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bhrvtvoo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wuqqfvry.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sspfkfyo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kybviblt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2trqhpqub.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xrgctbbl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ictlxxes.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vbzaoxdz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2qgsjjvpq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2rbmmjwig.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2kjcobjgy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pefvfyaw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2lxmpwdga.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2wqwrzlyb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dczdybxy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2tcknzoqi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dszentmi.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ypsdnhga.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nvxxualx.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jfxxdsjx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2bgncyaor.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hsypsqce.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zxfsfukx.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mgcgsidd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ocybrggo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2eupmpyny.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jrxnikhf.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2eabvmujb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2micalnsn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2qwqwhjlo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tabnzneq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xronpblu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkuwzhh.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gljjdnqz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2htsvjvks.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2haefbkxd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2aphlxdpm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pqfkiqev.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2vodlypkk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rjgyanil.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ehjbsnwq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ioykezbh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wjuljuws.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdwomekb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gedozkhf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xhbzsion.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pitgghsf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wvkrisgy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcxwnwix.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wkkfgfcg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ukosrklu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xxnosljo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxwiaop.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ajyabgib.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2tdnvbpym.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jkvolytz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ifizxtmk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mycozvce.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vdssqblf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qcstiyhi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lnoaqksk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2krsxexre.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2dbuytsvk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ilrrsbue.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eitzdduw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dvqrdivv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2rfvfbdqh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kctkhske.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lgvqavan.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xzyhybjg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wyggjmai.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2gwwvjrxo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhiwrepb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nsfjkzku.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2sjinfwvj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ubsqdwro.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2yhxhgdao.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rkbwkbse.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2yuxvhjqd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2pvujjrca.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2grrunlab.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2heyocycl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xoqgsugi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2taelsupr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtkbgjer.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xdlftoyr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nfwrghge.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzcthtqt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tzgohkud.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ruqvwtvp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bagfoevw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2btqqhrss.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mypyijbr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2unmuxcrb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2glwdcvsk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mbehmcxk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzyqetqk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uftoapug.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vbqbfomz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ymbhsjqj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2rmselwxu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2iudjpdta.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pqubgqsm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vzghmgbg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2urdwgfbm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sbggmmbd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2djjbefam.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozeyixsg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mhrjqfbx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ecvbmvqv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wdwtehdx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2righjwia.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ineojdcf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nmoyrwto.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nafkduln.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewmwfpcp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mmprdfrz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ttvvzaxs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2oqqyzzeg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2gecogsqs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eepwwnjz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jfyncifp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hkaequjy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2actzhmac.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghbdwopa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qzvcduer.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xkxhqbca.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kvuyutri.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2roxsscns.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rducsmfv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pkhilamu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bpupqhnx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffctgosc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktgosfly.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kitegjsf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qetlucbh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ekfihllo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2igxwurey.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhsreteh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wdkrwezx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2adajvgou.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rbwhgqqu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ogugdtqt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fmfxgfix.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rrzbwlqy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2bohoxeiz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zleupppe.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqwlemfb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2nbcdyoyd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2smhmprih.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ldtukjko.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rexupnmy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2etukaaeu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sggxlkud.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kmbslopg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2txfdzwak.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2opdwxzqg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2paxcqbwb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2icqmwawo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iassheys.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fegfdbvu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vtlapotn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zztfuwkh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qmqvnbav.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2srdbvbzu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ltweicgl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cblsdlzp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbuzlrp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsbqzkrh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iewcttrm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qyoybgmi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xecjuwzc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zpieqdtq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2govhitfp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmwvjeru.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hqnvcatp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kjtagups.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uzhjgdkl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kntztecz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wvuaqfqs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2htcfhdtb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ofqgtdvd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bgmviptn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2oqmhhalr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xvnxhtbr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uumbesnb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2cvaruimk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ttdvliva.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ewkrnbzn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2alwpgehc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2cmzwmdry.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2uufnrlfv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mwwcgdgy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wgmlwxec.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ajnzblsz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2qftemqvy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rthanjdj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tnyyxame.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qglualnl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ncffzpai.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2otetgvvv.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2goyvauye.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2deycqivy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lkxeqfis.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2stzzxogh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bpiedzwj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zvcmbyas.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2solikgaz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvoncvp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yleeqpbj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xczjotlu.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ilryvqxv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ehtgsipt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2knlkpeiu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2prcnlcnh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vytnmxmr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hwjqvims.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uakbouxh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2chuoikrj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2txtifffx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pvgwgitl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2drblblvf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2khpcaaje.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kiogsbzl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wvullvve.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2acjlsjvg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rwxpawgj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2uenctezl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ayohixne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qshrprlo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2alvphoxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qomgqflr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksohmrll.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ewtpkpoj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2locyehnx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyibnzbq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2muzpggxr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nvmwjgwp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xibifzmf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nlanhweu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2crhkequi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2qgfgefkd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ngknctyd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeugubjx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aisouqxw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tkscagtk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fitmjatb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hqisanun.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2izvolktv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2idivtiem.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2cotuztey.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lzirfeid.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qadxwtlf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wqkuysqb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqidnvxe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wncmxrde.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdtfunw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cmavklyl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xanekirc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2shftajdc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xzcnmgna.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uoklunzn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fswpndjn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vajetmvk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mwlbqovu.html


<!-- 参考信息 -->