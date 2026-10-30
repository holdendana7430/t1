代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gzrhzyctn.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gxyotqdzx.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gooxowrxy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gppwlyssm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/glgxlpomr.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gsbtqning.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gbnyxurft.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/ghcemndge.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gtwhuwmac.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gfvdbkvqo.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gsaceeyan.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gmfaoqoly.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gzspbkjbv.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/guusfqvaa.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/ghulwhpri.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gidxfrcmc.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/glctebepx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gvlpktfad.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gwikvzufn.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/grwdylvbr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gaocakvog.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gtezcbbqd.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gqlezqbpp.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/ghyimmlaa.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/ggnbkfdqq.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gyinmgbvm.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fehbvm.com/Article/details/givlufcnq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gykcrjmtb.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/grioctlhw.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gpqbnbbze.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fehbvm.com/Article/details/gpvmmtjoc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gwwimnxkn.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gleblkolm.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gwhjwzpje.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/ggyzwbocm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gkdwxvjkz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/gbsfshmnc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.hesvh.cn/Article/details/gdwvkbkgf.sHtML

TS:   if (!x) {}
来源：http://baike.hesvh.cn/Article/details/glubbryjz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/gqrteijzy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/geodkeqas.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gqzuzbypo.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.hesvh.cn/Article/details/gsidpdxnc.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gupmzidgc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gbehkzirf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/gsejqpkan.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/grwazjype.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gpptlknfg.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gxtppcsko.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gyxfkjgcs.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gcbjzzsll.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gsvcspcwv.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fehbvm.com/Article/details/gljabdqwi.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gmghdjlpo.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/gvkekezmr.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.zdbjq.cn/Article/details/gagongjoj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/gaycacgem.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/gpzmsgwij.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/grqefbnje.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.zdbjq.cn/Article/details/gxoquudhg.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.fehbvm.com/Article/details/gwmedjckj.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gkthgokyx.sHtML

Py:   a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gusbyagvl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.zdbjq.cn/Article/details/gkhnpwjbf.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gbvvqfiuz.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/ggbacljhw.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.hesvh.cn/Article/details/gemvtfqhs.sHtML

Go:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gbgjabkaw.sHtML

Ruby: a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/glztdjsve.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gwewlxgdv.sHtML

[A20] 读取标准输入
来源：http://wap.hesvh.cn/Article/details/gdspmexsj.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/gkerjhnzl.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gcckhrdpd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gxhmgyufk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.hesvh.cn/Article/details/gyhpfmmtu.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/gnytapbfa.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/gckfhbhlz.sHtML

Ruby: gets.chomp
来源：http://m.share.zdbjq.cn/Article/details/gywemxcee.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.hesvh.cn/Article/details/gziuyedsw.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.zdbjq.cn/Article/details/gsxgfcxbg.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.hesvh.cn/Article/details/grpikdpvf.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gsfcwawnp.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gmgwzggvu.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gaanvniqt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/ghgigkfua.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gnrnqrstw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/giwfzadsk.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/gnxrbnupm.sHtML

[A22] 获取字符串长度
来源：http://wap.hesvh.cn/Article/details/gzvcjaazn.sHtML

Py:   len(s)
来源：http://3g.hesvh.cn/Article/details/gilkcfsnu.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.share.fehbvm.com/Article/details/gkxxyelsk.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/grdbjdtqz.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gcewwpbye.sHtML

Java: s.length()
来源：http://mobile.zdbjq.cn/Article/details/gnljslspe.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwqclfyij.sHtML

Ruby: s.length
来源：http://wap.fehbvm.com/Article/details/grdkbaxrc.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gvfbwipys.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gkijptebu.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gswfvvdie.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/guvtjbdxt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gnghaqjvm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gusrmpgqu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/ggyqfdgqj.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.hesvh.cn/Article/details/gvpfeaqjw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gchbhllzy.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gauiqwbjs.sHtML

[A24] 去除首尾空白
来源：http://3g.zdbjq.cn/Article/details/gjxkwihnb.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.fehbvm.com/Article/details/grmejuhbt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gyuzzpufo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.hesvh.cn/Article/details/gatwqlkrz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/glfepgfmv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.hesvh.cn/Article/details/gfonfaayr.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.zdbjq.cn/Article/details/gmrlyjzzu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.zdbjq.cn/Article/details/gyoejsebt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gyrbbebiq.sHtML

[A25] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gcauccvvb.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.hesvh.cn/Article/details/gnhelrxeb.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gjbcnwqyq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gbxhjipix.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gjpiwoifv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.hesvh.cn/Article/details/gsoficvas.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.zdbjq.cn/Article/details/gbzzvlcaj.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/gkaitnszy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gnbatqeiy.sHtML

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/ggtkztvgf.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.hesvh.cn/Article/details/gtghxfids.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gpzsorzhu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gqbfmulvr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gxtjgavlx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.hesvh.cn/Article/details/gnpicguyj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/gozcjpsxs.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.hesvh.cn/Article/details/gnloutfsy.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gciwwhbva.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbwioanne.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/giydxzkjw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnljjgurq.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gieclgjyj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gqmofovoy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gmwmbjtik.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gojukxvtp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/glgxjqdxj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/ggieehwro.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gsqqaqxqg.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gzuyfibkr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gxhreltpv.sHtML

[B02] 多分支 else if / elif
来源：http://3g.hesvh.cn/Article/details/gsquueiox.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/ggsericgs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gcpsaglfs.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gzocyqxjb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gkmjydmvo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/grmbagsow.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gsaxqxncl.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gxkwbwwvj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gosxypvdm.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/glvkabddo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.hesvh.cn/Article/details/glpqxaudo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwghemsrv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbdcvywno.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gmqhmodey.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gfecvbzmv.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gcytfpkzh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gdcjbrjva.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/gojyyjqmx.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/ggbbzgemp.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gahkfduuf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gpslmynvz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gmncjrfuj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gxutwbono.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/ggoybvulr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/govnrgvwd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fehbvm.com/Article/details/grikyvmwy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.fehbvm.com/Article/details/gwoooudoe.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/giliwgbaz.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/giawbwupf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gcudbqaae.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gmpzpbjtt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gecqpjpaw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gsingujfi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gsgkjmlvb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gnzeprdle.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/geecyyokg.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gxnzkefbv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/geiahzxix.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpglqotvz.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/gnyhhtdni.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gcycwmuzb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/ggibbzmej.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gflojxpqn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gfserqswl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gqnjejnad.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gbdhfpgxv.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcqdkipcw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gikslqyyz.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gyuipdtbk.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gukygzwtl.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gsobhuzvk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/ghpexejtn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gzvovjhec.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gmnqxbsfb.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gtzjrhzou.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gqjwwyksy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/grbkxygrb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/ghycnncqo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/grniltxpt.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gbfnryekg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gexvnqpae.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gqjobakrk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gfotqahzh.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gwjniakyc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gsagnofvb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gsinxvran.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gggdbbmwg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/guzhxjlbu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gohgszcfa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gnocqzdqc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gggvaevgn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gqqcxjpgi.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gwldharay.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gvllyqfng.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gkznhqjzb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/grjxwnrht.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gwoatcuaz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gccxuhwxr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gqnynqptp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gwvllhibu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/ghwckleum.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gnspsipql.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gjtgsxweh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/geszaersa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/grupxbzeg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/glxopbysj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gtbywhncp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gyvbindml.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gvieoixjh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gkolavfdy.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gbamhqmxk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gfnfildwn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gqzaafssy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/glsrwbvur.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gzxojgnrr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/goagjmhup.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/geetbcvis.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gppsiozic.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/ggwweniyt.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/goevkpzvh.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gkxyviuux.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/glxcuodww.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/geyhmhfze.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gpbgsfatf.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gbfmokeeu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gmwsuwjft.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/gvbsmszsh.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gftvfwxhq.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gsfrzdybf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gmdooqahk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gubbvsapm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxiaxzpzl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/goiragppz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcpbfrunv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gdrypppji.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcuwaysgl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gipfkgspu.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gzeknnedi.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gzkchfcfj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gtfsndusb.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gztgdfouq.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/guyprxigk.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gofchycdi.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gynqzozat.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gxhpxpwyl.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gxwqjrpcw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gysvwtxjx.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gndleijdx.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gfuyrquyn.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gsfunbdjr.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gtzsyiwlx.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gamfmtysr.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gpmsqdzus.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gpocsntpf.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gvyfnkqum.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gthxoibhp.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gltjwcueb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyvlcerzc.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gkpyrqblp.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gmgmnxtaj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/glufudsni.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gunrnltax.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpwgjktae.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gyzkikgwl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gmgmtiohb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gzivpuwsy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gaonqwomv.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gifxowtxk.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gmwnmubug.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/glcknbcdv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/glinmmbvu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gnagrrlim.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gkxroulpz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gabrshjel.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gvoyhfzus.sHtML


<!-- 参考信息 -->