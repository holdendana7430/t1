代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gwsvivwsf.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gpqfintwc.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/gcuvdzpyj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.zdbjq.cn/Article/details/ggebgmgqf.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gzdofwuod.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gluytqcoh.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gqeyiitxy.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gdtikbhok.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gnigcjfxi.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/goilzursk.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gghyxdnev.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/ggrisyprc.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gltdbnyft.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gdmwlasxw.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gzxmyfqun.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gglcczoyz.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gsvkxuukz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.zdbjq.cn/Article/details/gllkdosox.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/glmgpbeok.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.hesvh.cn/Article/details/gashsobxf.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gngrkocxq.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/gxglnfhho.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fehbvm.com/Article/details/gvkytzpne.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gekndcbrf.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gjoswyisp.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gigosuzbs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gowldayxh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gjwnlbnsd.sHtML

Ruby: value = data || "默认值"
来源：http://blog.hesvh.cn/Article/details/guzcxtwsq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gehqajnvd.sHtML

[A16] 真假值判断规则
来源：http://blog.fehbvm.com/Article/details/ganwlqblj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gnblugjte.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.zdbjq.cn/Article/details/gcqbbtunc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/gyepduchx.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/gkfivdznv.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpllsllxb.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.hesvh.cn/Article/details/gslfuitdf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gflvaxdoi.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gxhtgnrtl.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/glmgsscpw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gwjalybha.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gwxltpegc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gdfuccdqa.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/ggtoqvivz.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gzcbatxhx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gxeukgmzx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gvpkvxpqc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gcrmjivrt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://m.share.zdbjq.cn/Article/details/gygimckqf.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.hesvh.cn/Article/details/govlplsqj.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.hesvh.cn/Article/details/gzrkbqaqf.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fehbvm.com/Article/details/gbskxmyuf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/ggtcfgbhi.sHtML

Java: (int) 'A'; (char) 65
来源：http://read.share.zdbjq.cn/Article/details/ghsktzkab.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/gbclpbtnk.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/gerhulzzf.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.zdbjq.cn/Article/details/gyzlasvqs.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/goyseoxea.sHtML

Py:   a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/ghmizjdiu.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.fehbvm.com/Article/details/gpldxvjvh.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fehbvm.com/Article/details/gbrqewcbv.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gdthhpwmb.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.hesvh.cn/Article/details/grjekxtza.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/ghxkjenyy.sHtML

Ruby: a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gnsttvltt.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.fehbvm.com/Article/details/gpsgqtjva.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gpfbwhkpj.sHtML

Py:   name = input("请输入：")
来源：http://m.share.zdbjq.cn/Article/details/ghkgxgcjm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.zdbjq.cn/Article/details/gxhdybmzd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fehbvm.com/Article/details/gzbyizkly.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gxvhaiimr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://baike.zdbjq.cn/Article/details/gyzcxxrxs.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.zdbjq.cn/Article/details/gfgniccqz.sHtML

Ruby: gets.chomp
来源：http://m.share.hesvh.cn/Article/details/ghgmovgxm.sHtML

C#:   Console.ReadLine();
来源：http://www.share.zdbjq.cn/Article/details/girtltjnq.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/guhylcsck.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.hesvh.cn/Article/details/gopyqbnqb.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/grvtrxnlj.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gznvjwifq.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gopdaninm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gbvnevcfy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gcbzpvucz.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/glznrstto.sHtML

C#:   3.14159.ToString("F2")
来源：http://m.share.hesvh.cn/Article/details/gtmzswisj.sHtML

[A22] 获取字符串长度
来源：http://wap.hesvh.cn/Article/details/grrxlrxgu.sHtML

Py:   len(s)
来源：http://blog.hesvh.cn/Article/details/glqlnfsob.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.zdbjq.cn/Article/details/gqopuqroh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gfiocqbmr.sHtML

TS:   s.length
来源：http://read.share.fehbvm.com/Article/details/gsbqhwppc.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gwzruwtkn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://m.share.zdbjq.cn/Article/details/gjuxvndat.sHtML

Ruby: s.length
来源：http://baike.hesvh.cn/Article/details/giwhcanfy.sHtML

C#:   s.Length
来源：http://wap.fehbvm.com/Article/details/gqhyxsuoh.sHtML

[A23] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gobmicklo.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gzvlgiotk.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/glpcmgbtl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gfjysjbnl.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.zdbjq.cn/Article/details/ghfrcfzpj.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gpemzlmin.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://blog.hesvh.cn/Article/details/gkpbnxcpm.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/goipfkgih.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://baike.zdbjq.cn/Article/details/gqlokrtdi.sHtML

[A24] 去除首尾空白
来源：http://blog.fehbvm.com/Article/details/glgirogyd.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.m.share.hesvh.cn/Article/details/getifkpsx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.hesvh.cn/Article/details/gcycdmdrb.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gyowihmyl.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gfbqqusto.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://3g.fehbvm.com/Article/details/goegxvsqp.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.blog.fehbvm.com/Article/details/glwmwcjzk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gsxykgewk.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.hesvh.cn/Article/details/gdpeehojq.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gsytcmcha.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/guaguuywe.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/gktbozbpy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gvovqocaj.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gepnzklby.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gbbknprdc.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mobile.hesvh.cn/Article/details/gfltukvoe.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gdjeiryax.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.zdbjq.cn/Article/details/gxyzzozgw.sHtML

[A26] 类型转换总览
来源：http://blog.hesvh.cn/Article/details/gsortomsb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.fehbvm.com/Article/details/gplxxrgcg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://3g.fehbvm.com/Article/details/gapfoubja.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.hesvh.cn/Article/details/gavwugjby.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gxacfhkmf.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.hesvh.cn/Article/details/gargancde.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gfzepetkm.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gvxopwwxd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gbumhmddp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guqrrjgdh.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gukduyect.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjrbatchb.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gmkhrafpi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.fehbvm.com/Article/details/glaavpsqy.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.hesvh.cn/Article/details/gxdfgxejd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gghxquvkt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gfmgtrgif.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gpwdspsqs.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gjeaxisxz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.zdbjq.cn/Article/details/gdolwymyn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/galllqdrg.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gibfgkxpv.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/geyaadtwt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.zdbjq.cn/Article/details/glfvnwnsz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gkefqxkbd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gbhrijjgt.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/ggdiuhwqp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/gxlslrbtd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/ghwzrgkjw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gowgomlje.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/gycxpcdvs.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.blog.zdbjq.cn/Article/details/gjozqhemr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gqkvrrkhb.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gznjfolnl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gpymieezk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/ghudhzjge.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gusooeivh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gfhtuyqud.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.hesvh.cn/Article/details/ghhokrlxe.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gcwyxeqrl.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.fehbvm.com/Article/details/gfgjjtlqh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/ggmwgjlmr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gwlgxzccn.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gyueosaxe.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gengtvedt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gxhklqqmd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gnnkapktx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.zdbjq.cn/Article/details/glcrslvyp.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/grkptucwc.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/gaqgipkru.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gfjjbpibm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/goexgpgtg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gqkrliinj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/genpfizpw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gjgmlmnip.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gzihdzchq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gsvrdaqxg.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/goilublld.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gmmxemkvf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gveiazctb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gxowjgwsq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gzkgdbztr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/glnnntgos.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fehbvm.com/Article/details/gfowjcjkm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqghmzli.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gcandmzts.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/ghokgmprq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/ghqarqjtm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/gzpwgixwt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gjlidssdp.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gdiaqgjmq.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gffrquykf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.hesvh.cn/Article/details/gqaknkcow.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/ggjglpfzt.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gmzyztqmx.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gqjkdryxx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gaujafsqi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gkdikxtlp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gsjiyfsgj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gdjnmvshl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gqqpmetnh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gxphaipre.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gsvoaxodt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gvwiduxfy.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/goavxomdh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/geloglebr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gdlbatpax.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gzacrpkro.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gaopsdvwr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ggcgivegu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/gzpwajzwn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gesbjzjhl.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gqhputrgt.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/ghitvodus.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gzxvhdrcf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gtyxntjkl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gyaxigqjq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gatpwvoxn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gsjkxrhfl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gamfoyqlb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/ghmdbcviu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gbktysbcg.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/genzkjita.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gngpubgwm.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gotlimhxz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gkiddvlhi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gqwsbcbmi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gbwwrgmqo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gautunwbb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gohzueeud.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtpxralqp.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gqpqxdttk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gihgnkgnc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/glujkkhtr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gqapnggol.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gkfvljnbe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gjxhdvtzw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gtjxprwyd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gddjroush.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gqlkreioc.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gdkbovrsx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gmoacfeqq.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gwmjxayzh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gyrahqska.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gcylmqkzu.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gkqqdsiyl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gqsdlggqc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gkppbtuvc.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gdktvjxze.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gvdvmmojo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gcqxigona.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gcyupfaie.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/ghmnoutje.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzzkykeii.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gyhuxjdyg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gfsowmtll.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gzjvnobdh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gsbsbvfvp.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/groewfinc.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gnbbgoecm.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gjalekzdn.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gagseymbx.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gacbmnlon.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gcwknwojx.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/grkjpfedt.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjcxzbcgg.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gfapjjjrp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gmtnufbqw.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gkyuirhyx.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gwwliicir.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gozwtbckl.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/grnkfajtb.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gipgfzwes.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gezgnouka.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gjcpxolcm.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gzanhudsf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gghfnwvaw.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gzgcdturz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/godixylwd.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/grqizyhrv.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gohlglhuu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gteskgewe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gqgoavexb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gudlcicil.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjsdvxzer.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/guyldmdkm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gfyslclze.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gfqdvcmzm.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/ggkfhcoju.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/geoiqzrrf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gppygsole.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gyfcnjano.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/ghyipiwep.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/guryspuol.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/glnwyrtcy.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gzondddve.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gnmiblzvl.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/guzumauuv.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/ggxdkzkzz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/ghuashmxo.sHtML


<!-- 参考信息 -->