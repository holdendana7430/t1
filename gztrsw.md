代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.redwolf501.top/gtnhvtlioe.html

C#:   var value = data ?? "默认值";
来源：http://hz.nanxuanxn.top/gtdaqmgdhz.html

[A16] 真假值判断规则
来源：http://hz.chenzaomai.com/gtrsorhgfh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ydzc1.top/gturhgjkzo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.ydjk.org.cn/gtekkzztjr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.cashguo.top/gtaqmtlume.html

TS:   if (!x) {}
来源：http://hz.daria6918.cn/gthbfxemwa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shangyingyoupin.top/gtsqnedkss.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.ppjwa.cn/gtqiqszduv.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.hysaishi.cn/gttzlpxzrr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.9152youxi.cn/gtlmhefssn.html

[A17] 位运算
来源：http://hz.fzhhl.top/gtcsbfcasj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtrqlhfhtu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.ivvv.top/gtirzrugog.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jyoumei.cn/gtsaswemok.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtvkwgxupm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yangfankeji.com/gtiobarxkj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtsarbvnxd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pycfn.com/gtjkmqjmfp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.52xcode.cn/gtgcauhapm.html

[A18] 字符与 ASCII 码互转
来源：http://hz.sysykeji.top/gthgnluvrm.html

Py:   ord("A"); chr(65)
来源：http://hz.nwbrower.top/gtnxmpopic.html

PHP:  ord("A"); chr(65)
来源：http://hz.sxryk.cn/gtcvthdeti.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ydjk.org.cn/gtjqtktcdk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sxryk.cn/gtgfpkpnlx.html

Java: (int) 'A'; (char) 65
来源：http://hz.hfpthk.cn/gtpfhypjbi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.gzhubu.top/gtgmxevlzu.html

Ruby: "A".ord; 65.chr
来源：http://hz.yangfankeji.com/gtumcobilw.html

C#:   (int)'A'; (char)65
来源：http://hz.gogol.net.cn/gtbvogbxcc.html

[A19] 交换两个变量
来源：http://hz.zhijiandao.cn/gtwjcjywvk.html

Py:   a, b = b, a
来源：http://hz.ppjwa.cn/gtdfkxmdof.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.kuanghao11.cn/gtacudkaeg.html

JS:   [a, b] = [b, a];
来源：http://hz.pengpengdd.cyou/gtotgamnwd.html

TS:   [a, b] = [b, a];
来源：http://hz.zhijiandao.cn/gtdwwsiava.html

Java: int t = a; a = b; b = t;
来源：http://hz.zhixingplan.top/gtzstmphcr.html

Go:   a, b = b, a
来源：http://hz.cheryme.top/gtnarwwjxb.html

Ruby: a, b = b, a
来源：http://hz.hfpthk.cn/gtedvwjbbj.html

C#:   (a, b) = (b, a);
来源：http://hz.zhijiandao.cn/gtnlzwnjte.html

[A20] 读取标准输入
来源：http://hz.hfpthk.cn/gttojtafrw.html

Py:   name = input("请输入：")
来源：http://hz.gogol.net.cn/gtabpzrhoz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yangfankeji.com/gtmvoyailv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.hammf.cn/gtxmwrdlgc.html

TS:   // Node.js：readline 模块
来源：http://hz.ydjk.org.cn/gtomfyjvvi.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xingfuxueyuan.xyz/gtdmuynmzj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ywan-chungtsiang.top/gturorixda.html

Ruby: gets.chomp
来源：http://hz.hywenlv.cn/gtuxphcoly.html

C#:   Console.ReadLine();
来源：http://hz.hnqzz.top/gtwllutied.html

[A21] 保留指定小数位输出
来源：http://hz.chenzaomai.com/gtiwfdiinp.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hysaishi.cn/gtcunilsxc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yj20258.top/gtheczqlyt.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ivvv.top/gtqlwvfumk.html

TS:   (3.14159).toFixed(2)
来源：http://hz.xinyue.icu/gtfitouvko.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yj202588.top/gtmitvfhez.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtwarnfslf.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.xuanzx.com/gtexhidakv.html

C#:   3.14159.ToString("F2")
来源：http://hz.ivvv.top/gtopzonzrc.html

[A22] 获取字符串长度
来源：http://hz.jyoumei.cn/gtvimhoyib.html

Py:   len(s)
来源：http://hz.iojbl.cn/gttyjbrqox.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.havefunace.top/gtpusvhscz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.sufxvd.cn/gtkhzhksqi.html

TS:   s.length
来源：http://hz.ppjwa.cn/gtrhancvnh.html

Java: s.length()
来源：http://hz.tanke756.top/gtzlrnpxmi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.nwbrower.top/gtscaycush.html

Ruby: s.length
来源：http://hz.hywenlv.cn/gtcmkresra.html

C#:   s.Length
来源：http://hz.quarkkingdee.top/gtjcatkpbk.html

[A23] 大小写转换
来源：http://hz.shuidangran.top/gtpwnfmyjp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.xziqi.cn/gtdkxrlfcg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.hnqzz.top/gtgacuyjkd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuxming.cn/gtzrfnsxci.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.pengpengdd.cyou/gtudbenxlq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj20258888.top/gthciwbexi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.cdnleiting.top/gtyphtbmsy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.birdmap.top/gthxawjnup.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.xziqi.cn/gtpkksuabs.html

[A24] 去除首尾空白
来源：http://hz.yanxiufei.cn/gteieebulw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jlsjyb.cn/gtcqqnysqp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.dashuyun.cn/gtmjzibira.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.fengsongda.top/gtazgghhue.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigfzy.top/gtxpbmjwoh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hammf.cn/gtbgsqhkuf.html

Go:   strings.TrimSpace(s)
来源：http://hz.xinyue.icu/gttskmxzhb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ehwqpu.com/gtiphcltpg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shanyushiyangkeji.top/gtwklptphp.html

[A25] 字符串比较
来源：http://hz.jinqigufen.top/gtdrfzddae.html

Py:   s1 == s2; s1 != s2
来源：http://hz.gzhubu.top/gtdwdswaqe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cqqwz.cn/gtszucocxr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gzhubu.top/gthuyfpglz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zycfv.cn/gtpovrgvaq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.aizwys.cn/gtqmljnyhs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yueranfly.top/gtcbkeylab.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.c1oappe.top/gtqhtoqgyg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xinyue.icu/gthfnxfztd.html

[A26] 类型转换总览
来源：http://hz.pycfn.com/gthsasxeoy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenzaomai.com/gtioidjyhe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cqqwz.cn/gtgiawrrpm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ydjk.org.cn/gtvpclmgso.html

TS:   Number() String() Boolean() x as number
来源：http://hz.chenlongwang.top/gtslibxzxx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.dianchejie.cn/gtvhknkfhl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jlsjyb.cn/gtxbplydfd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dianchejie.cn/gtpthxozub.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jqgufenzy.top/gtawirntmt.html

================================================================================
来源：http://hz.xuanzx.com/gtijlccqpo.html

B. 流程控制
来源：http://hz.jinqigufen.top/gtgulvywip.html

================================================================================
来源：http://hz.cdnleiting.top/gtxpruyqst.html

[B01] 条件判断 if / else
来源：http://hz.hnqzz.top/gtgfnzqtjj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.dianchejie.cn/gtmsdbkzdg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.aibaodan.cn/gtshibqrts.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shangyingyoupin.top/gtcokokyos.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtkfpezozz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtlihbjutz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.fzhhl.top/gtjolyinzp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.chenlongwang.top/gttwvsmybt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gtkgncisqn.html

[B02] 多分支 else if / elif
来源：http://hz.shuidangran.top/gtojooukvi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.52xcode.cn/gtnfxnaxhb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.pengpengdd.cyou/gtjhywallq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenzaomai.com/gtufhwgdnj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtcywnmbuy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nwbrower.top/gtwhqoubev.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.chenzaomai.com/gttkvunuxh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yj202588.top/gtosrejfjc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gturdqvvew.html

[B03] switch / match / case
来源：http://hz.hfpthk.cn/gtcxncpqaj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.svipenyu.cn/gtyximgskk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.bjfxy.top/gtaxbwdphd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yvedp.cn/gtzqfzlqkz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgufenzy.top/gtripcyvhy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yuxming.cn/gtmfjsnfxu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.smart0.xyz/gtnaefcvbl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hywenlv.cn/gtklzrxrwv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.shzxlz.cn/gthenqosfd.html

[B04] for 计数循环
来源：http://hz.jiagoushi.top/gtdbsxfhvf.html

Py:   for i in range(10): print(i)
来源：http://hz.shuidangran.top/gtcwuetfoo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jianghu66.top/gtpprqbpmz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.daria6918.cn/gttvtuqnua.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhengqikj.top/gtzmgeftxg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jinyuanbaomall.cn/gtvvpyrujm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.iojbl.cn/gtfnjribcm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daxiang520.top/gtrwzrsvmj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jqgufenzy.top/gtfcgwwmxa.html

[B05] 遍历数组 / 列表
来源：http://hz.chenlongwang.top/gtihvwflzi.html

Py:   for item in arr: print(item)
来源：http://hz.nanxuanxn.top/gtqfpjudpd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.andypj.xyz/gtkwmjhruy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhongyouzk.top/gtneyabfwi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtlbghshkg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yonumen.top/gtsssxlkzb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.chenzaomai.com/gtzjpvfcet.html

Ruby: arr.each { |item| puts item }
来源：http://hz.wangdashe.top/gtzjwjpemq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhaomingkeji.xyz/gtpcjtglux.html

[B06] 遍历字典 / 对象
来源：http://hz.jlsjyb.cn/gtkevumfkf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cdnleiting.top/gtawovvlsh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.316326.xyz/gtxquhainq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhoulong.xyz/gtrmxfhhmx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gtfahvrwqq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jinqigufen.top/gtwwjywojx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shzxlz.cn/gtwxnoapld.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yonumen.top/gtltaqjrhe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hammf.cn/gtmdqdrduv.html

[B07] while 循环
来源：http://hz.yvedp.cn/gtmuqproxn.html

Py:   while i < 10: i += 1
来源：http://hz.jianghu66.top/gtvofuvziy.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.smart0.xyz/gtpxwaixzz.html

JS:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtpfywpfno.html

TS:   while (i < 10) { i++; }
来源：http://hz.feifeiyinyue.top/gtglxzxjae.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtpbrfjggg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.sxryk.cn/gtnxafrsxu.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhijiandao.cn/gttswliihz.html

C#:   while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtkqutpumm.html

[B08] do-while（至少执行一次）
来源：http://hz.yj20258.top/gtipurpbyf.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shuidangran.top/gtgvavrxle.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.cqqwz.cn/gtmbfjppge.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xinyue.icu/gtitzydphh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtkvitayej.html

Java: do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gtgroqtriu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.tian-w.cn/gtycpzytku.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinqigfzy.top/gtcgrivmld.html

C#:   do { i++; } while (i < 10);
来源：http://hz.pycfn.com/gtrobqqfpk.html

[B09] break 与 continue
来源：http://hz.ybcxt.top/gtycyutbhs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhixingplan.top/gtjwslwchy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.fzhhl.top/gtsvpvppca.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtbuevlahk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtnppxjren.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtmodklmga.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.feifeiyinyue.top/gttwhsrxtk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gaohongyu789.top/gtooivynld.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sweek.top/gtzlufxkbk.html

[B10] 遍历同时拿索引
来源：http://hz.sufxvd.cn/gtxpfvfhhn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.fzhhl.top/gtlhrqdcru.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.wangshuangyany.cn/gtsnpxldbq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtwcfgyvgg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.chenjidiqi.icu/gtmffasfds.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zycfv.cn/gtqevalchp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xziqi.cn/gtryoivurq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.mhx1999.top/gtxctmlcla.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gzhubu.top/gtmxhwhogi.html

[B11] 生成数字序列 / 区间
来源：http://hz.nanxuanxn.top/gtutvuqhdy.html

Py:   list(range(0, 10, 2))
来源：http://hz.yonumen.top/gtgakdowlh.html

PHP:  range(0, 10, 2);
来源：http://hz.0kj1m.cn/gtrshphyvd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yueranfly.top/gtcesjbcvy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nanxuanxn.top/gtdxjesadd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cucudq.cn/gtkgbbjbtu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigfzy.top/gtlypbwhzd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.haohaochexian.top/gtelxpcisa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zycfv.cn/gtekainlvc.html

[B12] 跳出多层循环
来源：http://hz.zycfv.cn/gtyqspcvjf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.bjfxy.top/gtsnbmefya.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gaohongyu789.top/gtiyiiaonj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtlicfdsvr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtarcujany.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtgjzutpag.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.wangdashe.top/gthwnaqycp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xuanzx.com/gtjnwbntbp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hysaishi.cn/gthrnnyjpd.html

[B13] 判断是否为数字
来源：http://hz.shangyingyoupin.top/gtjwnluovg.html

Py:   isinstance(x, (int, float))
来源：http://hz.cdnleiting.top/gtcmsozqtt.html

PHP:  is_numeric($x)
来源：http://hz.jinqigfzy.top/gtqvdganiy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtynwjkzla.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtklwpauje.html

Java: x instanceof Number
来源：http://hz.yongpay.top/gtnyelexzy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cucudq.cn/gtogelxhhx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhiwuduotai.top/gtfnibpano.html

C#:   x is int or double or decimal
来源：http://hz.hnqzz.top/gtzmodtxdo.html

[B14] 判断值是否在集合内
来源：http://hz.jiagoushi.top/gtgljaogja.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hammf.cn/gtgyjolojm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shuidangran.top/gtjorjbtny.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xuetiantiany.cn/gtjjdptuxt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.aizwys.cn/gtgcipbgqf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ehwqpu.com/gtygyoskiu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cheryme.top/gtthoobuwn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtxngeprev.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cdnleiting.top/gtrfjvbaxk.html

[B15] 布尔运算与取反
来源：http://hz.zycfv.cn/gtcsymrehn.html

Py:   a and b or not c
来源：http://hz.ywan-chungtsiang.top/gtzmdbzgkt.html

PHP:  $a && $b || !$c
来源：http://hz.xuetiantiany.cn/gtkhhvmgla.html

JS:   a && b || !c
来源：http://hz.birdmap.top/gtdslaebzq.html

TS:   a && b || !c
来源：http://hz.pycfn.com/gtztdccigg.html

Java: a && b || !c
来源：http://hz.9152youxi.cn/gtwpgmmhtw.html

Go:   a && b || !c
来源：http://hz.xuanzx.com/gtabttjvfp.html

Ruby: a && b || !c
来源：http://hz.yj20258888.top/gtmbjuuadl.html

C#:   a && b || !c
来源：http://hz.yuanzhike.top/gtvelncibt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cashguo.top/gtwbgegbbm.html

Py:   if not data: return
来源：http://hz.cheryme.top/gtjhmjycvk.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtsfpxyoyr.html

JS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtknvzliqu.html

TS:   if (!data) return;
来源：http://hz.shzxlz.cn/gtiqduwdgc.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtlgrxivvv.html

Go:   if data == nil { return }
来源：http://hz.nanxinkj.top/gtyiokpmmm.html

Ruby: return if data.nil?
来源：http://hz.jyoumei.cn/gthwvplxax.html

C#:   if (data == null) return;
来源：http://hz.daria6918.cn/gtrjapmlbf.html

================================================================================
来源：http://hz.pycfn.com/gtbpczpktj.html

C. 函数与作用域
来源：http://hz.jiagoushi.top/gtzmnulpmy.html

================================================================================
来源：http://hz.sweek.top/gtwtjqugqp.html

[C01] 定义函数
来源：http://hz.vqdsnc.cn/gtzhdbhyuk.html

Py:   def add(a, b): return a + b
来源：http://hz.feifeiyinyue.top/gtnmysbnqz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtorfnyxyi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gttqokckpk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.andypj.xyz/gtgbabtrmt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nwbrower.top/gtbxbkfidp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.andypj.xyz/gtfjzvomrb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ybcxt.top/gtezclnomw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtotwzqoje.html

[C02] 默认参数
来源：http://hz.sxryk.cn/gtikxmicly.html

Py:   def greet(name="World"): return name
来源：http://hz.yonumen.top/gtnxeiqqvc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.mhx1999.top/gtwjbqlivq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cheryme.top/gtxinhevfc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.mhx1999.top/gtggpmjpvs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydjk.org.cn/gtdwgmtgrr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cheryme.top/gtkderrgpn.html

Ruby: def greet(name = "World") = name
来源：http://hz.kuanghao11.cn/gtalwrbpoi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guowangkeji.top/gtwnqzeiyz.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtetezornn.html

Py:   def total(*args): return sum(args)
来源：http://hz.hysaishi.cn/gtprauxbiq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gzhubu.top/gtkuaohwak.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtujhdprdk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuxming.cn/gtyrmmgxxq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.9152youxi.cn/gtjgvkemay.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.andypj.xyz/gtarzdaool.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.smart0.xyz/gtvinjkdob.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.316326.xyz/gtiorwfgjd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tian-w.cn/gtpzwgxqhx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ehwqpu.com/gtfvqlhekr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ppjwa.cn/gtgpumbkbt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtsdxuvdpo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.svipenyu.cn/gtlxltyqxe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yanxiufei.cn/gtaosigayp.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenzaomai.com/gtjqdnizul.html

Ruby: f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtolyedltt.html

C#:   f(a: 1, b: 2)
来源：http://hz.jlsjyb.cn/gtumphpbky.html

[C05] 返回多个值
来源：http://hz.fzhhl.top/gtfqmzzhmx.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtbgkklkjd.html

PHP:  return [$a, $b];
来源：http://hz.cdnleiting.top/gtnvwhqesy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.snrcjt.cn/gtdnpvyxag.html

TS:   return { a, b };
来源：http://hz.ppjwa.cn/gthyqiepkf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj202588.top/gtgfdfwfex.html

Go:   return a, b
来源：http://hz.yongpay.top/gtaxufazhg.html

Ruby: return a, b
来源：http://hz.shanyushiyangtech.top/gtuvlvtame.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258.top/gtixzbzoyn.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtundwavbl.html

Py:   square = lambda x: x * x
来源：http://hz.9152youxi.cn/gtwrvjuhll.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gotoacloud.top/gtbtzykrjz.html

JS:   const square = x => x * x;
来源：http://hz.mhx1999.top/gtwfqqbhuy.html


<!-- 参考信息 -->