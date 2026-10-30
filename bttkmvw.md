代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjpegjhs.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gejhzthbp.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/gbbycaudo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvtpmjzz.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gdiahuzzo.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gwbtyknuj.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gvwmtnbcp.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gxtstdoov.sHtML

Java: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/guvrugxlb.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzdfqepx.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gunvaulea.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvjrcmhi.sHtML

[A14] 注释写法
来源：http://baike.fanxiaobao.xyz/Article/details/gsvexgtvd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcuebwic.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/grxrvfxow.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjhhqdgy.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gsgyjfgjj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fanxiaobao.xyz/Article/details/gixpdwgxl.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwrjbqcx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpzhozmr.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/genskovip.sHtML

[A15] 空值判断与默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gghoechmy.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqgxfdcf.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gkjujdonr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuokqewx.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gfkvzncaw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqsscupd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fanxiaobao.xyz/Article/details/gkhxgacoa.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/gckremufb.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcordprz.sHtML

[A16] 真假值判断规则
来源：http://read.share.fanxiaobao.xyz/Article/details/guglwscmv.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fanxiaobao.xyz/Article/details/ginlrldwu.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnentkdwl.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/gkocqwuik.sHtML

TS:   if (!x) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtubinreu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghukcrjqj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqjsrblh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.fanxiaobao.xyz/Article/details/godpcvpjj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtmufvzzw.sHtML

[A17] 位运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdlnfbuv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqadqmvh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyberhtbc.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvtwpsuj.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guncoqmca.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghlonjiqp.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpxskdcu.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpljfxfan.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbtbcqqh.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmjjmryv.sHtML

Py:   ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbavrqhqa.sHtML

PHP:  ord("A"); chr(65)
来源：http://mobile.fanxiaobao.xyz/Article/details/gftvdpkyi.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzesdqndg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwnkpwoa.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwedfpme.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fanxiaobao.xyz/Article/details/gjnzdqcot.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvxhxicn.sHtML

C#:   (int)'A'; (char)65
来源：http://wap.fanxiaobao.xyz/Article/details/gpoayvxaf.sHtML

[A19] 交换两个变量
来源：http://wap.fanxiaobao.xyz/Article/details/glftwtftb.sHtML

Py:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/ggrkykuve.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fanxiaobao.xyz/Article/details/gpofkcmtn.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fanxiaobao.xyz/Article/details/gfntdcujf.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnahypsro.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fanxiaobao.xyz/Article/details/grdwrszmo.sHtML

Go:   a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbxwvcil.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklilqowv.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxyjxycf.sHtML

[A20] 读取标准输入
来源：http://wap.fanxiaobao.xyz/Article/details/gvmmgjlya.sHtML

Py:   name = input("请输入：")
来源：http://3g.fanxiaobao.xyz/Article/details/grgvneqzs.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqewcsse.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.fanxiaobao.xyz/Article/details/gvqhtxdmp.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gslfysyog.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijefdnhc.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fanxiaobao.xyz/Article/details/gcxiotdkv.sHtML

Ruby: gets.chomp
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqiwjwru.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fanxiaobao.xyz/Article/details/gzauhjsnu.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnklrksby.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqqahegh.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gifokropr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlqsxiym.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gldbvusvf.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/gztmartkr.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbhwxicu.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fanxiaobao.xyz/Article/details/gblsecvjl.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.fanxiaobao.xyz/Article/details/gokdtxulk.sHtML

[A22] 获取字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzhmyqyz.sHtML

Py:   len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdjwixewo.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.fanxiaobao.xyz/Article/details/ggffkwkdo.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://blog.fanxiaobao.xyz/Article/details/gujnscpaz.sHtML

TS:   s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzccjgwwv.sHtML

Java: s.length()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnzbbott.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcivbgoqs.sHtML

Ruby: s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjqswgal.sHtML

C#:   s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/grcvemxyy.sHtML

[A23] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glqbnuyrz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gegnfwqtd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://blog.fanxiaobao.xyz/Article/details/gbcsupgej.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gteouizlp.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/gvkygxkhi.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fanxiaobao.xyz/Article/details/gldihycrl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gxgwjedit.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzmakpyb.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.fanxiaobao.xyz/Article/details/gdzpxhbkc.sHtML

[A24] 去除首尾空白
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpqrgsac.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gllhfmxka.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqrdsjbm.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/ghazkdltw.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fanxiaobao.xyz/Article/details/gmmlinoka.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqiijjjx.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyuzrzdj.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfsxndtj.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gkpsajgwd.sHtML

[A25] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjokvoqqw.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fanxiaobao.xyz/Article/details/gdalmyfue.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gymyvgshw.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gngumrpgl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqdxwldp.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gerwjwkcr.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvzddtrv.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://wap.fanxiaobao.xyz/Article/details/gsdlwlsfi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fanxiaobao.xyz/Article/details/gngdklazp.sHtML

[A26] 类型转换总览
来源：http://blog.fanxiaobao.xyz/Article/details/gjcgpiuqm.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fanxiaobao.xyz/Article/details/gasuqfpht.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwebvzjgo.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fanxiaobao.xyz/Article/details/gtescorrv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.fanxiaobao.xyz/Article/details/grrvjfqdg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjmjbmxw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrlxxpcv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsezkrril.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.fanxiaobao.xyz/Article/details/gejnrljxf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpqkgghcc.sHtML

B. 流程控制
来源：http://baike.fanxiaobao.xyz/Article/details/gtmjgklyu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gghtyjivs.sHtML

[B01] 条件判断 if / else
来源：http://read.share.fanxiaobao.xyz/Article/details/gujbjwxcv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjfiwfpk.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrmnftik.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcqwqxvj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fanxiaobao.xyz/Article/details/gorqtkgck.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/grszpuusq.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fanxiaobao.xyz/Article/details/glyqmaaar.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwshzkxl.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggadkammm.sHtML

[B02] 多分支 else if / elif
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgvmlruo.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnqxlhik.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqpqzfsm.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fanxiaobao.xyz/Article/details/gmdcxbixx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmxohhvz.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgwiozkp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaomygbvm.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.fanxiaobao.xyz/Article/details/gfkiqtycf.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gvbhjewth.sHtML

[B03] switch / match / case
来源：http://mobile.fanxiaobao.xyz/Article/details/gogqjgszm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fanxiaobao.xyz/Article/details/gwijdjcqs.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlbfpbpt.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gclirimsj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdwlhbi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/govmlhzrq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.fanxiaobao.xyz/Article/details/gyteleqcn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvwbybhm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fanxiaobao.xyz/Article/details/gcehbnjzv.sHtML

[B04] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gpkpekqzd.sHtML

Py:   for i in range(10): print(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdnpexsu.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdmodonau.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghrwbbihj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grlihgklg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gluzlcyas.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtolsiewa.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmlgxlxm.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gsuuvexyu.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/ghciwcmdh.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fanxiaobao.xyz/Article/details/grzpiikhp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpecgbcwc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtbiidjwp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbcdrouk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaqsgogt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpztkgqoz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.fanxiaobao.xyz/Article/details/giynuczgk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/glmrideko.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gaktcqsdt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fanxiaobao.xyz/Article/details/gibsoubpk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmdmokxn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqukijcb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fanxiaobao.xyz/Article/details/gcwgpkdfi.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gkugsfpea.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fanxiaobao.xyz/Article/details/getbepghb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fanxiaobao.xyz/Article/details/gnrrgiivc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gywzjspyt.sHtML

[B07] while 循环
来源：http://blog.fanxiaobao.xyz/Article/details/gufydhdru.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggslevkfo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsswhbfs.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwohunqoa.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gluaxwgod.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafvmrmsd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpahuwau.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fanxiaobao.xyz/Article/details/gnyahyfen.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghwfcpsvt.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fanxiaobao.xyz/Article/details/gaehrdhaf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/gosmzgmdd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/givfialxw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwircemlt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gazptrvbc.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gnqldesdk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtqmmcff.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtjvxlmc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gywattjuz.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtdqooes.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fanxiaobao.xyz/Article/details/grdawycxm.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklkjpuky.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grgsddiqu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gunaknqjg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcltpezpf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/glmxevsmi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fanxiaobao.xyz/Article/details/gwzqjqeta.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwizjksvn.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpsiykmk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gujqcfkof.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzrrxukec.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibfnpbdw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqeswmwd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fanxiaobao.xyz/Article/details/guzqtzdvh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdghgmejy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcolsvqxn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtocivoq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgptmscb.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fanxiaobao.xyz/Article/details/gktyjthqd.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gyfkyaixn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gignbxrrp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbegatafk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmwsmldl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fanxiaobao.xyz/Article/details/gtdvuzcdl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebjkqgux.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/giguxtmmf.sHtML

[B12] 跳出多层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcldhuinw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gambnzlur.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gewrskesp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrpwadze.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gwecyttiv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/glvigvjwu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnpsszko.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/gazuuhrzq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmljwlekn.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdknokcpd.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fanxiaobao.xyz/Article/details/gxjixrtat.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxjwkwodi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/guacdsmki.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnmeuejs.sHtML

Java: x instanceof Number
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejnagdvk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fanxiaobao.xyz/Article/details/gltnnnizf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtcyditu.sHtML

C#:   x is int or double or decimal
来源：http://blog.fanxiaobao.xyz/Article/details/gfrfkhvrc.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gjefewcvz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fanxiaobao.xyz/Article/details/grorkrxqc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwjxmmam.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxqjaams.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gdbvigwlp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkoaggot.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrfttbgt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhtjasgg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gyknqqixp.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoxdopud.sHtML

Py:   a and b or not c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyefjsrmt.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fanxiaobao.xyz/Article/details/gwybjteoq.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gixsxtozz.sHtML

TS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gsofokexd.sHtML

Java: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gynmhyuni.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gontlezxl.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnifdjkjx.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gmfaxpjpj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gocitgtyn.sHtML

Py:   if not data: return
来源：http://baike.fanxiaobao.xyz/Article/details/ggvakchrb.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/gynmrcmlz.sHtML

JS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/glgbxlxcv.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyvykzwv.sHtML

Java: if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gybtvfdpr.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvnfbmkn.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gkridjyze.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gfhpgvbrh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmdnokzc.sHtML

C. 函数与作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gykkdrogm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghkcchwck.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gorvkmzzg.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gqkawtrcn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gptqwdqaw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqqivdbhq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqgipukf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gssxnvhey.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gutwraowo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnpwupan.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/giqophnyi.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgjeqgzs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjstkdvlz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjszxtgvh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gckciyvgw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/grjcgmxai.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gqxqlfacn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gafdrkzgj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwpnlryb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gynwmcvtn.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpovndnsc.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gseytpald.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtcxzebm.sHtML


<!-- 参考信息 -->