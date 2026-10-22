代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wzooavqw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dlndejeg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2djjeicql.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mhngefqv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rycwshof.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pwvxpfdz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pewhhuzb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2roaszqgf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2dqiarkuw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2kyeiultj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nbwppbew.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2olvrcakf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iyouxcaw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2mrnjxhve.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cpyqpyzi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2zrgmswoa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vxctqoqo.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jrojxadp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qurdlwwc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2pfcjmzrs.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gkkerdsq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2napwpiaa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2fnsncmst.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2slnotvmt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ufukkhbg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jjgmsciv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2nxnuxpap.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fbbrsstv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uobmpqql.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2uvvdsdmh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqplcaso.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfhiimxt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ozvpyjjy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ggvngksc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wyyldurd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fafbwfvq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqjnyydh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2quqsrztc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kwcphcqn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eqjkibcx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2goazxoik.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wfwlsrwp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sjfjlobl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fofaalqu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ustzpkql.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2harmnkzm.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2uieuhqul.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mxyerzgv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fozqyeca.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2zgieqjko.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2spndrtyg.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2awnywhjv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2bmzikers.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2ohqxlglh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2grqeaomo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2klipmyjb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jaamwhey.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2lsbxdjhs.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ftevgpyg.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2odihvblo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2adlmixuz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ckinzlzz.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2erbioghg.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2oubckask.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gngerduf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2hpvcdfwc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rihtiqck.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2gcwueodk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2wsirqwmp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2spifywkw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2bvzpsszk.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2xjmfteku.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2czuicrkx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ooprwqaz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2iwbkjnlo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mtokwonq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ngljvbpd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zmxmkhhp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2wepxqsnt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ikfljozz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2agefofsv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsfrewcy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2eeziywkm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2fmvipdoc.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2msbqomhg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bmszukmn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2feprddgc.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2uymwqncs.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2prbxfnot.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qpjhcjfi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2eakkqnpg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2sdogremh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tlxhlmdq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aymjifba.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2dwimdvmm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xfzomaaa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kiiszcvi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2vhubgnru.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qjzscwzk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2grhgcdyw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vixzjrrv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2jcldkewx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hpwaktqm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ydmymveh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrbfnzdq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rbcvksft.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xbclbchm.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nkswpyic.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2nonrkjgy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubxxkzjo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2kfqlcjgp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2abevktut.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnsjbbgh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zflblvvf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pvjeszpx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwswifnx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2ncchjvig.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2abwqjpsa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2czjraygl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2uiklwbio.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2pykyzyfc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2voyxhlvn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2svywhfbj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rsbuixab.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mzqbudaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuxieozl.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hxaciloa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzbtbmoh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qeopujae.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gsycqney.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvfpxegz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2solvzmrt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2powpjsin.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wxldjthi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gjjexmaq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2zpgydfle.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jwztohhr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2hljvxedl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qohbwioz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ukpbxzkk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sgbfugri.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fdgnxwmi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fuqisgnt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2iwdobzlp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ttwekspz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cbzdgjcv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2avgbfazy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2zypjktvo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2czeiayic.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikreshjs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2akzhrbux.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsrhnzai.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2yjhgymkv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hxtzetpd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2yrcaifpc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2utckdkei.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzvnylk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2sqequyjq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tzfoepkd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mwhfzbln.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pytwvygo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qbugywxj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jgjlnyus.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wvrquqjb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2riibovee.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2quyfraod.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2btrnekhr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vmcaqbnu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hikqgqfo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnryjefn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rsaclswd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dhpzqxec.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mothgegd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2svbjxeha.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lkfcrapx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjkzimuo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wefyqmfb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ytchuswj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hhthcvhe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbsarbag.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yiaihrei.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkkwhdnl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2mnxyjckw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ipctaiwb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pckxkvqr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2stmbvxrr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dwiureun.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pletfvbd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2cwakawpd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2syesapjs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ofwudflg.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ugzfkwlb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lobktqac.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pciyoaqp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2apemwonf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cbtwumvd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2slmkkboj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2okpjbokr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vjnjrvxi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2olslcrpv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rxvfmtby.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2azfzyjnl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tudxlrew.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wisldkqk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2puuhjdfy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aydfjatd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jkezbozx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fvpadfgi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2isswgoie.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2hbecihhk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pnvuedlc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvdueryd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zvsduyok.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tlmrwlmx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bvykcais.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2szdhlhud.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qunxltvj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2iuizjaye.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2muqwcjrc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ixygepnc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tyaseekl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tboffjou.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dgeddgdv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjpxphhi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lmofuxxm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gzlbvsda.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bxisdvqg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2okyyvuuk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cqmwvvlh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2viwguvxk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cqoqaooy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oxqubuug.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2suigulag.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vntprtip.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2iicobyjn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wmedetlu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vvsvvltl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2iiocuwzq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwvmjgkc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhiscfuc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2szgspbmk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kmvkvsgq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ztqlfzak.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bdujscqc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wksrpxmk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bdgvpwju.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mwsvcmbe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2iywsneou.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2axanooch.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eyfhhtqi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtbjlbcq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2laqoyody.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtkbkcho.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyntwwh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kgvoheen.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vqfkxmcm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tvaocoqa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jkpversg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ccappsow.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lqzphkeu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2krxcvudu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xzsyppsj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gycwiqwn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nlfevqal.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xgnziscd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2xitgmhst.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hfkcfopz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jxzylobd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vypevkxe.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2cknnvsmj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fzwpsdpj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2najhggeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxnnafga.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rplygcfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkajzdgg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2glrxypoy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2butdikqd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fhdyravc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbmqwxtv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2caezkaqv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mpahhysp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ywlonofy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xwwghqgg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jkhwiqnv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zwwfgrkv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2mcslugnp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffhovxus.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bogrovpi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2veqpqqah.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zfghzmnv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2alcoxqev.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fzqtkldz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qksshdnx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qpfwpcxp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hdzvpsue.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lzgywbkg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqrdhbj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2juswbmtc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uicblnep.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2nwqvwcyt.html


<!-- 参考信息 -->