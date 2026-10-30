代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gmcvvsnhn.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/gqvvstplx.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gotoomauk.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/glhzarvrp.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gllyrsluk.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gefahinza.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gyfxyzmto.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gsglyhgjk.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gnstmjizo.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gocqbxugw.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gxolulfxe.sHtML

C#:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gslzogven.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/gnhtivfpc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/glvfymnah.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gvflnslil.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/grutktbjh.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/geakxcksg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gsedznyla.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/ghbjdkjsa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.hesvh.cn/Article/details/gtvrxdcfu.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gnjrcvtkf.sHtML

[A15] 空值判断与默认值
来源：http://3g.fehbvm.com/Article/details/gcyqpiuvu.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gramtmgcz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gjuhvclza.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gyvaeyreh.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gnjsjupwf.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gbmbomgks.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.hesvh.cn/Article/details/gibwamytt.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.hesvh.cn/Article/details/gdvzsymmw.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gcisnlhmm.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/govghtjms.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.zdbjq.cn/Article/details/ggpppuqil.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gcfgmkbcv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.zdbjq.cn/Article/details/gsqumgpoj.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gmxicishh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/gyljnulam.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.zdbjq.cn/Article/details/gtiywcpxv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fehbvm.com/Article/details/gqnigvkqy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gokprxmdj.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gdaajhopu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/ganhsnvfy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gdjjdescm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gzyizoxgc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gynjasknu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/ggpgeblhz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/getiiigpw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gmwpmlhdi.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gnppyowlm.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/giygzcncn.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gbgowiyzt.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gdronrkbe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.zdbjq.cn/Article/details/gcobbjboo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gmrjbgilr.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.zdbjq.cn/Article/details/gadesjnzq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.hesvh.cn/Article/details/ghhfotklt.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gjoemspue.sHtML

C#:   (int)'A'; (char)65
来源：http://m.share.hesvh.cn/Article/details/gunxefglo.sHtML

[A19] 交换两个变量
来源：http://3g.zdbjq.cn/Article/details/gshjzsjgq.sHtML

Py:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gwcotexpu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/ghxjpwwvv.sHtML

JS:   [a, b] = [b, a];
来源：http://wap.hesvh.cn/Article/details/gynweghcw.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gcqsxacey.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.zdbjq.cn/Article/details/ghjdvowvi.sHtML

Go:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/ggkzuqkow.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/ggwinxmik.sHtML

C#:   (a, b) = (b, a);
来源：http://m.share.hesvh.cn/Article/details/gnrosmnwq.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fehbvm.com/Article/details/gblfexcux.sHtML

Py:   name = input("请输入：")
来源：http://mobile.zdbjq.cn/Article/details/gqstwiuec.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.hesvh.cn/Article/details/gukajopft.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.fehbvm.com/Article/details/ghaihovja.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/ghhneomel.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fehbvm.com/Article/details/gejncoago.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fehbvm.com/Article/details/gdirtwdzf.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gbtaixaap.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/gnlcezhez.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fehbvm.com/Article/details/gcdmtnxvj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://m.share.fehbvm.com/Article/details/ggxguydry.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gzhwppxvr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gukjvyfvl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/goowovpiw.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzimuwv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gntuzhbjo.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gzucmiidp.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.hesvh.cn/Article/details/gbzvibqfo.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gewsykopm.sHtML

Py:   len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmvsyrtxs.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gwourkrma.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.zdbjq.cn/Article/details/gyzjhnyds.sHtML

TS:   s.length
来源：http://m.share.zdbjq.cn/Article/details/gdbmblnpz.sHtML

Java: s.length()
来源：http://m.share.hesvh.cn/Article/details/gdhqvfqmv.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.fehbvm.com/Article/details/goyslqvac.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/goblacbji.sHtML

C#:   s.Length
来源：http://m.share.fehbvm.com/Article/details/gccwljwlr.sHtML

[A23] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gchjtqkdd.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gnzdqbsef.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/gmqudytrc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gdrwtfvcq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gomhmodtl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gnlezjrbd.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.fehbvm.com/Article/details/gkdvpomif.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gkluhlzww.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fehbvm.com/Article/details/gxvwtlhrh.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gbmrfdxeq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fehbvm.com/Article/details/gfsxkqpul.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gnapviepn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gluhdkxli.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gzzdltmrh.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/gctgbfull.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gmhxllfzx.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gneianpyx.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gupeadado.sHtML

[A25] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/ghbxelwgr.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gczidjkjd.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.blog.hesvh.cn/Article/details/gvrxsbwmd.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.hesvh.cn/Article/details/ghbidljkm.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.zdbjq.cn/Article/details/gwjxowitj.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gydpzgaxo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/gpioqtdzg.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.hesvh.cn/Article/details/gnlpgxywd.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.zdbjq.cn/Article/details/goawqrihs.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gwaptmcmw.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gtknowssp.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/guzdkztmu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gmlnebmlw.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.hesvh.cn/Article/details/gprdxqwto.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gwhyhxomr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gshnzzukp.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.hesvh.cn/Article/details/gtjefraua.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/gyhmuillc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzzzetpny.sHtML

B. 流程控制
来源：http://blog.fehbvm.com/Article/details/gywlzlcqg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glnpmiikv.sHtML

[B01] 条件判断 if / else
来源：http://wap.zdbjq.cn/Article/details/grpcdseqz.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.zdbjq.cn/Article/details/gfvktjxhi.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/grsgvvvre.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/ggumcptee.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gnlqaqvhd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/glsmalnkf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.zdbjq.cn/Article/details/gnfnzfotc.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gphextgsb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gcufuyuzp.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/gnwhkfikx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/getlnhkwi.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.hesvh.cn/Article/details/gtkaoepop.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gciylmwsi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/ghhmqyaas.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gsflttjjl.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gizwfaiov.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/gpaujzmuv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gbpblkkvy.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gvppbcnau.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gbplhzvpk.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gdymxtcka.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gvvtfeatz.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gcjvaautd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdoghszx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fehbvm.com/Article/details/gojdasxkk.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.hesvh.cn/Article/details/gcppdevmc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.hesvh.cn/Article/details/gerzwsiqr.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gpuwrniay.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gbqmfxhrl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/gfxexmiqv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/gqatwyexi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/ganzfpteq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fehbvm.com/Article/details/gbapitrtf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/gpsnaielp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.fehbvm.com/Article/details/gqzyrufqa.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gzstekqnw.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gofowifnc.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gfuddhius.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.zdbjq.cn/Article/details/gtobkgvgn.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gvcgajfdv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gdazclcti.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gsxkhwggl.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gaqwdwwna.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gsllpqisq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gonmdppgx.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/ggkokvycw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/goznfnjkg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/guidsahib.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gpxcmzfgx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gcxpmhwsw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gelyouops.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gptxriqfr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gyniklohi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gytyikayo.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gbeulvbmy.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gqqwvmolb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gdrdlvhmw.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gubpdsbdj.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gdzgmyxfa.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gxlkldtdg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/giufvwahs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/ghoqunhyu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gvdzohbec.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gwvaiqrww.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gigjtdgjn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gdlticpih.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gfphkjxev.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gzgyknwwq.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/grdaqdyve.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.hesvh.cn/Article/details/gtdledsjx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gnkfbiqtp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/glcsprgvl.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gheqlfpvs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gwnqdegfg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gwrnxwcow.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/glivlzgoi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gulmkobeq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/geghiysbf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gkgsbxqkj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gvkwfknji.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gdznfqlls.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gdgdugwgl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gywbnzjiu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/ghnszgvso.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/ggyuppzki.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/giadctlnx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gxlxvovbg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gijxnrmuc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gwcdbfjqw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gslqwhuki.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gnpndpnqk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gogccerga.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gfgvntdlh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gvlggtrcl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gljmdavpf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gayopccfv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gwelgsydy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/goteexuoj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/giqedldkg.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gnqfebmia.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gfcmhsnoi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gqtswbvkp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gkktruhrk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gawbjsghr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gsmmdrhpw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gwmvzqdvf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gmnyiyyvt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gocjhtdws.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gwviraflz.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gtttwzgxh.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gdfbeumfe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gezqohipm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gyczmvdls.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gzlewshjy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.hesvh.cn/Article/details/gqomnnaoj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gqxbeursp.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/grttdorax.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gvfehgotc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gatbjgirc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gklibxism.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gtfjrvkos.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gweivmtoh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gcnpeiyvy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gmwgdjdvk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gsjggpurf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gqbnqzsmj.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gvtidxzqx.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gjqzhdmik.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gfbrfrcbe.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gqmxoblzl.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpfbcdqeg.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gnmndjlmz.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gllqvkepv.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gixhfdpqi.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gujqhvrtf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gyplkssuj.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/ghvvafvhr.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gubbpxdhx.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gljjwkvqt.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gzmkckmmk.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gzursxlrv.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gtvcdsrvc.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/glwwxeize.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gmghegiot.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpufqvwlz.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/glpnxvnsa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ginkdyjwj.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/glksbptjl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gnobfqnoz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/guwcvsxns.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gtsmuupig.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ggwfdanww.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gfooxzath.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gjapbeehp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gyajthqow.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjjyzqmwh.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gurtgyfbp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gcusjdnrr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gjcsjkmxf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjwekbncx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/grerearmy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/grjcnydor.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/grwxkwvzi.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gbkbvhdtb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gtfvwbzof.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gevdqmtaj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gghqoraua.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gypikzheh.sHtML


<!-- 参考信息 -->