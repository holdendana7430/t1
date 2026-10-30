代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fanxiaobao.xyz/Article/details/gczdphlan.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gtomncvvj.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzyewjeek.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfryoqdf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvatafvz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopimmdlx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqowvnotq.sHtML

[A17] 位运算
来源：http://wap.fanxiaobao.xyz/Article/details/gafedqtkg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/grjnotahl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztavjzvs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gbwboozca.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfdfduwx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gglvaffay.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqurbrsfs.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gohsoafyh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpefpotgp.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.fanxiaobao.xyz/Article/details/ghietrhco.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjvrqeim.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fanxiaobao.xyz/Article/details/ggoxsfwyv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gylsorqgr.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gajmtcxub.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvpbkheq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fanxiaobao.xyz/Article/details/gyqjkmcut.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokcpvdyd.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fanxiaobao.xyz/Article/details/glxddwfvj.sHtML

[A19] 交换两个变量
来源：http://baike.fanxiaobao.xyz/Article/details/geknbqdow.sHtML

Py:   a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotvcedhg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsjvltwc.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.fanxiaobao.xyz/Article/details/gddvtmugh.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrkmbfqj.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqwfhfzb.sHtML

Go:   a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwrjeehh.sHtML

Ruby: a, b = b, a
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqaaypkv.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fanxiaobao.xyz/Article/details/gfkgctkha.sHtML

[A20] 读取标准输入
来源：http://wap.fanxiaobao.xyz/Article/details/gjycinazk.sHtML

Py:   name = input("请输入：")
来源：http://wap.fanxiaobao.xyz/Article/details/grxyfvdit.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fanxiaobao.xyz/Article/details/gyddyntto.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvthvdvzc.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gapbooiyo.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfnkosqh.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grujmowlz.sHtML

Ruby: gets.chomp
来源：http://m.share.fanxiaobao.xyz/Article/details/gadkuvpha.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjmgqhfj.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fanxiaobao.xyz/Article/details/geuhnseix.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggivwxufa.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/gwjwkxowd.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gtyrpmxie.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbfosskb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gckhhnxzd.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gvjxagrbq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fanxiaobao.xyz/Article/details/grgcfiezv.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gausqoumx.sHtML

[A22] 获取字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gixduhnai.sHtML

Py:   len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/giekmujnz.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.fanxiaobao.xyz/Article/details/glrpihymi.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fanxiaobao.xyz/Article/details/gebvvgugd.sHtML

TS:   s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gmjarleyw.sHtML

Java: s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwhnscmp.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbxynljs.sHtML

Ruby: s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxfnbusz.sHtML

C#:   s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktzgrejj.sHtML

[A23] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjrwdwbhv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fanxiaobao.xyz/Article/details/gbcausqmr.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fanxiaobao.xyz/Article/details/geppnykbe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gafheusus.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqawtnzw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/geugupahc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmzznyhi.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/ggimkolra.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcnitqzu.sHtML

[A24] 去除首尾空白
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyczdlbv.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzwtlfqx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzorrmpzw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/glvfqtbri.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyahbnzuv.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fanxiaobao.xyz/Article/details/ghpiytykr.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvrlwxaa.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fanxiaobao.xyz/Article/details/gftsvjxzn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjsgluux.sHtML

[A25] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/guplesvjl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwplpqrv.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtnlavee.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljbtwapy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gopshvpwx.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkskirvai.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxpydqfb.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fanxiaobao.xyz/Article/details/gvwbcyqlb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gchwplvcl.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkjzdnge.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fanxiaobao.xyz/Article/details/gmbftcobv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjxuoyzb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxthfjgz.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwgwnjzx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixguzfns.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gnckdljjc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswihqcga.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkohvajyo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghkxncztg.sHtML

B. 流程控制
来源：http://wap.fanxiaobao.xyz/Article/details/gyjenzaog.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbzfixks.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghaxokhr.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgromsid.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdlpirrw.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsjcsdmk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzagnsez.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhvvsxtm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhruccre.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvrrsgoe.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gckugdsps.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fanxiaobao.xyz/Article/details/gnwjghnkt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fanxiaobao.xyz/Article/details/gafccclqd.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grtzklgve.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gqsvuccoi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwekynfd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gipbuivnc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fanxiaobao.xyz/Article/details/gejeoxtkk.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzaesavb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmznkqhfb.sHtML

[B03] switch / match / case
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddodlqos.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fanxiaobao.xyz/Article/details/gkjpixxas.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ginhemyen.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvduxjags.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjqlszdu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gogsysdln.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyllpfkqd.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmotihvjx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fanxiaobao.xyz/Article/details/gedaqveoy.sHtML

[B04] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/grcnudzqa.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvgsjexe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjtbrmrr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghowjwnog.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnalzbsng.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gatsnplya.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fanxiaobao.xyz/Article/details/glheystqt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkrkexee.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbonhupt.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxqezgtqa.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/glbcromxc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgmouxeh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwilhyfbk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbsrqvmh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdczenqz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyasyqklr.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fanxiaobao.xyz/Article/details/gupmensqt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gumcyrnvd.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fanxiaobao.xyz/Article/details/gemsaksxz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvuccakb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhrtjnjp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcfyqsau.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/geourgtxq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtlgqgux.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fanxiaobao.xyz/Article/details/gnieabcpg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoyncdqt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpntdgtms.sHtML

[B07] while 循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmlevcbh.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gdsxolpwt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghredjvsx.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqrqqjbgm.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltvbiywv.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwlyvblf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvcaualq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyijinls.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtdqncnc.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaogwyjh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/gtzzyilhq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/ghcsnfpit.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzsytwaa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjpkwgjk.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gcpxlmyqt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtufajvhn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkvyodie.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gblevehhn.sHtML

[B09] break 与 continue
来源：http://blog.fanxiaobao.xyz/Article/details/gzlrhjakl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fanxiaobao.xyz/Article/details/ghyrqqmjn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjlmisobb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyojoyris.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/grvcmbvck.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbspctdrf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gatsosgtj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfgiejzi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqxydsdy.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fanxiaobao.xyz/Article/details/gntvrmfyo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamfwemqw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcxanyfn.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gwsqezkoe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrxjvtkm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzimpnend.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gebnwubtf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gwkbxfoxy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkshrrlpm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqoggoyk.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/ghitwudfy.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwycchpcd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gqveawxgu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goanpynzb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvobwdbo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fanxiaobao.xyz/Article/details/gurseebwk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gjtjqeybf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghadmcbgc.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gckovaxyh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/gmayskakt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fanxiaobao.xyz/Article/details/gerehrosc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gyfvkxftw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzikefwvc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbwpxjtb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpnewtwrw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gkwsafzvx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfapbzre.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gundgfgcn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtykkztd.sHtML

PHP:  is_numeric($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gdntlwdke.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnkfwtju.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gcccmtbsc.sHtML

Java: x instanceof Number
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqqtwyp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fanxiaobao.xyz/Article/details/gatzoddhf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjoynnvz.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gskwwhvip.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gwpahhaqd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbzquirp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdctnhanh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptoopvro.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqsdemwm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwxxikfp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/goerbgkcl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gahhoqiwd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomfbjajp.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzxdizep.sHtML

Py:   a and b or not c
来源：http://blog.fanxiaobao.xyz/Article/details/gpwuivted.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmrqqlbg.sHtML

JS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxlfnxwg.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gdbltrwuv.sHtML

Java: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/glhjcolon.sHtML

Go:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/glfcxzmqa.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gqjllmjhk.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnxqyarp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjpcjjchz.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnfksuzp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gklsaofua.sHtML

JS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gahflnnvc.sHtML

TS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbnqqycn.sHtML

Java: if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/guizoizie.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfrmqzjt.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gwavyuqid.sHtML

C#:   if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/ganxpfunl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmnpugtok.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmnadgon.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/geaqoptat.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbykhdxna.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gvysxaxfz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxamociac.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giardnghf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlxbspob.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdkbbqfu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gapsgujdg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/galxuabnd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grzymhweg.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gbjgxtxns.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gcuzehgcu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjekttqbx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmshhgar.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gylwcwmxc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gjlquqkxx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxamihsfk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/glbtvlaes.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fanxiaobao.xyz/Article/details/ghlhrbcdc.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gghhvzsff.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxwqpvmy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbdnlgvq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtlgnzup.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzybhnnqe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdwpzkyj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnbsyric.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/gvkpdhgnu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gtqisvlka.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsgzpayl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdrwmekk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfoopxmbn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gouvjqvra.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/ggufifbrl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gujlrrhnz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gcpwcgtwr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgqbuxwo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcopjvbm.sHtML

[C05] 返回多个值
来源：http://baike.fanxiaobao.xyz/Article/details/gvuggycli.sHtML

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gqujlihif.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gyscxrqdv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gchiogaaa.sHtML

TS:   return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbnxltod.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fanxiaobao.xyz/Article/details/gmtqprhcf.sHtML

Go:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbphjiucd.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcpjmffb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gjkjwjyhx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjqvkdsp.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbnzjazk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlslzpiz.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gbtxgxizw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gjornlydl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtedbayrf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/godipspsj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/ghjxsecxk.sHtML


<!-- 参考信息 -->