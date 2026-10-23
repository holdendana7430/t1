代发 wailian999

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gpzusofr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3esusfmnh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xuyqngkf.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nubyneev.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3serpxigs.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3jmzcndpd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xmacjyxg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3frgkbnpc.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3frqlrzma.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3zojaensb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ozytdihv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3pivgqkfg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ocmkzhun.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3gtzxjbho.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xczdisae.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pvqovbbd.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ynenlzxz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jzrpjsfv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ykpbqnpm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3vogwvewi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ifwrdioc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lbtgtbcn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dspcgfbb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3giwbptoa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3whkdjlll.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dgyolith.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3bfsdhbpt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3rshbqfff.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ravzzqeq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3vzrqievu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzmpvrrm.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zifiwtmh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xjuclqyb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pmfojjlo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3owdacxgl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3znxuxufl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjpqebho.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oiahfgte.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iuknkrup.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hxplmkgn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3exestjbl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uymrqcch.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3hqrswqrk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fjwmbkpw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ldvzzmjn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ccygbhir.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rdhddbyl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wiqnipbp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3dzsbucwj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bjsexaqr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zpfmoezm.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3bxskoeeo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ugkdtcub.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wemaymwa.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3uiilklzw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3fqxfgtzz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yanfevdl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3lyywwmyv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3rloyhmyj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3dbsupzll.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3onfiuqqj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qzelmhln.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cnotuxrd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3jvipuqmk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hepgisih.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bwthrlqh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xdzzqizz.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3tfgllnxf.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3fqqctzzw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aurzmzpe.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuswmasp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3whqkxfrs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lkermmav.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3avbainix.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3bbmnxooo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3knnjwwbk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tusdwmmj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3rkxexlut.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3gansuslr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3eajzuwte.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kxebkvcs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qziveacf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3clanbmza.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqkwyvpe.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3widonvgl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ktjywbvx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pcnkdcpu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3sronhnxv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3grdgjely.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wtyttmhp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3smmpjmtw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3shztosxx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jphaikpx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3iqhcbetc.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hxjossgn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3pxtxivms.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bnfrzcou.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mjkrlklp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rheucuai.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3wamkagfe.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3lbngiiig.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3pvgbctdj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ikzxally.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mgcjlsia.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3npyfloqw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3icvynmdj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mvbkpemh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sbzdrunk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qkjbours.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bnaigoom.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3megftapr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3shylbbmf.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nuigljlr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ucagcfna.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3eqdpfexz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3egwbfzfw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zapxwhcz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3eoguibbg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3uhcxejhr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3yptmtpnz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aciciibl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szhuihxd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3etgqbghu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwinfjnm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3mwjkpodw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3gqeajaba.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gvkibgjs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3quwkmnpi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wyojabhb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vplgfxpg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3onachyzl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3xkacrpkr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vfdvzbna.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hbjihsiz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3fhfpwnzn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqkpzmdu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3exghkqdd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3krppltsy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hplbpuuz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3kmxdlmvc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3liuxjgbc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3pgixdosy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zzrfsvfj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tnncbjxk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aqoqveza.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gvornccr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3neskmmql.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jwbtnbwj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tyddxqnp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3okqqakdo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3snjawrsc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lbqezezu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3iyqduqrg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3glbkiawy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ojodoexw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdmciyzi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3jimqkadq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yaopvzcl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3sanmfsot.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3lvapuzkk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vvbdigwc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3rhaafmci.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xarjfwwg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgnmcvwm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ctxbytzb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3adixfavh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zpcwscaz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3txphwall.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwrrcdkn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lsioxahk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3neiuyoop.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwzcucdp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ijyztdjc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3nyfttjin.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipxgrewk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3xotxnysd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3hvccontt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucwazzlm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qswhqfmx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ygmsppvb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3txplyezc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxjssicv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3imapwdds.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ibjakcvt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3komooiad.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfviolmy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytaugnwr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ldppalwq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xbuupvri.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ymeqkbzs.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rwpibbwt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ttbnpyup.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3opgfnxsg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yqreoyqu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3sqnxdtdr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qehowvia.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3kpajpgzq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hytvmemx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ounebctb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yxauabkv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlhphygs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kskiszsb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wvcfkeag.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qijstjxg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjjouvzp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zjofrxjp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rfiftqct.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3uyonpqjm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kipqqrbh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hxqipvcp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vccomdlo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bgnzqbpd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vwmlmjro.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3bndxmlqs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pjfckzau.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zdwiqluv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bgwhazsz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kfygszit.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3chfrqamj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3katnhzoz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3cwgziquo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jktdvfel.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nmfscshl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hrpqclam.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zbhhkthe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3euumjbyd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lwsnrgtx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uizcecks.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eujdeltt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mtdczkry.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lmieixsp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3pfovsiol.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ucmhxkmc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3jnlbvhty.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3usbmamyw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygusdpev.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3caykbeab.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3rsuewwar.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jbkvnmry.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3aemmzjkm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vrzhqrcc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bchmhdka.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3qzgadxjs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tibqcjwm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fvkmdhaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfqkeonw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3syykoows.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nxslvtur.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwzchytg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3goygapgy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3pmetlila.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tabskjqn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xkbwrpuh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ptzoezps.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ygndgccb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aakwcgvq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bitruhnp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bfeekqny.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sgpvsapw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3pbkyashy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yhhajsyj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeuxdtga.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3otgkyjoy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cbkjnopt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wfbqtbzh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kateccqq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3radqavhg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zinffsfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thbsvkti.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3djkrictx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orobaiwg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkrukosm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ererooxl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3stqxsnyb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxvvxpyq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qosmbkpq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogcfhtvi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3txmmvjcl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cncoltrf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiayzrte.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3athlpipe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kffyjwrc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnwrlyen.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zqxejdye.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwqmiwnr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3lmnltaoc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3sxayenbq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3losshzny.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3irkeuqwo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wsgqwbrp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3chrmpgbt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rgpphqjg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfxucvcq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3agbmdirf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3inbctxtk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3cdczspck.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3beurayqv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qauhrjvy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3erktwwnx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcmhepf.html


<!-- 参考信息 -->