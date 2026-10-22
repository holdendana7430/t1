代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vavdzshh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kewkwgxa.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jcxepjga.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jgwdpwid.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2mprynduz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qjctlbwr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tjurhdoc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hiqqujpk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eocfjpnv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rlngaeqg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ytkgrscx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2xdejnukj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hgfmqzjl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rukteqql.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qbamvmkd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2tuvdwlrq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uvafkiuu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hfyovejd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2uqrklquv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xtnexgfg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gdriisju.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2anpnyrft.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jqwnnktf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qrhclosa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2pfbktfxs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2hdemqsge.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2btxwjjxc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzcerfap.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2uighakbs.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2fbsndtmy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbpdbgrv.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2uutnfmka.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqbgcfvi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tmwrgozh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nzstwmnk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mteeuoze.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aveprvqb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2plblddae.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dokyufhv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hlrruxia.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2gunzcofz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2thjzsfri.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2lnpwnqth.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jtevvkjy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ylsyigau.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ieuubacr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2clxvedmt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2sjhtolbk.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2svlphhak.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2aiwivuzj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wdzptrrf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ofmwphsg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qgxqhgxw.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qcguyfby.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2yjqtoxtu.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2boosjfvq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tkmllbom.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2slwuqeqa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2pbstzett.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2eujuzgxs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2vfyhxwyq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2emhvnwcc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2yqeupeol.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2rcoflcki.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2apycwree.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ksbgtyfs.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2wtcplsns.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2lmowkzhk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2vxyayoxz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gkmymoao.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2psguuwfa.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2blcpxeqm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jhwhriel.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kfkvlgtm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fdrnetps.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ytjznyqj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ahcznjhq.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xrebmtut.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ntgqsizv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lbxxqxpu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cbwgcqjh.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2spdgfqvy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2srgreceo.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aqdsulvn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qvbatwmo.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2puojfzko.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2brzmeuoa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysbgiivi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mhbgjkto.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2odtatfhh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2itfihmrb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwikzimt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oontgjmv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2mfsfifuc.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2hirhbzkf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ngmvnhsz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zfytkkdj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ommptjdn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xtrzctrt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2fxmmmaha.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2vlunfzqq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xndqtfbi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qbqixdlz.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jvxnwxdi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2icmajkjt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2gcjfacsl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lrudoxls.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vwbixxbf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2qqdakbej.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hqowqfvg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2aswomiqz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ldinbhqy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2itymsltq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2dpvmcxjq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xcfcjgpv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wseeurms.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2evpjypui.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dhygstew.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ydhraaca.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xdckvnll.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zwwxagkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nifhvoiw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ucuupzca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmvoxmll.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2pijpogvy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2oyywnwoe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2eifyeijg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xopaexre.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jhtlcrsx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dhpqdvhk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2qyjrjfyc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zptgxyep.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2omnqgaqb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2zrrdplbm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zdulrfxb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nzhnpenu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vcdtzcms.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mfkvaivo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xysozzeq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qnuzflzj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2oskfvxgu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gzroextj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ewyldjem.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2klykchnn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ckwrhqmx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynmhcexk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtppuidw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdnnwzdz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2sfroqejw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xklkffqg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2osstosbe.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pseekdbl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2xkifmhaj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2frqopryp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtcxrjiw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gjaitbkl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzeeumki.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qolyivpe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2svvyduqx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wbyxvgiw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2srytkrji.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrgijaz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mxsfobqk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvfvtdfe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2uzwbkhrk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjphtwcu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2rqisaerm.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xgyylaan.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2apltdelm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xclctqdr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2orcfjcwp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crerqnau.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwpvkbxz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2farcenrn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2kusrpogb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wiguxzhq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2adzxjlgc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ctngeicq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ebfqthkg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tgqmeyzq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2faisjcvq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftocsypo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nvekiefd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ophbvlop.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lcwkjyhx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldvpjsos.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2onpvlmba.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2vqvcyjgo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xmljbbit.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fuabdklk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kwrgwkrz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ylogoezo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ggijuyqr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtgvsee.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ljtnmwwu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2scqpghgb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2sjapihjf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2dgrvvebk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2osfgeoyj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2shjnpuso.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oplktkhd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2suybadiw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2teyohwcu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2axzcqtiq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcdsxlvb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2puvptklz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2pidlrdou.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qetlgghy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rxqoghgq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wbyoqvfj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xphsrygg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rsfksncq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vnzjgjqn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ovtjtvvh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wicfvcjq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dysdtogv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rsilsjjj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bfhgmxxr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vzeidwcl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zkrtogqm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gcmbodou.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pwliufab.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xohsmkim.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2phsnluqf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hwjlsjwt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pxdjuwpf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ylqvvkbg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qrmmvgux.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2okhgvimj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmjudmxh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2aetlykwh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2niscglrr.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wwusuuqc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tchmlczh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ijowozgn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qbaxytzv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zjwzumvs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lmyixxia.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2kfinzrpc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2nqqufpwn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2mtjrcgno.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lyaevuwv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2txfhrzpu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2keyptwto.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgznifaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjszciui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zerubwfj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfsnbzd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dsdjrvhe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2btytdnhm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2opmgtuon.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2kvzydrjv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vsisqlke.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vgfbgpgy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2psvcdrca.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2twnptalf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kedzexne.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ysisokme.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gmqgnhza.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2blbdkuhs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hytbvpor.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2lnhtpscv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uqpkdjcd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2moqmduid.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vfvzdyro.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vjxskvcb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cdauopzv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tzlrrjbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbtzgpeb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2fdlfkahu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyddwjtc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wzjipjve.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2glydoihi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rcjgudyi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vpztxwvk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wulvksqc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mucfmbbw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ncuofzrb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwrqumnq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2obtllzte.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2sizlawyd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hjsdcqxn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nuhbtcnb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ifudjtws.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dwatjjtq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wesdfhtp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zmlxumkg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2yddaywfq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xfvumetl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dmpzyxrq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2snrxtsbv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuovlcpz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ldmoidbx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2opqgpbpp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2cxypjlzl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hyschwwi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fmuleqxx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ldrevmsj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xnumdftq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ziarsjzt.html


<!-- 参考信息 -->