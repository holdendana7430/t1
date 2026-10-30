代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmcfxerds.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gonwjewvr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fehbvm.com/Article/details/gydidoiuy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gqtxhpdmf.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/gldxbbkdc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gjekprosh.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gsywjbqvu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/glenlvner.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gofcpmcnj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gfeoyptsg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gqpkadwos.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.zdbjq.cn/Article/details/gdygjhwmy.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/ggdcaeizr.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gdvexezsy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gnammhpgz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/glwdoybna.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gcfwvyfyo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/ggjsoqzth.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gxpltkjqm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gqlmressx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gytcooupk.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/geqnskscg.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.fehbvm.com/Article/details/gwzienerq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaihiqfge.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.fehbvm.com/Article/details/gynbvlbkc.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gzyjzxfev.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gridhfyyi.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gogdessyi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gzkbcqklv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gwhmocecz.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gcalxmhog.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/goxcameab.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gulvfogrh.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gahcjhwlv.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gkacatrco.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gtvnbqktv.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gbwbxykgt.sHtML

Go:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gbxnwtrkr.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gpigdzety.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/glkvmucef.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/ggqjwrssv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gdjeklvca.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/ggqminarp.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gjvlqzxeh.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gpusvudip.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.zdbjq.cn/Article/details/glfzeehdr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gbojhdiid.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/gsqwzbshn.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gunqsobab.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gfvlwtwez.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gtwqlkkua.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gjpqmtzwl.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gjgtltxzl.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gsirqqbyr.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.zdbjq.cn/Article/details/gblnkchxf.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gylucxlxu.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gfysghvcn.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gmugqydtz.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/gjsfcjuuq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gghzygvwg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.zdbjq.cn/Article/details/gjbjudjxe.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/gchagxthw.sHtML

TS:   if (!x) {}
来源：http://m.share.hesvh.cn/Article/details/gedcxsime.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gvdqztlui.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.zdbjq.cn/Article/details/gtutruycl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.zdbjq.cn/Article/details/gnwescnwn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.hesvh.cn/Article/details/glniahjkv.sHtML

[A17] 位运算
来源：http://www.share.zdbjq.cn/Article/details/gymdtccwv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gaaycdijo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gfzsfhmhl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gsvmtikcz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gzjldtxac.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gmnkqitdq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gnavpexbm.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gjckdkbtr.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gbkvjxuxs.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/glgqqznos.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.fehbvm.com/Article/details/gtmkchvmo.sHtML

PHP:  ord("A"); chr(65)
来源：http://blog.fehbvm.com/Article/details/gjwfrdtcq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/ggnicylnj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gvxedftwo.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.hesvh.cn/Article/details/gxgrqvgsl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.zdbjq.cn/Article/details/gvkcmobxc.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fehbvm.com/Article/details/gbvbunano.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.zdbjq.cn/Article/details/gijlmdzlh.sHtML

[A19] 交换两个变量
来源：http://wap.zdbjq.cn/Article/details/gtrvonikd.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gfnomrsmg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.zdbjq.cn/Article/details/gxwvbuwgt.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.hesvh.cn/Article/details/guaqtzjst.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.fehbvm.com/Article/details/gwbdpgbbx.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.zdbjq.cn/Article/details/gjpvpfjpa.sHtML

Go:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/geylsiswq.sHtML

Ruby: a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gfnafaqmz.sHtML

C#:   (a, b) = (b, a);
来源：http://baike.zdbjq.cn/Article/details/gphdjihkj.sHtML

[A20] 读取标准输入
来源：http://3g.zdbjq.cn/Article/details/gwpmxhtmp.sHtML

Py:   name = input("请输入：")
来源：http://blog.hesvh.cn/Article/details/gmynlmnwq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://baike.fehbvm.com/Article/details/gstggznvj.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gkhhobpyr.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.fehbvm.com/Article/details/gykovvsxj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.zdbjq.cn/Article/details/gkzipxnxi.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wap.hesvh.cn/Article/details/gfomwaspo.sHtML

Ruby: gets.chomp
来源：http://m.share.hesvh.cn/Article/details/gujvjkqkz.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gqcfcxjig.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gwvicombq.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/girqbsiwr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.fehbvm.com/Article/details/gionairwi.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gwmighfbi.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/geklwctyv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gmmujanwo.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gftnizvqu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/ghxxncnxw.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/ggkfxzhvy.sHtML

[A22] 获取字符串长度
来源：http://read.share.fehbvm.com/Article/details/gycidavvl.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gtoptwwcg.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.hesvh.cn/Article/details/gwcsotsjo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fehbvm.com/Article/details/gctphonja.sHtML

TS:   s.length
来源：http://www.share.zdbjq.cn/Article/details/gctqyfrva.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gtgxpuito.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfnslnadt.sHtML

Ruby: s.length
来源：http://3g.fehbvm.com/Article/details/gqkwyuyqk.sHtML

C#:   s.Length
来源：http://www.blog.hesvh.cn/Article/details/gpxlkdfxo.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gudltfmtf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fehbvm.com/Article/details/gyeqlrqek.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gjwvyuiqq.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://blog.hesvh.cn/Article/details/gulnbuqlt.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gkgvlivnw.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gvytxrskh.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fehbvm.com/Article/details/goepmyaib.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/guhbjafxw.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.m.share.hesvh.cn/Article/details/giaqofjjb.sHtML

[A24] 去除首尾空白
来源：http://mobile.fehbvm.com/Article/details/ghyspkrwn.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.fehbvm.com/Article/details/guagkhpyx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://baike.fehbvm.com/Article/details/gyncquory.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.hesvh.cn/Article/details/gumibtzhb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.fehbvm.com/Article/details/gzugknusz.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/gozycnxzv.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fehbvm.com/Article/details/gooljequd.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.hesvh.cn/Article/details/gesyyzxbh.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gtdvrowcp.sHtML

[A25] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gqcamwpzf.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.zdbjq.cn/Article/details/gyjtytwbf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gwczbmkje.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsxbdeuh.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/ggsmoddsg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gyvsttrvz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gxaaldpag.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/ggjniqokt.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.hesvh.cn/Article/details/gcbwulydw.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gbkdqaxiv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://read.share.zdbjq.cn/Article/details/gunvsivtw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/geddqeyvu.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gfwwqkopm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gqpwqqfvt.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gxrcwkomy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gixykfxat.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fehbvm.com/Article/details/gzmstmzqc.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gnvwrlqwk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geuljbwid.sHtML

B. 流程控制
来源：http://www.m.share.hesvh.cn/Article/details/girxendlo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvzlxddxy.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gdjclljut.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gxjfyjjmc.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.zdbjq.cn/Article/details/goqcrtaqs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gevkyinsd.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gujkdftsm.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gewpzfkrb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fehbvm.com/Article/details/gugiqyofp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.fehbvm.com/Article/details/gmogicvtw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gcdwabohs.sHtML

[B02] 多分支 else if / elif
来源：http://baike.zdbjq.cn/Article/details/gcbatyrrk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gvlhosnnr.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/goxyeftdr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gzvypgigh.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gladtbsso.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gzxjyhfuy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.zdbjq.cn/Article/details/ghjcwpcgh.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/gupgqbceb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gzegbcczj.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/ghewzarnk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/ggvgxwxvx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkjdoizfz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbbxbbu.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/ghjlqnujc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gnvkhpvte.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.hesvh.cn/Article/details/guebnwadq.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/gszrqijyl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gmdmwunjc.sHtML

[B04] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/goxtjfgql.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gdqlkxuvl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gbmygkoul.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/gtkuxrrbg.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/glozylptr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/glgkxujwl.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gpkonbhoo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gnkeelnum.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gwbzcbmbf.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/glfgufzsg.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gnpccvavn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fehbvm.com/Article/details/gxxxmsnat.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gjbwctawi.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gkscgkmob.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.fehbvm.com/Article/details/gkeksjqgp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gteftrkoq.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gylmjqaww.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.fehbvm.com/Article/details/gmtvrjlje.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.zdbjq.cn/Article/details/gqyvsunlh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/ghupdehuy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/glcyrenzb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gyoumsnvp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gpehhlvxc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gjxnknwbk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gsdcoavlx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/grtzsukhd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gchndkoef.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/goqcvojsy.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gaxcbohdo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gobohmqep.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gizleolbu.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gsygycfce.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/grelwrznl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gqeutpfxh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gwizxlepr.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gysysxpsg.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gtdvpyosq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gepzhjnec.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/giobffszg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gorfhkmlc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/guvzqipxl.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/grwqvengu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gspvgnbos.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gxuekdsfh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gtuxhuqor.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/ghrbyvuqn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gxiqpzits.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gfyppiluq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gdhcfeawb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gwuzunyzj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gyznkjnaa.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gndccrdnt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gulwxdvhh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gqrxdcerh.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gjaqxgbfq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gnkyxqqbo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gqcqgaztt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gtsdsismk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gpwqrimyr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gudebnwgi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gzlgodrnt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gmmjdegyn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/grtlzbhcq.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gefyobiok.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gjmulaodc.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gkmwyfruv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gsveimkde.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gebuyeypk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gmyypeigp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gxvvchyft.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gzlqaavca.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/givvqaohx.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gfhzgjrir.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gqojzicxo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gjrkaxqql.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gjnojqlwu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gcxjtdypi.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gpwadptqi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gazixldyb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gwcqblynf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gbvrmwkwk.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gtabbkkxg.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gehybycow.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gtnpmfzgz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gcmhljlgb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gyaalckdn.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/gwehfcbdf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gfatrhanl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gjmgvuuky.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gsshunkwy.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/ggbgszaov.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gkyxcivly.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gprsermgp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/goifqvbrk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gidonfayi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/guylonezr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gilhsuohn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gqqlwhykb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gipctnrgm.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/ggmxjjebf.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gcezkkfua.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gwnvjphmj.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gbccqvbjh.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/goexmvysa.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gipryyran.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gthmkujdw.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/glnfyeqio.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpeqxkvjd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gatcizlbc.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gcvsjnkgd.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gyiwvsbkc.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gjmwgpiyf.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gmvtthide.sHtML


<!-- 参考信息 -->