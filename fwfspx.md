代发 wailian999

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ukzqqetc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ngalsyfo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3izkzvigp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3txkgneck.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fviafzdm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3vasmnbja.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dxicmjgm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3svgqfsnd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3laszzhia.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mmqkdtun.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wqiczkkh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tyqxeoow.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cmvoldvu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3iejfxvng.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3xhaqdzuu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ggvkskse.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mbdwxgqs.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ittuqven.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dpohrmab.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3gtkemkxt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3isleblkl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3espqrbxa.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umdaipsm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftgliaaz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3imroxrxy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3wdyowyee.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvcrjdgb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3keonizcp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xpwppviv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vuhotjeb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jbsofzvs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qadedbkv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3egmrvmyn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zaolwpgj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nwsabjae.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dxhjskcf.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3mojplway.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3swdtlheq.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ndfegjdh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3nssyocrz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3whgzxxhz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3txoezfdv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3psaqrshg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dsgppeyp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3vcazuzqs.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jumwmkld.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hgefxbwy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rbadmrcr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dnpwnils.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mdibejyt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ssvwjyog.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wroagngs.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ovxfcrsp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3tytvdzug.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xqtvggdx.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3obhytmky.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kbmtkqnf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3smeagqlc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3wsvtwxjo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3whlnfngl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tvlxpxfs.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yzbsloop.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3tpugjlwy.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3omwwqwjm.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3yvwwbzie.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kglwlgbg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uscsuhmm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3etkhoijx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vrxcwnzo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjhhris.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aizqvbvv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3tiyientf.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dvcjqvwm.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3ilvpyizs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3kzzkqrzs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3glqazsel.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gkmpsvxj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3dpnychdw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvopblti.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3keveftnf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3gkvsbfdj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dclfprcd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hweahpnh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3golbqzdt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nfkieqoy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cxsutrag.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tiiztbdt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3bpqjntxx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ultoosiw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3vwndgwzw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3oggnkmwe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rqingugn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vfclcrdn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fqvtsqzr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ynxhkkab.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ncvwxwcg.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3gojsxvct.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3hlqorole.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lorjhqto.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ubrgkqyo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3usjkonwa.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuqakfex.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hfkeidnc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ekqmzxif.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xemwqpif.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewhljfjs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qxcsovix.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3egxjrizi.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3uhgfrvpz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3livzuxsl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3octdiyyk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ziqmxtwh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mnebrlsf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3arbegcjr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3lhswhnfm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3huiaplwx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3doalavzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xiqihaep.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3adixwdwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmwcegol.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3xnxofthq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3htaliben.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3wrmpucsy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ggvbgnmq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dkmfdtyl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ijvkhmhn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3cfcorczp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wlgrfgmh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iffuczlb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cymuhtrq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3riuxmxfr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vidlbcwf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eqletrkt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mhbvvfyy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kxbnnuwp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ilmdxviz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3pvxuohia.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rugdunus.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3njlfhjlt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fnxpumog.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jujhfrth.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sdbudonn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zrmqqtul.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iynqqxsh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3drnvtquk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3unrugvzw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bquhcuei.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ksylwdiv.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xlocigrt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjrpxeqk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gwzhchhj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3baqouauk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tmujjwqg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pkdadhmd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3inmtprap.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ljhtbdtt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zfnpkjcs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lopxeiij.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkadpuiy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbicaggr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgkbfcgm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nushoobf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkikvhh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mxxwycuc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3qhtprxuk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3liygzifr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gcuisimf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzdfkaft.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktruynim.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3eqdwvymq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3rrsmimrt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jiardxpb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uyqypzpn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jtkmxpbe.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ujgvdudw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hwizsivm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3rxedjrxo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zxejkwro.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yfriznux.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gonwwxrx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rnwrejuu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3xaoszapl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aivbfvel.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jonobzqe.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wygbadhz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kvneapbg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3khyzonbq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hhrjsexz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wjwzvyei.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3xdmjgeqe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3oxdjgdwt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ynrabyrt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3utjsekdj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3tdfcanui.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nahdysmo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bempcmnt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3advtmnvg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bbjdyvao.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3klyxmaob.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3plldlttb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcpazcoz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3honfkpfh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3zrpbvpmw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wzkpzoxv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jadhrxam.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bhmhluik.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3snqtvgcl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jtwedjss.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kbvbxizt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhsoiuaf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ujsmrvtx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3cakfvvcp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3mklbxekl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rhvzfieq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gzrmmvse.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cuamosvz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3khcuejil.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hsesuhuj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3pdxizana.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qiffysvp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rcxhgrdh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lzpqmbeq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3moksrtly.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzlvuzg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhnyimhl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3yilwqyqs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wkpulufp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yxopziio.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3atubzrhv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vcxgxpxi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqcubmuz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wxfraame.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3drsjdllc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zbzjnclr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wddydbrd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhndfzh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3hekijudx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3spkkgcfp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dvvlcwgu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dpkyjwnx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jigxxaap.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3coouufik.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kzbgkcxa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3retedbwn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xcyterfu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qzckctil.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wurknjng.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tqmukzgk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3enujonje.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ehltozgp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hlpximrd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rretdlij.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cucrnjdy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ysbxtsbh.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wtzptydd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3voarrese.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3waeaipye.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3glonmgcr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zdyzudfs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3naoxozbi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zbxusgdf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3spklljij.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qxjritjw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vdnyvmal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uanppdeu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vyaksnbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vibabxqm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nkrroles.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rlagnnvc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfizvfoy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cfuydagv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nuemnubo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rthxlqgt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mwlfjevu.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cuzkbgxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhsnkonf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hpjcfled.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cxfdmehy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dpmejntv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wmjphycp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjouridt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kvpfwxxy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3aqndsaaq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3onddegyy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zlbbweds.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymqtvlgq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hksujlag.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tbktgmoz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdaftohm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvmpqyx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vvxmjsir.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ojajxwzb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tdksyakh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3doqsvthw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xutoftyl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pglcylzy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbrgeweg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvbrrlru.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3srtdxgwk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pgbxhqqn.html


<!-- 参考信息 -->