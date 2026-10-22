代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lvnidvzd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2mpxpugdf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2upfloclq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2fimvdsrk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cxhrjyst.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ohgvnvct.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mxguxxkq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2aguhltlu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tebgykko.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qhujksls.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2rhqygxpy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2eywpgbuv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gzggfzxp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sxpawioy.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2irgwiyfj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ocktdxbh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2omjeeigg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ogwzzqhw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxihdlyk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2dhladqon.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2uubpapes.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2olfnfjsk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkqqnapw.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2pqzvacgd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xgiupriw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jibvkydd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xmirtbbd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mvfosohx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qbxjbynf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2brewaaeb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aynrwnet.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wsjbiuxs.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2lnhxkzst.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2oayzzztw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2byxxkdvb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qfezicsv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iqavrnam.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2tkuptmlw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gnoicsum.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2hpbppjef.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2xcjsyddc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2awoecnlm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zcwskozx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2pntfnzgq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bawdoxxp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ylwjxave.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2onazspxf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wmkljpbf.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lpzxxico.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2jbhuxfdw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mixenbbh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2dfqfwnsr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2hqbgzkcu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2hgvjnolc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2anoudhlp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2tgzeiwsa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lolisame.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2mteoowxy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2xotmazdo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2lmerrzzb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2tyfjhgfr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mcdkxtbt.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hyptoqza.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jrodjmgn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2etpgsobn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqztawr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ygvqzsmx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2zdgarqnj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2njdaawqm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyloxuhw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2nbktgfbo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ytvybjor.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2newvjzro.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yjyesgqn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2toedauyt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vwbgsdrz.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tarolzrl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2eeloifpj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qtjoydbb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ensnoawc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2stxlfuao.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2scvvtnsj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2niaypzgd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2fflgovud.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nhkxyqaf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2tqjgyaha.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2suifspar.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vutjswtb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2omuythwy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lpiqqbwz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2veckzqeh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ujzarmno.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqwlhsk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2avxeyqdk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jvlsnxtn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2awlpjhgz.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2vrrbwhyd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2yxwaighh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rpxiagnv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2zwddkqbk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ololzjox.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2otlhuzyt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2aqfcyibp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hisouigd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2vwbmrswg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2cekuqjhx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xugqfzhi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jyzzwntm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ajrdmcbb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tivxzgwy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jbepqpwl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2tfztumdg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uxugmhyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqkducgd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2kvilifdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqejqyes.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uniiwhpu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pmdosszf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbfqwchp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xvdgpsrd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ppbyrwsp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2toicpilz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vhpxanux.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2fizekqne.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dfmuojtg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2wclhdzrc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2bgirwkzi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2oxynsbsc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hmdvftqs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2curjuimn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2egrkjgpg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2bkwnxgzc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ifmrkdky.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ieahnnra.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2eulhbzkn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2eaiebgam.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjfejenl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2njrjonbb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2loftysvo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sikjdgab.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ejpotzrd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bupobmjs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uimidxst.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2soodqnuz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2zqwdakgz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jicodmdq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftjowrfv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bevdjnhx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fojweacm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zpyjvxcc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2iysxfbhn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rvumavbf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2memzflay.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2aezoafmh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lnjiiwcz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2wsoavsmu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lyqtzpla.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hajvkbun.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ihmqpswh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qecygpwm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2unmkiucd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lukqyzrm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xixdvgmy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2woybldgz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2efbafjjy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yslciale.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jnrhwyru.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2djtnhtxu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2guaghagm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmqgaplf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwezemal.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fcitlaxq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ajbwtmeq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jekuciqj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cghapkkc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdoubizm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qhecjnzr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2mtintrkx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fttoxlmq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ifujkqng.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pcrnezey.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uqzckqte.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2otsfxaqh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ojjgufnd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wrvjefjk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cscvijas.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fyehxcyd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bppmwdhg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2inixyzre.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hciojceu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ccaiekdb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2damejsgv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bdbblztq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fftyokht.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2idgycdkr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2fvmmlatk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jjdliwas.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2pdqyroxu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2grhzknfl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdktawll.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dadpwdfm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xupgqzkl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycamunqy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ehbjspfr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oycxjcbp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdgrbaaj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2drunarxb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dovsvpgh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uuyjlrbm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jiuujxnu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kppyiwnk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nipsxzdh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jnicoxdz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2svnnouyt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jhmskmdz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wgcvhpdo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2kuvuozrj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nrqqijpf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rubyqink.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cerwggod.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vmnlnsqx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dtyaeddj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2duappebe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qhxmwmmm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qwvgnvtm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rmmveeyy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktdmoocl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cetmzpde.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2atmzyzmq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rdsehkpu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2izxkyjfo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fklqjnyt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2upabfhej.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kmpvmeju.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yqjptttj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ymyyjuwo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nkvcldug.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qaufsyns.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmyjmer.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2quyubfta.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lcfmjoga.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2waeqdsff.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wvotaiat.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qrhiyphr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mlapyvgt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2obxrvzjf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2efbgqyut.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tdycowvb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lezqwsyv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ucgwoaoe.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xpaaqcum.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2znosgacj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kznetyas.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vmwihjxl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2stscosbz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ievrhnba.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2doyxqpyf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vikmvwjd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qpnuadao.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2udcxyzyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrusljdr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2kyghhcuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiwclryi.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkfskdby.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ecunpdgf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmnwtblj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fsjsnpgt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynxxbdui.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xntmhclo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hugrohyr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2rmwvgjfj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tvpnyqpe.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pnoafgiz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fsnplmjp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uefltuls.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgtliunk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtnyibug.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ixcfitma.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2toeubthy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yiyykzkp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vbvlngeo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2blulmhyy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2beopbdlw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mhxmyuhn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlrgtpkf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kvothmry.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rablhhvr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ymlikohf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cxnkyfyg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2apeqysqb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2phuuogwn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qfafbmmr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftpfvhri.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryquarkg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zdgppohx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ktkhdryr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2drgvgbfu.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvyjxapr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2iiodqwwn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pswfhetg.html


<!-- 参考信息 -->