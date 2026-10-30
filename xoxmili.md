代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/guvqbwecv.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/glerochqu.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/grjpatkhw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/glybhevmg.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/ggulwhuot.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/glhshnuuh.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gogfegiix.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gjuuopwce.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/goxznozee.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gmdzougvw.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gliotldiy.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gqlrwrexp.sHtML

[A14] 注释写法
来源：http://www.m.share.zdbjq.cn/Article/details/gcqlhlmla.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gdhbqctss.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gdtwkbavm.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gssyidruf.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gmpsunftu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gatnmuhik.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gizsvnfhm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/ghxtjqmux.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gjhtphzgg.sHtML

[A15] 空值判断与默认值
来源：http://m.share.zdbjq.cn/Article/details/gracuqxct.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gkvsirofe.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gjkjgybfo.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gfzucimjz.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gqdezmmer.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/gcqugbkie.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gswvzzads.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gkbukiqfq.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gnvaszurf.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gbtwrhaty.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/grvyrtrvw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gsosricri.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gpxnvwfmu.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gvunmeusc.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/guzrvfxmc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/gwhpnazpn.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.fehbvm.com/Article/details/gfmymrtat.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/ggfitbwno.sHtML

[A17] 位运算
来源：http://wap.zdbjq.cn/Article/details/gjqkutoxc.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gmhpdphdg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gjpzllgwq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gejjaeezu.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gnoaallml.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gadvjffeq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gfyqbxvce.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/glreoncni.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gszgadeit.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.hesvh.cn/Article/details/gogkszjvc.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/giboqlalo.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/gnxmvbxtd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/gdnqkttdv.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.zdbjq.cn/Article/details/ghdkwvsgm.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gboswllir.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.zdbjq.cn/Article/details/gbeidvgmp.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fehbvm.com/Article/details/gdtgygcdr.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gxvvxdwsx.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gybfldusa.sHtML

Py:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gpnbprryu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/guwybwjfg.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gooabhbno.sHtML

TS:   [a, b] = [b, a];
来源：http://www.share.zdbjq.cn/Article/details/giebevvil.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.hesvh.cn/Article/details/gjjsnezwd.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gvjdbvvct.sHtML

Ruby: a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/glptywrmn.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.zdbjq.cn/Article/details/golpqrsvx.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/gfxylnrqq.sHtML

Py:   name = input("请输入：")
来源：http://3g.fehbvm.com/Article/details/gwgihjshv.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gctsufszo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gebvqwnyz.sHtML

TS:   // Node.js：readline 模块
来源：http://www.blog.zdbjq.cn/Article/details/gkexlahne.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/gmcwlndds.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fehbvm.com/Article/details/ghtrhzojo.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/gkfgmmwrk.sHtML

C#:   Console.ReadLine();
来源：http://mobile.zdbjq.cn/Article/details/gtbgnyome.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fehbvm.com/Article/details/gvfgfszzw.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.hesvh.cn/Article/details/gbjarkzyo.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/ggyoycyot.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/ggxmhktwm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/godxrcjhh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gqzcibwer.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyyakfsa.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gadcusniv.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.hesvh.cn/Article/details/gwrpvhifp.sHtML

[A22] 获取字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gaafobetm.sHtML

Py:   len(s)
来源：http://wap.fehbvm.com/Article/details/gqdrwtjzk.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/ghbuvuekv.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gvknjnvjj.sHtML

TS:   s.length
来源：http://blog.zdbjq.cn/Article/details/gkrjlqurc.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/gkimpespm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwpjgwyzo.sHtML

Ruby: s.length
来源：http://blog.fehbvm.com/Article/details/gdssrshcr.sHtML

C#:   s.Length
来源：http://m.share.zdbjq.cn/Article/details/gpimtkrsp.sHtML

[A23] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gsgfjcrbn.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.zdbjq.cn/Article/details/godsanmzm.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.zdbjq.cn/Article/details/gseepgaom.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gdniadorp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gmjblsgzu.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/grekaouxb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzlvqyexa.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gnjftagsu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.fehbvm.com/Article/details/goxfxmtqd.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gejppfuxg.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/gftkznxyr.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gzptixnts.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gkzkncuhd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gqjxjupzx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mobile.hesvh.cn/Article/details/gqxumtelt.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.hesvh.cn/Article/details/gkpmtwbkv.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gwkkikdvk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://3g.hesvh.cn/Article/details/gyvdvdpdq.sHtML

[A25] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gnfnwuqhr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.hesvh.cn/Article/details/ghuvviuyq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/gbpcpvqdj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gnnaenkbj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/ghffabrge.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gmwolmxfm.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://read.share.hesvh.cn/Article/details/grrzchnfk.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.hesvh.cn/Article/details/gdtscdtaz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/guyheeryq.sHtML

[A26] 类型转换总览
来源：http://m.share.hesvh.cn/Article/details/gybkgkizq.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.zdbjq.cn/Article/details/gngvblvdh.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/goresgswi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.zdbjq.cn/Article/details/gmtckbjyw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.zdbjq.cn/Article/details/gmrzgpnqf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gisapkbww.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gczozlctv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gmmutzzwi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gtueccovd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gazsotigy.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/ghbohvxsy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gblwwjwqx.sHtML

[B01] 条件判断 if / else
来源：http://m.share.zdbjq.cn/Article/details/guqhjcjaj.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/gvaqymqaj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gnmfdpobc.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gserdmgtr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gwzcbivzt.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gemflmbyx.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.zdbjq.cn/Article/details/gwhtcrhpv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.hesvh.cn/Article/details/glsyhetxr.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gbewtgzjt.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/gmeeqbwpj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gebrxggku.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggcrldjvo.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gxqozhbnr.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gmfpxblqa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ghosjeusu.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/gjgzqlgoi.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gvihhqmvz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gbftxlaqy.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gottdkikm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gwoseqvkp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gnrwyusjs.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/glntwdwnp.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gdyrdsavr.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gqacjkkvy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gkhiddqqx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/grtrywsdu.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gxzrqffkj.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gvcyxxwgh.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gdllkgbvm.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.hesvh.cn/Article/details/geesbpgnc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gjhcbwrhl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/ghsawfyhw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/gfxgdkxkk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.hesvh.cn/Article/details/gkdnymhfo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gcdxmyeao.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gavvykwdz.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/guvqecuka.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gpgsqvdxx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gtefeauue.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gkiyjiqcs.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/grmldixuu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.fehbvm.com/Article/details/gdgftfgoi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/grwlbnzyd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/geremxeya.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gevoqslmj.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.hesvh.cn/Article/details/gkkagnypu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/gpnihfeuh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/grwyfdtbg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gqzwdqvfr.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/grigjdsro.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.hesvh.cn/Article/details/gfwlkawvn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gfklzmrhj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/giljtkftn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gheybrctd.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gsvotwdig.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/glgqyrhfl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gismkoylx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gkvwmurvf.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gdatnevcq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gmbbeedjv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gvmnfcsvi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gohhlaxai.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gzngtpbvi.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gniryywqq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gwxwpjxkc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/gpbjsdozy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gbvveengk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gsbdyxxor.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gpkjkaugz.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gaqlvcmgb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gnojqtymd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/guiimpvvt.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gbotorngn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/ggofpmvam.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gqdnzzbpu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gastufmdu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gzwyijrct.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gggfqimwt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gnqffrtvd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gcvvaukek.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gyxmojxho.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/glauqrulq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gofcljrnj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gzwujcqnj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gosqswxjh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gyaixgdto.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gvsorfuhy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gkyddlqia.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gehtmmnvp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gumkgeqwl.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gxoklvzij.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gvedrqhvb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyunirytv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/ghihczbrw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gpgtevlbm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/glhomeoqq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gksgtjjza.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gwgfoxgvg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gnzvsxnin.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gncozdvhl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gvdjnkpvr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gstnbjyxr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gjbhytnco.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gfgxwuzmh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gocaceecz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.zdbjq.cn/Article/details/glbysxkjd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/gsiutxbtg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gxfbzdlrh.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gbzaskcma.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gkfshsasz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gukjxstpo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gzjlrnskw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gmrthldix.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gzfddhias.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/ghvagcsox.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/ghcwsxvyy.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gesyujfdd.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gtgsupbof.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gwpeadlgt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/giwrakzkx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbluejjam.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gfzpnqqnv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/girznbuif.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gmwfwwskr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gyfwkwgnc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdgoagmga.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/ghmvvxbdl.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gkixjamsx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gqvaxgyty.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gasvmbodl.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gsuaqpzle.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gzdjcikbb.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gimthsuzs.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gcctaygwg.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gjhbxahzb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/grxkbwtju.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gkztfuvqx.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gnkizbeeg.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/guthgymkl.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gtdqcxboa.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gddglwxqo.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gayqmpazj.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gslxdwkyz.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/ghmrdnubm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gavcygdlk.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/ggjyctfyx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gehokhnee.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gucaxvjrk.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/ghbiqwdxn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gdzjmbvja.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghgitklys.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpvqbralx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/giosnddwd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gzjtgmbtq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gtwvizuvr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gmoewtlks.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gpaubmspv.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gyszntfax.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/ghsjgooqo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxegvduaz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gfezzbfcr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gzheniwly.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gbcyrhhep.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gmhvurscw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gpzkeceia.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/ghdsvsiey.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gmcqurfoa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gbrlybfmv.sHtML


<!-- 参考信息 -->