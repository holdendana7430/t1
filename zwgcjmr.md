代发 wailian999

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqrxglak.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fanxiaobao.xyz/Article/details/gygqktvni.sHtML

[A16] 真假值判断规则
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuabrchw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fanxiaobao.xyz/Article/details/gohnlrjml.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fanxiaobao.xyz/Article/details/geirtkxct.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.fanxiaobao.xyz/Article/details/gdcqruzlj.sHtML

TS:   if (!x) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gakcohacq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjupumbmv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzbkpheyv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/gnhvetkex.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/goudrjcvf.sHtML

[A17] 位运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxihmzrj.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdzxszia.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzbpdkja.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/geemoepok.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/glkxqkjns.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gewysnoix.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gxpzsontr.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjxxdquj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/goixifudu.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggugdwavp.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/grgkewzje.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxbbxspd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fanxiaobao.xyz/Article/details/gzvgmzcpm.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkchiqhtg.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.fanxiaobao.xyz/Article/details/gicrqtcnh.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.fanxiaobao.xyz/Article/details/gtbwrfipm.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fanxiaobao.xyz/Article/details/glbrgjjtd.sHtML

C#:   (int)'A'; (char)65
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwufypktt.sHtML

[A19] 交换两个变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoodfcvp.sHtML

Py:   a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnziuaxgn.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.fanxiaobao.xyz/Article/details/gbggmpmei.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbuoanav.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fanxiaobao.xyz/Article/details/gjkvnasfu.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gykgnffkl.sHtML

Go:   a, b = b, a
来源：http://m.share.fanxiaobao.xyz/Article/details/gttzhljdl.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzybzdkom.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.fanxiaobao.xyz/Article/details/gemrzvvsx.sHtML

[A20] 读取标准输入
来源：http://3g.fanxiaobao.xyz/Article/details/gcaqneafq.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikgwrvxs.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.fanxiaobao.xyz/Article/details/gcajenyzy.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fanxiaobao.xyz/Article/details/gvauuduhe.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.fanxiaobao.xyz/Article/details/gntxkvoal.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvxzcfps.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchwfepxc.sHtML

Ruby: gets.chomp
来源：http://wap.fanxiaobao.xyz/Article/details/gmperrppf.sHtML

C#:   Console.ReadLine();
来源：http://baike.fanxiaobao.xyz/Article/details/gobsksmvd.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrqpsfkj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxttiyygo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxrfvqax.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxsoacfru.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxhqqmluh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzvadqpr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gglbdzivw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggplmpvhe.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtcivkva.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gksefnuwf.sHtML

Py:   len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gegjuuvwg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fanxiaobao.xyz/Article/details/gzsqyyzdn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcbkpubg.sHtML

TS:   s.length
来源：http://wap.fanxiaobao.xyz/Article/details/ghyzbqpwd.sHtML

Java: s.length()
来源：http://3g.fanxiaobao.xyz/Article/details/gzchsphli.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwlqfxgn.sHtML

Ruby: s.length
来源：http://wap.fanxiaobao.xyz/Article/details/glgrymxnk.sHtML

C#:   s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldriskgd.sHtML

[A23] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gldlptrnc.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.fanxiaobao.xyz/Article/details/gxrewrysg.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqnszlxt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgxglbrb.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gylrrcxyn.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.fanxiaobao.xyz/Article/details/gzirempwf.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ggjvugoge.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gppdjdqnx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/gdyaprmkd.sHtML

[A24] 去除首尾空白
来源：http://m.share.fanxiaobao.xyz/Article/details/gfexrxqpz.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fanxiaobao.xyz/Article/details/gdqpgoali.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fanxiaobao.xyz/Article/details/gmcsosdoj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gogygkdjc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gujrisafn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fanxiaobao.xyz/Article/details/gdpwbjmeb.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqwamsae.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gzemkzokv.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpbdtsvh.sHtML

[A25] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbjpcusd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fanxiaobao.xyz/Article/details/gxkghzhvn.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gohgplikc.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujltehiw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvhabfut.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/genlwqaqe.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/ggjiqekhi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fanxiaobao.xyz/Article/details/gunaphkos.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqwhsdgy.sHtML

[A26] 类型转换总览
来源：http://wap.fanxiaobao.xyz/Article/details/grffnpbky.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtogefpt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fanxiaobao.xyz/Article/details/gynbotqss.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghumbldyy.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fanxiaobao.xyz/Article/details/gummjqtxj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gedfhpwhm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkkgzssn.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvdoldtu.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gpjqclabe.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqbnselcq.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gixvhheys.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvmnijand.sHtML

[B01] 条件判断 if / else
来源：http://wap.fanxiaobao.xyz/Article/details/gpmpdntry.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.fanxiaobao.xyz/Article/details/glxynbztk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtksabows.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fanxiaobao.xyz/Article/details/gbeofpvmy.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gzmetqnan.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdqloyie.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfsvymdu.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhpppbba.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzqiimyg.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fanxiaobao.xyz/Article/details/giwlvjrdr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyesmqho.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqbzeybsd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/glchkijva.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gcqrklwzz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gyqplrkev.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fanxiaobao.xyz/Article/details/geglcieno.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fanxiaobao.xyz/Article/details/gdrvvhgga.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fanxiaobao.xyz/Article/details/gppvjxwho.sHtML

[B03] switch / match / case
来源：http://www.share.fanxiaobao.xyz/Article/details/ggavxhsmm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gskemvpme.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcrbisyss.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmejkikms.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glruolneo.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzedeuosd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fanxiaobao.xyz/Article/details/gwxgslony.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqkzbkxj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgncudqk.sHtML

[B04] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gexknpctr.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gpumvkcjb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvilvids.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtveoyima.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnnijcfo.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzunqhyzf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevfzooqu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.fanxiaobao.xyz/Article/details/gmudxcuhz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/goptmafnh.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkhencpf.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkotowotg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkikyhwhz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnbpmvtft.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkjardpi.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfbshfae.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfefxuto.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmneorsmb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfuikaqv.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/glvxfwhqj.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fanxiaobao.xyz/Article/details/gtciyjtpu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gefbrzvmw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvjfjuax.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqcuygil.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnoirvmbo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngtvhiug.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwadjxqax.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgpacihp.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjskrjkxn.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhatllkv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtrmwdgcc.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmcqkkchw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkvwqwvt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbwpxnlb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gobskbuqn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrcloeno.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtemoqrqf.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fanxiaobao.xyz/Article/details/gmhimcyge.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkqtvkaq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/ggrbguzjm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gmqwhjduq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gafcjwagh.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gqbskxrjv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gpbdyzxup.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/gaeglkkrz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gllfcvsbf.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxhzkzer.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfirewooy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsqhiqyn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqytbzph.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grlqttfax.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpoftchs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcejzlzqo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fanxiaobao.xyz/Article/details/gdjgwbqlv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnfdtpvo.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fanxiaobao.xyz/Article/details/gpuemwyvx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/glkiawjro.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsqtajps.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gmcwwoawp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gccctmtfo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrgzjhhs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/gzbpqypbl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gftkkucza.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/grkomjwsz.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fanxiaobao.xyz/Article/details/gzmptipqh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fanxiaobao.xyz/Article/details/gdzqwuofx.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/grvpinxoo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmphfohe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhakteaz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gfyqdnutl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmooxrsr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gbldxhacz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxupwjvx.sHtML

[B12] 跳出多层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvubaiwok.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnsigeoa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxawzkoe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbleukol.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gndzpeksn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcyrfooj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fanxiaobao.xyz/Article/details/gerxohhyi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupibsaht.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkkfdnvx.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gulaougbm.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxhaxjyi.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/ggdbvjfua.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcfuyoee.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjkfvfyi.sHtML

Java: x instanceof Number
来源：http://blog.fanxiaobao.xyz/Article/details/gqslcfhjb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghladlatt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/ghicjcaka.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtlyqhmv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gufmyvjlc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fanxiaobao.xyz/Article/details/gwdntinam.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/gfuizavsl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbuobptk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgtvgxhl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmoclrat.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqikbabq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/glsymoekt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzsrgrri.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/ggxwjxswh.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqepoqx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fanxiaobao.xyz/Article/details/gdsbupxqd.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/glbvnebwk.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gugeybaxg.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gtyybnrmp.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazasoopv.sHtML

Ruby: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwkjvehl.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqkswabx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gtksydypd.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvxpiadj.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtelsxjgy.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/goemkotin.sHtML

TS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/guzothymt.sHtML

Java: if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/ggyreovzl.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaixyhxo.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fanxiaobao.xyz/Article/details/glevnxywt.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gibdnzggu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpdpwaxgs.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/ggeewsvxg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrycnufw.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpokyilcf.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gudtpnqod.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gchtvrssf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbplvrzyd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyltuvav.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhpcycas.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaouxjpf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gkfhourba.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvngqgki.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/grjhebtdk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxseuigd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gszekcnyy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwvmllwi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdmzwses.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/gnojmjide.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgrceoza.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/goatzuush.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/gbasqzzgm.sHtML

[C03] 可变参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gopsthycp.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fanxiaobao.xyz/Article/details/glbrolkwo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjlcbwxc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gadzvdpkl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmvwxhtl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gizhidpso.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gdhejwlui.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/gcjtcrsxk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gaevdanxz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkfuyqpe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaiorgrp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gauoxwhcm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gboqidgbr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gxnzrfubu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/ghokjyzwd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimlvdjcu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucpmdxjs.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gamygeinv.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdzyivaf.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwakaieqe.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldryudat.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gcatcvetx.sHtML

TS:   return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gadgcgemg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fanxiaobao.xyz/Article/details/gwcwgulxt.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzhcwybq.sHtML

Ruby: return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gzluiziku.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fanxiaobao.xyz/Article/details/gernyfpdy.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkjebwvg.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/gammcqsou.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gscalgatj.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/ghsgvkvfs.sHtML


<!-- 参考信息 -->