代发 wailian999

[A14] 注释写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwnosypr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fanxiaobao.xyz/Article/details/gonstiiuc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/ghpfmsckm.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkhtfbcp.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdvsslaa.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbwalqdt.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gxiisadcd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgxmbptp.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gonvwkzrr.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjformoh.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbxremak.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gafsyvifq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwojlwfw.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxczlkzfl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfhuzprv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbfqhzre.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/glbbajzhl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gicmyoqyp.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpiyfcld.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gwugkndql.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fanxiaobao.xyz/Article/details/gbiputcfv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gbkxzifxd.sHtML

TS:   if (!x) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpewimwn.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxmuatdr.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgmvvfqb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgifxlyn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggazmjasr.sHtML

[A17] 位运算
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuheayds.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gtunjdujj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gjjpkbyyh.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/grjbybiov.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gyourjgvc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/grdvyohbk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhcofcqo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gencbeouu.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gycoseeha.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/grgookore.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fanxiaobao.xyz/Article/details/guubgzbqh.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gxidkxmck.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggguoyjta.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gkclhxbho.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseuxauha.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fanxiaobao.xyz/Article/details/gufjkujba.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.fanxiaobao.xyz/Article/details/gzjpcllax.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfmxduxq.sHtML

[A19] 交换两个变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmgihqty.sHtML

Py:   a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzxzkyve.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcomvojqd.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/gkdbcxmfa.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/gdcbuymgo.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.fanxiaobao.xyz/Article/details/gujwmfhqj.sHtML

Go:   a, b = b, a
来源：http://wap.fanxiaobao.xyz/Article/details/gxjduygjq.sHtML

Ruby: a, b = b, a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyucjtal.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfllrwtr.sHtML

[A20] 读取标准输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpnqlkdx.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fanxiaobao.xyz/Article/details/globtnvmf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fanxiaobao.xyz/Article/details/gqrqdazkb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfujquht.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpufbnota.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdjlhkdt.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.fanxiaobao.xyz/Article/details/gmpryevra.sHtML

Ruby: gets.chomp
来源：http://mobile.fanxiaobao.xyz/Article/details/gouknsvht.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fanxiaobao.xyz/Article/details/gefvglmpm.sHtML

[A21] 保留指定小数位输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwymvdzy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghiicaalh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfryhdamj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyyekabp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gdepyhkkg.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gjccravbr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gucfikicx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gazgmfwac.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gufuxcyfr.sHtML

[A22] 获取字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwonicidm.sHtML

Py:   len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmgzblpx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fanxiaobao.xyz/Article/details/gdglnlrgn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fanxiaobao.xyz/Article/details/gqowyrbby.sHtML

TS:   s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxcqggqo.sHtML

Java: s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghprzlnov.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzmcfiflt.sHtML

Ruby: s.length
来源：http://wap.fanxiaobao.xyz/Article/details/grvoqtafn.sHtML

C#:   s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gltylzhte.sHtML

[A23] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gxxbburpq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoezhgzz.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggjkiprrw.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqtdhadq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gwmfruwsh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnelmahft.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gipxkdtiq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fanxiaobao.xyz/Article/details/gvhjrqvjn.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.fanxiaobao.xyz/Article/details/ghimchrhg.sHtML

[A24] 去除首尾空白
来源：http://blog.fanxiaobao.xyz/Article/details/gtpmgrmbr.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/grreaizen.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guheeoeyo.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.fanxiaobao.xyz/Article/details/girrzzukf.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsyttinx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fanxiaobao.xyz/Article/details/gkxvvqhbm.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gyswwsxpx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fanxiaobao.xyz/Article/details/gkksgsbww.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfhjhyye.sHtML

[A25] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gaigyqtzg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcdincuv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grvtcuhjr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptqwiobc.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsiltmpgm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonpcgezt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gtnczibwr.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fanxiaobao.xyz/Article/details/goopgzxgb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggmzzjcti.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsnblexb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxraufkss.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fanxiaobao.xyz/Article/details/ghdoewfon.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzffxupjr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsmfxprv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.fanxiaobao.xyz/Article/details/gdtpgqzzq.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdkulygx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdlwqvjz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkampfdfo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxezvgnij.sHtML

B. 流程控制
来源：http://wap.fanxiaobao.xyz/Article/details/grdnlvovq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gybqbscor.sHtML

[B01] 条件判断 if / else
来源：http://wap.fanxiaobao.xyz/Article/details/gsrczfcrp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fanxiaobao.xyz/Article/details/gcknraaam.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpuvsuvao.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gowhfgrkx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gqcuyvmmk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/grzxrcgwk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfowhwasj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzvpvrov.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gpqzprloi.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fanxiaobao.xyz/Article/details/gebtuqhqp.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.fanxiaobao.xyz/Article/details/gjsnvrpuu.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grrimpouy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gicgbxgej.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/ghhjvqpdt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmrtlqxd.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxukzkmo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvhxxzte.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxsdhgbu.sHtML

[B03] switch / match / case
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdqaxnqp.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjoetqpg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/grnrzcuvh.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyrcwonuj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvyyousa.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzqoigro.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/ghsyjplso.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsutbtiyq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyobttrut.sHtML

[B04] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gpxybgjsm.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfycgzr.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzbqypqlv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/grnjgtgmy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjzerxlk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gapwxgwyl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskakemto.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbdyewio.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdhhflucr.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgsfemjd.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fanxiaobao.xyz/Article/details/ggajbbtdh.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxmecfxf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gshyjixra.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmsbwjmnu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzhphwhl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdamncjxv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/glxysjmjt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghugugxmv.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhxhswuu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/grxrvadwg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeeusxyx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnwetvaw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fanxiaobao.xyz/Article/details/gsaidkkir.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegwehndv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gipdeztvw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbwhggvk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpvwmdxw.sHtML

[B07] while 循环
来源：http://3g.fanxiaobao.xyz/Article/details/grvqcnqfd.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/goeaavnjd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gptbmorkq.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gskocjxzy.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtwgommgj.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggfiaoxle.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtuauhap.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gljisceuc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtiwjenf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtybuyrrn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/gomehfneu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjwjhtwa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasfyqclk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjmbcxxw.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/ghybiwsge.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuehqkje.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/gzhxfsvgt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqfekxmh.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/gvlakdbzz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fanxiaobao.xyz/Article/details/giwccjpgd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghulmoxvn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrdkfljg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbkvvyjc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwojkmsyh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdobbsrd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzymzdkcl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/griftwdpa.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fanxiaobao.xyz/Article/details/ghrzfxkgo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/gcipcncle.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrytyzuf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjqlltli.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgikvvdy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcztclsg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gudlhtfik.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvhkmbly.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtjxxxob.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guonaunjt.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiggkefk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfneoyhup.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzpfmocs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gcgmhthjv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gnkrcupvc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fanxiaobao.xyz/Article/details/gjexjemzh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/giozqlqhy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gugvtzvbw.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtuegpeh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gwbvtojgj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrawgogi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gvyubwhxp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gptmikzrh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gmywcbjsh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkusscoxx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fanxiaobao.xyz/Article/details/grjhsnetw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnmfvsor.sHtML

[B13] 判断是否为数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqnumqtdb.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlsculog.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzewdxyh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/grbzlchue.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvczpupu.sHtML

Java: x instanceof Number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxofbvstb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fanxiaobao.xyz/Article/details/glcdjhwgn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehildckp.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gujrfxmlw.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsemibhvu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gveeluogk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvvymymv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzljmujil.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrsunowj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/goxuvhfhz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gddaerdom.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/geauqrrks.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxbnwvhno.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjxgtgvj.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyvewhcv.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fanxiaobao.xyz/Article/details/gsbonhtgy.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfiixhqd.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwwlewfw.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gjopzhdma.sHtML

Go:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gemzeqajv.sHtML

Ruby: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gljhpwoqu.sHtML

C#:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gvatauvnk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gidigmrgj.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhyjtdcl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgbbcgki.sHtML

JS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gsanplzvn.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbelvtnvz.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjqkasmm.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gltflucqt.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/gnjgelwwg.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gpclpfjoq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqljzlng.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtzcilop.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grhglhbev.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpsagtocy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvlltwif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gethtqlgn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxhwntldx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtjtnivt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmqnnjsmd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gpwygzzyf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/grhnwezdt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklamgwmk.sHtML

[C02] 默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsbvvbeu.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gruzuwfbo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gydeiunki.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjaqkmxi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqvpppgt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/glwnjtzpm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/glfchmqos.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gotssnafs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fanxiaobao.xyz/Article/details/gwvgtboqi.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gjqxbbopo.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwudijlij.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fanxiaobao.xyz/Article/details/ganwxuhxx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gasfnwdzz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmmyeqpo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvicihisl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fanxiaobao.xyz/Article/details/govjoiwuh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fanxiaobao.xyz/Article/details/gdqvofuta.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfomtwqlt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fanxiaobao.xyz/Article/details/glngqordz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gkqaojvoy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfryqkra.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gteujvsuu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gmaefqpoo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gadbtodmf.sHtML


<!-- 参考信息 -->