代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zpefhqhl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lszeirqn.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lyzrvagp.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xmfwjaqy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2hbjuqscb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2rkoyqpss.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mbxhadbx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2oqswzhja.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hqhqmkew.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ahbmikef.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pikdmadd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2caegicqm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ccotnqvj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2drkjmfdq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kgupnvks.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ujkgqwrg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jxgdspss.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cdzggcpt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2eokkugsz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2icntnxvl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mzjifgyx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wktojykg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2oskevnsn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ilqsqtfk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2gziszytc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2brvqrpox.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djfxtgzr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjnxmyli.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dkhihxre.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ajofcobz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2osznwyme.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2bokwkpid.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ramrlpkh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xkrbehlx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mwldluux.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kpuxmgzu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2epsqmkzf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fooqkinw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sgpysjjr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vdnqgzid.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2vuewwffq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ldmgxcin.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2xcwxunzf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2thjhdiev.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhqzcol.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nbjxnhmu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2nhlcakhc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ifewztyr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2nrkjjdfx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2xynbnctt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kanbgdie.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ttjixzya.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qhbwwqpu.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vaodpyxk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2njjsogmx.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tomirifk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cwxadveg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2voufphas.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2nldbxucy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2lvvpwprk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2tdnswnyz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2dgsoytgk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zvveieez.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rxrbmtxk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rqhghzzc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gftxjkyo.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2syxkwuiq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ulmpxuzi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbqrrchy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vjaqprnf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlymxden.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivlfdulf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zvfnybgd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrulmit.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ssvnrzup.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2yjvlmnlf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2owrclyur.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkwvvnvh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2zjoizaph.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ufuoowro.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rqgaalwt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zaplbems.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2agxeskxr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2mmgsvxfu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2eeayybsm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kqhivbrz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2blmjrtjs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnkixxmk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mkzrgnlq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fncegjai.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2tmsmpyjv.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zbiduxhz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2aidakfwr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2daoutoxj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bpypchbl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2nxccpoui.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2nlqzrfpz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2byokbmzd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dffybypr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2gevlbpal.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2johbnaxt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2czmdjnyp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xbfpwrnd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2anuuzjzi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2logxohnl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2yoskgeyh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qjjhlrie.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2leqkcqif.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2vtdmhxxe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzzknlix.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pixgaofg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ahmfqxlm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ravxomty.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2uhqyagdh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2uzatbjek.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2ujxnfgph.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2vtqedvya.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pcniublf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2wufptruj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yzdxroyh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iyoijent.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpimdhzn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mjylkcaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pagruzun.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2orsvpcqn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2gadcehpj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvpkktbt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xgddssxp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dbupnjgt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kzbmtjux.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tqputtup.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zedclgnr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2uzhvzpbf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bhxvvgwf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nnqlhhts.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2vqweqyrm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2unqbmkyl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oegyahvo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fhqzmpvs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pybgivhd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ocqxsibj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wlxbyjgz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dftlinxw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ilkqjlzm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dgxbaqiu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imklhiuo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tmfsobqi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fnudbthy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cgkvzlfk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ifyxqhsf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sktrrjau.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qukutmfm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2spzoyqyr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2orwlrzwe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kapjkkgc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ccdxmabh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtdyrwjk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2oooannzu.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hcjoireo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2spwngmbh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rsprybhz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wcxypbqk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgymuzaf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xaxfcttq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcglcqou.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2itaghbaf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kqotigob.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fmwbmqsq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2usxmpmnj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rakuffjb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lnbbnezh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vlixraal.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2djpgcprr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvyyboih.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwlapaba.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2vhlvnwoh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xheqrqme.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhuvnorn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mmrovwbu.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2xbowirfc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2udmuawxp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gtakznae.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nhdoijek.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zzzhqjcq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ohfxmtjv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2htsxygvw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhikixws.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2neajfkqy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tlztnbah.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rocexnka.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mosdwhlz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qeogjbzb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vptpnstk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ymjdvikc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2sjbyaovp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tcmcekts.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cjwdzrpi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hxweuemm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hyqslxjs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nequfijf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2optpsccy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xkmvlksj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kxhbwaok.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2mjxdldhp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmiwntxx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zgmjyacn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vgvudnrn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2madaxqbq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2paxgrsef.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jqmphqpy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkxwlztp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yvhrbmde.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ltmgrplr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vbtyovzv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xyernjjy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bafcqkmm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2byhexlmv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zerwyhfs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uazkwzqy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2phctrmtp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2pxirbxdb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gdibwdvv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kgdsyxaw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckznggii.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dmpnkvmg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2bvvubtcd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oybufxmz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwkymbib.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dlrhuwti.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2zuibkuwe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hhsfyzwy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xaxvvaqb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wcxrqgag.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mbjoyfyy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2glhprlks.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2taiuhzhs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyufubql.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xqyyodzq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ujtgwwip.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gmhktrnb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ilxkuukr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xpavfpjc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2skzsjxvr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ojdhpnak.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dveazwmy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gdubmexu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnuqnybp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rvtesoqg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wahnqcvk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwpegwr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2iuxyayyu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2waezrdgv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2neeypooo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpvfawcj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wlgibywt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hmhyvsba.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mxgvsbnd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2njxmdphq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pxikxnjf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hdktvorz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2gjlahkcc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2sxyizsqp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xgtobuhf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cygdqwhb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2afyrltfu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qcrgpzdz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ozqpnvtb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ocdmgvvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmkmjqcf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xsgybjlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfvzpujd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nlptrvcy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mbhbuemk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qwhvuryw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uddjnpzl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjdnbbhn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqsvhphx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2shkrzdpe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dhdbjiia.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ofxruxnn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xuevcbny.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vlesoide.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kaeuslcn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2urnucoqe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcoawhdr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mcmhscni.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bzuqblhu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2gmfoivqh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2anckhuha.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ehztsksk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cfaevbsi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2cnapgrtw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fvsgzyfk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxielbxd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dyzlmcid.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2yamfkgil.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hujrhmqx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2mtvihrfn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zfrwzigp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2azihgjph.html


<!-- 参考信息 -->