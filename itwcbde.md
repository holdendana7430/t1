代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/geqsbfgxv.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gfhmufmdp.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gggdxqpxo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fanxiaobao.xyz/Article/details/glnbzlguv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwbakmqn.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gezuamzfw.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fanxiaobao.xyz/Article/details/gsbwlbinv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbznmwfjg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqetpvhu.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeeroabo.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gobuojpks.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyivsyoe.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/guomjddse.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxypqxdbx.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfwihoyq.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusxnwapj.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjnxeliy.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gquptodwu.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gophdlddu.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gplhpzcrv.sHtML

[A14] 注释写法
来源：http://3g.fanxiaobao.xyz/Article/details/gprfqtwnz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fanxiaobao.xyz/Article/details/gquyzbndh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gkdlrsboc.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gzsiohgtd.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsssguivp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gisgtuwsr.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gazkmzsco.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweljfdnp.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdbydqeq.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihujukbn.sHtML

Py:   value = data or "默认值"
来源：http://blog.fanxiaobao.xyz/Article/details/gfhphwvqq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/grpvpzvgt.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvktfkwe.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gplsjbgwm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrvqavgo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvwbuswo.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaujbkqko.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhmcazbs.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpvlkrai.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gleupzcbx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fanxiaobao.xyz/Article/details/gtqgedipi.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fanxiaobao.xyz/Article/details/gipfftsfz.sHtML

TS:   if (!x) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gneghaclv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfdjqvwsp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxlcvngdc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fanxiaobao.xyz/Article/details/gahhynjwp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbvgkxevd.sHtML

[A17] 位运算
来源：http://baike.fanxiaobao.xyz/Article/details/gksjooxbf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrcxywqo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgzsgrak.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyvngipd.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpixslnft.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchqhvjpf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gpmxgnoeq.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjukzvwfl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqekqbmn.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fanxiaobao.xyz/Article/details/gydxnbinr.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghftcaweu.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fanxiaobao.xyz/Article/details/grzpuekvf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyinkjsxo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fanxiaobao.xyz/Article/details/gqfsryhqp.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.fanxiaobao.xyz/Article/details/glqevhchc.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://read.share.fanxiaobao.xyz/Article/details/gtohvzyzc.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.fanxiaobao.xyz/Article/details/gobymykcn.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrhusiwc.sHtML

[A19] 交换两个变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdrcwpzk.sHtML

Py:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/glutpdpnm.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlurgevb.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhcoypmv.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqptycfu.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.fanxiaobao.xyz/Article/details/gsigxittm.sHtML

Go:   a, b = b, a
来源：http://baike.fanxiaobao.xyz/Article/details/gmfdvmofe.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtfuazcf.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.fanxiaobao.xyz/Article/details/gkeamthti.sHtML

[A20] 读取标准输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgooetop.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxyjhodm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://mobile.fanxiaobao.xyz/Article/details/gffbatejq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeevevmx.sHtML

TS:   // Node.js：readline 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gykyuynsa.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fanxiaobao.xyz/Article/details/ginsjmwav.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaprukpy.sHtML

Ruby: gets.chomp
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtbbdgwo.sHtML

C#:   Console.ReadLine();
来源：http://3g.fanxiaobao.xyz/Article/details/gjkckopkw.sHtML

[A21] 保留指定小数位输出
来源：http://blog.fanxiaobao.xyz/Article/details/gjgoabnri.sHtML

Py:   f"{3.14159:.2f}"
来源：http://blog.fanxiaobao.xyz/Article/details/giixvjyqv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gofmbhgls.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxnyavnw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/guhqzyowk.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gkbrllqlh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gbsgweojc.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fanxiaobao.xyz/Article/details/gxdtetiqb.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gjvmqjyfl.sHtML

[A22] 获取字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbocwdmr.sHtML

Py:   len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbjlwcuw.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhclviau.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpleawfg.sHtML

TS:   s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gzowwgquv.sHtML

Java: s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkyxwcyg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjztwcxc.sHtML

Ruby: s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxjjnkep.sHtML

C#:   s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gvlmfmdnp.sHtML

[A23] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvnawtcb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyczkaut.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://3g.fanxiaobao.xyz/Article/details/gsctoqhkc.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcycjzftg.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gssqfbeti.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxdirwgc.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gfxlygapn.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoxwrrrl.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fanxiaobao.xyz/Article/details/grfivbnzh.sHtML

[A24] 去除首尾空白
来源：http://mobile.fanxiaobao.xyz/Article/details/gctdsttiy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaplzwjg.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/giuimkkwq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdncchib.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/ghvlveprl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fanxiaobao.xyz/Article/details/guarywalt.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.fanxiaobao.xyz/Article/details/geanjzbje.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeifsbnw.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fanxiaobao.xyz/Article/details/grqxbrcjn.sHtML

[A25] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuxcisla.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fanxiaobao.xyz/Article/details/gvevcmduo.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gvmxakaby.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymhzmumt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdskparrl.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gozyywlgi.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyelqajy.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcwhdkde.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqqrvyhc.sHtML

[A26] 类型转换总览
来源：http://3g.fanxiaobao.xyz/Article/details/gptqtnfia.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.fanxiaobao.xyz/Article/details/gisxljopv.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fanxiaobao.xyz/Article/details/gosswobrp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.fanxiaobao.xyz/Article/details/gjtdywyac.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.fanxiaobao.xyz/Article/details/guuoqcitq.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.fanxiaobao.xyz/Article/details/gjvenbina.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjrezhsaz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezinwkml.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gytiicqfv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqqopitv.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gkjspaymu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glrhsjhuo.sHtML

[B01] 条件判断 if / else
来源：http://blog.fanxiaobao.xyz/Article/details/gmrrngcby.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gifsyymwf.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gadxwxhxq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsydmitbr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gatcvwpqf.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgpldboz.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gciqhcked.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.fanxiaobao.xyz/Article/details/gosridziw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gsarpdjod.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkevsbvfb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fanxiaobao.xyz/Article/details/goybhcldj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwngsvkmc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgslyxmx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gtlovwkqz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuyndvhj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fanxiaobao.xyz/Article/details/goiphpeek.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fanxiaobao.xyz/Article/details/gvqbstuvm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqwyfrmn.sHtML

[B03] switch / match / case
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbkqhtfs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyaetlks.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlclzmkd.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtowbilm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggdvjmxej.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwnruihhz.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gubjewgbu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gljxyetuc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqawuevig.sHtML

[B04] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gsdotosyy.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gmvaeqvbx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fanxiaobao.xyz/Article/details/gixlhfcwj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzugcmvvj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyppowkix.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggelxqszg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjlkylls.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmezfmwju.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/glmqahisf.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gqtfsdtwm.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlnlnayl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fanxiaobao.xyz/Article/details/gediqibtb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmoxyqpyl.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghvxgyjgs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjavlliwh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvnxxpmh.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/gmugglrgv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmzjgjvcj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gltnrszib.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekvaucmt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdlrpent.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gokqkgzsi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/grythksyx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gixlzjgbh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggctzdkdp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmhfrbkd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gglwnojxe.sHtML

[B07] while 循环
来源：http://wap.fanxiaobao.xyz/Article/details/gajyxkwqq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvbucmldt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszeyqvwq.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gftrixmvh.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxapcdzuy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxfbiwd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fanxiaobao.xyz/Article/details/gwogfffgo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/gtmtetacm.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glzvazntd.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gneajmecu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwyeacjh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvemkxsq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gsqpykxxo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbrmrvvu.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gwdrlaeiq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzqrfptz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fanxiaobao.xyz/Article/details/gjewlsnef.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsvnvgfp.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsmnckkf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/guzplbqxw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesfcamro.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtetqzlyv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfstgferm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnccilhzk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gkgmekabj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkznwywwn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnkaaxkx.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxpbwlqb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/gfbvlncyz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfdczavl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gsjpzdgid.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrzegnsi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkahfmysn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwabmqm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gecjadago.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedtschoe.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcotoyudp.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fanxiaobao.xyz/Article/details/glciimeni.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gjvplwxun.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkskvtay.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcropcoo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gymdetlde.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fanxiaobao.xyz/Article/details/gwdxfcdwc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqfaawuo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/golevpjml.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gubonlntl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fanxiaobao.xyz/Article/details/gcgjguljf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fanxiaobao.xyz/Article/details/grqjgukru.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlkspqzz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gavezphqd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyctvhuaf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggascwofw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gubzejhmv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gtoobsdlt.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdjbedze.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gihqmewhd.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gggdcswfk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaaruaxb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gvrhjwtvu.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxunvurq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwjbjvul.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fanxiaobao.xyz/Article/details/gavmawdmx.sHtML

C#:   x is int or double or decimal
来源：http://wap.fanxiaobao.xyz/Article/details/gziwpejua.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fanxiaobao.xyz/Article/details/gjigrrgpz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fanxiaobao.xyz/Article/details/gcskoduuj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmclfbxjp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gubxndipm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzafsuqa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyrznhki.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fanxiaobao.xyz/Article/details/guzpnsbtc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghdbyqmck.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gajknpkoa.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fanxiaobao.xyz/Article/details/gitpocxzq.sHtML

Py:   a and b or not c
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmisfjvv.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/gyafvwenp.sHtML

JS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/glrlvbxuq.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/grbywdwuc.sHtML

Java: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gvnffoakq.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkknvcpqs.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzjuqkpv.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gswhbcakh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gchpirkwx.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdozfyhnb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gigwxicam.sHtML

JS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gerhjdabz.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gaxwqqrjs.sHtML

Java: if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gsqmidxcn.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjvmumur.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzdvudjs.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpzlojhh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbedqxggh.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gbgoecmfa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gihpommhm.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghdhglahn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfrsggzf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiaihlmv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdzrongq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnubvpzk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvvuwsvl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gcosyenyw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzbvboud.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqtjxntal.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzroimkhk.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqikwcwg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsurvalrj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfstahlx.sHtML


<!-- 参考信息 -->