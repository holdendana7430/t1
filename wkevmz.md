代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mmwslhhs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kuoceodt.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wwxteehw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bfrjkjek.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3phlhxryc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xgsnfxey.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3meyqxpdm.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cpdvtehp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tcwkpetx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3hmbfxzat.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fvdgoiba.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3holqofrt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yfrzvdtj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3tscwrqre.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qscxtttw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3iyfnmsyx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cmmouzlm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3fsrcustd.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rszgbiou.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xgqnhyfs.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xewmcxle.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3piwqjymd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3sppuaqml.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3aiudpwbf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xwsygfih.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3brxobnct.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3bmnefcjj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xvsptqrb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3oanjfcbe.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3vhhavkwc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3weusseea.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flyvefak.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3aiwlosbt.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3gjqdvrnq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vgaiumwy.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3mpspancb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hxfkdekv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3impxgysq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lrxpowtb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jcadjdue.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rlxykkqc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3puferidg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fsslklnn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bxudezuo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3pfnamvoi.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vvosvqhn.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hvxvxoul.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3emnkgbcd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhluvjw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3wxmwfgfc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xsxycinv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3lduwjxlk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3tayyuasy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdpxdhcc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kcvcfyoe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pgjdslyl.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ikahgznh.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pibrkgcn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3aacfoimd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nvjknxxm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dqgcrutm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3cetszrdg.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3crpwvpns.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3mkzwgyss.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rvruvczt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3znzikezn.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zdgojnow.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3ucfzrgsb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3uelfafqy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3cgcmmgra.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cybvruyn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3vbdebtqk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3fxxntnfa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3szyssygp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxorkldb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vdbjqkke.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pwwqdwxb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xrstaomz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxlcokd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3sujmfyqa.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gtuzkfas.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3chpruxbm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3zddojuyb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3prwgdjfz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xxrdlyfx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lwmegkdf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ohzozkuw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxtdxtug.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3hzphudql.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tfwnjwjb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3pjcsygna.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zbfpdfnr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3epvprbjt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3iyfzxswm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ewslovjn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3tchzodsj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cxhalpbh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3unmdjxcs.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3qguaaknt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3awhxeqoe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsmyfhbg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pzpgkplv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3nkahtaij.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3aqlyzysf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3cedcgaiv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3noxfvftt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qawcjizd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwchyius.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3mxqoamri.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnratgvx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kktqdwib.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ahdhnwlx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3kfuryjbn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pamzouwc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3goolsmfx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eytfracu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3quizwnhl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3dfndjhhf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3yqqcsvue.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pfxcyekd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3etxizupv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ntvjqlgv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3cvkincwz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jojjyojr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xhdtadmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwwoxswu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wjdkcxtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3piddgpiy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ahepxjee.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rrevpiwj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dekxwqoe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ivpmtxdt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3midbnywf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3romjpolu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rzqrknpn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hrgbparg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hhdsbkhb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ssiiwtjn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ckkkmkcj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvmpdjtp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fouapabx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vvxlqbqz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ltecxhry.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3tikcdybc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zkdyfcay.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ddaslmyt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3jgfdxekm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3cvfytbpy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qlvzfioi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rauerdeh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vncciwgu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzrerpim.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvcoiot.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3pdpzwuvq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3qrvfrngu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3eqcaliad.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3oghmflmz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3yymjiguw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lukmweof.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzkeklvt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3jehxnxec.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ysmtkdgs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3fvqghvdp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzvoleb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vxojevye.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bppogdov.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfuckwki.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3osooampf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nibahysz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3twteabgm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gsxiwrhu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zdchukjq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3awbzcefz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3miycbxnq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tcjdmmre.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ludpubdg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bccemjkp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdhhcvzx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3fexfwedz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xcfncnkq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mjhyvatu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3npjqtgim.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rwyzycfm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gadelxjr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdlylmnc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xflkrilz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpkjloto.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hejggqwn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qnuitgre.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3edivhzrz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpbhrufn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ufqbasyi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3unkfsjii.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3scfexdpe.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wpoxxhyp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tajqphad.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3eqxhqnxx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zitpwkfo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jkznbhjr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3brzhcaep.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3nilxrwcq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ikwpoytb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxcfqywa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uymyocea.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tahrvdys.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hozlhrjm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ftmhhxht.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jttkmhpz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqjedgzh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wqonylhs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qptboqnx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3drwgvoch.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3difvrfuj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eerrckii.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3recuwlni.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3afdberhj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3urhwnkks.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tboihgso.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fgprvbpk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3kzfxtiml.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kvixfafi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ddgjdgtc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3khnyaqdh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3bchgrswl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zoppabyr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xpcjkyvw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wjszlkim.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tyedunur.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fyixroud.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hqzxwnby.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fphiolvz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cyxpgnuj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3unpfprzw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ehmpnxjh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ejepwhgd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dbohsqdl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3sjaacysb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ypnwaqbz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mrdshssq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcedgyhl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktmbsqzo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3yoibzfue.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rrugmolu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3jxtohvek.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3tesdipoh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pbxzrirz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3oaskmcuj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tpradhqf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ntixctri.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vezkorop.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmolbvkx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ddzbggmg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbjcvggh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dfjaztom.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rozsxxuc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rqhxjrib.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rxuhyoxe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pgiysvtc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cyzcnyxh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jaagcyxs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fonrxwje.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mmmimcro.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xakwpeyq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3woptddct.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3szlylxvm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3smennhxy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3icjvsgwq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kimqikqq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lagkeggy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zzmlmwte.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jnuhymmu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xalzeaot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oetgucdk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3brpxkzuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tewjyddn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nyommeqn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hggwmikx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tybmshpi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zwotmqvw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lniowfxl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rkerqcqc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3wjsvvjhs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wkyfbwex.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttkkmmyt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xmhqqwtl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xudpjizg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jdhvvcdp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3thzitynf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhprpixi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fvskgsfu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tcedrzhu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gmslxqgx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aquqomdw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gefpxadr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kftsottk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wwdaktju.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqffifdd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gpxwslyg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3fktwvmcl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jknkuejw.html


<!-- 参考信息 -->