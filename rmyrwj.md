代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2fnmoiywv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2jysfxldh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ybahdrvv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fuacbgmk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gbalexvh.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vlblgqoe.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mzzywnst.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zugiiqyr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vpjdrnrw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jxblbfxj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2klikgtgw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kpefrnji.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2pruziwuh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ckjfxgla.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zcbcnkza.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tekipuky.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pjzujivl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2drnooprv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2arpihmzi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2rfdndvre.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jlwarrlf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2xmxxrjhq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2urygzkji.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mudsaaac.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eixehpsg.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2czschweb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vyyiesmg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zwyfxqyz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2loltogor.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wxfcslyy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xsnribig.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dliyjqyo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2iovtyazp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2pqkupvmu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2tokfapsn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2mygywpto.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ktpazmbh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2woweskok.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2eltjimgm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ccucgvso.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2herdrtis.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2udejkppe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fadybkhf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bbbqtbiw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2odynobeo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qkqvwyeo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2izpbpxjn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dsqsbfgx.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2fdwkpwqs.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tegmcjeu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fxbnbslf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dxsnhtre.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdaixjz.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2hxwcsmbq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2gcdcbwyn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rprrsrwc.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2dcjjtjrt.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2vjjjnbkd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qyuvnoli.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ytsjkqtr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kpbfhnec.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tvmyevaa.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2zvlxrtop.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uszrdcoc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vuezcgvb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2wymsaffv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ztdusgtz.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2hjwneiue.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2hgsqnjdl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ojdsuzts.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fnfsyrqr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2dkfapipy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2mzwvrhnx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wxjbkvml.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2dsipjqmm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ttxrxqqz.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rcajruom.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ebvctobi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wspoiycz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxuunbz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zvzhmyus.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mpmhlqbh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2eulyesoh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jfupzbwv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ykltalpi.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzycthsk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2celnltbl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2eftqmwrc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2pkavbpqo.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rjxyhadt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvizqcjk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xujqssjx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wtiazfrk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2unkxhhif.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ddcjuzkx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ehlonicv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hrtzekfz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ayqmnlct.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lrmfjarx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gncqxhtu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wyycvyhh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2bhxwfrmx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tffpnicp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2csltkyhk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxwrriqw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qvkluute.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2cvckfiaa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2whpwfqce.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ubpppjef.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ttnqxlwr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vcrgmfib.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xztvksvo.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2wgqxfmwe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2wndysybs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bcyoxqft.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xobkqrhh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2csnbitrm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2djnuafrk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qhtlsayu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfebnpd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2tuwxvnge.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2iwwamhrl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2kbuegcpm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hinifbnn.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gsxbkzwe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nklgwdlz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vahecppj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2vyjzvvzu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ejbmctmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgtmnmck.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2elphewaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sssltnfw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2zoqevvbd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2iaiuvbcq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtltflcl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hqabieuy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2szyvljhr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dltsqdgn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2pplsrsqq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ylavmjop.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pvwqslco.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qforgtgd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2vunmvgap.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpadahkm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2upcywjzd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jpwflzme.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yxqauasa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wrfhzjsg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2txoyyzcg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jzhdqkdb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2jniidlld.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2knebwyao.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2puzcxahx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwlrxdwb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nnnzxuch.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obneknbp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2wlyssdze.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kvpkcfze.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kzkurtqv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bqevvkkq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2dwsouukx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlykwsch.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xxedklcc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjyjcnzh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvausjkm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2tetchodw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ducyqtig.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aeczukhl.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2epyckfbz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjyjiae.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kebiadjy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tofbprjy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2onbfeqmr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpgwqpyv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jsisbtnf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2cdmjvomc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2wzpseilz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2blawczbq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qaybehio.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afcffols.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zykuavit.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xpqybibb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2eudxlkwh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2scwfcfdd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jsdjmqvt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdwmjahc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vmwlcyha.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yaodevcs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2esngqfdt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2buyjiutn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xccqehbq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tutejjsu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ieuhnxnt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2fxylvvji.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpwjtxhn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2bqywrpja.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ozlfhaki.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kpkshrlj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yqlnshqq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ctjnnlvx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bpnxaxsh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gzlotgsg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hsvbfajz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vnfnynsp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bnlthbct.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ytdjvxtx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbtkvqih.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhjiojnq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2opgyntwj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iakrzilu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wshrmyfc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdlcaze.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cguzszzj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xxqbwvtb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mycuethl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkflevqr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fqgpkrvt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xmbseyni.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkwjkojd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uxxadtbw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2cjepizgu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdjhvaoa.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dlhwosxq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2perhvfdh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tqvtsbfo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fixldwmp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cowpdpnb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2cyjuaudr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nbuyazyj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2noxgfsfw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ruauhstl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vfbtogdo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2iydnmcsw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2svryngwo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iilfnrvp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eppziqub.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sqqjplmq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2rdjpfuwu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gidyxfgy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rxlejafd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rdjppckk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jeaiumyo.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wxflilrr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2guikathw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eviwjfny.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nklfaxfn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2yuptvrqi.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qihkwfps.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2zmkugqli.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2shbembaf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2qzsiazjw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hpslwzxs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2frquqato.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2binslyom.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yradbdsn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2locfcwhg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfvwgsff.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2irorbkqb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vnyludse.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2boawjelv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2njqtcxzd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mmxgucwa.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2epnwyuxm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bwjynwev.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2idqjdpis.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hypuepkp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2twqzeozm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2gknjhqqz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dnjznsub.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rsygzfia.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hhhkxoty.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nkdkitpm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lvrhrfph.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xcckzkxk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2gqpxutcu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ovujplxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzxaqybh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cymnanun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgnfnibv.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2totlpght.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ricphdwz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkphyvao.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sjhtzimm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gukdsyxk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2abeioqwy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2eccvpmna.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xfryawlp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckeovgtv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xsfzzsnv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tforocwn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ilcopniu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rzrwqjzy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uqzxmfhr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ztivomks.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gitwtoji.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tjjznmrk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nliipkmc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2lbdowzpl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zhnpscre.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ahzakfzu.html


<!-- 参考信息 -->