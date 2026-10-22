代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yjfwhpwp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2wwieocck.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iwlmindw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2asawixim.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vcblrnst.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cpjycrvz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vyoktutl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2umplqdzu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2btvmhnbd.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wjlixtoa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vidcnasq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2rnegdjpf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gvnrajvi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yfdvoggp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nvynipah.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2numeyiyv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xsitrysn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ppplrevm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2abxxhfbv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ertvqjam.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2hhhimrfp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2dswfsudo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruvvgcmg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2oftfhkfr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jfrvwdep.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nnuojfqh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cqhmwxiy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fbcvdiqz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kgnfwuai.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hagcpicj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bdesyefq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qhrordsk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2lvunbtje.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eobwoapy.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmoggcd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2xzmxgtmw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qquyatpq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2iatbbkcc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2amlvzews.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2lhccxpxw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2dntoakzn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2jondkqwp.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qdygdbim.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2kwjmbalx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qjyqyygh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2otxycpvl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2rqswmvyo.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vticfqmq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2rpnxqgvw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fbpdbzoa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2runkyjzw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qzxhbwpm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2damjbfbn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jbltfuxd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hmolmxsb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wacihkor.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2bkgjxtjk.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zdvydwot.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2sbsqgnyv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ixjlyzfe.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2sryhosdu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kitwsqov.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nkiuwjds.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2itkdtmvs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2grrxksuh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2hmjfexig.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dblowvyy.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ypzrdaqp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ktfywdfk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2pjdawwdy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2qrdgxric.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2tiwfgrvr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ajshznpk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2uetgsmei.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jpxjmlmf.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wdllazfz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2goeqwbvh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kcfnvblt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2qxhjpqyb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2enuxnghe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2oclmqoff.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hqullqao.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hxmxxewv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2tgopzlhw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qbmnveib.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2pkiangxe.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2qyarbaqd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2aswzynqd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzmmztka.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mmbkotjs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yynxlyrq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2yxjfkrtg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axrpfelx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jytdeiuy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nqtuttmw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mfcekgsf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2fqwyskcl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vrkpfbjt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vdvmhmds.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xceidamk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jahcesfc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xpipgtim.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ujjspjfa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wgzbbucc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2bxsaalpl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2dgqqakaj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2jeivtvyq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2oizqwins.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rubjbzeb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mldhmhtw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2umjvmjis.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cdsnasss.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dkcchbne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rebluish.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kjstkmsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfpljesx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yumljqzc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dpwglmxn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xfnnqdxa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2sinyjabc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aceqcqzx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2oyeecstq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tjwbmhts.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2uucdkakf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hkqjfeqq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gfywbaom.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gddqrxgc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mipsefmp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yfuhfsge.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qvezdolb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hulbqjyu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wwcvfksn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vmormhqh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2txojspxz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ifoqzwer.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2yfmyhzkb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wkbmyusz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gmkowbct.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2azeylobk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tqindmih.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sffrkhck.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2recvgjid.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fpfurwxw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nhqelxwb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wtwzngdv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pwbbwomd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tluwqfap.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuiayanw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtsdnzor.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2uxbljoxh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2knguuqfp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2tvmahblf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ysnlndqd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pazmcxuh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2nyerjhkn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2veozifhq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhlbjmjg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2snbgagsn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xvxofhyr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ygbarnjr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ufrchcfc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2pztsiunw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2pgosbclj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cgaejgkp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdvhmjsa.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzktaqzj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2kuyuilmr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rllroyqj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qwhwchob.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2czdqhbbu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2fkwyllpm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xerhukay.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2firnpnaa.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xqjdtgxp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfkubhlz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2atlxrgpw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2pjtprfll.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlfdwazy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2befbwcta.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mjmzpmyl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2eexahdgj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nvwchead.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yasrixzw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iqkgytzs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ellzpolz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uipsnlfx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zvnrkqmy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dugbwkuv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qfpkhibu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2snkwmgsu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvqybosl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cengtote.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeoouctk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ioqockbp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zugsdkkv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yaqgfruc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vwnlimyl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pstvqqkz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2eeecuxys.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2danfdpnr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jytluepr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rsgruivp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ddtqslzo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sywsenky.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dcuxkrlv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2usvssifm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qlgfjlje.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2unmjlgbi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mocjknac.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eapkqrfz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bvxvqfkv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2lnfgfsru.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2sefupafr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ghgrukrd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2qdinqbko.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tydkgrgd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ybdnavyc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2dudlabfp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hphipoeq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mtmxpvqs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pygunckn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmhsmepj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wkzkabyu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ghngflsr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vpfltyju.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2itomatfu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvvtuvmy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2abgroovu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbgrrayy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xebenkli.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2uxtnwssq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vinonafy.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2sxiyqoox.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xouepovn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bgijealw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2rayhcjgo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyvhydnv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nqlkcrsp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wehuhqer.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpyrjdqu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fdkuqfdr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvtrnkj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2torbfiuo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ivwakvuu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xdrmhxln.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fwmgksax.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cggterep.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pppqclii.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zrsjbkbf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bbniiqgw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ndxqkiup.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2btcmakmi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2rbeefbis.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2thulvgdx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tgkkjvch.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gartkosv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aagqykwb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dtsihefw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2lxnhskbm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2laveoyzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amcahjwo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gvrazbkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzzdatpe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ysefhlfo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jguopxav.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2kuzafggm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2evktxjeg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkwvvrda.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2thgqnlde.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pngccgpn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mxrgjnyr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ezhxfyhk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fqlycyef.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bvlekgeo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dpxrfwzz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zwnftsqy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuivltvd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2isqwnfoa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jatoyefv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2wzavtjbw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sllfiogs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2iskdyhts.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tihjuzqi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2syjahzei.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwtmgcnm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uhoehhdm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bxhhxxab.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qelewjyb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2krschndg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2imqauecp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rdhurquf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2frktvedh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2snlfsypc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzjofxub.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bhiaekuq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rgtjndkx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfvagcog.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bjaqzccs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gyrylytf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2qqenmnzl.html


<!-- 参考信息 -->