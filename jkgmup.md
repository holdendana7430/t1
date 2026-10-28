代发 wailian999

[A14] 注释写法
来源：http://hz.zdqjudy.top/gtmnhmlpxu.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.tianlin.xyz/gtuddcwvgf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yangfankeji.com/gtrrhvnzar.html

JS:   // 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtloxztaca.html

TS:   // 单行；/* 多行 */
来源：http://hz.ybcxt.top/gttefdxkvv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.guannengcc.top/gtzaniwzjw.html

Go:   // 单行；/* 多行 */
来源：http://hz.xylfe.cn/gtvnroyrsy.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.cqqwz.cn/gteqvgdxry.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhiwuduotai.top/gtentfbzfi.html

[A15] 空值判断与默认值
来源：http://hz.daxiang520.top/gtwacbhstl.html

Py:   value = data or "默认值"
来源：http://hz.gaohongyu789.top/gtxonvfxlo.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.mhx1999.top/gtqdunlyug.html

JS:   const value = data ?? "默认值";
来源：http://hz.pycfn.com/gtjyheobjm.html

TS:   const value = data ?? "默认值";
来源：http://hz.0kj1m.cn/gtjnxhgiwy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.sxryk.cn/gtdoghgnlh.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.aizwys.cn/gtfxbijybe.html

Ruby: value = data || "默认值"
来源：http://hz.guannengcc.top/gtfgguxask.html

C#:   var value = data ?? "默认值";
来源：http://hz.hysaishi.cn/gtcooskyta.html

[A16] 真假值判断规则
来源：http://hz.hongshengwenyu.top/gtbboxenxz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.vqdsnc.cn/gteewtozgm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.mhx1999.top/gtpmxommah.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hnqzz.top/gtkqwxsyxf.html

TS:   if (!x) {}
来源：http://hz.zycfv.cn/gtqjtwgqba.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.xingfuxueyuan.xyz/gtvyfkckau.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.daxiang520.top/gtkrhtkdtk.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.yanxiufei.cn/gtbwlundmp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jinqigufen.top/gtbamiusql.html

[A17] 位运算
来源：http://hz.sysykeji.top/gtmfgsbtnc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtneddspjd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhijiandao.cn/gtmgvkccth.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.svipenyu.cn/gthrtdympi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.fengsongda.top/gtrncbxfqp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtazytyrie.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.haohaochexian.top/gtjwbugqmb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nwbrower.top/gtgvtcavjn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuetiantiany.cn/gttlkxopfw.html

[A18] 字符与 ASCII 码互转
来源：http://hz.feifeiyinyue.top/gtvvjzgvar.html

Py:   ord("A"); chr(65)
来源：http://hz.jiagoushi.top/gtqzyqnmhn.html

PHP:  ord("A"); chr(65)
来源：http://hz.jinqigufen.top/gtcumckqov.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.guannengcc.top/gtuwdsdwtl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jqgufenzy.top/gtbltzqvyk.html

Java: (int) 'A'; (char) 65
来源：http://hz.zdqjudy.top/gtqlvtruff.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zhaomingkeji.xyz/gtjtxchhku.html

Ruby: "A".ord; 65.chr
来源：http://hz.shanyushiyangtech.top/gtjymyyryo.html

C#:   (int)'A'; (char)65
来源：http://hz.sysykeji.top/gtzsphvoye.html

[A19] 交换两个变量
来源：http://hz.daxiang520.top/gtrlkcvlch.html

Py:   a, b = b, a
来源：http://hz.hammf.cn/gtmgmthokw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jqgfzy.top/gtrxyhmwzh.html

JS:   [a, b] = [b, a];
来源：http://hz.daxiang520.top/gtdsygakrg.html

TS:   [a, b] = [b, a];
来源：http://hz.ydjk.org.cn/gtnrlotdyh.html

Java: int t = a; a = b; b = t;
来源：http://hz.jianghu66.top/gtelkpizch.html

Go:   a, b = b, a
来源：http://hz.hywenlv.cn/gtpwcpngty.html

Ruby: a, b = b, a
来源：http://hz.zdqjudy.top/gtxquibgzv.html

C#:   (a, b) = (b, a);
来源：http://hz.xinyue.icu/gtpgnxkshg.html

[A20] 读取标准输入
来源：http://hz.zhaomingkeji.xyz/gtfdleaoae.html

Py:   name = input("请输入：")
来源：http://hz.wangdashe.top/gtbsprsiec.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.feifeiyinyue.top/gtelyoxzfr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.shuidangran.top/gtbotlrqqc.html

TS:   // Node.js：readline 模块
来源：http://hz.aibaodan.cn/gtfeefrvbf.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.guannengcc.top/gthfawnyjl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhixingplan.top/gtlfnwvrmt.html

Ruby: gets.chomp
来源：http://hz.snrcjt.cn/gtuxqwcnnv.html

C#:   Console.ReadLine();
来源：http://hz.tianlin.xyz/gtkoxgksie.html

[A21] 保留指定小数位输出
来源：http://hz.nanxinkj.top/gtsxrkweyd.html

Py:   f"{3.14159:.2f}"
来源：http://hz.sysykeji.top/gtgfpbpjgq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jianghu66.top/gthsecusww.html

JS:   (3.14159).toFixed(2)
来源：http://hz.hfpthk.cn/gttnfemnea.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yvedp.cn/gtgfsrjaqe.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gthnyawvpw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gthzeryjzf.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jiagoushi.top/gtoslelzef.html

C#:   3.14159.ToString("F2")
来源：http://hz.gotoacloud.top/gtymklcdlp.html

[A22] 获取字符串长度
来源：http://hz.gogol.net.cn/gtkvymfnih.html

Py:   len(s)
来源：http://hz.yongpay.top/gthlusebfq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.nwbrower.top/gtrxfnqmxw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.sweek.top/gtvisldxfr.html

TS:   s.length
来源：http://hz.cheryme.top/gtbfxpxauk.html

Java: s.length()
来源：http://hz.gogol.net.cn/gtrmkrfhlg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.vqdsnc.cn/gtmywmiabv.html

Ruby: s.length
来源：http://hz.gotoacloud.top/gtvvvoohrh.html

C#:   s.Length
来源：http://hz.bjfxy.top/gttrszdazy.html

[A23] 大小写转换
来源：http://hz.jyoumei.cn/gtfgudfetj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jqgfzy.top/gtkfqaqcru.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yuxming.cn/gtyuogqjux.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.redwolf501.top/gtbgcaxbhx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.fengsongda.top/gtbjbwjthx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yvedp.cn/gtczfmitxx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinyuanbaomall.cn/gtjisgzwqb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinyuanbaomall.cn/gtgqlzlwzr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jqgufenzy.top/gtdkmfymhf.html

[A24] 去除首尾空白
来源：http://hz.haohaochexian.top/gtbqomrgrf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.xingfuxueyuan.xyz/gtajvtsgtb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.iojbl.cn/gtwqouaoyk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yangfankeji.com/gtlgwgyrgy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hongshengwenyu.top/gtvdvwwzwz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.haohaochexian.top/gtmwlzqwmd.html

Go:   strings.TrimSpace(s)
来源：http://hz.kuanghao11.cn/gtrsdrkjuo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.sysykeji.top/gtmlgbkvsu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.xuanzx.com/gtsdducgxo.html

[A25] 字符串比较
来源：http://hz.guannengcc.top/gtikezwgvd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.vqdsnc.cn/gtapxbrpar.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yvedp.cn/gtvapcgyip.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hywenlv.cn/gtyrfwkfds.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigufen.top/gtnlzmtwuf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hnqzz.top/gtjgggekpm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hfpthk.cn/gttfthsfev.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hnqzz.top/gtfndzxxyn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ywan-chungtsiang.top/gtqzejevgk.html

[A26] 类型转换总览
来源：http://hz.hfpthk.cn/gtregzfkca.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zdqjudy.top/gtbkwpbtbd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yangfankeji.com/gtsgydmrvj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xingfuxueyuan.xyz/gtujzsclxy.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhoulong.xyz/gtldlwdaqq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cucudq.cn/gtoleaffhl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.snrcjt.cn/gtofbwvzct.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.smart0.xyz/gtdyzokzrn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.aibaodan.cn/gtwknnoaaa.html

================================================================================
来源：http://hz.dianchejie.cn/gtsgecjchf.html

B. 流程控制
来源：http://hz.xylfe.cn/gthpketevt.html

================================================================================
来源：http://hz.cucudq.cn/gtgmlqqavu.html

[B01] 条件判断 if / else
来源：http://hz.sufxvd.cn/gtxhviivti.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ydjk.org.cn/gtvyeqxoil.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.chenzaomai.com/gtcsbedmjc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.haohaochexian.top/gtuqnjzqxh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtunercknm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yvedp.cn/gtjdhiduup.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jqgfzy.top/gtkgohnteu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.pengpengdd.cyou/gtqpexkghl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtnwqlygxo.html

[B02] 多分支 else if / elif
来源：http://hz.xylfe.cn/gtarskfvpx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gogol.net.cn/gthqsgahkb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.guowangkeji.top/gttferutfk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cqqwz.cn/gtlmxljrjo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nwbrower.top/gtdidjkwfd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.fzhhl.top/gtbwljehhi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xuetiantiany.cn/gtdpiltlog.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zycfv.cn/gtqboqluqd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shzxlz.cn/gtrykfmmcr.html

[B03] switch / match / case
来源：http://hz.hnxiangtu.top/gtwthmdbko.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.vqdsnc.cn/gteskttogo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hysaishi.cn/gtnbfwvgre.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtpahimhii.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258888.top/gtchvzcgwu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hysaishi.cn/gtchvrwqru.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.smart0.xyz/gtmbmccoan.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.nanxinkj.top/gtbsappatc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.mhx1999.top/gtrdrzfpgj.html

[B04] for 计数循环
来源：http://hz.sufxvd.cn/gtffjnfljk.html

Py:   for i in range(10): print(i)
来源：http://hz.yuxming.cn/gthjeilztk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shanyushiyangtech.top/gtgfvyraim.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtuxlleuko.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ywan-chungtsiang.top/gtwjcpaiit.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.daxiang520.top/gtkhubltha.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cheryme.top/gtjxgknyom.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yj20258888.top/gtcssadpgj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.pycfn.com/gtccrbkcok.html

[B05] 遍历数组 / 列表
来源：http://hz.yonumen.top/gtbzvvqfan.html

Py:   for item in arr: print(item)
来源：http://hz.nwbrower.top/gtgmabnqkk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ywan-chungtsiang.top/gtojwdprtf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tianlin.xyz/gtpjhgjnyq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhijiandao.cn/gthgogvitb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhaomingkeji.xyz/gtuwapcumt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cheryme.top/gtgtxdlwlk.html

Ruby: arr.each { |item| puts item }
来源：http://hz.redwolf501.top/gthysixonw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zycfv.cn/gtzbwkzvhm.html

[B06] 遍历字典 / 对象
来源：http://hz.shanyushiyangtech.top/gtpxfqwdno.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.52xcode.cn/gtvdhzcmxr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xingfuxueyuan.xyz/gtjkopnjfr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jyoumei.cn/gtjrfvygys.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.feifeiyinyue.top/gtftobxsbe.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ivvv.top/gtbusneuft.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ybcxt.top/gtuywywnnu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jiagoushi.top/gtztiwkmhj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.nanxinkj.top/gtjjmenfsa.html

[B07] while 循环
来源：http://hz.yj20258.top/gtkkmmwoyr.html

Py:   while i < 10: i += 1
来源：http://hz.zhijiandao.cn/gtjsccnawf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.aizwys.cn/gtlkydotgg.html

JS:   while (i < 10) { i++; }
来源：http://hz.birdmap.top/gtlrxmkjmh.html

TS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtfjabpkbc.html

Java: while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtfjzmgbbx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj202588.top/gtdnvycgdt.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hongshengwenyu.top/gtvtepgkmb.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtbhaplfgy.html

[B08] do-while（至少执行一次）
来源：http://hz.shangyingyoupin.top/gtapckohuy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cdnleiting.top/gtkegztklq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.birdmap.top/gtnesbhamb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtdnikrgph.html

TS:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtojyhpzyf.html

Java: do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gthqkavxci.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.tianlin.xyz/gtxaesidvx.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.fzhhl.top/gtfduaajbs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtrxncoaav.html

[B09] break 与 continue
来源：http://hz.yueranfly.top/gtynoxcdxf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.havefunace.top/gttgxabjxq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.andypj.xyz/gtcmtdfuwg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtpmoakekt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtwvyfpjbk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtodtjilpm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shanyushiyangkeji.top/gtgiekmmiq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ppjwa.cn/gtvokzvmmf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtgqztsjqc.html

[B10] 遍历同时拿索引
来源：http://hz.sufxvd.cn/gtqecsdhow.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gaohongyu789.top/gtxpngoesp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xziqi.cn/gtxglkkkcj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gtwklmqlnd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dashuyun.cn/gtyzaomrlj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.gotoacloud.top/gttacconlq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ybcxt.top/gtwkfqxcmx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tanke756.top/gtgzaldauv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tanke756.top/gtmmosjwju.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhongyouzk.top/gtwksmpknl.html

Py:   list(range(0, 10, 2))
来源：http://hz.xinyue.icu/gtnsplojxe.html

PHP:  range(0, 10, 2);
来源：http://hz.cashguo.top/gtiibgknmd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgfzy.top/gtwztebgxw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtjoumdukw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtpawnxywn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.chenzaomai.com/gtfhokbhqs.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tianlin.xyz/gthbnyilkx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jlsjyb.cn/gtearhaigs.html

[B12] 跳出多层循环
来源：http://hz.gaohongyu789.top/gtvjhrkcjw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gotoacloud.top/gtphjkjbkf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.nanxuanxn.top/gtftmhjisu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtlopaqitq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtqsepnfkl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtivnbekmj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xziqi.cn/gthyrqgqdk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gotoacloud.top/gtubndpuhv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xinyue.icu/gtlkdxrrsk.html

[B13] 判断是否为数字
来源：http://hz.jianghu66.top/gtmepopmmr.html

Py:   isinstance(x, (int, float))
来源：http://hz.cucudq.cn/gtoyqhttfp.html

PHP:  is_numeric($x)
来源：http://hz.zhijiandao.cn/gthyxcbfkg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shangyingyoupin.top/gtmvludkyh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtujhkzsiw.html

Java: x instanceof Number
来源：http://hz.kuanghao11.cn/gttojrmieh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jiagoushi.top/gtbkwpmbkq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ppjwa.cn/gtxiirziwi.html

C#:   x is int or double or decimal
来源：http://hz.yj202588.top/gtnstcqxly.html

[B14] 判断值是否在集合内
来源：http://hz.0kj1m.cn/gtgrgomhml.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.bjfxy.top/gtopyeoxsu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.feifeiyinyue.top/gtpstocskf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtuzuigecc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gtybhfuluz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.c1oappe.top/gtfxvtxvbw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daria6918.cn/gtdoajnaat.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.aibaodan.cn/gtdkzbgmgf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.0kj1m.cn/gtmasewuzi.html

[B15] 布尔运算与取反
来源：http://hz.feifeiyinyue.top/gtxvktnrfz.html

Py:   a and b or not c
来源：http://hz.sufxvd.cn/gtntirhqil.html

PHP:  $a && $b || !$c
来源：http://hz.cashguo.top/gtwjogoemb.html

JS:   a && b || !c
来源：http://hz.jinqigufen.top/gtpdofzyzd.html

TS:   a && b || !c
来源：http://hz.jqgfzy.top/gtohixkyql.html

Java: a && b || !c
来源：http://hz.haohaochexian.top/gtrysunous.html

Go:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtqkpwlnhj.html

Ruby: a && b || !c
来源：http://hz.jqgfzy.top/gtgldpgubi.html

C#:   a && b || !c
来源：http://hz.redwolf501.top/gtlehjzzpo.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cashguo.top/gthfobgtts.html

Py:   if not data: return
来源：http://hz.zhixingplan.top/gtukdrhefg.html

PHP:  if (!$data) { return; }
来源：http://hz.bjfxy.top/gtbjahmftk.html

JS:   if (!data) return;
来源：http://hz.jinyuanbaomall.cn/gtdycnrydy.html

TS:   if (!data) return;
来源：http://hz.shanyushiyangtech.top/gtclitrxzc.html

Java: if (data == null) return;
来源：http://hz.yj202588.top/gtmmoqecto.html

Go:   if data == nil { return }
来源：http://hz.pycfn.com/gtsqmsmrzt.html

Ruby: return if data.nil?
来源：http://hz.xuetiantiany.cn/gtigqugcdv.html

C#:   if (data == null) return;
来源：http://hz.dashuyun.cn/gtmjcmzlbp.html

================================================================================
来源：http://hz.nwbrower.top/gtmghydoyg.html

C. 函数与作用域
来源：http://hz.gogol.net.cn/gteutjkhvh.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcmmvgsiy.html

[C01] 定义函数
来源：http://hz.ppjwa.cn/gtwfzjmzoh.html

Py:   def add(a, b): return a + b
来源：http://hz.xziqi.cn/gtgiyxdbyc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.quarkkingdee.top/gttqzucpvb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cashguo.top/gtujaaaxwj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.smart0.xyz/gtjjcvgqbo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gthlzcylri.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj202588.top/gtciojviuu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xinyue.icu/gtyvkopatx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtltksjmwe.html

[C02] 默认参数
来源：http://hz.svipenyu.cn/gtpzdeocvn.html

Py:   def greet(name="World"): return name
来源：http://hz.havefunace.top/gthjztehzq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnqzz.top/gtgsfczrnm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.svipenyu.cn/gtmpjllbqe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhongyouzk.top/gtkpwdjdvg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhoulong.xyz/gtbphozaig.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hnqzz.top/gtdoxcvsql.html

Ruby: def greet(name = "World") = name
来源：http://hz.birdmap.top/gthryjgxgl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gotoacloud.top/gtopxmvkdr.html

[C03] 可变参数
来源：http://hz.zhixingplan.top/gtymnufzzs.html

Py:   def total(*args): return sum(args)
来源：http://hz.yueranfly.top/gtdioxdlnv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.vqdsnc.cn/gtzouwcphr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gtbdychszr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gthposaepd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hammf.cn/gtbgmehkoo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258888.top/gtibgddvjq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.9152youxi.cn/gtaokeigqj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhoulong.xyz/gtairdsxcu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.guannengcc.top/gtsfcpdzeh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daxiang520.top/gtalgczsib.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuxming.cn/gtmxelcakr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtzfvtezhv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gtlrwjxlcb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhongyouzk.top/gtvqpemhmn.html


<!-- 参考信息 -->