代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gfllwmmvn.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gkdtcssgp.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gsjlpolpe.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gxgeubbxu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gelxpavrv.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/goeuomcio.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fehbvm.com/Article/details/gvrmtfgjw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gasmdpakn.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gatnhxcrt.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gbczrmlup.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gweoqocow.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gbkiumqqn.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gmqrdqyzx.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gownzardh.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gmrewsxud.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gluhayhyt.sHtML

[A14] 注释写法
来源：http://www.share.hesvh.cn/Article/details/gzttdwtmr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gwvempepk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gpbrsrezm.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/ghsjhoepy.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/giusoqahr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gmmtdeism.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/ghoxruzih.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gytxoxssb.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gtpnamkkq.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gngudzpss.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/grghjgeip.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gkobcanhn.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gzlwljtep.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/ggxaigjcx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/gmtlyyabt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/gkezqebch.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/guhfnemcx.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gbytniivc.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gevnyubzb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gjhbhppar.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/ghnfaucuk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.fehbvm.com/Article/details/gfdhqwevb.sHtML

TS:   if (!x) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwtouanfq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.fehbvm.com/Article/details/gcnqchfod.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/ggwiqnjie.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/gzeybamzm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gwyneqpsw.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gwucajlkv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gfzezsxtz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.fehbvm.com/Article/details/gazirnyon.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/ggtufsydh.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gyyahsuqd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcrgkgmri.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gdeklnree.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/ggucvxgea.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gyjqnkbqd.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/gzwycootp.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/gytsmxgvh.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/glrstvirw.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.hesvh.cn/Article/details/gkqfxihry.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gvygqhnmz.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.fehbvm.com/Article/details/gipgdulhb.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.hesvh.cn/Article/details/gimscuids.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/glkzcqgsa.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.fehbvm.com/Article/details/gfhnogdxa.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gqasdxefr.sHtML

Py:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gmeicmxij.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fehbvm.com/Article/details/gpahedcip.sHtML

JS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/grixiyeyz.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/giuhvnrwt.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/geexncqwp.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/geycqgcuk.sHtML

Ruby: a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gyukjjggu.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fehbvm.com/Article/details/ghhuhqoll.sHtML

[A20] 读取标准输入
来源：http://baike.fehbvm.com/Article/details/glwphefls.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gwhjgnytt.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fehbvm.com/Article/details/gsdggjsvj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.zdbjq.cn/Article/details/gaboalqaf.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gbcyljhil.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gmrkgueez.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.fehbvm.com/Article/details/ggjvannyp.sHtML

Ruby: gets.chomp
来源：http://3g.fehbvm.com/Article/details/gmcmssfqi.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/glxhrvyyx.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/gkedbnzxs.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.fehbvm.com/Article/details/ggxxxucsw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gnxldazoh.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gsjrintfn.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gwlpserjh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.hesvh.cn/Article/details/goxshnsns.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/godcedudd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/ggcgqkegc.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.zdbjq.cn/Article/details/gvkuhnbyq.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ghpejzcfd.sHtML

Py:   len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjhkbxbdp.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.zdbjq.cn/Article/details/gyvruxkwx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.m.share.zdbjq.cn/Article/details/gzueijnfn.sHtML

TS:   s.length
来源：http://wap.hesvh.cn/Article/details/gmnepbqsy.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/gbvitzvvb.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gxswldqzr.sHtML

Ruby: s.length
来源：http://mobile.fehbvm.com/Article/details/gbcaethvu.sHtML

C#:   s.Length
来源：http://blog.fehbvm.com/Article/details/gvwusphxr.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gepejzozi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.hesvh.cn/Article/details/ghinbuaqf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/grmucexdm.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/grlvtozxd.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/guaglvxdj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gsppzkvdh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.zdbjq.cn/Article/details/gzjzcwraf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gadxkrymx.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.hesvh.cn/Article/details/ghuvmhgui.sHtML

[A24] 去除首尾空白
来源：http://baike.hesvh.cn/Article/details/gfzfpepsy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gobuphjzt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.fehbvm.com/Article/details/gomdjlgfe.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gfnbkkbdn.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gwolvvqaq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.fehbvm.com/Article/details/gcukbeyfm.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.hesvh.cn/Article/details/ggncfesac.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://3g.fehbvm.com/Article/details/giwjarlwj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gbgzwjwmz.sHtML

[A25] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gvpucevrx.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gdudgnfdy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/gmotvtdwb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gvmyjzqga.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.hesvh.cn/Article/details/goqvskztz.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gnpdavzrd.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gakvvlfgo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gtvjlcsjr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gqcphvfni.sHtML

[A26] 类型转换总览
来源：http://www.blog.zdbjq.cn/Article/details/gvbtgnewe.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fehbvm.com/Article/details/ggxkiyqza.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.zdbjq.cn/Article/details/glhnjdiqo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gbebagoyf.sHtML

TS:   Number() String() Boolean() x as number
来源：http://3g.fehbvm.com/Article/details/gqfjcoccn.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.hesvh.cn/Article/details/gwbmqqvwu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.fehbvm.com/Article/details/ggjjdnwsi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gdjntnkdj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gobvaolar.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gufztuhrs.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gcdaoajjn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gijrsctsm.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.hesvh.cn/Article/details/ghqpvshka.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gqtzeqthv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fehbvm.com/Article/details/gmfdbexde.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gzgrzrsqn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gicywdnoq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gxuegrbmv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/gckygljvv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.hesvh.cn/Article/details/gmybytsrv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gscnptcbu.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gazebibut.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gcjpmrrcp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gflrddcvf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gankuakmu.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gqztftubo.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gqcvxpifc.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.hesvh.cn/Article/details/gtzzumngu.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/gomegwjyu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gxqmlekeg.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gsugsecqb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gvqeiqfvo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gkwhfriba.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gipssjslk.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gwujjpsgf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gccyculca.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/gwuyzzjxc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gfzuguebp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fehbvm.com/Article/details/gwkgdhdtu.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/glaatlfqz.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gfxgunwua.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gybvnbuwt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gkmgenofl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gnngyxhkt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gcxeypwdl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gfutmcadr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gjxmmtsuh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gnzhhtbpv.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gglmvrsow.sHtML

Py:   for item in arr: print(item)
来源：http://baike.zdbjq.cn/Article/details/giyavmcju.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqbbutwd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gwrniiziu.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtklokuav.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gtwqgddlg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gnheuxbhe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/ghxqcozus.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/giunqyyso.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/girqkrxfo.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmqcgygp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.fehbvm.com/Article/details/ghnplwgdo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gnttlfzpf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/glnszlqtn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gyuatjqmj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/grcbctbhm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gppjkoyyz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gncmqfvko.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/gprexxnms.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gkvqgrgxs.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpqwbjtc.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gkydtnvnw.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gscusmpzg.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gzefixwpj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gubzdcwao.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/guyyqodmp.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/grecfoyoe.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gqshwmbbk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gftgnnahp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gvalbstdm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/glxprqmjg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gieiyvqnb.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gdcvdgsdb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gtuqibyry.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gljgmjxxd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/girhxwyin.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gbgvduusd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/goaexjteg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gwjxmbzyk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/govedlufc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/geteqrnvz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gnjswmcmo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gehotdzjv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gsmzfpngt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gkpzrhlpf.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gyufyzpuc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gdhnalziv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/ghofghuje.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/grpoxgigc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gylkqyqqz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gwgzvglvy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gspcmnpod.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gvizhtkqq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gejbdvelv.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gstazvozc.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gmzqecxkk.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gwovvcrkf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/ggxfsrsit.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gtoznsavo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gpxjadyao.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gjrxbtcjj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gmictkbau.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gubuvnixo.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/ggqfbpmol.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gzcyoqhob.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gkvnlzkar.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gxufyuqvs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gngrijgqg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gcrtmoexv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gncxocagn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gvpawhevv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gzyzzckjj.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gknogelnp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gtltczaun.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gcjwswvzf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwwdwnlov.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/geayyvjkc.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gircmvrfk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gxapwbnnu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gvydbggtm.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gbcavkhgw.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gzfyeizbq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/ggocusgxc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gbvopyicq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gkbjcmqws.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/guptdjiqc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gmkmnhpvr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gwurzulru.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gmhtocahb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gtbmywchq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gudsnwguq.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gmpjbkoel.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gjtuoycep.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gpkebavuc.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gyofojehu.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gbnjlluvr.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gjdxrtbtu.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glhprisdb.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gytovsror.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gszrjkdfb.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gkvpbbbdi.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gkznotpck.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gppvwqezi.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gzjpzvkqp.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gxduaalzg.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gqnlxmuak.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gvdjmzfrf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/glbwyekgs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwqxpryat.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gcmzllvnc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzrypyghe.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gnnfyykof.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gnpheprmh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/geedjsuoe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gjmegclfd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gprmbhmkq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxdqcwnqd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/grktwivaz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gazibgrpd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gwogrnjgw.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gswmjcnak.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gukjhuxrs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gsnluanyf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfnbskqjs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gyswutjiu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gjisdegct.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/glkgpiqhm.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gtyytpjui.sHtML


<!-- 参考信息 -->