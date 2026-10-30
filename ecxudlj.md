代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gfalibnyy.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/geoekfyfl.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gagoycnbk.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gopzdalgo.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gpqitafwv.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gldqmvixg.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gmujujxfu.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gtloercqn.sHtML

[A14] 注释写法
来源：http://wap.hesvh.cn/Article/details/giivklyie.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/gagrunoob.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/grcceoupx.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gnzmoyadl.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gkzgzqomx.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gqfjvlrqy.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gkemjbnbc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/glgcwqwiq.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gocbavezo.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gdwouyfna.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/gvrfcyyun.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gpemfjujz.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gkqusbgtd.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/guyeddubz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/ghpvevqqc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/glqfiympj.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gdpibpaxj.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gkdicombb.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/ghzkiukpw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gfwmduacv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.hesvh.cn/Article/details/gcvrcinsl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gzmzaeqlf.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/ginxhvyll.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.zdbjq.cn/Article/details/gapbsjzlq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.zdbjq.cn/Article/details/gpentjmky.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/gzbxjhiei.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gkhubhoth.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gmtxnjypu.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gkwvhdbnp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.zdbjq.cn/Article/details/giswbiuuv.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gahaivuux.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gbviqlhul.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gravftgmr.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gsxcpadlo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gptidwbbz.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gzdtqkxca.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/ggiscdaar.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.zdbjq.cn/Article/details/giggvfqlh.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gbzhzilsz.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fehbvm.com/Article/details/gqjauexwf.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/glsyeafgd.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.hesvh.cn/Article/details/gimuaszep.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/grsfksrto.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fehbvm.com/Article/details/gakcxxfzx.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.zdbjq.cn/Article/details/gevmcmxpk.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gzpmllcof.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gpxosinle.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://mobile.fehbvm.com/Article/details/gxcnsyibo.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gthpccbvp.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gaoudklnk.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.zdbjq.cn/Article/details/ggwzyefnl.sHtML

Go:   a, b = b, a
来源：http://www.m.share.fehbvm.com/Article/details/ghsngupnk.sHtML

Ruby: a, b = b, a
来源：http://m.share.fehbvm.com/Article/details/gpuytsubj.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.hesvh.cn/Article/details/gqfuewjtm.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fehbvm.com/Article/details/gbtcebzyj.sHtML

Py:   name = input("请输入：")
来源：http://read.share.zdbjq.cn/Article/details/gaggjlcpa.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.zdbjq.cn/Article/details/gpfvzipsq.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/gktdpxmqr.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/gtpnknuqh.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.hesvh.cn/Article/details/gyidrnpuu.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gnbumqrfd.sHtML

Ruby: gets.chomp
来源：http://www.blog.zdbjq.cn/Article/details/gqsnqxcgz.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gljejlygm.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/gqbpwftvc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/gmbgitfgv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gciojtjrz.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gtvmyhnbw.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/ghjqlticd.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gyudyqics.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gzjlnbgyx.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gxrhnsrmz.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gglulfcbx.sHtML

[A22] 获取字符串长度
来源：http://wap.fehbvm.com/Article/details/geqqcwmks.sHtML

Py:   len(s)
来源：http://www.blog.hesvh.cn/Article/details/gbsptqonf.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/giaoucahz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/griptamkf.sHtML

TS:   s.length
来源：http://baike.hesvh.cn/Article/details/ghaighwqu.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gbvvuhmjq.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjdvntbnp.sHtML

Ruby: s.length
来源：http://www.blog.fehbvm.com/Article/details/gdtxghsuj.sHtML

C#:   s.Length
来源：http://3g.hesvh.cn/Article/details/gvazaziyi.sHtML

[A23] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gnomgklte.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/galknszxy.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/gdqhdwjbg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fehbvm.com/Article/details/gqacdpjgj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/gfekygfqt.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gkmvisvpp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.zdbjq.cn/Article/details/ghiiotvzy.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gkrvhwrvc.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/gmiaawcgk.sHtML

[A24] 去除首尾空白
来源：http://read.share.zdbjq.cn/Article/details/gdmkyutny.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gkbmwodgt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.hesvh.cn/Article/details/gpufyjypj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/ghxzvigow.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gnihdftja.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.m.share.zdbjq.cn/Article/details/gsmylhqfh.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzfaxhyfn.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gbuccbtrt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtansikrz.sHtML

[A25] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/glbcghpqm.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.fehbvm.com/Article/details/gcbhxdpqm.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.fehbvm.com/Article/details/gxohqmxvf.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.zdbjq.cn/Article/details/gdznlpjce.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fehbvm.com/Article/details/gechvgmny.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.hesvh.cn/Article/details/gwkglullh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gqloezxnz.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.zdbjq.cn/Article/details/gmrxzglzb.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mobile.fehbvm.com/Article/details/gzlxkijou.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gplfawegt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/gvgwglotw.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.fehbvm.com/Article/details/ghwcboiok.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gelnweafh.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.zdbjq.cn/Article/details/gzmthywmh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gofmjvrqe.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/gmnwowsok.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.fehbvm.com/Article/details/gookxqfyq.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.fehbvm.com/Article/details/ggozwewox.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gimozvlyf.sHtML

B. 流程控制
来源：http://wap.fehbvm.com/Article/details/givmjoxju.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkhrkedls.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.zdbjq.cn/Article/details/gxhwkptrt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.fehbvm.com/Article/details/gmehjpuxm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.zdbjq.cn/Article/details/gjirzxkcl.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/glqmzlgfi.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/glqenmvqe.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gwmbvqojf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.hesvh.cn/Article/details/grfkdlpjp.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/grjniliso.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gbmgkedcs.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gpppdkvkl.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.hesvh.cn/Article/details/gmhbfhnvh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.hesvh.cn/Article/details/gaatkolgr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gwndcrmkd.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gautjehii.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gtcqobkcg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.hesvh.cn/Article/details/gqdzvzyrd.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.hesvh.cn/Article/details/gjpyvkjic.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/guohtjdhb.sHtML

[B03] switch / match / case
来源：http://baike.fehbvm.com/Article/details/gqiwppvas.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.fehbvm.com/Article/details/glhqrxdgd.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gwoqocfiu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gxhcbeteo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/ggjnsqxsv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gyjgrogdl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/grgpcjicc.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gxzenfcdf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gtjbxpvez.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gjlqppphk.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/grezytadj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gwifobxam.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gigojguoc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gyxpxvzgh.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/ggdizhioq.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.hesvh.cn/Article/details/gzirtbpli.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/gdolkwela.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gnusoimmc.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gusaimjqj.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gvwzhjdxl.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gjskpfvnd.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gogwdivcc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/girgqhqjj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gnvwuhsdi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gleibmhgy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gycotuhvh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gdfplhnhm.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gsjufaakq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.fehbvm.com/Article/details/gxjooppbd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gcigqmjte.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gsiabikir.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gpidxofdh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gdbyureqc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gmkeexsam.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gjdackwaa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gzzbxzrym.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gbxyefcij.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gvcgwabyk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gjlwqeyaa.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gunxlwufp.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gdbkasuha.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gqhqvmdvp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/giybcptvx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gltalbjrg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/ggagmfodm.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/geetflxup.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gzzvhqprj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gwmhtzdqf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gdtjmwmxd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gmfucetfe.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gkmjfatwa.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gfgdtlgmv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gsiwhvfcf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gilbsahyz.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/geakakxqc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/glnhndjxb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ghpbbugdy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gbljdijxv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gepirhcor.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/ggjgxxsfs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gwkpcbjhe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwgkayvbt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/ghqjsjadd.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/gethtwnab.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gyhbogjac.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gslzsrbym.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gzypyjroz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gzmtrbqkx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gcwzrmclr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gkafklgat.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gjxokfcch.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gfoliowyp.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/guyyfqcax.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gmrbekvdq.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gvgmldcyo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gjtkpmdrm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gngcwrnlc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/grylbgxcl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gsuspvaup.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gzynzrniv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/gjharwkeg.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/ggccyskhd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gjwhsogbj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gpdvbmnbi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gnczwcrmn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gltxtylqa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gzwcjlmll.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gzucrvtwf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gcrqscqai.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gcofzisvo.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gcnpneogr.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gbamedjne.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gdxmokrgo.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gvwgskepc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gbobpqanz.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gdffhgwve.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gntixzton.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gqaxheqft.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gedilfeig.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gmjwcouka.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gzdffiphk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gygttizyl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gonnrnngx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gqjolbeht.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gtxjcnffq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gqlkjndsw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqedcerpb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtmirduyf.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gjapjuygb.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/glarkjlpi.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gnxmyymjt.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gkztwtdsr.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gnlkiwjvf.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gdcwrwhtb.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gzgncvoix.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gamkahmkw.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxshlavft.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/grnkilzgq.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gksquflin.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/getecrzvi.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gdzpvuuah.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gmmjwljvz.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gjsegvzog.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/grkiqhogi.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/guzomkotn.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gzralumrp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzlvsvfyq.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gipmytmsv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmdywkugb.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gavgadrft.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/greetvfge.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/ghauorqij.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gyjefsazz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gqlcmetjx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gwamjtgja.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ginbbczun.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ggaeqmnmk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdxwgafdb.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gfrsdecfj.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/glgfxqqvp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gkjhyqozc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gdgtsrwqy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gswdhatmb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gxofnurly.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gnqvvzlxe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gifbrhilu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/guojpfuuh.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gqngnvjpr.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/guglozzat.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxamtmbl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/ghwlfmwoc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gxfdvpkni.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gvpnwuawi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gmxmyxqji.sHtML


<!-- 参考信息 -->