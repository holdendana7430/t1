代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jprolbxn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jlumllxk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hhqgsavv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hehauydq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dapotisu.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3divnwrqe.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ujhspzee.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lfqqtoob.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3luyrxqid.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mrkmrydg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3dfxdwzuo.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3znveicfg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wskrwtug.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lqainbxv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3htawiqqw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3rsrvuprm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3nmzjkscf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qkovrqpq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvikylyn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3trrdrknn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ostfpttd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3sefhvpky.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgthwbqm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qjqymvef.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3meyeplfs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kdliosvo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3amtovygl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gmkkpvst.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xutyqhle.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rflrvqmy.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bwghcxdf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3avhzfsha.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3magjugtk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rmcjcnsl.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3czpjewny.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xmlybewc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gfgxctpf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3dwguvowd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3kdorbrud.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3phijmqxb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gahylghp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3dqqijjrp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gzpjqkrk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3iorguhbx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3fkvwvbsv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3jvgbxgha.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3dmmxtjco.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lrwxuspq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rsykotay.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3aoltfiah.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3dreqvdop.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jzuajsyl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3mbekuzer.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3ajwuszqi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ccsnqsqt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3cbecjivg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3pulogczb.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3fqkcunig.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mfojyhlu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3erzpppzr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3iaiibguy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hfvfsmja.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ulxhffam.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3olfiexhd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jbzsmvrz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3egtfkfcr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tvuahfgs.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3egwcpymb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nrspzxkl.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3wazfmfna.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dtkekfqt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3xsyknpxn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qgtxbmny.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hkrmayfl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3usftrfbe.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rfdyezoh.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3luotebrh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kvafgobn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3utguxxwc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hsyxucck.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xywcpygo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cjbrgtre.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3baisjgbo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mhqjqmpw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dbyqsdvx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dzvttscq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3gkespjtc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3yjoqcfur.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lxmdqtpr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tjenbesv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mleysdau.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rpfdaocs.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3rmmvsayv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3thoztsyg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3zkhralgp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3skpnxbkw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ofztwhgl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ybecqdtg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3buecnslh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ililihjq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wztznbyh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3skiqgsvb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3shqlplwv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qewyyjvx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3fwdpiran.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3pbpikcag.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ptiucvhu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3lhufiiba.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3cmkgyzgf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxliybm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ulqzouli.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3waikkmmr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3myiefvcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alozrlni.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3eksnktyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggprcfjp.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3apmpcmfk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kvttcqtb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3azvdkkao.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kqasmwia.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iztthcha.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fyichwsv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3msfruwec.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3udfgyfru.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ojtiyqur.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3rptgodah.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3mlpjwsuc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kgupfyfl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lpzzxorz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hkgagrnw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lxenvdbi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ghgrchcf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3vpfjhdbs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3brqwbwvn.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xqsrfwgz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ppblelas.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hegdkfev.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zfmdglum.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fbunizrt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ljsqaqza.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lpquyvza.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wxhbpncw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3bnfwqcdw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dibibhqo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ifyaekxy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecduooko.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3usvjlguv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fwgvuldn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fwpnpvps.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vhyqgpul.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3agwwpehs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbkqmass.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xogivojd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3qrgpiqqc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3flhhcthd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3idcmfbnw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nktyihgz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3szrlcqps.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3uldmtxas.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pfjnftqk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3bifputzb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bzusxcep.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3oqjphrxh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3slzmkjwx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mpglzvoy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbitfnyd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3osxuncwj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3faeizmmy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3bcwkzyco.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wsmkubuw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3aemqnxnd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gybeoyxm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3eklgfvgm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3whkbgvrz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3onuxacjp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xyncwtwh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3sskpqvbz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpwcfisr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bocklurm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ohpjhizc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3rqygiujh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dfmgoxuw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ggfdqroq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3scabyhpz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dpidzgsg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfjmukac.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3phlsadpf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3phrlqjwl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kfpxhcsm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xoltegrn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fztzypgc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sopcpiwh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xalopkeo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uxypyejr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rhiyukth.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qiirdbwg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vqapomva.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3cmeipwck.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ikkijsbt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gqfvinuk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fmwzptqv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3twtpsjbj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3onlnxuox.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wfgbiqlu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zeodzhqv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ncyuykbo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eodpknst.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3iyqtnham.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3aatwpboq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jtdezsvy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iqzycmxe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cshgnwfs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jxibbnfo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xbvzlqor.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oirepnua.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cngnepgm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pnpsuwoi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3boudcvnt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ipacojgz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kjmrvjzf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3amdtihgi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3uqdxhbvu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3efrpqayj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3oxtnvkfl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xhuxctdk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zhhxpctc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3egtiziye.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bsolkxkw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nflweeqd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rdtapcpf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3uzavukms.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlgidvz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3dchiodgd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kidtskwk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xsdjlpmj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3eaesbqwn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zdinvmrd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxokhtfi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3owwdxvgu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhmhmrgx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxsapmva.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbpvhhga.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mshkwrul.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3epraalcz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3nnmprgsn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xjoidrtv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dexrdquj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ugbytgmw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ibtkfwgm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qplgpzbs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ibqrfebe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qqypgvql.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fpmpgarn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgqnikur.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qncraehz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wmegebed.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3buikykcz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jkvsmser.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3icseqjaj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ubrmfoah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jswysqhf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3nuaiiklz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvmojpri.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tykdtubg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xqthhyxy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uzldzazt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rrdcqjag.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xyzrkihi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lunduobi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gakdhpyo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hvhduard.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3trltlijm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3brkverad.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3cjzmrwky.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzfapeun.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ufkthcco.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3scpfxmml.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yxfjbwbc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hnrrzzkw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kzdcfiak.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bhabzzfs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xhndstrs.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3cioivqlf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnimcjwe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3unuqrcpe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybzrbwnd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gucbrjjf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ramtrojc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kvzdfnev.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zlmrwxfe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bnphknxd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bgefjznl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gbhnsbdh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omiwlazi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sdlhqged.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3sypdfhff.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kixovpcl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fsowuvyt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3chdknmdg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qqreaymq.html


<!-- 参考信息 -->