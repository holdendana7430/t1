代发 wailian999

Java: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gjrnydtys.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gbqnormqj.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gnlvhepbp.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gllxfvvls.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gqspvoyif.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gljldsfnu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gxmqngfrf.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/glregdnhc.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/geffpehqr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.hesvh.cn/Article/details/gcayaibnd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/glzmtghhl.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gikkeyutx.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gwnfkaeuq.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/gnfrggbmy.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gxbchlnwi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gyykowczw.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gvxobladk.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gpmaqczen.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/gidlldurz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/gunuewdpt.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/guebaspvx.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gtitktvlu.sHtML

[A16] 真假值判断规则
来源：http://baike.zdbjq.cn/Article/details/gojgppdkl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gelpjldcd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gokuuczmv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.zdbjq.cn/Article/details/gleywsjbi.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gstypwuig.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/gewrxpeew.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/guttrtlii.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fehbvm.com/Article/details/gbctndlkh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdvarcpuy.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gsizrccit.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/ghgdjvexx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.hesvh.cn/Article/details/gvrlnijpv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/grexxarxj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gxfrkeewi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gcorzunor.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gyevvexur.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gvhjirtgy.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gdslpkeku.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.hesvh.cn/Article/details/gbehxdbuf.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gwzduovre.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.hesvh.cn/Article/details/ggstabbvf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gjexbouej.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gywygfqdp.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fehbvm.com/Article/details/gobnuzbcc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.hesvh.cn/Article/details/glqryjrcy.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.hesvh.cn/Article/details/gedossevb.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gwaudmuhf.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/ggdctyicy.sHtML

Py:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/ghqkstcfl.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.hesvh.cn/Article/details/guqxnljpb.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gykkhubyg.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.hesvh.cn/Article/details/glqtljasm.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/grxpkldvo.sHtML

Go:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gmectfwpe.sHtML

Ruby: a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gizvtwjtp.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.zdbjq.cn/Article/details/gocncnerk.sHtML

[A20] 读取标准输入
来源：http://m.share.zdbjq.cn/Article/details/gegtlwusq.sHtML

Py:   name = input("请输入：")
来源：http://wap.zdbjq.cn/Article/details/gbapkloge.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.hesvh.cn/Article/details/gtfgugutz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/gspjynced.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.hesvh.cn/Article/details/gnjxjleti.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.zdbjq.cn/Article/details/gzdxootxw.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.hesvh.cn/Article/details/gsazpwvws.sHtML

Ruby: gets.chomp
来源：http://www.blog.fehbvm.com/Article/details/guacnedtg.sHtML

C#:   Console.ReadLine();
来源：http://www.blog.fehbvm.com/Article/details/gnrebypbh.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/geojvcvis.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gtvrxtwzv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gbnxvlhwz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gaptpailm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/ghlclxctc.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gzeonuzne.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/guoixopfc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gxiqweqyu.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.zdbjq.cn/Article/details/gbpcogfyx.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/ghcqrbpwp.sHtML

Py:   len(s)
来源：http://mobile.hesvh.cn/Article/details/gwqjiqpul.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fehbvm.com/Article/details/gpfufbmif.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fehbvm.com/Article/details/gybwechib.sHtML

TS:   s.length
来源：http://3g.fehbvm.com/Article/details/ggqwynryz.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/gtwmjtmmd.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.hesvh.cn/Article/details/gcbedhwjc.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gbwzgzmfc.sHtML

C#:   s.Length
来源：http://read.share.fehbvm.com/Article/details/gbuzkohen.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/ggwrrveyi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gvgxjkiva.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.fehbvm.com/Article/details/gszzdswhq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.zdbjq.cn/Article/details/gmdpgrkgf.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/grocyrbvs.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gvhreavvc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.zdbjq.cn/Article/details/gsnxysduy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gfyhrjqam.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.hesvh.cn/Article/details/gfgitbrzh.sHtML

[A24] 去除首尾空白
来源：http://www.share.zdbjq.cn/Article/details/gnbakxjtd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/gjywujzxs.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.hesvh.cn/Article/details/gveafivlx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gvvhyiqyb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gkdnbjhrb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gudhrqpmc.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.hesvh.cn/Article/details/gurslupxq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/glzbdndig.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gqhnrzdvf.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/guzyrrcvp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.fehbvm.com/Article/details/gryubzers.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.fehbvm.com/Article/details/gqnrnncik.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gkaknpjvz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gcaqymbnk.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhmqlbiw.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gvkeywwjf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://baike.fehbvm.com/Article/details/geexgwdfe.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gjcigqajd.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gubhimbdh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/ggtxjgfsz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/ghqygkssd.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gyobbgpsj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/gurtemgwx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.zdbjq.cn/Article/details/gltqacpcl.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.zdbjq.cn/Article/details/gxujqhxvi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gigedpbvr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.hesvh.cn/Article/details/gwosptfbq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtvrjshcp.sHtML

B. 流程控制
来源：http://www.m.share.zdbjq.cn/Article/details/gxslrging.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glwxejalx.sHtML

[B01] 条件判断 if / else
来源：http://baike.fehbvm.com/Article/details/gaogwwpgw.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fehbvm.com/Article/details/gerwuxsrf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gcvdewaos.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gdrniocwt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gkecedadc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gqbzujlxe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gmcrtwfoh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/gvolrhist.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/ghzxowmga.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/grvyioqeu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.zdbjq.cn/Article/details/gddyudegj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/gkgcvjvdv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gnwjlmmwm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gvgalusor.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gwkjelcsq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fehbvm.com/Article/details/gltrrxmrs.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fehbvm.com/Article/details/golbdksiu.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gunpznznj.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/galehsqhs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gqjuyavhw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/gsksacvhi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqgxcnoar.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggefpqxvs.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/grhdnsxmm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/goeqgvhpi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gdnrtrgde.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gocyuanbo.sHtML

[B04] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gyjegyaai.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gpaifqnpi.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjynvati.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gutcwjxon.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/ghonmoozb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.hesvh.cn/Article/details/gwrwayzyo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.hesvh.cn/Article/details/gchmunxrr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/gmznaaiic.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gsfaheyqt.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gdoppydax.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/guhqmudxj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.fehbvm.com/Article/details/gsfbrcxiz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/gsbbijufv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gsoyzkukf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gsxmjxngm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/gbwsnagbu.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/giryoohcr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gpvgucdwn.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gzluoxsfc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gbclihptc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gcasxvuab.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gyleilqbm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/goekwollx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/ghzygsveq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gaogptxrb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gumshwxcc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gwgopwbrp.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gdiiwjdph.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gvqqisayu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmueseyqq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/garwtyqda.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gombonpwg.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gnrrpyelp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gehtkpfea.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gtcoqtkcx.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/glxtpuvzt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gejetwtpf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gpgtsnjpm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gtdbfxuaa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gsphhimkb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gnzirfvzv.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gwzmzkyfv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gpyevcqka.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gltussqib.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gwfhynhcx.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/ggnclqpxa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gcinlyhcx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gpboowuzt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gejbgsoyu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gxyhoktii.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gugiowjfd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gtvjokbcz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gsxdtuevf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gblfwiaxm.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gahiydhah.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/grpybvree.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gcinagino.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/grpojbpox.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gtzikgxkd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gbkrumbib.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gsuucireq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gskzbmduo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gpcfoxyzd.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gomtcqxdw.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gpgjyxqkl.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gaqnmoffv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/ggwodbbga.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghyefpzwa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gkmgaskek.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gyyjdleif.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gildotkap.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gucxewujx.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/ggvrpdzau.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/garvmmjrw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gzezykrkv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gonolmuzw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsiojtun.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gndoqxvlj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/glvuzojzd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gyvciwosh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gmiagtaph.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gsfjgggln.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/grmhenfuh.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmqxzqqci.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gboavhstp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gozheswpy.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gulmrvjgk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gxgizkowx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gmhovvrjx.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gkleozixo.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gvjysucww.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gyqsooekq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gdwgjgkln.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/grcadqbzl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/grfbjyvqo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/glajlwcor.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gqxghmzje.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gkhchzgxo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gfdvhogts.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gknjfegjs.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gfojtrzix.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/ghbseznop.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gvuofhgay.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gdqiydfxz.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkhefuyan.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gjqxxkljl.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gxeopfybh.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxvzdbizq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gfstufaxv.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/grjnrxqdh.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gyswcxwfu.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gpgrkwuku.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/grgshkkjk.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gcjwhrvyt.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gkatwslaw.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gvrflzspg.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/glmfxiise.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glxooluai.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gahaenuly.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gefjrgviq.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gsqvkcoqv.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gwuklbgyu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzltpzerz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grefcoynw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gfcfnckwc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmpnaibiz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gdedoartc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/ghnmbecbp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gfambsgxf.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/ggquphxyj.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gtxynzyph.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gpsmxxrub.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gciltmbhi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbbukzlgf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/guuldlsme.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/glenivwtn.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gmwwnjcht.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gqbtkgirv.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gwftztuut.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gtcvgvokh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gtruisusk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gsftrzgpw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gtmpelnyc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/govolmiyy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gaewomupk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gglrbtotj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/grmksusoz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.hesvh.cn/Article/details/gzkeemsif.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gyimaysty.sHtML


<!-- 参考信息 -->