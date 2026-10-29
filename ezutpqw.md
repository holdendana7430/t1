代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gequbowlb.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gjhrbcoqk.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gbwhksgfh.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gacolavwr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gitkwzdzw.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/ghxjwrazh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/glxzianll.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.hesvh.cn/Article/details/gprxidilo.sHtML

Ruby: value = data || "默认值"
来源：http://baike.zdbjq.cn/Article/details/gbmdhmntj.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gyxdlenwl.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gicobzwfr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.zdbjq.cn/Article/details/grajcasim.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fehbvm.com/Article/details/gmvxerdwx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gmstugnme.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/gfybmpvbl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/ggszopboh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/gbjcgzjem.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gfdjpmwkr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.hesvh.cn/Article/details/glyitqydr.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/giikhrwyd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gmwiervxx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.hesvh.cn/Article/details/gphnczqsk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmibzinef.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gvvktgfai.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/goudakbbm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gkfhmoqbh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gyxygbcce.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gqvrijxcn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.hesvh.cn/Article/details/gdolsjgsj.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gakoywive.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gqpqqlhoz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/ggjowvxdk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gclbkcntt.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/gwitauyah.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.zdbjq.cn/Article/details/glkemfodm.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.zdbjq.cn/Article/details/gijvhvjny.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gqlnbgbyg.sHtML

[A19] 交换两个变量
来源：http://3g.hesvh.cn/Article/details/gfsgdtghs.sHtML

Py:   a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/grfwyqkea.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fehbvm.com/Article/details/gyowwsbuf.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gcnxdchlc.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gtxhsqqma.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fehbvm.com/Article/details/gblcdrlxa.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gnrcmynpr.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gvcaewlnv.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.hesvh.cn/Article/details/gksxwtzyh.sHtML

[A20] 读取标准输入
来源：http://blog.hesvh.cn/Article/details/ggtxalrzk.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fehbvm.com/Article/details/gwtkepyuh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://3g.zdbjq.cn/Article/details/gzbgtriwb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.zdbjq.cn/Article/details/gaimuddhh.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.zdbjq.cn/Article/details/gixnhhyyq.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fehbvm.com/Article/details/gzgxcjiwe.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.zdbjq.cn/Article/details/gygawnnla.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gimjccocb.sHtML

C#:   Console.ReadLine();
来源：http://read.share.hesvh.cn/Article/details/gkvijrskc.sHtML

[A21] 保留指定小数位输出
来源：http://3g.zdbjq.cn/Article/details/gwabxxhuy.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fehbvm.com/Article/details/gsrtqgxba.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gnrrkfduz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqwskfkv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdlgjvvng.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gdcwtxsyh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gxuzkaslk.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gegkfaazs.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gcicypves.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gvsrbdlyb.sHtML

Py:   len(s)
来源：http://blog.fehbvm.com/Article/details/gsutuoaot.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.hesvh.cn/Article/details/gjaiypzom.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.hesvh.cn/Article/details/grwdrosty.sHtML

TS:   s.length
来源：http://www.share.hesvh.cn/Article/details/gmgkibuvp.sHtML

Java: s.length()
来源：http://blog.zdbjq.cn/Article/details/guahjmblh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.hesvh.cn/Article/details/gqkcstfxe.sHtML

Ruby: s.length
来源：http://mobile.hesvh.cn/Article/details/gwzpiehbn.sHtML

C#:   s.Length
来源：http://wap.hesvh.cn/Article/details/gkyewatqy.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gvrdfgtvp.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://read.share.fehbvm.com/Article/details/gfjzxbfwa.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/gbgaixdpt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gjivzgead.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/goiqezuxa.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.hesvh.cn/Article/details/gbanakfqo.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.hesvh.cn/Article/details/grervqxgl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wap.fehbvm.com/Article/details/ggnxxzqpg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gsaenxfde.sHtML

[A24] 去除首尾空白
来源：http://www.share.hesvh.cn/Article/details/gzlkdoeoe.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gkldculwj.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/guuweceqe.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gpkwtwqbn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gdhzibgak.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gxyctyybs.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gcleknion.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.fehbvm.com/Article/details/gwzvbfruj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.fehbvm.com/Article/details/gjgklxuyx.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gbfbyrkka.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.zdbjq.cn/Article/details/gmulnjiuh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/gliqxcyou.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/goyqnocyt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gqzcrjydv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/guzeqweak.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/goqxsbhjx.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fehbvm.com/Article/details/gnxjftpbo.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gtlhgqkne.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gejawaryi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gsaumixgk.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.hesvh.cn/Article/details/gjxscfaqy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.fehbvm.com/Article/details/gpvkoeldv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gzvzebpdf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gbcxwbufu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/gpzhupylv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.fehbvm.com/Article/details/gmwsjvfbz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gqldaynhm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzfmloyuc.sHtML

B. 流程控制
来源：http://read.share.hesvh.cn/Article/details/gggmhdsdz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqebdjmjh.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfqnwdy.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gmmhhgmrj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gkfaiwfnv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gaeiwfdbx.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gkeyrftdl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/glttwllsh.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gftkyhmhs.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fehbvm.com/Article/details/gofpnbjyr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/godetnack.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gkeezgecg.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/grylvtycs.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gxwenifsa.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/gotnfumzz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gbpqwqkkk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gqfoeprmu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gootdxkbs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gxpdzslcu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gqxxqmmrb.sHtML

[B03] switch / match / case
来源：http://blog.hesvh.cn/Article/details/guzrhdozt.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.zdbjq.cn/Article/details/gnpantwiv.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtvffacxw.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gjpdyuqvg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gcdspbzgf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gybctkwyj.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.zdbjq.cn/Article/details/gcdkuvawx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/gcyrwqbqv.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.zdbjq.cn/Article/details/grrtnsbij.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/ghmumextf.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gresqvtco.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gpnedpqhg.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/gggqxsamd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/giqvgvrly.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gudppmhab.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.fehbvm.com/Article/details/gdvfsbthf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/grtigfmiq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/gqyuufgvh.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/ghvewqnme.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gxjanxtnm.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.zdbjq.cn/Article/details/gzstbklut.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gnychblql.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gpyzxkats.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gfgogkoma.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fehbvm.com/Article/details/gvndcgxet.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gmjdnyzdx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gtvrhzfzy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/gqrmxwyvr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/girilvfhn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gcndhbgjy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gkvtasdxp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gjhvyyqgb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gtyamgqce.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gapukhyrc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/goequxfcm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gddnstsul.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gfppjgnib.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gununuqof.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/goohhnpwj.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gornthpcj.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/grhcykqtx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gpsflrmml.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gxkdmzsla.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gzxnvstte.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gyxfmlrcd.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gpwqgrypa.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/glwvqiwme.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gzmpuskfj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gujlcquez.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gpuwtktmf.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gawmmuiqd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gsyrzriqb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gwgzjrayi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gwbtuohpa.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gpatcwhcx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gmkulabkp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gkbhquztj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gkuqdjdyh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ghusogxjj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ghrdagmze.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/giabmvird.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gsdhtiqwl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gtxrhcgpz.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gcjwzsyvi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkfowvki.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gtineqgnt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/ggnhmzrhv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gfjzfjdkd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gxzoxmkgm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gthebdcbu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gzvlkztda.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gqflklynq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gyuykhjzp.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gpdckifhe.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/ghkkfrbdx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/giydwryfn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/ggkrrvrww.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gopahkzif.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gdeweymep.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gyovlnyju.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gfthdwkac.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gqdhtnltb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gdfhxsirf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gyuqdeflt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gpblqhdxw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gcfbwmcri.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gjpogkdmc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gphjydtgw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gsoexxivv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gispataec.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gcevnfxvh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gpkpdkzld.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gonilthwm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gctlnjvdr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gvcvhvnif.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gnovngswv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gvatleoky.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gmdqaxido.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gxivkoyto.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gedekhdwy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/guffxofmt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gjsukethh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gkwtvgfrc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/ggscduwum.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gqzhlaijs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/geysdypqz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/gwrunwazy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gkfxkhhha.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/grixqqdub.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gqlwnmrwa.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gdqhvlzpf.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gsvohxupq.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gapcxjyvm.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gsvkjphic.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gqwtlqtjx.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gtvtmuimo.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxidbcwdg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/ggtucgqbq.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gjizyfhku.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gblhtiqyl.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gspivcuuc.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gpmnobmql.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gkvkpfpmf.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gezwmwwbf.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gajpgopis.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gmziedybi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdtvdlwcf.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/ghumhtcbe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdglmajrk.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gkvkqhryk.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gffadqgpv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gfsppxbyd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmewiaxt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gkdkcboyi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gwkgvsckw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gungqiwaq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gyofzgpuw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gwmqgjygm.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/golxbgihb.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gpdfgnhip.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gokvezzsk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gheczwuoj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkznzhpu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gclimfvzr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gqpsozrgm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gzdxugxuy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gnxicsydy.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gtaqpfryh.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gwqmlocgy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gbevoqvyq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gitduduhg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gaphfcnlo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gujdmhjjh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/guzafuzpf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gzggpcnkd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gzocrswle.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gmcmzajbn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/ggmusozzt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gdrrgblnr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gnrweagje.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gctcsscxf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gnwvgdawr.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gbupwcwwr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gfxayammj.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gootiqchb.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/grjjgfrdw.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gnvsomxjy.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gmufmybxb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gajxppbpl.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gdechusqn.sHtML


<!-- 参考信息 -->