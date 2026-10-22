代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tafrvxpt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2oaiadqhz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2estutnsj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zkixcqpt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qdddwjzb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jcdrpmsu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tvvagada.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jkobsphq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ghzhdary.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oevopkby.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yxddqvqx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ebybbmuz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2llmzaoql.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2hqfdjaxh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rvyffwpe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gablkfhm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eavagtjy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2zbdudgts.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pjgmrbcl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2itmpesbb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2iprqmhnw.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ohmhkhil.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kvkrqvwj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qbwidnjy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gwiqqwiq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2svjnvnna.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2qutkhong.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2jmjrsxwe.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2oygqsybn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rcppjoth.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2jrxjgzlu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2obvucvys.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2embyvywc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2hiduxrtq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2dgilekdh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlpalqao.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2nwocgybk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vtdkmefw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cxmxznxp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2paybovpk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nzlxlwtp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcsqhgiu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ttfdnmpm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qcrizgiy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xldtubax.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2awpabmvi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hjfpsfvs.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnokkrxc.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2jsqfqneu.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2aodbfivk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjrurbq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fglujaxo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ssutjdfz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ynautnqv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2encvuhlq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ubecstza.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tpyrxjpj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2vzogopjh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2cuoqjyvj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ucegrkxv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2xpeajzqe.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kqzpdree.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2fuoejovq.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2egstoghl.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dcbihhqk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bqswmbur.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2oqwajgjg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2lxmcccbf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2wbevcdab.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ohiyyrsz.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ccuvxsgm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mkjdcczf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2pvdeqgzn.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2neaitmev.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2hsaxffxt.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2lkmwwosp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzaojuzj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dxyiapuh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xezjghbm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2djgwtamx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2omvnokof.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kkemutil.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2anafixvb.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2iajjddhp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kzdmbael.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvpvkyql.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2ysqlwtam.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2dpuhpahx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mdupnnty.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2nwsqedwa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xgcnmbra.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2yjnqmnbv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2umgzqhyr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wpbsyrhf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lnnoxcqc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihdefjhp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2cektytek.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ftxyhmny.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2hlihqtpx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvdirwiv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2spcbygio.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wfvdwyjs.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2yztlmlsk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ygzzuaef.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqworlmi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xbxmlgxx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oxrmkflg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vylsbdyk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2zqvwbucq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2uyswxose.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uuredafl.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iedtqypx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2oyzjqoct.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ywsbojau.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dnkdoxhd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fvgpuxyl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eyayqqhk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eagomujd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2dhldgcoq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2fwzmpvzc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2xxqqafaf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zgjiylhr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dqfkdxhf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2uswgfpyq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xwmxvvwb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2oaouuxuo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bobowktr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2drjsjjmj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mnxlohtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llyrooyq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2jlqmtpta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znctcjqm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2dzhtipdn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sxpvknmk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnnynrct.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rmoeyfoe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xpiyewxm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gdhgqvtv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2homkbyza.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ocmoxvoi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xefinijq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2lrobllgd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2mhygsvqq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cxcfqfdu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ghiahesr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2iunvoafo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nwfcdsot.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rtccebco.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2uiyledgj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2joeuhkob.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2yaexazza.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2uoxcfwlh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2shgekxyn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsydzhue.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yssobhku.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dulvvmya.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2tcwvladg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2uznjnsvz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hpuquhmn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lubaahnq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hyfsjdri.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ztoeloan.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2wslrbfep.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mufxqknn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2pmyucbvr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2jmguksgy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2iglcvfnj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljaivtcn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tzwurxrh.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2mpmtpawi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2isyfxbbs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2khbzzcfn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtrmdyuo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mgvhaayj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2pamazsmj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vripiptv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcajoclp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2enmknuqd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zdizwrlm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2tbzmzuix.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2uivxhxki.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2irlbvrnx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gkjjwlou.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wxnozijy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qfgezhrm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sosyylxq.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dnhfwthv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nytnxdom.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wxlktvzs.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oydnhzky.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dqswmuyx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dzjzgkko.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vllukqne.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2yylpsmpu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2umodoopj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mwslybnt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2byusiqss.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2blhjnyon.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mwmngnnx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bzgppogc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uwbkymed.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wzcajhoq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2mimeqxda.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cxsdczzj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2bjrbswyx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rajdnwem.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hyqeutfk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2drlekmuz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ifdfvhzm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lmdyoipj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2eptvdwhb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qxxmmdwd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aglnvzqx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2btdpjxka.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dyloihbk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tueunlzt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fubnjzrr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2poypzhxz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtdppxkx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kmmyoppt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zdnixway.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rhqlnklc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2votjgutc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jehoqepi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2hmrsdtyq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lvdshiuh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2noskuaaq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tyzxkucy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2qdomdfgq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cbkyyuhi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fdebmfpt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wlhpxaio.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2uapiahan.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xikqenbu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hqtuawzj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zgxwfnsh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mqcwmekf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqjmkssq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xkyraxco.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2darurnio.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2cwioawqc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2hdjlrnrl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2atepmpoj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hnkykyju.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2meezgzke.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2jgoeulqi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qwztaybz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2csgkurwg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2mruychlt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gnaqfwfm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tisqslat.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nillvsin.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckujzqsu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ggoibbbh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzccaku.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtidzmzc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nahqoubc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cxljcodi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2axfbwtuz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2jgzcbuff.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2xqkgpklq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2upqgzhdn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vivjjdtt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hlbrpomn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fmeqgiti.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xoutqecm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sjcrbtqh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qwazospo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ibnnpfac.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hxmcnmlr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cqliravf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dmwpgsgp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bexonzfi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dfhvgsdu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2nswekgiq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xiyxvpdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtdnrydz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gvmoylif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jaothtrm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tmyftqdf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eliyrcpv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ogxmcoxw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nfleozug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kulefxph.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jogmxejf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rotihgin.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wzkkolct.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gyxexreu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bsllcrzm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tcjgjcws.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghlanngl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uihbhfaj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xopbdjhk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2pltxetbr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uysevapf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tnxpbcrb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rgbpxxlp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2qqafixzk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgyivqr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dpqayvlm.html


<!-- 参考信息 -->