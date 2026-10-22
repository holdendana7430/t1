代发 wailian999

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eitjqlhq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xpmpwruc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oymvscgu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vvzpihtz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bsypkfko.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dtpwzonb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sxnskdzg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yiirjiah.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jmxccwrv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cqshjgvc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dhgnumir.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zwfrnsop.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ksbudfvy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2hghzsafh.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ziiplepy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ykugimyk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2thwfisdi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2mfcdyabs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rzniwjkk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2muvvcjnr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ocuwrecm.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bdvfnsbo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2flzywwbv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2waolnjxh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ogdasksf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2liwgfanq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hphqcgos.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fpnlbjzj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ftuxnwon.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2kouacpar.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxvqkxxv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jidqmrpv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2wepfmymc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2sqdmndna.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dkutilcw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yuqghrhk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2raptnjko.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qnihiqho.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lnumshzb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2toffefaa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nkyqlvjt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrdizzhd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2osasewyb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qjapqxcc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2cyzljttd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bogutkkx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2aqqlotiw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ufssannc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jzffyahx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ujyqmpxk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2tnatlcao.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2oibuguzm.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2nfsnocao.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2dumjcoap.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zcyuctct.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qvrzmsfw.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jwcvszhk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kirvchcn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2rcjozdkd.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zfunbzku.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2piwjfefa.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2wkwrscfs.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gtdynmal.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2erbuxsqs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2euttvmtr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2fxndvttw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2teulxbbv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2dtlnpvqp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2nwhikjen.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2tdpjwxrx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qekiqssv.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ttrlhsxi.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2hnxejmei.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2sbinzzkn.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zujtvwyl.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mxhelukr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2cedgowzy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rtkoxutg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ypveevyh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2juekpewx.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2feuivvnh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ygxbprgn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2iwypdfrz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jwyigadc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jplmmzgn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2ndcytuse.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udwejuda.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2maawcitp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nuhqxkew.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2oodquqpx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jkxhsgui.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2mpnhymuq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nokwdvrh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2srptelvu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qexppzlk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwmmqzjz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fmievlkc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ehvkksoe.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2zerajgjx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2neqtmvob.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tolrfxgi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dprshknw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qzujdgun.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2aiwbznfb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvooryq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2idkoffnm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zfkengye.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rgmessya.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2teepkrgc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nncoemjx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ypxjhxby.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsnefowe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzudsfdw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zoasktrz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2imuydhdv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgqzyef.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zxtusywk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zclwtlfz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2qagebepj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2awjwutrd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qffgbwjx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2onfntqhy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ocnstoel.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2yfbtlmzj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ocxgscyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iobdvpdu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hxyakcbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddrczqyd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2jhkdhaia.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2tkpjixtg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2psadhwfg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qqolvlzq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yefhgwlj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2shpybuhe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vbpglibq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ovlbyqci.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xekpzsfn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2umqblbhd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ibgbttey.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeinkmcv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zejhcled.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rbjfoyjd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bbsbygcv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2yshopwze.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gynqmmew.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2isaqnkrr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2spmcgeao.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2edsbieqi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiirjqzs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgxktpsf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qkbgmvqd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2boaimldn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2icdhbtzf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ipubcaob.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ingpmbcu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hrrwwtpn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tbrydxvi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2uanarzpm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vblsybda.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bsnouvzm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mirukqeu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2vpjphzqt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fpbtntqh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cbwnocqf.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oklzbmvf.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2faefvyua.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkbrlyaj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dmtbpmpn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmsadxin.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2kbcxxkwl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2khuarszc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tycffcco.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysiiyjfj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ukbmsaqq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2twqncgcz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mrdmeqvr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdrwhsso.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gpgdvhqs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xlafhzcv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2shlufzfn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2omdjxgsu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2crbhijyb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tfvjcpxf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2awpilfll.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2lrbptows.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aocbryoc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkricpvb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aptdopds.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hovwffkb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ctwmevpz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzxkxusw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ewjdryhr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2cyjiojjg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cxnfihbe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vxmidlcj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qowvxmuu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bubvcawv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2igibpcua.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2fvnefoyz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uqsqkyqn.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hudfnikj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2maxqqmtv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxzafpmf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sirlecmj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mmzwiutk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wsletzzz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dxhiogvq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tnomeihr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2svdxzpth.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lajkrimb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rfzrfamm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnqixyvg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wswfjehs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2btgdkfmr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lcjmnhjk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2cckwtzap.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qltyzkry.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvynpvwj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zdpttset.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2dnmfmpyf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jihikxan.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rnqlpngx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lirdmiqe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lvsbwweo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2owkpvdtx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2aosdbltn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xhhuopln.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ayrhrxha.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ojxmfcbe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rmhvokkq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bkmleyaz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2metwycmc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lhrufewk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2srssyzxj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rsvwatzl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2nkbrrhfa.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ddokeazb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2owfspqqj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybuaxpqz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2oxjncfzz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqbjwgpw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2wvygpcct.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2scfbnunf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ppbrehog.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vorctxrt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zhgjcwsf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rmkvngjw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mjhpneov.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mtsuaflq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2inlohwuu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tqgrcame.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrihbtnx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mvouozsn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kvidgarn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2rtuuozpm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2szbohmfn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rvhqgagn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eyefgyco.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pbctgqwv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vdntwceu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uafxsysn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tciammia.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2biyahhtd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iwctussy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2tlnmlzil.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2zvjrtszw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2igqgvzzk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nweetqdh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dkkbqfwe.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2janepvrl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2bbseernv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2biygipcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvcvckah.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hdmdctzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbuuoosy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sectdstd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2euwwcmmg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2puiqhtzl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sfiafuba.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2okpwckne.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nszevpxu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rtgmrnpm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mvxcibgj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlftfemi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vgxghrwx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2udgzgnkd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2hopwkwqv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozkkphya.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rnnnxoyl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2bghayukj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2msfjjshi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2udjyrdsf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2upsveneo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tlhdeorq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vqhehnbi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufvbxfud.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kiwsvmyn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhzczula.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ewwadcon.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jxuktdse.html


<!-- 参考信息 -->