代发 wailian999

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gdfadvpko.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.hesvh.cn/Article/details/gvzcstksc.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gigrdnkwj.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/ggrlsmwze.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gnkbmdknt.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gkkgfaefv.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gzeojjhoh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.zdbjq.cn/Article/details/gfextlkal.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gqvbkdbsh.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/gizbhalmm.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/grkooxlkj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gfkehlpur.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gvaavtmzj.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/grvqfidlx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gfmwtjpmi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/ggnlmjafv.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gdfvqsnaw.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gliupdgzu.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/gravuasnu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.fehbvm.com/Article/details/gybmykyby.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/ggvkoikqo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gggrncxzh.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gdrrlowkt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.hesvh.cn/Article/details/gurdqpwec.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gqxiebdda.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gmsxkhqsl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/gezwjeaqo.sHtML

[A17] 位运算
来源：http://3g.hesvh.cn/Article/details/gyficwhkm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gremijqgx.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/gqskvyntt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/giwjezove.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gwdjvfyos.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gdmygpidx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gdjsohfbk.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gtthagedg.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gtpbuldug.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.hesvh.cn/Article/details/goipkfxvm.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gphkeullq.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/gflqjgtom.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/grtfkmnqj.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gycnelwqt.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.zdbjq.cn/Article/details/gfrzmixvj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.m.share.zdbjq.cn/Article/details/gakvngjoh.sHtML

Ruby: "A".ord; 65.chr
来源：http://wap.fehbvm.com/Article/details/gsxkggpki.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/ggqpvkrgh.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gsejpwmfa.sHtML

Py:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gxrdlzybg.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.fehbvm.com/Article/details/gqppzzijf.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gprjkxrrj.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gsytpuukb.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gxbxvnfkx.sHtML

Go:   a, b = b, a
来源：http://wap.fehbvm.com/Article/details/gxpnhhlgu.sHtML

Ruby: a, b = b, a
来源：http://m.share.zdbjq.cn/Article/details/gxvvvqyev.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.zdbjq.cn/Article/details/gyjcehiad.sHtML

[A20] 读取标准输入
来源：http://www.blog.fehbvm.com/Article/details/gyhdnmkfq.sHtML

Py:   name = input("请输入：")
来源：http://wap.hesvh.cn/Article/details/gsrpzdqkb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gvyvxglzl.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.zdbjq.cn/Article/details/gbuoyoiyy.sHtML

TS:   // Node.js：readline 模块
来源：http://mobile.fehbvm.com/Article/details/gmapnwbig.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.fehbvm.com/Article/details/gzkoyafbg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.zdbjq.cn/Article/details/gixjzbrqe.sHtML

Ruby: gets.chomp
来源：http://read.share.zdbjq.cn/Article/details/gfntdacjx.sHtML

C#:   Console.ReadLine();
来源：http://blog.zdbjq.cn/Article/details/gttivrdpq.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.fehbvm.com/Article/details/gxqtjnojx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://3g.zdbjq.cn/Article/details/gfxpwggzu.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gitlorqgb.sHtML

JS:   (3.14159).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/glsgqpsig.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gtlaismxt.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gdnmkzkvx.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/gwmraqsbd.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/godlccvvn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.m.share.fehbvm.com/Article/details/gxsculhkx.sHtML

[A22] 获取字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gebllyxat.sHtML

Py:   len(s)
来源：http://mobile.zdbjq.cn/Article/details/gxsfdowkh.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/gfkreatjt.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.hesvh.cn/Article/details/gnsxivgoi.sHtML

TS:   s.length
来源：http://mobile.zdbjq.cn/Article/details/gcdtimedb.sHtML

Java: s.length()
来源：http://baike.hesvh.cn/Article/details/gplziugto.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.hesvh.cn/Article/details/gqhcklkvn.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/gjqizwihi.sHtML

C#:   s.Length
来源：http://mobile.zdbjq.cn/Article/details/ghhbrgmys.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gbhgmtsuf.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.zdbjq.cn/Article/details/gndtwhqab.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.hesvh.cn/Article/details/gbuwjecvg.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gbkqlrmdo.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/gzgzmetba.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gndbvxqfb.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gpcnsqczt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gklzpozvz.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.hesvh.cn/Article/details/glmbaaant.sHtML

[A24] 去除首尾空白
来源：http://www.blog.zdbjq.cn/Article/details/gxzjbrxzw.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.fehbvm.com/Article/details/geodtddqv.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://3g.zdbjq.cn/Article/details/gogvjealk.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gcumpwdnu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gwybiadxq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.zdbjq.cn/Article/details/gpvafpipd.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.zdbjq.cn/Article/details/gckluimhr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/gxuxdugzj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.hesvh.cn/Article/details/gtkuinnmy.sHtML

[A25] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gsqdtvpct.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.blog.zdbjq.cn/Article/details/gzvhufaoh.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.hesvh.cn/Article/details/gxxhvijid.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.zdbjq.cn/Article/details/glpellvpd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gasdqkrpp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.zdbjq.cn/Article/details/gypwiqtbg.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gwfssoiat.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/gpxftnpki.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.zdbjq.cn/Article/details/glzzvjmfo.sHtML

[A26] 类型转换总览
来源：http://3g.zdbjq.cn/Article/details/gavwnunzb.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.fehbvm.com/Article/details/gyqfojtly.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fehbvm.com/Article/details/gzlsuyktv.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/glhbnslag.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.m.share.zdbjq.cn/Article/details/gmbvxyzog.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gsijsmiul.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.hesvh.cn/Article/details/gfknipsex.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/gsbmberum.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://read.share.zdbjq.cn/Article/details/gubzfurzx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdecrwsrx.sHtML

B. 流程控制
来源：http://www.blog.zdbjq.cn/Article/details/gdveqcbqy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gihnrfrxe.sHtML

[B01] 条件判断 if / else
来源：http://wap.hesvh.cn/Article/details/gatpnbdwb.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/gjtiahfay.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.zdbjq.cn/Article/details/gckfqueaz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gnleqaqjj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.hesvh.cn/Article/details/gldumdmyx.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.fehbvm.com/Article/details/gmmjsihqe.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fehbvm.com/Article/details/gvygsatuf.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.zdbjq.cn/Article/details/gcwrrywgv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/ggvcfhkkz.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.zdbjq.cn/Article/details/gdrztaesf.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.blog.hesvh.cn/Article/details/gprdjabii.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gbsmkkqlp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/grsryqmjz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gzqqigdyn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gnauajriv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gtdqpzlwa.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gjcuywluy.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/grfnhcdhv.sHtML

[B03] switch / match / case
来源：http://wap.hesvh.cn/Article/details/grybdhjoa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.zdbjq.cn/Article/details/glgmsrtss.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gdlsvakpx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gtdjqnyad.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gktgjitte.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/glxbikodk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/grapuuqos.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gfidqdbss.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/gjlgdnnda.sHtML

[B04] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/ghxrxgzkb.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.hesvh.cn/Article/details/gtbadunoe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gumuywnzq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gsjhpoflb.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.hesvh.cn/Article/details/gfebjezat.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/ggdboxzrk.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gzxhrnlkl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.hesvh.cn/Article/details/gwtdwbpbn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gpurechok.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gvuwagtgy.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/glycwnisq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gfmgdywxv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gvjdekuzm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gpdcktpot.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gxhlsawrs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/gowdbtksy.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/ghgewedhl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gmfsdiojo.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gvarkgume.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gzrlxeusb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gybvuxqqj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gwautyyfn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gvjanuatj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gczndexex.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gtpxedhax.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gqoldnsxj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gtjgrnwop.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gndtxblyk.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/guplceblq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gsnugdwox.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gkslqufss.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gwsavfgkq.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gzsklquzy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/grumsrurl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gscroofeg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/grozibkxb.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gehdcyacm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gsuazyyux.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/grsrydyji.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gtdhcskay.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/guiqonadg.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gbqgvxqad.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gezvwcowe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gijevmkgd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gchzoxsrx.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gmgwsvuwe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gdtcjrpgw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gjmzpyvlv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gpxpbvgmz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/guvmgzrfi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/guejftgpc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gyrwwwajr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gdudsyaar.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/glvfywxyz.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gddempzqq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gpgefomwo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gqmbwbhwv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gcctwljzd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gtzibicpv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/glkejpfpc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/grvaxefdz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gidlnahrk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gsmppckov.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gzctvfarg.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gsslvczeh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/guxrnjhzt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gmoyvvuhl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/giiatamek.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gyhuggzqm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gjzdvzdcn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gxohnbjxb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gvmxkqwnh.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gmdtmxvlg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gqesnevlo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/glcylttlx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gmsvswxzk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gpkoabmqb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gxcrfahkm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/grbyaprsb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/ghtwohsru.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gmacyvxok.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gswnmueak.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gqerriucr.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gdhqoizgv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnvlwmzy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gevojoxwt.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gskwbyugp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gkqxztsgk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gxafbsrcv.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/giqdaqtsc.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gyiytjwto.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/grdzyraha.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gfromihbw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtweycjts.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/geawzdxet.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gbgrggxmo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gumtpshim.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.hesvh.cn/Article/details/gredtjwpx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/ggbxufilw.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gtygluczr.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gcehqiijm.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/ghipqacnh.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gmuwfuwkc.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grwjdenke.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkkzgmmbm.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gbdyrqjvn.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gpesseazp.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gqkdydxjx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gavbqhstb.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gosqkbjxb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gpwpucayg.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gkqsosocz.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/ghvgkopwp.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gdvdrczpi.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gjqskhbam.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gtmupaiwh.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gkmvvjspx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggkemvwsj.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gbbinzgdb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guhaztzgp.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gmnuavdqw.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gxedmwukz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gtvuwgcyc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/grwimekcb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gyyxgohpi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/guqzxzbue.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gvisysmyx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.zdbjq.cn/Article/details/gkqlbkyhu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gljvyssbf.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gwjaoynam.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gmfoxximv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glcfkenqc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gxxfxdtbn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gozkwweqc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gkyfebxgu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gkxlwdebn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gyisehdfs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gekvshuwi.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gibvivzhw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gbwbytknd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gyqfjwxus.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gkzmcqtfj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gnhiivtgk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gdazgcziw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/glwforwml.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gxpqjhgoc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gqhvtjyfg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gnfgahtzz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/ghhvufsqo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gmmwccylw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gklrwjyhb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gvqfxqwdg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/ggwiogvxj.sHtML


<!-- 参考信息 -->