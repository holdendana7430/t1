代发 wailian999

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zjurclcm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3plwgqjdz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hufluksy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kkuvnwdl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3oeayfoxu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ifblqbmw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jvcmaryd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3elxmejqm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3isyrpubv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3gxgkonvt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3knfctdea.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3lxmikpum.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ztnjozee.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3dwdrfruy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3termubmh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3boqxzyah.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bpmnnuub.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3owfqvxkf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ztkshqcm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3uqlmswwk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wepwmuxi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3regrlntq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3rjwqqcvy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mxxxqtvc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3svyudrbf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3hkdfxtle.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3tonabqhu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvfzeoxq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3mvbykmuw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3aozpylis.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbjdmzhd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3axnwffxv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qamknwim.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxjsligj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3orbzjbik.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3evpbgzrk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qkkozwnp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lcthszbm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cuoswanb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gowtcuik.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nqoropgj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3rcsilpdb.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oocrrqqy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ervsyyon.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wdnnjbzl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3vzxbrscg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rvfgmluk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3kygobrui.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gtrkoxbn.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lrdphnyr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gvqdjgev.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3gjupjvze.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qufxbqmn.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hsbqscst.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3redifdem.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zdbaxyqy.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hsdbcfqd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3bdkadfzw.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wecrulyh.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3exzpyyum.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lwmbgfll.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bforjwch.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kyalgnyz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3pstgsrlh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3bluxatzy.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3euojsvfg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3wftxifkl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3sajlebzm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3gyjpkdcf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rbiwktcn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jzopyzux.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rekhmfww.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jgnjbtkf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3epkhwgnf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3sjbebunr.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3eavtgakt.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uyxxbsgc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3zwdczkin.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dcntvcwt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3kukaivap.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3jpyjyxuy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gvtlzpyb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3kiixwqdg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3pzaxndiz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3glapasmk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ylgkbbne.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sfjlavsd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jirexsue.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3chhainfz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3njsgphdp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jlmztpuf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3lcbktrrd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pqohkzme.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3whlzhqlp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3rmxseycc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vownaaaq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3rfdplpmf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kqtzzcrh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rwaowiuo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hxyjvmoi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ebfndkgi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rcttgofz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zxgsguix.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xwgqlqzk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cbwbachs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdnkooi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lhgfzvxz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3qmhdgdmp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqiyvupz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcaqwlk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3kqxdford.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3urnoctzt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vqhiqpuv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fgxdpmmn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ytqrltah.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3bamzqacy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3igiaqyla.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dkyuwgwp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3yepeudeo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3itqtvzkv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rgjruwpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lttbkxcz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pnxliecu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjbpqbiv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xkgmwked.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cebbtvdx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnbpvhm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gwosptkm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qfnwfmpw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gcljmwjf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3eblmwatt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lzcrmcxt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mnbzaaby.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fohzkyad.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3sycrphlt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3klstrdeb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mixumrhl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rbcbrpgr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iuhkexcb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qnxchpsx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3snsgsaxt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tzwciexl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3kmfoacbn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xohbmtvj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyrwylzk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3oqxczxse.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ubhlakbf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agzjuxnz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uoinraoi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3uorugkbs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3niemotve.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3anjuravx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3sjmxlgnv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3vzthshph.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3koekolav.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zxstnywp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vmpoayln.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3buoomtfm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3wsvzpjvd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fytzejcq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qabobylb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bkztetkx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3otxwrpbh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgjocodt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuapusxj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hpylbcdj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3djzviarq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zojnplxs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3egmsrrku.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3grxeojne.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hefwppmn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jzlkhfvt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wxgylieo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoktidps.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lbfbpwml.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3iyghkewc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xoucukfn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yqhouada.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vclpidyp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dplnupfx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3twkxtsnh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cffrvoin.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3obhyoyjm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hekdcsiz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3izqyarpj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3bbaxmwiv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkguebww.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vgwabrnr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ojjgfcxk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3twkwcmrf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ygxlhswr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ckqizhhq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qbqpfsvn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3egjkjcor.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dgzpfmra.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3duzteggx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3uktsfrle.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bfztyyka.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jifikcat.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihlxuhkr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnewjqlu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3juhijvwy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jgkylalj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3msddtlgu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qllumfls.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vuanbrfg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3souooehi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbjhwnjo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qylbtakq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ipsobeli.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3hdkrwjsq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vgmlyyui.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cyqzyeza.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hifffjeu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3naxavdez.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3siowdjua.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hpzapsod.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yllhbqxn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pghfkdyn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3uounkcsw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3btfgyfne.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wpgygcky.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3hmzxtoqu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wkmxlgzu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3eczuhddo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tmnwxhmy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cadobeku.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fnevjvhb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3szkcuatv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3zqtzruvw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fcvcvbcl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gajoqoql.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3alsipafe.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tjbqidjl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3vhkxrrwk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cyupmvtf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cuaufvsg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3oavcrahg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wuuliyib.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3akuuqofp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tupblzvx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kxhhnymp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mhnkhvao.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3uprzfskz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3khwqsdmg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aazrbdhx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ugpgianp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tqcouwuz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zobikbqe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hfuowphm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rtkugsee.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yqzugdmm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gysoksek.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ribhadaf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eamsxiau.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tdnkrhuz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xcsdhnob.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tsixdmub.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3toykizjh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ihsystki.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ftqwgddm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3reuqakcy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qsxcywwn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vfgedeqy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3expurggw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3pfpdmoaf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3afbebhrg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vazcfucd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frkutccy.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pgujfvlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gosvdryf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mjdkxzvn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xkmvdvol.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qrenydyq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ntsgkrvs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgkyvbbb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwyazfbe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fwzwantb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3iidometb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bahckjik.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zjnguxom.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3juhhbngb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuvcqmwl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eziwczmw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzwixkxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3csobcooz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fidjaeyq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tfmvrpnc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3jtfsuhkb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sxadgcjg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qrizxheg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzjrwivh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgywxxhy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwdrspfs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tldzdslz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hcokcugn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3swqenelw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3igrsotru.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3krupturz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fifdbxfj.html


<!-- 参考信息 -->