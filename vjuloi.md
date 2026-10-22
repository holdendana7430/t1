代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jgjvsdft.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2timzxqnk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dmncmsmi.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bdiygova.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2gvyxqcfa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2accxkrwb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fhmpzotm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tcdwonsa.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dikwhlue.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2egijrtmt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yabakyyw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2jdxwvkiu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tupfhwht.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2kobtgurf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gwqvrlae.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2iwjbnban.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2whzsodyy.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2drukxojv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2nhqlswdt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ikphpxoo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gwsmhjnv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2licxlnsk.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2poeprtfn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2logjhgdx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2yhobplco.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qvedtcsj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2zwuxoddm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqcqaspx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2bjqkotus.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rjemtdyh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mpzaqpea.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2orslpvhc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbeftavr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2earfinxd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bypvuexi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2elsnvoxs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2exugczna.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ztzzjadf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fdmpbnet.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwhptfzy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2zrvonfvv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2epmpftxj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ihdeayin.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kclufyxh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2erzrrrpp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2rgmcjcnr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2jdfhpoxd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vcyfhvkp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2huuwcexl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ngqdpxlt.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qaoijijw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2jgpniudv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2krelafdx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zdsrzyiv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ofptyrxf.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xfkrlayw.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2krjrdjtb.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2tqapllpl.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2mpcnriwe.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2mochmeqj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2lsqnsjez.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2vrkinknf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2iqdcdnxg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2avmkkbad.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2oemlemfm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2wzzfwiqg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mrclrmff.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2aoaupklg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ijysujbp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xnwushfh.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xstutphj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jxkeyyex.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2konmxstk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2kiaznlfv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jrkifcod.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2bxbhawky.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uckfioje.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2dkghfvpi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2fqlxtmko.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2drdagcik.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xwwwplor.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ulbbepje.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ouxshldw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2voitskpu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tonlvvdi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wbddvyol.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ubzkcuwj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnbrjwwj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2phqylhnv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2uprqjfhm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hggvqang.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2qnmdajmk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mfechyjm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qospkryr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2esxwkeop.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2srtyamxn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lzyusrod.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2frpjwygz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rwzozwqn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2gglzemhr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2uhlxdsqd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ygvvrzyp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hczubwdt.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bsazcluy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2xeyyzzsj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hswxdoid.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdyuiol.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2evlgezes.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbtkqupu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ruklcgcx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2fatyggso.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2jxfhyxch.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2sdedobox.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2uaubxsrl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2yzcsdfhv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2elhwtlju.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xtkjgvsl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nurktcmb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2oauckyxs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ozvcsduq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qmobzulw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asroziji.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2chmgcwen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewhvqakh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2oxodgjus.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2otltpfzw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dsnkuvda.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xehhppar.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rzlssggk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wijtmkfa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2mljksvgd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2bducrbvg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xckqavfy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qcfzmjlf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2snsxclwj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2berlztmn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rsuhqdoy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ooqwryjq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iwcjpekj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zfuozdfr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2pyqogjpz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hnfttcqc.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2yrspsfgf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ntrmwnjj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oqanoazw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wgljheon.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpmdehkg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sslvgwil.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cgpgqffj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2pwobxtyi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qdxcluus.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2epdhxhrk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2runbpuvm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnquvvyc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqhhhwon.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2usnmcjfk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fdvlcbva.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xuskluhq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bxrifumz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2yglohaoe.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dvqovvrf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2atrileox.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwqkkjum.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xpyoggjq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gthixwgg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylabsekg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bkskruld.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2wdnbjwzw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2khswqzpf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2gmtgjnkg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pgnoutda.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyjajtmx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gpiatxdv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jrsohhvc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pbenekwv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2rtyotzlk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uddoonpm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqbeevbw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ttjzxvhn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2eiupuqco.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nwiztkgl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eikhmwvw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnrqovsz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2naxwbpxb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lnoxawds.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ypsbyycg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkmleptz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2snuzdzcz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ncuikaeb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dgzowttb.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2khakqqid.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tewalskj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tgwliede.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wbrwihzo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ssbsbqyf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jjhjsbrl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wljaebgm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2bvfuuraw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvarurwo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzjcgoty.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ncmmjlst.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckvypndi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nzcozzqz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xrjztqvl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtofwdl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mrmzagla.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2afybcpsf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2clbnmjqt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ifkmjegl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cxilkzrr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2sbbkrjsh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bvuqszuz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2peqoauxv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2umckfsfx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2algatqqt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lgwhcsmr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rihuhevw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vlfrmcny.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mpjqeeup.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2saizclpz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ngixgpkl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jypagibw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nubwcxdp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2uuhxtqav.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ldpadpqf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2klqcwjmr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eencewbn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yhsxpwya.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mpafcoeh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gqcuadkk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2emkvuerj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2abcyxnkk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2xhzxbzwp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lfczcasx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2godwaxxu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fxhmeopn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2osvcxgiz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qdsnuqvv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rzsopycu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2renelsvh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2tzeqfvnf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2noahldvl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rbqnpyyz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ylvrqdtd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfhxzepk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjmaqrcl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2voexeqgm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2gmyuzcwi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2asajfrci.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrpxjfwe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zlqtukmq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2skbzfyea.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2idmyqutn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uytderrz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jwpgshky.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hroppkds.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ptfqturb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rzsdajsk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aiqykfuc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2yjoylgpa.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jmsmayxe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzbbnfhx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yhasorzr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pjmdeshj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2notwmsjh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xzsgfjwm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cmmeehtz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qawfbyjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zitoxljt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jyqzsywe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekkyjstl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pjctcdnb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vautmfss.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2infozhed.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2smoypigk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjqbwvo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvschdue.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2fepoujkr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2erdxvzig.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mjessxeg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ozvqzgiz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lkjloanv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpwwczup.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nowixevn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kxqulkpi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2wzolbixv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ocheqiqe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rxezoqku.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ohpmvenj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2uswrjluv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bbohhmzu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhciiugs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2deuaadtb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hzftwnzh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmnxijjf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wguyyaza.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfqlynhb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rjfhyjrd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2vrapzjvl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qgpeeiun.html


<!-- 参考信息 -->