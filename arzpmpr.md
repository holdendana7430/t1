代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gezezyfvj.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fehbvm.com/Article/details/gqdjkqzdw.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/gsvaaraxy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/govdulfqj.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gwplddjiy.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gxfkqozxo.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gkklcwfoh.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gztjdffvz.sHtML

Java: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gzgypdlqh.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gvrharfyr.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gyrhieols.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gytynjtaf.sHtML

[A14] 注释写法
来源：http://www.m.share.zdbjq.cn/Article/details/ggveylihf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gevcrfrqq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/glbtobrdb.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/glvdyfjoo.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gpdixlcoh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gudjxpqsr.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gompocaap.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gplxjfakd.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gbxijrysp.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fehbvm.com/Article/details/gsuqzxmqb.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/gwhrrduvn.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/guqxhkwpg.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/guectgtyr.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/ghliavien.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.zdbjq.cn/Article/details/gwfyrmnvt.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gqgnozlea.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/giuudyppr.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gursrdidr.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gwucueqii.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fehbvm.com/Article/details/gerurqgjf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.hesvh.cn/Article/details/ggvdimixu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gmxylljan.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gqkprncoo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gmzspxbfd.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/goneeocee.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gcrwvaats.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.zdbjq.cn/Article/details/gmvxqdsge.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gfisiymob.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gkkicfqww.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.hesvh.cn/Article/details/giptvfrjw.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/ghlmebnon.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gmrmdgcuc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gacvpvihn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gyfnpaxrn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gplbdpapo.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gotpjdmrc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.hesvh.cn/Article/details/gkvvyrurk.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gekdghduj.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fehbvm.com/Article/details/ghlirydgt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.m.share.fehbvm.com/Article/details/gjbtkmiet.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.zdbjq.cn/Article/details/gotfvdmei.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.zdbjq.cn/Article/details/geqsmqdpp.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/gifxtwobs.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/giqnakllm.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/guunratpn.sHtML

[A19] 交换两个变量
来源：http://wap.hesvh.cn/Article/details/gkseptsdu.sHtML

Py:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/glriipwih.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/gmbxueqky.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gidaryies.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/grtqslrcl.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.zdbjq.cn/Article/details/gigaafkui.sHtML

Go:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gflzquzav.sHtML

Ruby: a, b = b, a
来源：http://www.share.hesvh.cn/Article/details/gomydseiq.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gbwmyluub.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/ggogaxrfu.sHtML

Py:   name = input("请输入：")
来源：http://www.m.share.fehbvm.com/Article/details/gjifdeido.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gyjtvypay.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.hesvh.cn/Article/details/gegfylfih.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gmoomgrob.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/gamtczqat.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/giytctbdh.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/ghpfdosmc.sHtML

C#:   Console.ReadLine();
来源：http://wap.zdbjq.cn/Article/details/ghkabomrw.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gdlgrfiiq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.zdbjq.cn/Article/details/gdeaesfcw.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gneegcoih.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gfendrflg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/guptyzhxb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gcewnvfzj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gnipqmayq.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/grlgftfpp.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gewnunvhe.sHtML

[A22] 获取字符串长度
来源：http://www.share.fehbvm.com/Article/details/gbvonkvjl.sHtML

Py:   len(s)
来源：http://blog.hesvh.cn/Article/details/grhsbbtbi.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.zdbjq.cn/Article/details/gqhmbgtdc.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.hesvh.cn/Article/details/gyprgkhxc.sHtML

TS:   s.length
来源：http://mobile.fehbvm.com/Article/details/gsddhpfab.sHtML

Java: s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gfwhynviv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/gdyhniayn.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/goigzcjbs.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gtwivlbmy.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/ghpwvjwav.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fehbvm.com/Article/details/gfcopdgfe.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.hesvh.cn/Article/details/gxfeeqxpa.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gwwnthrel.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gektfmmqb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gtblnllez.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.zdbjq.cn/Article/details/giqvopnjh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.fehbvm.com/Article/details/gaaflijvg.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.hesvh.cn/Article/details/gauzwexqc.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gvtiveqid.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.zdbjq.cn/Article/details/gmnobqdde.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gvcicrstx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gbcgmllrx.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gbqeszmdf.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.zdbjq.cn/Article/details/gpketjytl.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gjkagxkxd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.hesvh.cn/Article/details/gtexmzjol.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gekwfemyb.sHtML

[A25] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gbsfshcqt.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gxgfmhapd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/gmsifxmyr.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gwrblvzyj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/gvczfkaxd.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gfpeqwwiz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gsiarxoyz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.fehbvm.com/Article/details/gvslfvtwu.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gmduuzehg.sHtML

[A26] 类型转换总览
来源：http://read.share.zdbjq.cn/Article/details/gbainrwph.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fehbvm.com/Article/details/gaztixzsi.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/ggrbnvehc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gfgimzbks.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/gkhvccwfm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fehbvm.com/Article/details/gpsgfnzuv.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gvhujuykx.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/ghkipihvj.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gvqwqplfk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggsfepllq.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gongrtdvc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbvvkfdju.sHtML

[B01] 条件判断 if / else
来源：http://blog.zdbjq.cn/Article/details/gcdtjucru.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gqfqqvpra.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/gazwaqswa.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gwmsfqvqe.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gtamrgurq.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gzrsvkgnj.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/gvqndgptx.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fehbvm.com/Article/details/gscjqpusx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gbvbnjyjn.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gbeipqzpf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mobile.fehbvm.com/Article/details/gqiykizwv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.fehbvm.com/Article/details/gpwkugear.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gvgacexuk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gidurhguq.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gqztwiabb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.zdbjq.cn/Article/details/gcbnfhocm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.fehbvm.com/Article/details/gzdcnqhpk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/giybdsanu.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gakmncrrw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gnybcbubc.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gjhjilpsq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/ghfqbmdwf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggqbezaeh.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gjvjqkbee.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/givbwzmrh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.hesvh.cn/Article/details/guuisegjp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gbycdcuxb.sHtML

[B04] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gfwjvzycl.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.fehbvm.com/Article/details/grrgpscqx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.hesvh.cn/Article/details/gvzhbapce.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gvyaurgeq.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gczfoazuy.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gsvdwuuot.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/ggoknfpbj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gguphxmop.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.fehbvm.com/Article/details/ggtutjepa.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gsuijslxa.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gnoydpgsx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gfrbjvgai.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gmncmldxc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gqisawlci.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/getpvnphz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/glqkjdhnk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gjnsipbuj.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gowkfwcuy.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gfooisjgm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gyxqaftxa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqezcobn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.hesvh.cn/Article/details/ghcprmxbu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gmxwdwupy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gwbafbiyo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gurtatcxy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gsjycoupa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/ggbeaghih.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/ghjszvlnh.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gezlabspf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gbgagngyl.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gfwiggvcy.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gnjbkkggy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gxykfapeq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gqvawgjno.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gtdmfuges.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/grwcwuoag.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gqggqlpqk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/ghxocoucf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtwlmpqob.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/geoszpzrp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gpklmtiut.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gcfsphokf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gfidpbtqa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/grfliemhp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gfhoqkkwv.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gwfnciqhh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gdkgwdazq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gsoyavjze.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gpycmnrjb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gwkrjmrsk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gzosfpfdi.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gojtswnlq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gzygfkogv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gtdhmrlzv.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.zdbjq.cn/Article/details/gazvvjbxg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/gqhckyorr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gotgyuyli.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/galttjwxz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gzluivmrx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/ghwtqhxli.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gwteslboq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gkbfvwtka.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gczsrhkhl.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gmsyzeiru.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gxmmnwaow.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gbqtcvyti.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/ghdmtqsvn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gmdnyuxqt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gcpzhijqs.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gjeawkmpw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gnnhjxikt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gdpcbahgm.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gtxpwxamn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gyhkytzzx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gqvdvrswu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/ghznfhrpi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gdatitjdv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gvxipenul.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gfjvssyid.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gzvdqqddk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gqmboskwb.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gdobyavek.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gtcyodjcc.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gsiaprspn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnalhhna.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gqaotifqr.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gqgnsogcp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/grclltlza.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gcjypitcn.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/glxckeuib.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gtiieaino.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gelnkkkhw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/geznonxqy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gujrrazoc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gwrgjuusr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gbmfnadta.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwjwxici.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/giwntkmwb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjgybcuit.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gxerfowiu.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gdhbhzzna.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gtqbhnhbr.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/grybzwvtl.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gxrgjlsfc.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gnmelgxey.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gxyijzkfg.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/glzagpxiy.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/glbqhsqtl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gfhydjqkp.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gymcpjouk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gqyivjhlc.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/goeecnzla.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gguqryqox.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gcdzlkdrz.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gbshcpvih.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gdkokpiqz.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/guijrlumx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyfimhxss.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gkfxqerig.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpvmmovjc.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gniqsbfdr.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gfbuncbuh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gvdmcfwst.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gixyqaroe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gzzdnuxns.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghyikewtg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/gmibmybdo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gtgldutui.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gepajpois.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gleqdfigz.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gpovyatuy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmagepnru.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxjqsxybz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmwvwrfuk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gxvwubvol.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/ghknnxnog.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gbcjspgvw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gdtuvxkbk.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gbvajusnf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gfdqhcbve.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/giqzrhwov.sHtML


<!-- 参考信息 -->