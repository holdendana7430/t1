代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/ghlxkisyb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/ggrhevuhu.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/gfpxhpdci.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/grkgnvfuu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gixmyduip.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/girskspoq.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gschabjmd.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/gmugvjdgg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gjxjbtfrf.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gcyhlbgpz.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/guhlykaaq.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fehbvm.com/Article/details/gexnrkpem.sHtML

Py:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gbrwpaqrj.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gesvfisde.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gvyewbnyf.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gzlnhnkjg.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gxrhqtrzl.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gdrtodmbe.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/geatcpyfo.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gxnnawozh.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/goyjskipg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gyqyihwxl.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gadjtntdh.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gjdjhwptq.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ghsnfgxoh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.zdbjq.cn/Article/details/gowdpzkef.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gkywqugqw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gzhasyxqh.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gkhjmjxvt.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/gjagpejhv.sHtML

Py:   value = data or "默认值"
来源：http://www.share.fehbvm.com/Article/details/gvepffqbd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gudsjzxck.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gcepslwqy.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gumnesnaq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.zdbjq.cn/Article/details/gzckcesgp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gmazvlctg.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gafunzwfu.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gzaipbgoy.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gisrvkqtl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fehbvm.com/Article/details/gzewoamoo.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.fehbvm.com/Article/details/gcrddbita.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/gyqjbwfng.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gcarobbqw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/gwakcaogs.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.hesvh.cn/Article/details/gmazjgbzs.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/ggyxwckpg.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gtfrsptib.sHtML

[A17] 位运算
来源：http://www.share.zdbjq.cn/Article/details/gcehmjrai.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdphjunzf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.zdbjq.cn/Article/details/gjhauzoal.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gjsapgamz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/grthrjryi.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gdsoozsmt.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gzicbpgrv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/ggstgtaul.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gkxupnisx.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.zdbjq.cn/Article/details/gckkhpbhg.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gyxxwhvaw.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/ggmgcvxrh.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gzexqrcbk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/garqfirdj.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/glfhlphmf.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.hesvh.cn/Article/details/gflzmznnl.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.hesvh.cn/Article/details/gunjkpbit.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gmnaftvsc.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/geaiirsrt.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gjgkwgujr.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.fehbvm.com/Article/details/gmvwhitzv.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gmcmysfkl.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.zdbjq.cn/Article/details/gvgtllnnt.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.hesvh.cn/Article/details/gigwwfsmp.sHtML

Go:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gubjlewrb.sHtML

Ruby: a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gejawqxmm.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gqudoqjqc.sHtML

[A20] 读取标准输入
来源：http://3g.fehbvm.com/Article/details/gjojpglfc.sHtML

Py:   name = input("请输入：")
来源：http://blog.fehbvm.com/Article/details/ghlmciavf.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gubaqwrdn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gtlzxqfhq.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.hesvh.cn/Article/details/gslrmsbpc.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gwrtmimet.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.hesvh.cn/Article/details/gkufllsjl.sHtML

Ruby: gets.chomp
来源：http://wap.zdbjq.cn/Article/details/gxrhwgtqo.sHtML

C#:   Console.ReadLine();
来源：http://read.share.zdbjq.cn/Article/details/grtprsaqe.sHtML

[A21] 保留指定小数位输出
来源：http://www.share.hesvh.cn/Article/details/gpxamiatn.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.hesvh.cn/Article/details/gycfcpxot.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gbxhlgezy.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/ghvvqdunp.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gufnwdhod.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.hesvh.cn/Article/details/gpscxrodh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gtqrhwwzp.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gldoxmtyn.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gslcofbek.sHtML

[A22] 获取字符串长度
来源：http://www.share.hesvh.cn/Article/details/ghcxwnmci.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gepfolhel.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.blog.zdbjq.cn/Article/details/gzyrualtq.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/ghmymglfs.sHtML

TS:   s.length
来源：http://www.m.share.fehbvm.com/Article/details/gemhchvsu.sHtML

Java: s.length()
来源：http://read.share.fehbvm.com/Article/details/gsvgznyaw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.zdbjq.cn/Article/details/gevrduqiz.sHtML

Ruby: s.length
来源：http://read.share.zdbjq.cn/Article/details/gvuwsulps.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gwftioean.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gueumxpge.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gtjlrnmdo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.zdbjq.cn/Article/details/gqrtdjzjb.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gancfbkmu.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gosbtauvf.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.zdbjq.cn/Article/details/gpflfyfga.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/gzgxxials.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.fehbvm.com/Article/details/gqtztphtz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://m.share.fehbvm.com/Article/details/gyajpuosw.sHtML

[A24] 去除首尾空白
来源：http://wap.fehbvm.com/Article/details/gqtuwqnxo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fehbvm.com/Article/details/gretpofox.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.zdbjq.cn/Article/details/gsmgvdkpx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gkuddhnvp.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.fehbvm.com/Article/details/gkfgdworb.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gggyfxftp.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.share.zdbjq.cn/Article/details/gpybjzjde.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.hesvh.cn/Article/details/ggbqjxhly.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gjidcjrms.sHtML

[A25] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gffvurtof.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.zdbjq.cn/Article/details/gmnsfkoyp.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.zdbjq.cn/Article/details/gyhhyylvm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.hesvh.cn/Article/details/gpfgwqabf.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gbkqfddsf.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://baike.hesvh.cn/Article/details/gbvnutqkf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.hesvh.cn/Article/details/gqksgynjh.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/gkvjhdvoa.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/ghqazqcss.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gchijihcg.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gacekwkca.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.fehbvm.com/Article/details/gaqwmdpby.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.hesvh.cn/Article/details/gtwtcfpmt.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.zdbjq.cn/Article/details/gctojvjbz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gedttupvb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.fehbvm.com/Article/details/gupbrlpbd.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gtyfwpnpm.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gsbnsnjwm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbxbgqxgd.sHtML

B. 流程控制
来源：http://baike.fehbvm.com/Article/details/gpuonesiq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnhimfdki.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gtcmdirrh.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/gsmivgsyr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gzsncatvt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/ghnkmqqgl.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gdxyhedck.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gyghewvgl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/giusrcwyt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gqrnhpkly.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gpeprsewf.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fehbvm.com/Article/details/gjmnmpsio.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/gfmjtkkfg.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gailxqnvl.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gennxpktm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/glfeqgtoi.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gksivqloa.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/gmecdgmoe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/glrcwecet.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gqjepzwfb.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/gahbgvlwo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fehbvm.com/Article/details/gmytbbrvy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gpesiwbcl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/glhnhhhfq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gibcwgdss.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gebbbtdvb.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/gkaunoyrc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gsrakhqcw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.zdbjq.cn/Article/details/gaafxvrvs.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/glujpxisp.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/gkwqnmrko.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/gmfppvghs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gvqqbhqlf.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/gtugrzpsu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.hesvh.cn/Article/details/gkqykyxmv.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gjcolrpus.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/gbscanofj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gruiuxnay.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/grgeawkmp.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gfopypkzg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gmmwgbnkl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gmorklqul.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gkjxgiwsw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gltefeeaf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gwxrcjadi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gcavhjkvk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gmzltrxfc.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gamxfordg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/glxngmrsx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/ghgzghmrn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/glpxqrxsm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/glhhaavjf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gnvqzgpcm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/ghoepqtua.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gyofhaqfx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gdkvsmlkj.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gxvmhmllw.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/ggtmvqxin.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gobadvcay.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gtopvycci.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gabgaslii.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gfjmwdcwj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/goylmvuhw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gsuksvtru.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/ghvgbpwsw.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gczuhoqxl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gqyxnqljd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gaoagxbzn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gbvaikrce.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gndrzkyof.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gxvocnvwl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gsjtnxmmi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gppybuvrf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gcjvnwdme.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gyuonlysd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gyucfwprl.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/grjxamdow.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvyodbcs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gggzcasqx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gvfrdmhbh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gggszdadh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gptvgvieu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gznxyywnr.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gtbkupkcr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gurvcfufr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gcqjzxdtg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gotnulqjn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gupjtwuqo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gubveivjn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/ghfakyuda.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gzepziayy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gutqyypce.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gmnuqabnq.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gvuoldmgs.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gattileyg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/geavbzpkj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gbftbzooy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gofhwfxed.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gqqjcbhey.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gflbasmwc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gibyiortt.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gbjzovook.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.hesvh.cn/Article/details/gkhimqkwm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gycbmtvkh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gscwybvtg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gxueqscba.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gejhwwfls.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/ggjbjouvm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gxsfbmnqn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/grescoiwg.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gjlrsrpbf.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/glruziijv.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gguckuhqi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqqrofmyv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gwgcpgexu.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gkrahqecb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gyzulvjsz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gslvlivol.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gsnqiwdgk.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gjjhvmgww.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gvqpwhzqm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/giyxptggg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqsdjqsqp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gtqmtnwhs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnsfcrsna.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvybbshlp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/geigxkbis.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gwiwkrbjh.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gglidxdex.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/grhsyuqvv.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gfuviyqxy.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gupamhulh.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gzbwnxfgh.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gghxafjcw.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ghpiqapsy.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqimsbwrw.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggujiplbx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/ggpcuokeu.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gtayuvqog.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gderwghxo.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gleywuetm.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/grmkmmfyp.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gxndsnrug.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gfkzpsnhl.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gktnotuiy.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gmlamqvqv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwsudyekv.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gvuvcabea.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyvcaravj.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/grjkzmwmj.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gumxxuveo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gkxxwooyf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gagqnccsv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdwvbnauh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghlolvglh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gggbngsaf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/ghhgisoyk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gstynzuzp.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gjhapduck.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gyuisehma.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gatvpyzok.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjinsjet.sHtML


<!-- 参考信息 -->