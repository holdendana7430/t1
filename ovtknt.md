代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2edypscuz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2tfvztfcw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kjymlzxa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2cnxawtfi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwiskku.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2oslhjkpj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vzvbwqsl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2axndezwv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yytxihqy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2clvwyapk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pytaheks.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bvbxwufi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2htqdwprn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2whjcsrsf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xxmdgqxj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rlopkufp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2zmgigyaf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2rhtndrdl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2buzawmnl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hadlgauj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2thmioyqx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ywsavqof.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wqjzgfgt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2qvpemzpx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xhpscotl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jquajjjl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jiqwbzid.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nrhwgimj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zzxywugv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jhofcdgy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2tguygurj.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2nygnbslw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2cjhragvr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wcrtigtq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ifetzdnk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uysrrnei.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bldusioz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2esjsqczr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wzyisaam.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrsvfovt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2twfiskzd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2qlzjczoo.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bfkfxtld.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2dnghlrwf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mgrhpeen.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwiuogxt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2afeodscm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qxdzrwbu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2untfxacc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nuyfhohf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bddfhgjt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cezjajjh.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2kbtivgol.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nvgaabim.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wbfvubmz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2envzevku.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2isdaqbon.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2bkkvdzrp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2giynrtht.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2xamkozqy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tvxqhybm.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2hybindlr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2atdvmgpr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2aaczsaeb.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2ipxhvvld.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2aafvynba.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2jxxieeeq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2celnzgjc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oqbcrzpf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xmvhwddi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2fyzfpdyd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2daxlmehn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2lxugciwk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2xqcsbwwy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dydrmvrm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2raequjbi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2iyffklrx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2vxozmasz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2pxpgettq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2evltidxl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2lpprtlgg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bhshjnsa.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmhivqmi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dfwthpch.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wphnsvfn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jrkdwtfh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pgoyitxb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2fecryuom.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ugidhblh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdmkskdb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2vngdlqlw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2gcrxdqgn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pthhkarw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wdyvtsct.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cntohiyt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2urbjpdlf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gsddfndc.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qhriduon.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2otvserij.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyqdbnpb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pvcmblxu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ytmcjcls.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jlribvhd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2gctflozb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ogygbzxd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2zvrbwepg.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ejnujjag.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2psmidxot.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2dcybzyql.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vrjjmgzm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wcajljwz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2mjcifafm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llwhcvtn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2klznfzol.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vlrjblnn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ecpebgvl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qcvfcxrd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kydebgwn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fmcamxaz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmaflwjc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pncirbhh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fpabxedd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2dmyjiwan.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wcaeuntk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ticlitva.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2jsbhcvkv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nsuoebls.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ssfhjjpm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2oxsyxiid.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2esjlaedr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2amtbmjik.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2agdsqzin.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2najjtfgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2haeawzcn.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2afclzovq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsbesdbn.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xhntmmut.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2aifadihf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2atylyqrw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mdiguwoe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2afatppqv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vdpkxzbq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gkfbpjpa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bvfofsjd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wowklhib.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2nwdvkmgn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wdntnqbv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xaxqexus.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2chixjutd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2knwxewih.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ttrlbqoc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2njvfkyhl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gsbtyume.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yjvbrjfe.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2plckjrfp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2dfzhtdjr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nfjuxmkl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksqcovcu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbyfkzlj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgdenypj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bbcnnvjk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2tunvitvr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rujxatqa.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rydajfai.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2idzoalsh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2lopdgusd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2swckygtb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbjebypc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fkqwtldc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypsncpex.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lqmnezsd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2guggvzyv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bqwiifbx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ahshimwf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogtpjigu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ecmtjlbt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2cbzpcdye.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlbkeskf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gkmmpury.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2olevsgly.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2jyctrmpm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kuyvtmvg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2whdfltcn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2llervdpp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2prtkxdqe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2icfmgqot.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ajgdnmiy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2sghknnfc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ztroerxz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2eqrvanzt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2wnygcvvd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xfkcvszk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijyuhvoy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2veivoibk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gcegsxrz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hjlxcmdp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mkryoulx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2powsvpvl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bgcbpcwv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xymxasqr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2juyohxlu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bsmdebok.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hrevbbjf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2usjmihau.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2abfjifkp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2fgzmvjst.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2pmgiabsx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pgphhctv.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yyhnbgmd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2kpcuyffd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rkkodytz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ezdcyxxd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytortqvk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vbutdhgv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vtwnxxqm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qcrvlmpi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2znluisww.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nadzhudo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2wsvrallp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtbnmirn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zjyosipl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2logrzfis.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2weiykncg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kfktmhhx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sltxxxqg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtvzwnv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2eaquctom.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rstrjalr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2antgowrk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xvziraeb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cuqhgmmt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2tswubtyx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rpcxbegq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pcgrwdxo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zmdltkcp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2poxeslda.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hfqcwoxl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2odebourk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zsydhhif.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kyobwyka.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bfhjwfpx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yopaktas.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bebhtjqr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ikgzjqgq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2bqfjkrfp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2nndecpik.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkdhjqf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2twlxzcvb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qxfwtebi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ctyunwpr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2qjiohggr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkdgjer.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2cxiqxayi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2sdizotrt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rtqsebsp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2yhqnowkl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjikkma.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2affvqewn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mypbtpdl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssmqylyg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2apkpqzft.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vffackox.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yknmjrkn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hjdwpxua.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xbwuvtiq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dofofulp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fdjvbavl.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2juvofhyi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nafjthuh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2widptpfs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tekpdjwc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kiosqksy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2inzkdbpi.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bkvtqqql.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wfybrole.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gydwvykj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nzamsdvv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lzkxijpq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ngmhslrg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gdranrwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqcmasfz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lzdihahu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tloojfgi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2isatyobo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zhiiyaqt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctiijovr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmotgtpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2llzrslzk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jsqlyary.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ipxicgxn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2oirzyfwb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lzgbtrgu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hvizoppk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gczvdjdn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmmgkxha.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nzyjgyny.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2prjaxdaq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2oyfmydht.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2gdcjximv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2godmvgwu.html


<!-- 参考信息 -->