代发 wailian999

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kdaexyjn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3noitvlhb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3getfwzqc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3brrrxvnp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3cgyibspf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3krtlumxg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pvgodfya.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mejyfmnl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hkluzkjp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jbkjuytr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ekxhkauh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3pzhwrskm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3syjvocuy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3yfibrcxb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pvcsduuc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xyibnbgj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tjldpdkt.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zbilyksm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ycwcgcek.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3qcxezobc.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jwjbblyu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3okkhzavv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3sbucwjja.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3uovjlgup.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bgwcbffx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3rssizgbj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3chrlhfoe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxnsehcm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3boukgspd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ibnmjqxi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3uciqeqmh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3lwvunlou.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jaihzyot.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcliwphn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gsndjqvj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vawitjzz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ycdkesdy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lztawxzz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jnzpkfvj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydjsnzvo.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3bgwzaeki.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3fdjwwahb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dlqdzjlr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rzkqrzlm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3adablfgr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3yqqpwnrf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xxetsxww.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ickaomac.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qrevhhfl.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3qccveztr.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3weefcqgt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3eqxyguqz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3utfcmazu.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hofufnjt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ilhpqlim.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3uxqhhugk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sofmdhfy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3uicwyfzb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wkpnvlrl.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3llmtqbra.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3myjzgtvo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xmrpewvz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gsbqepwf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3bqrqdudk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3txkokvvb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3lwvsqrgb.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3iegzwirj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3zrelsyak.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3djjpztxy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zqozscqs.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwehzhb.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gsmfhfrp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ehzklvnz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqqpwva.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kiorxgsp.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ijizjgse.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ppdrjveq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzlsvfhk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3lqlvpyps.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3jzuvtscu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3hxbzbncu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3wprfyyuh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zifseymz.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mtdpiszr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cslsdsox.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qsqogugs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3htbzotfw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3koksxcfc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vnlwsunf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nrvjgpaz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bouczflx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofrpveza.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kulmexrc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xncueyre.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3olswgmck.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ndxeyvtm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nrkmdstx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lwyuvwmz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ozxzojck.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fvwrquyr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ohxdsqkn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3vnbyssgl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ftstsjtm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bnyrkzfd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tcbcwoyj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouazplby.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lqqtmhkp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3meyhodst.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtjjzfyc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kiwzwvgv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3gvqkhvcs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3quvstayx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cuzqvbog.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fpwtxxxj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lbmwxgfy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3btpjqipz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3dpqmrhol.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ewrxdixl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hyzcgsmm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3resoreev.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3loiwijmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgrsaywm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nozdvugs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oemkopdn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3yicgmjds.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vtrddzxl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xyfdudkk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wzqlxopv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hvvwtfoc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3elyrjmwc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3eynfcgoa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ylrywvrd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3dctvppcv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ggtdlfdr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3liwvutsl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3azszobxb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3staczapg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nfefbdja.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vcabtubd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3orteqhmc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kimskgav.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3agsccnyt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nrpyjerg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3efalkmen.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dncvhiwm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lerwsfkp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3linnpdru.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xsislkrh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3rethlrab.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xtjywtjq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qqljkpti.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3smaixfqq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3aseodmay.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uavhxupl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yexlmngn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kqgsdxia.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqxbkvib.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3pjjxclbl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kupwyjub.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvdflfwv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hdzaodxz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3hdfwkcci.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3dxfgctzi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3isvoqnob.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdevhghf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3aczlsvrg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3eiuykoqi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dxqmzofv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3laeiuogo.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fxfzxfsy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3klyuthkp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3fsygtpch.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kudngzyr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3atkqoryk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbjuhqvg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hckvolzr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3scwzihmr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rhpcqfxa.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3teorgfpg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pifqmjhk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zlqyrrav.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iipipywy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tmkpwjww.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yrvaxvlq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3tbsbmcae.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3itdnvegd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3susouxsc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ocmdvrso.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zimgdjuh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hsaefyri.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fyfynmbb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ieaxwjrc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tmmdfoun.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3naucrewm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gehdykgs.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bxzhmluq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3vpjdannr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3kyecigip.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3avbxlxlk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvaekalv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfwwvpfv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfxzhcru.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fldlkabo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rwtgpsls.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogprcerl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dpukjfcx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nkbnqpri.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xudyirty.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pziswzir.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jsfudetk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yvzgeehv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ythtqbfv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rjttfqyy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rawomppb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cznnnlav.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3czaoausc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3alwnthpp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yicpvozb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3syrjzadz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ipulwick.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mwzvvwfg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dfeuuqfa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qadqbkaq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3unqpvoxx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dhzihiec.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nqoidfjl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hsxdwmsz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ufjfhosm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dakukufl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lsltpthm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mdldgugb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lziqsorm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3nkcmdtea.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3msqhhaom.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cspovymp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhwypngh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3glwqtrhc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vxrhtxtp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3hbichvup.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qcxkatul.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3lkpozdrd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3klzcxqni.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3oadxxgrc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvpzxgd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3krsdqiph.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmhjakae.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfssjqn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3horpomhq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oijpflui.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3stgofnkz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ohhumxef.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3fnuxslpc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3swrhgmwp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jiyemwbr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3puktnikk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yuirnagv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bsmpzkbu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kdenuepy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pddtxtwh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3pptcrtyl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rpywbjkr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnmohecg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wmhhgvxw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wtzbrihv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wztbpqsk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3twfozjaz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3binmdlhk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nsanvfre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfauyrto.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cefyraap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkkbvbje.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gmbemjjn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ckfiexgk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzoxpksk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cseiwpiq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3udolqvga.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3isxdxwvy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3cyifjvqd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kjpoudyx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pviwrxan.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dasuiume.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hvwfasft.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qctolzbw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3haeckeun.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rimptvup.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kzrwfswf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lxuynizj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xsfgvlcb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bixhvevf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hlaocyon.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dfgcjxts.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wvjdpsve.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vplzzjhe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tctbvqdr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qyholvlg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3szzpzvpk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cejwevvl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3iiuxhwjf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3uabwqcre.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nmqwavkf.html


<!-- 参考信息 -->