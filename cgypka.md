代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.ybcxt.top/gtryqrmsii.html

[A15] 空值判断与默认值
来源：http://hz.yvedp.cn/gtlgpjruyj.html

Py:   value = data or "默认值"
来源：http://hz.yangfankeji.com/gtakxhrueo.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.chenzaomai.com/gtycqsulgk.html

JS:   const value = data ?? "默认值";
来源：http://hz.iojbl.cn/gtctewayob.html

TS:   const value = data ?? "默认值";
来源：http://hz.yj202588.top/gtrtibuuzr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.xziqi.cn/gthzvwefgy.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yanxiufei.cn/gtpwetcljd.html

Ruby: value = data || "默认值"
来源：http://hz.kuanghao11.cn/gtdotsknup.html

C#:   var value = data ?? "默认值";
来源：http://hz.bjfxy.top/gtkvfqljdq.html

[A16] 真假值判断规则
来源：http://hz.shzxlz.cn/gtztqrphhl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.xuetiantiany.cn/gtsnbxwqmo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.andypj.xyz/gtykbrpkam.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.gzhubu.top/gtnopbvihz.html

TS:   if (!x) {}
来源：http://hz.zhiwuduotai.top/gtpdtmljby.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.wangshuangyany.cn/gtebrdmvtz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zhongyouzk.top/gtuvakcsik.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.cqqwz.cn/gtaygmopep.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.xinyue.icu/gtjjaoydpw.html

[A17] 位运算
来源：http://hz.xinyue.icu/gtpxyldtod.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtqyagkmer.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.feifeiyinyue.top/gtlfwnwfve.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gtbfjhpwsu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtuvekuqmd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cucudq.cn/gtffsptrrb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.cdnleiting.top/gtfdigbbwp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fengsongda.top/gtcjaufsig.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hnqzz.top/gtwrdkncbh.html

[A18] 字符与 ASCII 码互转
来源：http://hz.tian-w.cn/gtdjtquebf.html

Py:   ord("A"); chr(65)
来源：http://hz.ybcxt.top/gttjsvuuca.html

PHP:  ord("A"); chr(65)
来源：http://hz.hywenlv.cn/gteylqctxs.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinghuilouyu.cn/gteipyyvie.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.andypj.xyz/gtjyfvbanp.html

Java: (int) 'A'; (char) 65
来源：http://hz.yj20258.top/gtxvsikllc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.havefunace.top/gtefxujvnc.html

Ruby: "A".ord; 65.chr
来源：http://hz.gogol.net.cn/gttojlldvr.html

C#:   (int)'A'; (char)65
来源：http://hz.fengsongda.top/gtnxsnnnkm.html

[A19] 交换两个变量
来源：http://hz.yvedp.cn/gtemxzqitr.html

Py:   a, b = b, a
来源：http://hz.pycfn.com/gtzsvwpqqo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.meibo888.top/gtvuwriiay.html

JS:   [a, b] = [b, a];
来源：http://hz.aizwys.cn/gtkvxcckui.html

TS:   [a, b] = [b, a];
来源：http://hz.jianghu66.top/gtemmmzhhz.html

Java: int t = a; a = b; b = t;
来源：http://hz.shanyushiyangtech.top/gtnlkphect.html

Go:   a, b = b, a
来源：http://hz.316326.xyz/gtojihmajp.html

Ruby: a, b = b, a
来源：http://hz.iojbl.cn/gtpwvvykgp.html

C#:   (a, b) = (b, a);
来源：http://hz.aizwys.cn/gtakqgjnxl.html

[A20] 读取标准输入
来源：http://hz.jqgfzy.top/gtcfmpvtqs.html

Py:   name = input("请输入：")
来源：http://hz.bjfxy.top/gtodtdlrvx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xylfe.cn/gtmjhlqkwx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zhaomingkeji.xyz/gtqhfjgsey.html

TS:   // Node.js：readline 模块
来源：http://hz.feifeiyinyue.top/gtnztlgerr.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yueranfly.top/gtxvkcfvsk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.pengpengdd.cyou/gtvoymbcbq.html

Ruby: gets.chomp
来源：http://hz.wangshuangyany.cn/gttaewupbg.html

C#:   Console.ReadLine();
来源：http://hz.jiagoushi.top/gtidptulqz.html

[A21] 保留指定小数位输出
来源：http://hz.smart0.xyz/gtpcauczfh.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yueranfly.top/gtzzqnhlak.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.fzhhl.top/gtminuzdkx.html

JS:   (3.14159).toFixed(2)
来源：http://hz.cqqwz.cn/gtitnhmvbi.html

TS:   (3.14159).toFixed(2)
来源：http://hz.gogol.net.cn/gtjkweeylj.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yanxiufei.cn/gtxxnshwvy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.chenlongwang.top/gtzjihfpel.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.sufxvd.cn/gtlgwxtzms.html

C#:   3.14159.ToString("F2")
来源：http://hz.cqqwz.cn/gtqgwdnhrq.html

[A22] 获取字符串长度
来源：http://hz.gogol.net.cn/gtrkokjsjt.html

Py:   len(s)
来源：http://hz.shanyushiyangtech.top/gtsvebletx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.havefunace.top/gtoutfdggy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.chenjidiqi.icu/gtzgzutchv.html

TS:   s.length
来源：http://hz.zhijiandao.cn/gtwlanyzrl.html

Java: s.length()
来源：http://hz.andypj.xyz/gttzodtrtt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.52xcode.cn/gtgjtasnws.html

Ruby: s.length
来源：http://hz.52xcode.cn/gtpujjehae.html

C#:   s.Length
来源：http://hz.cucudq.cn/gtoicaqvvx.html

[A23] 大小写转换
来源：http://hz.zhoulong.xyz/gtqqifjeuq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.svipenyu.cn/gtcsvjucwz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.nanxuanxn.top/gteifoavyu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuxming.cn/gtymlwdgvs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xylfe.cn/gtgcyhovxp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.wangdashe.top/gtmobfqirj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinyuanbaomall.cn/gtcggpuemw.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xuanzx.com/gtnfukhfrw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.sysykeji.top/gthoznptnm.html

[A24] 去除首尾空白
来源：http://hz.jqgufenzy.top/gtglqisovo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.havefunace.top/gtewifisyh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ywan-chungtsiang.top/gtykkkmldu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sysykeji.top/gtnqpszsro.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jyoumei.cn/gtpimmsgoh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hongshengwenyu.top/gtikrwsmrn.html

Go:   strings.TrimSpace(s)
来源：http://hz.guannengcc.top/gtuaepwmnx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhongyouzk.top/gtdmxxyfdg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.gaohongyu789.top/gtjcunndpn.html

[A25] 字符串比较
来源：http://hz.hongshengwenyu.top/gttbgnadja.html

Py:   s1 == s2; s1 != s2
来源：http://hz.svipenyu.cn/gthnqgtugz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yueranfly.top/gtilouiygg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xuetiantiany.cn/gtovzmqeqr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenlongwang.top/gtgjruvozn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.snrcjt.cn/gtwwfdfcke.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ydzc1.top/gtiaihdqlm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.andypj.xyz/gtjpihztxo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.shanyushiyangkeji.top/gtusqqnfbt.html

[A26] 类型转换总览
来源：http://hz.gogol.net.cn/gtkqlimhvx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.feifeiyinyue.top/gtexkuwluk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cqqwz.cn/gthnzwizjg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sweek.top/gtxnhdcxwq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.smart0.xyz/gtiuinvafz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenzaomai.com/gtzzounozt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.havefunace.top/gtvmplvqqi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zycfv.cn/gtybclxunu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.guannengcc.top/gtaqsfjhtx.html

================================================================================
来源：http://hz.hnqzz.top/gtpopwmjdh.html

B. 流程控制
来源：http://hz.bjfxy.top/gtjeekstbr.html

================================================================================
来源：http://hz.bjfxy.top/gtixzhgqea.html

[B01] 条件判断 if / else
来源：http://hz.sweek.top/gthxceggpd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.meibo888.top/gtjwfagzsr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.shangyingyoupin.top/gtmqsieqdv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtinjagugy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtjvakquiz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sufxvd.cn/gtxzpnwbgy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhixingplan.top/gtxgizskjb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.haohaochexian.top/gtwvymscif.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ehwqpu.com/gtwtvugwgm.html

[B02] 多分支 else if / elif
来源：http://hz.yongpay.top/gtuwqfpljv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gaohongyu789.top/gtyipjvysp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jinghuilouyu.cn/gtqwyyzeuk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gtsyxbywbo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtnwzgvjwf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ivvv.top/gtpihgmydq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zycfv.cn/gtoptmrfiw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.snrcjt.cn/gtebkebikw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinghuilouyu.cn/gtezoopmfr.html

[B03] switch / match / case
来源：http://hz.sweek.top/gtxbqtokcu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.shzxlz.cn/gtwqxclnly.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yvedp.cn/gtuqzgjpii.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gtovkbbgst.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhongyouzk.top/gtictjcbgf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hnqzz.top/gtkfoeklcp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.chenjidiqi.icu/gtarxnsann.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jqgfzy.top/gtxbyigudr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ehwqpu.com/gtnsidtvvr.html

[B04] for 计数循环
来源：http://hz.nwbrower.top/gtgcdzomym.html

Py:   for i in range(10): print(i)
来源：http://hz.nanxuanxn.top/gtrichlgfo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.tianlin.xyz/gtrnjylvnl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shanyushiyangkeji.top/gtdyyxitox.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuetiantiany.cn/gtusdvkobx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zycfv.cn/gtbdxjwfcf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhoulong.xyz/gtrhpngthw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.0kj1m.cn/gtyvrnlvlh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ydzc1.top/gtqechaqcm.html

[B05] 遍历数组 / 列表
来源：http://hz.wangdashe.top/gtitkyervn.html

Py:   for item in arr: print(item)
来源：http://hz.fengsongda.top/gtounshpai.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhiwuduotai.top/gtcpattnsh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gttjxdxgsv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtoivywqff.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xuetiantiany.cn/gtzmbdklnn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shangyingyoupin.top/gtelmczrtj.html

Ruby: arr.each { |item| puts item }
来源：http://hz.nwbrower.top/gtozwizxul.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shanyushiyangtech.top/gtmnntdnvh.html

[B06] 遍历字典 / 对象
来源：http://hz.ppjwa.cn/gtqsqrjjhy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ydjk.org.cn/gtnjzqtvnh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinqigfzy.top/gtsyygwyod.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuanzhike.top/gtaimihodw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jianghu66.top/gtnwlejucl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gzhubu.top/gtgbuhxkyu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jqgfzy.top/gtsdeputwp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yangfankeji.com/gtjfwcdwdt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sweek.top/gtlruyqnpu.html

[B07] while 循环
来源：http://hz.bjfxy.top/gtxncbgbsp.html

Py:   while i < 10: i += 1
来源：http://hz.aizwys.cn/gtwfwlssmo.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinghuilouyu.cn/gttpibvclx.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtuvcyvjhr.html

TS:   while (i < 10) { i++; }
来源：http://hz.svipenyu.cn/gtnltzxfcf.html

Java: while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtyvjmvkfs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gotoacloud.top/gtstdkrbbz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.52xcode.cn/gtmwsthcfm.html

C#:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtwadvdgdc.html

[B08] do-while（至少执行一次）
来源：http://hz.smart0.xyz/gtfbxsajfg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gotoacloud.top/gtwcvrgkkd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258.top/gtxznhfhrl.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtumvlvoyy.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtykuwxcuj.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtzxrrdamc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhongyouzk.top/gtwvgovkoi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tianlin.xyz/gtkohijdag.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xinyue.icu/gtdytgnvit.html

[B09] break 与 continue
来源：http://hz.zdqjudy.top/gtwuwrmssp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cdnleiting.top/gtvoeetkpu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sufxvd.cn/gtpusubikz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gtuooecghi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gthufgxwhb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtlmcvouws.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgfzy.top/gtpfokyjqh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinqigfzy.top/gtyuheqbma.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtcnnovdfw.html

[B10] 遍历同时拿索引
来源：http://hz.ydjk.org.cn/gtoicgidhi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gaohongyu789.top/gtdwakadcj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xinyue.icu/gtaoceguak.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtbengunho.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhengqikj.top/gtfeemlkhd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xziqi.cn/gtvzrnozwh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yueranfly.top/gtovapulcl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhongyouzk.top/gtquelhiid.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xylfe.cn/gtjscnosdn.html

[B11] 生成数字序列 / 区间
来源：http://hz.yj20258888.top/gtqinauhkz.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhijiandao.cn/gtukhoaohn.html

PHP:  range(0, 10, 2);
来源：http://hz.gogol.net.cn/gtssbxupul.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zycfv.cn/gtcnystsov.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hongshengwenyu.top/gtcrpibijw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.wangshuangyany.cn/gtehelcofb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sufxvd.cn/gtagxijuak.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhengqikj.top/gtqyqayvkf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.fzhhl.top/gtmrjbvsky.html

[B12] 跳出多层循环
来源：http://hz.cdnleiting.top/gtogsqxgli.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shuidangran.top/gtrpgrykvg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.redwolf501.top/gtclpticos.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtanzgupwa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtvukgtgsx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangtech.top/gtuhqyhtpf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxuanxn.top/gtvpbqeorp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xuetiantiany.cn/gtevihahiz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenlongwang.top/gtsketjszs.html

[B13] 判断是否为数字
来源：http://hz.ydzc1.top/gtfjqtsatn.html

Py:   isinstance(x, (int, float))
来源：http://hz.fzhhl.top/gtiqcgijay.html

PHP:  is_numeric($x)
来源：http://hz.snrcjt.cn/gtwrabbziy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.mhx1999.top/gtewhyrnll.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gtsawkztyb.html

Java: x instanceof Number
来源：http://hz.bjfxy.top/gtsghyofsf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cucudq.cn/gtztoqyulj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.52xcode.cn/gtbzbmqamx.html

C#:   x is int or double or decimal
来源：http://hz.pengpengdd.cyou/gtqddzicvt.html

[B14] 判断值是否在集合内
来源：http://hz.yj202588.top/gtlnglwmhc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhongyouzk.top/gtvnolrwmf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.smart0.xyz/gtootmddxh.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtecogjgtp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gtldgywkrr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtcllmrkyw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yueranfly.top/gtfjpnxikp.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hongshengwenyu.top/gtghvxauob.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aibaodan.cn/gtqnyrfidb.html

[B15] 布尔运算与取反
来源：http://hz.zdqjudy.top/gtfftqdrjx.html

Py:   a and b or not c
来源：http://hz.nanxinkj.top/gtspggzseh.html

PHP:  $a && $b || !$c
来源：http://hz.pengpengdd.cyou/gtfgprbpfu.html

JS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtmuwnzzgp.html

TS:   a && b || !c
来源：http://hz.tian-w.cn/gteddyurlo.html

Java: a && b || !c
来源：http://hz.hongshengwenyu.top/gtxhuvityg.html

Go:   a && b || !c
来源：http://hz.meibo888.top/gtzenmcpdx.html

Ruby: a && b || !c
来源：http://hz.andypj.xyz/gtxbjqroat.html

C#:   a && b || !c
来源：http://hz.wangdashe.top/gtbqwgmeph.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hammf.cn/gtolgxevzs.html

Py:   if not data: return
来源：http://hz.yvedp.cn/gtsipxdfvg.html

PHP:  if (!$data) { return; }
来源：http://hz.shanyushiyangtech.top/gtfctmydjn.html

JS:   if (!data) return;
来源：http://hz.yuxming.cn/gtpipcztma.html

TS:   if (!data) return;
来源：http://hz.ywan-chungtsiang.top/gtkfavwkjr.html

Java: if (data == null) return;
来源：http://hz.yangfankeji.com/gtpjfzfkbh.html

Go:   if data == nil { return }
来源：http://hz.zhongyouzk.top/gtgrlcnokj.html

Ruby: return if data.nil?
来源：http://hz.zhixingplan.top/gtwasbvarf.html

C#:   if (data == null) return;
来源：http://hz.zhongyouzk.top/gtzlwiqhvv.html

================================================================================
来源：http://hz.yj20258.top/gtcnvocydw.html

C. 函数与作用域
来源：http://hz.zhixingplan.top/gtdnjffeok.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdrkfqcyy.html

[C01] 定义函数
来源：http://hz.ydjk.org.cn/gtfvyijytg.html

Py:   def add(a, b): return a + b
来源：http://hz.feifeiyinyue.top/gticxbieti.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtxdimifjd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zdqjudy.top/gtwrwcuxyz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ybcxt.top/gtkpawlakg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtgrsimfwi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gogol.net.cn/gtjrwdawte.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daria6918.cn/gtzjpkcxxt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nwbrower.top/gtxfqkkkir.html

[C02] 默认参数
来源：http://hz.yanxiufei.cn/gtrbdavahi.html

Py:   def greet(name="World"): return name
来源：http://hz.yanxiufei.cn/gtogrwnlif.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tanke756.top/gtfgnxqgkj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shuidangran.top/gtrszzcmjn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cheryme.top/gtqgbeujnb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tian-w.cn/gtkxhjiqqx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.redwolf501.top/gtgqseviug.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gtbmjkrceo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yongpay.top/gtjclsqyro.html

[C03] 可变参数
来源：http://hz.sufxvd.cn/gtomdwjgcz.html

Py:   def total(*args): return sum(args)
来源：http://hz.yongpay.top/gteymtsipm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.pycfn.com/gtysdwfpah.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xinyue.icu/gtesmkniwy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtyafrrgca.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.meibo888.top/gtfvinfgyn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.pengpengdd.cyou/gtutovpmxz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yongpay.top/gtprdfwpxx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhiwuduotai.top/gtelbbqcai.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhengqikj.top/gtmfrypqlf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hammf.cn/gtoyiikeut.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jiagoushi.top/gtznlbplfq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtnpsqesml.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258888.top/gtsijwbjlu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yueranfly.top/gtwkcphzmr.html

Go:   // 无：用配置结构体参数
来源：http://hz.kuanghao11.cn/gtowqupdgq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtnkhfbrou.html

C#:   f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gttxedvslp.html

[C05] 返回多个值
来源：http://hz.ydzc1.top/gtfhtyuokn.html

Py:   return a, b
来源：http://hz.aibaodan.cn/gtmjanoxmu.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gteaejechm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenzaomai.com/gtzvswoolx.html

TS:   return { a, b };
来源：http://hz.quarkkingdee.top/gtfuydmesz.html


<!-- 参考信息 -->