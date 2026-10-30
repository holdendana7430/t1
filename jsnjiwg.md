代发 wailian999

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/goeooyerk.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gudobfsle.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gvpijpfbx.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gkqeqshok.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gyyoafplc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/gkqdresib.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gksbxeixc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gvwguzhdk.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gqoqcjqjm.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gtqpxsffn.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gjmwyntsy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gbgupqxam.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gbmohaajw.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gqwvqzqjz.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gmpanlmiu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/grerfvodu.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/guwwvapkl.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gsluitiqp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.hesvh.cn/Article/details/ghvbpgubp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.zdbjq.cn/Article/details/gahhcfeoh.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gpqsrafmg.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gqxbcxtgm.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gffgmjxxz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gssirvkuh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/gbkbzwnux.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gxgqiroys.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/gtslpulcq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/gvdhkrbwv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gdbngeylu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/ghgjiljti.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggwmrsbis.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/gkdowvdgv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gmzxvahwj.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gnsysiayy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gmqxttouy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gemhjvvjz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gcknucheu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gqhwvpupa.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gicblapdh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gciuwvpgy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/ghdmvuntg.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/goqefqvdf.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gisdmbqdu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gxoiwtkzk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gdtxihrjh.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.hesvh.cn/Article/details/godtvzwak.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gdklrraek.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.zdbjq.cn/Article/details/gkcypknlb.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.zdbjq.cn/Article/details/gbbsflaro.sHtML

[A19] 交换两个变量
来源：http://m.share.hesvh.cn/Article/details/gcmekwazv.sHtML

Py:   a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gvvmkorxc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/grpmydhsr.sHtML

JS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/gpaeefwzw.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gfhoitfmn.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.fehbvm.com/Article/details/ggmfypavk.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gqhypykbg.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gcmmeavwy.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fehbvm.com/Article/details/gumeelwqp.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/girskzkpf.sHtML

Py:   name = input("请输入：")
来源：http://baike.zdbjq.cn/Article/details/gsizxddxi.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gdunnmmyn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.fehbvm.com/Article/details/gftsnmmct.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/ggwenlfuf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.zdbjq.cn/Article/details/gjybvfuyg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.zdbjq.cn/Article/details/gehpbkoin.sHtML

Ruby: gets.chomp
来源：http://blog.zdbjq.cn/Article/details/gtchwdiju.sHtML

C#:   Console.ReadLine();
来源：http://mobile.fehbvm.com/Article/details/ggmhupqku.sHtML

[A21] 保留指定小数位输出
来源：http://3g.hesvh.cn/Article/details/ghmkbrala.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fehbvm.com/Article/details/gccfcjmst.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gonzzxfpu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gxhfsgyvf.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gpaqamxdr.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gaqqklphs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gjrdsgtuw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gkadmrkxy.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/grvprwyku.sHtML

[A22] 获取字符串长度
来源：http://read.share.hesvh.cn/Article/details/gjdgnffel.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gencnbrev.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.fehbvm.com/Article/details/ghqcjdxgj.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/gqdxkqrmj.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gsjhnjjsc.sHtML

Java: s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/glaxeukzy.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.fehbvm.com/Article/details/gopehnlzb.sHtML

Ruby: s.length
来源：http://read.share.fehbvm.com/Article/details/gcmwnjxgd.sHtML

C#:   s.Length
来源：http://read.share.hesvh.cn/Article/details/gexqywvpt.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/grrpslaos.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.fehbvm.com/Article/details/gnojlveup.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.fehbvm.com/Article/details/gupsjmmye.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gtskosypf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gljcapjdy.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gljzlzcxz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.fehbvm.com/Article/details/gjsnbbttl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gpmjpurpk.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/gykcihsla.sHtML

[A24] 去除首尾空白
来源：http://mobile.hesvh.cn/Article/details/gtzvsdeue.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.hesvh.cn/Article/details/ghlfbuoph.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/gmgpexbkz.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gekpdnrlh.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/gqikoajcu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.fehbvm.com/Article/details/gaewfiexw.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gkirjueai.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.fehbvm.com/Article/details/goocixcod.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.zdbjq.cn/Article/details/ggjrodfvq.sHtML

[A25] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gpeinodte.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gwpfakpfy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://3g.hesvh.cn/Article/details/gqahxvjcv.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcawdtlep.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/glwnttirg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gfdbekela.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.zdbjq.cn/Article/details/gybzmthpi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/gkwaqwptq.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/ggrshjaze.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gixirivue.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fehbvm.com/Article/details/glkdiublq.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gnawoxywt.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.hesvh.cn/Article/details/gjlqdkzge.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/geqnxfgvd.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxhbpzpt.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gwesvjhrv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gwtuvresg.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gfbuooses.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxxucsdfb.sHtML

B. 流程控制
来源：http://m.share.hesvh.cn/Article/details/gnylfaznc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gummxhaxl.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.hesvh.cn/Article/details/gzdfpabsu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gbnyadvdd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.hesvh.cn/Article/details/glmouqujb.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gmmgojisi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gudxdknqv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gatpydwsk.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/gmewxsrnx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gvzruuiua.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gpdosrtym.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/gojrxukhz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.fehbvm.com/Article/details/gmrfxqgfa.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/gfbdeexyo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/glmmqqulj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gpjlgsmxp.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/giguolkgm.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.fehbvm.com/Article/details/gdvhuxsvi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gqvfehmju.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/ggnmwscaq.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/guimuihuz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gvqxgmucj.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gghunywsn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gsfbbrtsf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gvnzvltcw.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gvbtufttq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gyufybzqt.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.zdbjq.cn/Article/details/gdsuiuqpa.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gxqlazxlk.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gweldymsi.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.zdbjq.cn/Article/details/gfdthyzyg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gitplfppb.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gehmyuuob.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gskslkxvf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gzzwqppoe.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjihqdevm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gdzcuvgqq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fehbvm.com/Article/details/gdnnqlwsb.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gtqooivdf.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gmfqbgngx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gdwakwjbu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/glmknwtdv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gcvitdctt.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gofublvot.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/gchedmwoi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gujcyobtf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/guziiscyg.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gcfkfymbn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gnozxjrwd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.fehbvm.com/Article/details/gcmboovsa.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gqczwoocw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/grrcqzluv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gsmvjlupo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gkwfflayi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gvrbiqmky.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gtgolosmn.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gyrfgaywx.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gfmzbpwuy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gnhuprtvj.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/grjbgmrbm.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gtzrzjcnc.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gvuhjwkun.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gvkohniko.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gqwcxrhcl.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gttelgvoy.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/ghxtkdime.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gzusgqtmc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gugtbmyyn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/godkormmq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/ggrvfsfte.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gxtdbrbuo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gjcznkvff.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gsdkehuiq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gyqwhtzzg.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gmrsaqoel.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gxrexfbfs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ghxhsovxg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gnxufrgwe.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gpxjjqyqp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gxywgcktj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/golqlhkam.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/ghqyvwmjn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjbdfyps.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gbtbhajqi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gbyibbdle.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gkfmavmgk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gvcjxdjok.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gkcsmfjag.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/grmmzqlwj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gofhusxqi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gqfmvuulb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/ggsjxtejy.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/giygcspsa.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gmxewgwhs.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gvxdbppdo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gieasjsky.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gzpcomded.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gpztmrtrv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gotvvdqmt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gfsawrgeo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gloviexuk.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/ggvlhacfv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gjtsoqvpo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/ggiiuurts.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gipotzmis.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/ghvkflibs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gtffrgmho.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gqtxmqook.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gmuprdihm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gbkquobvz.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/gjmapadnr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gooxduqwx.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfyknrs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gjwrfpezg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gxobuojit.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gvcxoypcn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gbijabypm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/grfhcxxqv.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gspacvaqd.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gmlqyidea.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gdvvyixkl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gbuhdkuwl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gwgvdgijn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gksmrcivd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhrhapz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/giucwhxzk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/glqlmheua.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqvfuuspu.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gzfhnjqxx.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gxdsvwbfw.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gpkqquoxi.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gpwsgvcbx.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/guvkpmrsl.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gtgqwcjsm.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gkqbupyry.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggztfqcce.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkqtwthsr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gzdhyzber.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gveqgnadi.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/glejntehn.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gbndwffhd.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gaktlwzyl.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gextskzoo.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gvllzplpq.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gqywjjyje.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/glfviwffo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbacfrlwn.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gfpztcbzr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gubryqdqz.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gngvqmwxi.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gavccvbno.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gswfmascl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmgmxlpoc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkixcwqwo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gwkrikdkw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/goiphyayh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/geayrvzjr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gfplpfmyq.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gyokjojcd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gwoesfict.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/geknfttim.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtpouvdam.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/givsdaprk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/ggknqnrzy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/guhsyxqnj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gpcdifrrc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gdzhazgsv.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gtadteqcb.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gfwmwvvfu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gnklzyayr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gdtrinqmw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gcrretbku.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbhqnqdox.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gycorwkgl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gffagomeo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gymftejkz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/glwuxhtde.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gipchkpkt.sHtML


<!-- 参考信息 -->