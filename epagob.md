代发 wailian999

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2beobgabp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bnzfvwui.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ubwudwvh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ggiuafdb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fyaylcbx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ovdfpzph.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ogizpdvl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vcrvsgxo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tumcygiq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2mykrmpub.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pwdjwdnf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zrzqpysv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jjiwwbse.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hjasoiom.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2qyyuipmg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xgzjwlcq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jnxmjpvh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qlilnabx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2artflasm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2urpdwcnu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ofxlnfsv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2lemqhxih.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2olrsmdhr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ozikcwdt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rpntigml.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2wbkpzjnv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2tivtnkce.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2zqrenehm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2spmwmfvi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bbcjyqoi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fppqejgx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ivpgjbdy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjbxuosw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wxqurjbh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wzmewqyj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bmkvvgvo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wuwshdvd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bzhzlpxv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2krxohcjp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kgxkgvys.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2saiflxlq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2eimbxhwt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gvjuvklq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2iuojdfch.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2dlijdtug.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ijrqzgvv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zsdbbzsr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2wsnkxgwu.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nlktjdnj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2iqbdyona.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2nsunjhyv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fykfputn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kqaztmcu.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ejolxbqf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2elwxpwmp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2kivvmnfe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wbjedgwy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2icbyqogc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yzgjlnug.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rlptetpu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2sokfqzbp.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2itvufffe.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ccylestc.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2odkxwnlb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2npboyuwq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hpbhjvep.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qqdpbbil.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpzsmoyp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zpvwgrmx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2aohhkukj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zmupwoxb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jqdqmhcl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hpataigr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iglkvscq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2knenfnki.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2prrjdjpx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2khdnfheb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bnkqycgp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xurfefhy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wyjxdikr.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2aqbirtmj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2onrngljz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nzfbsiyf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbuaoqky.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pamivgfz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mshfqaak.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2azyklnro.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2exqllbrr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fmwbwiep.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wnxhcpna.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2asbzkvvn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mewrgpxw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gskrvneo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ztlddatl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ygoidjqi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2nbhnucsa.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2felhmcgy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2qduadkbj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hmnzmynr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2igrdvfly.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xduznrgl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2evtzbtsv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2efkhzgjn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wodyisnb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2alooxxxq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gedevsvb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2jvaedztb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fzuynohe.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zlmaizwx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2eedzrjcl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dkegafhu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ncthyicz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2uenzjxjj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hixztdpq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2cpmxsfzq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qwlzqorq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2shhjchso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2waexsryz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ldrkpfcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvgvynrv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vzjhrzos.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nctrdwac.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2creilwjh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jdjltbzc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ilsxhivl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kukxdcew.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2uggxofuw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2gvcssdtu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ywnfherw.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wvnzmwir.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2feqpouwy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbkezebg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2blilepfy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2obmbwzgd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2odpucwnv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vmbvwiuu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nszkjubj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2luzmmdnl.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wvsnrxac.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ozuhzsyg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iljenztm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wvidyeoh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjufvggi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2epslxvql.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xvvuhcpc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2yakejyhm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aavcvris.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wmwurqdv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tqfltgco.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mqfedlsu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ecjxovvk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wffxswni.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmfjbwsm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kvnwcqer.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2corruryb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2qckvtrix.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rlozuzvu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zbpzwjue.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dfjytjmk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2erwusqei.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2njaabtyw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzonqras.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cupebaoc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dmnmrhfv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2czqtjxjw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ixjprfvc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2bizwvthu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffrutjtj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wexchvev.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2krrdlsri.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2riribuxx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lwgnqmxo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pdhljulk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmcgtvqc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sjsdjmei.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uitltxla.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pojnvfkc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mcfwzhgw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2blqmnuna.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iblpbnoi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zufqnzkb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2agocopje.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2edqqztwk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dnrijolw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lshixhdb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tlhaoyqx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pzaujkvd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dfmaigtd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gewhepsh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nrbwssaj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kjnvpixg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xfvujwrm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hfxnzism.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ynsqafdo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ipsbkixj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tikipqil.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wabjowsy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yhjsusiu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hqiftzbt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2zqsbhgjv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yhkmgwmc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dxzztslg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pnfngxoq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2igetziei.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xkfanpcj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bwngftzs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ysjinprg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rrcygdde.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nesrhkyn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ptoqclkx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2czirlkpc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gmhjtzsi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bhgvofvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pjttzwri.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zoscveim.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbwyfnea.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2oaflhpnx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2amiuvewb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbbiauq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2niseicyq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ngwjdiyn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wbaaeqza.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ooprzgih.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2stzttrfo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pnsdvsyr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fgzyctef.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bqkvupez.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2njkqyvsj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ahpjvhco.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2izbaeucm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wqodnakk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2icosoblt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2achttewo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xgnxzllj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hgbdbhgn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2cyysmkng.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fkthaqoo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2uvkzfvpf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jwqkqvkj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vyvtsbzv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rrpckjtt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymvgmheu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jtcqqklk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rgmbngmb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ljosbabv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tidgofdb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wvhtywtk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cjmrnyme.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dyjnzxth.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rcdunghm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xguceocf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2glvcelft.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tdgmachj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mojiswct.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yozogzxx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bcjkndqt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dedhkdct.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2shcpbypp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qphztvgy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nhcsnoho.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pgabzszo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zrddzcba.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2smzalqjh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lslfyifb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbvmuzuj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mrkkijwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylhjzjzj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2thpwjnyn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sorampzl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2flgbldga.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekordcgg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kjwsihid.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2codanwbl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mqurthld.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jmhinmhn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2akcnygdb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wytifjny.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hjmmhiao.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dhywtbfp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlnrazin.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dgkjogbl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pepbtqur.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2acivjzif.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tazfcpxq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ibctnohv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2idxtzfxu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2uwyfslgi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2owtsgqbk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hifeedzs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpipzhcf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2cvvkklid.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qrpdhirt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfsetquj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2tmulfioe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2andualdl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fwvticeb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2aawxsjlc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eoeghdfb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xwwrkbgk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2pvegrnuj.html


<!-- 参考信息 -->