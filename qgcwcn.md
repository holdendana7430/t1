代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://hz.hnxiangtu.top/gtbjssdbzj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.cdnleiting.top/gtalcydkyy.html

Go:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangkeji.top/gtyntqzawn.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ydjk.org.cn/gtwvgvtjgv.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhoulong.xyz/gtbutqsmsb.html

[A15] 空值判断与默认值
来源：http://hz.hongshengwenyu.top/gtwussvsud.html

Py:   value = data or "默认值"
来源：http://hz.aibaodan.cn/gtezpwbxcv.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.xuanzx.com/gtrvcksbyu.html

JS:   const value = data ?? "默认值";
来源：http://hz.chenzaomai.com/gtciihuybk.html

TS:   const value = data ?? "默认值";
来源：http://hz.cdnleiting.top/gtutcfkjvk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.0kj1m.cn/gtknwqugdp.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.svipenyu.cn/gtlsfnnisk.html

Ruby: value = data || "默认值"
来源：http://hz.hywenlv.cn/gtsnhgskfb.html

C#:   var value = data ?? "默认值";
来源：http://hz.havefunace.top/gtlcwzafbm.html

[A16] 真假值判断规则
来源：http://hz.gaohongyu789.top/gtglgucgls.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.xziqi.cn/gtikatdbfx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yangfankeji.com/gtomupjdhc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.sweek.top/gtgqvguxko.html

TS:   if (!x) {}
来源：http://hz.cucudq.cn/gtrgcnwbpc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jyoumei.cn/gtvkcvlisw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.tian-w.cn/gtztswbfrs.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zhongyouzk.top/gtfwsuxxwa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.sufxvd.cn/gtfoobveun.html

[A17] 位运算
来源：http://hz.fengsongda.top/gtfowstwmi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gtilpzbtjt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhaomingkeji.xyz/gtccpcchmd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jiagoushi.top/gtabqyusbk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtogtooelk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigfzy.top/gtfbsxhyyo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zhengqikj.top/gtwsohagde.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtsvzbxagc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtedulmutr.html

[A18] 字符与 ASCII 码互转
来源：http://hz.hongshengwenyu.top/gtxrlcdwth.html

Py:   ord("A"); chr(65)
来源：http://hz.jinyuanbaomall.cn/gtkyrdwkyv.html

PHP:  ord("A"); chr(65)
来源：http://hz.jyoumei.cn/gtsrnouphp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.andypj.xyz/gtrjaakags.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.316326.xyz/gtoszzpdid.html

Java: (int) 'A'; (char) 65
来源：http://hz.hywenlv.cn/gtpfcslfve.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zhongyouzk.top/gtsaqhminv.html

Ruby: "A".ord; 65.chr
来源：http://hz.bjfxy.top/gtvvwifwkk.html

C#:   (int)'A'; (char)65
来源：http://hz.gogol.net.cn/gtullwhwtc.html

[A19] 交换两个变量
来源：http://hz.jinyuanbaomall.cn/gtvaotjgom.html

Py:   a, b = b, a
来源：http://hz.svipenyu.cn/gtzguzbbod.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.meibo888.top/gtoswqfpdk.html

JS:   [a, b] = [b, a];
来源：http://hz.tianlin.xyz/gtpnykycds.html

TS:   [a, b] = [b, a];
来源：http://hz.gaohongyu789.top/gtcvmppepa.html

Java: int t = a; a = b; b = t;
来源：http://hz.jlsjyb.cn/gtxdzcsxdd.html

Go:   a, b = b, a
来源：http://hz.gogol.net.cn/gtiilxyhxs.html

Ruby: a, b = b, a
来源：http://hz.cheryme.top/gtiwqxrczk.html

C#:   (a, b) = (b, a);
来源：http://hz.zdqjudy.top/gtmggjahbs.html

[A20] 读取标准输入
来源：http://hz.zhijiandao.cn/gtbykmfchv.html

Py:   name = input("请输入：")
来源：http://hz.kuanghao11.cn/gtqzqzkjev.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.sysykeji.top/gthlityjlt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.quarkkingdee.top/gtqqnmayrj.html

TS:   // Node.js：readline 模块
来源：http://hz.meibo888.top/gthwnwfhio.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yuanzhike.top/gtgnzijjik.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xuetiantiany.cn/gtommewbfs.html

Ruby: gets.chomp
来源：http://hz.hnxiangtu.top/gtslbhqtes.html

C#:   Console.ReadLine();
来源：http://hz.jinghuilouyu.cn/gtztfwtppl.html

[A21] 保留指定小数位输出
来源：http://hz.guannengcc.top/gtwpxyfbrw.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yanxiufei.cn/gtxmpydqmj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.chenlongwang.top/gtirmsvbdy.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shzxlz.cn/gtaiafadzi.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ehwqpu.com/gtacxkbrog.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jianghu66.top/gtixjmiydf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.sweek.top/gtzwpmxwsf.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yonumen.top/gtvvcwlvzc.html

C#:   3.14159.ToString("F2")
来源：http://hz.yuanzhike.top/gtcqyiovii.html

[A22] 获取字符串长度
来源：http://hz.jlsjyb.cn/gtfahbyyjt.html

Py:   len(s)
来源：http://hz.chenzaomai.com/gtdlyvmpyv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.chenlongwang.top/gtaxxynoki.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hnxiangtu.top/gtzofnrnjj.html

TS:   s.length
来源：http://hz.zycfv.cn/gtmyznlwsj.html

Java: s.length()
来源：http://hz.yueranfly.top/gtdjdnhgav.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cqqwz.cn/gtghezsqig.html

Ruby: s.length
来源：http://hz.redwolf501.top/gttbsehipz.html

C#:   s.Length
来源：http://hz.meibo888.top/gtyxjoiwkh.html

[A23] 大小写转换
来源：http://hz.fzhhl.top/gtbtgtbhry.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.gzhubu.top/gtiqryousp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ehwqpu.com/gttelxdbrc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.mhx1999.top/gtqprznruv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yongpay.top/gttmeeenck.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.9152youxi.cn/gtbkwdaqyg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.chenlongwang.top/gtybmgtisd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hywenlv.cn/gtwbllzuis.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.birdmap.top/gtmwbhxfkv.html

[A24] 去除首尾空白
来源：http://hz.pengpengdd.cyou/gtqwidlxsd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.pycfn.com/gtoxolqmow.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zdqjudy.top/gtbngztyuk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.smart0.xyz/gtgumtmblq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yj202588.top/gtrmixjtnv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.9152youxi.cn/gtxvavvjxm.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhengqikj.top/gtuxfidaku.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhengqikj.top/gtwybzyjnd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jinqigfzy.top/gtqklhslvv.html

[A25] 字符串比较
来源：http://hz.shanyushiyangtech.top/gtbqudoarf.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shangyingyoupin.top/gtwtjtccpo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.quarkkingdee.top/gtyuxkhmlb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgufenzy.top/gtaeenffug.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinghuilouyu.cn/gtwenchpzt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.wangdashe.top/gtwueinclr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cashguo.top/gtbdxrtbpa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.iojbl.cn/gttcdxczme.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.cdnleiting.top/gtwjwugdyj.html

[A26] 类型转换总览
来源：http://hz.hfpthk.cn/gtqxlgxpfe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhixingplan.top/gtttgcmrpt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gzhubu.top/gtfjvaexmg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.fzhhl.top/gtklvozzvg.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ppjwa.cn/gtrhpjuifo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xinyue.icu/gtvdfnfpie.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yj20258888.top/gtlbhyuwbx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jqgfzy.top/gtkaepfmvr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.svipenyu.cn/gtoohdhhyl.html

================================================================================
来源：http://hz.pycfn.com/gtfvympzty.html

B. 流程控制
来源：http://hz.wangdashe.top/gttwfhhcli.html

================================================================================
来源：http://hz.guowangkeji.top/gtjrezxskg.html

[B01] 条件判断 if / else
来源：http://hz.kuanghao11.cn/gtxtpstnba.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.xuetiantiany.cn/gtmvlihudl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yuanzhike.top/gtkbfjqdkq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gttcuiziqn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shzxlz.cn/gticbkzguk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.guowangkeji.top/gtwdsgnnqm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yanxiufei.cn/gtahxcgbfs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gotoacloud.top/gtbhcgrizi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtpueownzl.html

[B02] 多分支 else if / elif
来源：http://hz.hnqzz.top/gtqykvbdnr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhengqikj.top/gtwwccdznr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.aibaodan.cn/gtxxeuyxlz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.316326.xyz/gtowdsvmzh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuxming.cn/gtkfdgjqxu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gtwwpcyyvo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yvedp.cn/gtjdroognt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinghuilouyu.cn/gtjdgkuurc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhiwuduotai.top/gtbrxehwhk.html

[B03] switch / match / case
来源：http://hz.quarkkingdee.top/gtuwotpmdc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.feifeiyinyue.top/gtuapmqrtb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jqgufenzy.top/gtpwfckxzy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gthdbxtkxp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shanyushiyangtech.top/gtfbrcusfb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.xylfe.cn/gtlfakatnr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.vqdsnc.cn/gtcidokziw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnxiangtu.top/gtoplgzzfq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.snrcjt.cn/gtlxtkjblr.html

[B04] for 计数循环
来源：http://hz.jinghuilouyu.cn/gtavfvnoon.html

Py:   for i in range(10): print(i)
来源：http://hz.yangfankeji.com/gtyvwanwkw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.pycfn.com/gtgaeufqmb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.andypj.xyz/gteekgeuri.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yonumen.top/gtgdkdyiyz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ydzc1.top/gtypkcehsk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.c1oappe.top/gtenxihyqf.html

Ruby: 10.times { |i| puts i }
来源：http://hz.aizwys.cn/gtsyckjadn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hnxiangtu.top/gtsuphikqt.html

[B05] 遍历数组 / 列表
来源：http://hz.sysykeji.top/gtrdwuhogk.html

Py:   for item in arr: print(item)
来源：http://hz.xylfe.cn/gtctmtfuqm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shangyingyoupin.top/gtgasbwyth.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ivvv.top/gttjgvnjhp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ywan-chungtsiang.top/gtdzzfgrmm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.fengsongda.top/gthjgwjnew.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gzhubu.top/gtcljfzxdt.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hysaishi.cn/gtalfilqsa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.chenzaomai.com/gttwuwtskq.html

[B06] 遍历字典 / 对象
来源：http://hz.jiagoushi.top/gtieriadts.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hnqzz.top/gtizhwfcav.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.daxiang520.top/gtmfocoork.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xziqi.cn/gtqdnpnftb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.haohaochexian.top/gtxxcazogy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.nwbrower.top/gtvwyihfyb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hongshengwenyu.top/gtlxrhvxnf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yonumen.top/gtjygpezym.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.nanxuanxn.top/gtqaztsyoe.html

[B07] while 循环
来源：http://hz.shuidangran.top/gtbhodzuze.html

Py:   while i < 10: i += 1
来源：http://hz.shanyushiyangtech.top/gtskerwoam.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sxryk.cn/gttkuuxrpe.html

JS:   while (i < 10) { i++; }
来源：http://hz.havefunace.top/gtefsznvwp.html

TS:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtswojsiwx.html

Java: while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtueacuzxy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cashguo.top/gtivgtuify.html

Ruby: while i < 10; i += 1; end
来源：http://hz.wangdashe.top/gtnfvopfvs.html

C#:   while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gtayoaujxg.html

[B08] do-while（至少执行一次）
来源：http://hz.yongpay.top/gtgxffbbzl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.bjfxy.top/gtbqafphwr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sweek.top/gtkjvcpwwq.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xuetiantiany.cn/gtpcoolepq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gtobffwgtf.html

Java: do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtowanbxdx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hfpthk.cn/gtyhibtpjp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tian-w.cn/gtrxzsczyx.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtjmngidxp.html

[B09] break 与 continue
来源：http://hz.yongpay.top/gtgrpluoqw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yj202588.top/gthzukttnj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sufxvd.cn/gtuudkbevh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtmsuhydfz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtxvtqlnmi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtfkvzedwx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cheryme.top/gtlofaeuny.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.smart0.xyz/gtrivaamkb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gturitjlet.html

[B10] 遍历同时拿索引
来源：http://hz.guowangkeji.top/gtgokycwvi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xinyue.icu/gtqckdlygq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jlsjyb.cn/gtjhakftor.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj20258.top/gtzxzkyotf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtqqpubreb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.0kj1m.cn/gtdczxuqzg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.quarkkingdee.top/gthevctnoq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhengqikj.top/gtfpudopsp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zycfv.cn/gtqzavijqb.html

[B11] 生成数字序列 / 区间
来源：http://hz.gotoacloud.top/gtohwfcekv.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj202588.top/gtdxddbqlp.html

PHP:  range(0, 10, 2);
来源：http://hz.meibo888.top/gtkoceufax.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj202588.top/gtnilgrgys.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gtkwiislot.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hammf.cn/gtefraojhb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.guowangkeji.top/gthbvpfbzy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cashguo.top/gtogftwyhq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenzaomai.com/gtmvtdmvan.html

[B12] 跳出多层循环
来源：http://hz.yanxiufei.cn/gtzqkoogse.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ydzc1.top/gtkpsqfrly.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhixingplan.top/gtjauyeqam.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtuqgggatw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gaohongyu789.top/gtebgltxpe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangkeji.top/gtskcqfvlq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtytzpddfe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj202588.top/gtzcbdmdli.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yonumen.top/gtmvhsbtyw.html

[B13] 判断是否为数字
来源：http://hz.svipenyu.cn/gtitqzideu.html

Py:   isinstance(x, (int, float))
来源：http://hz.jqgufenzy.top/gtaewnhmqv.html

PHP:  is_numeric($x)
来源：http://hz.0kj1m.cn/gtfwrfgioq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gtrxlozhyg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pengpengdd.cyou/gtzxzzcfgv.html

Java: x instanceof Number
来源：http://hz.gotoacloud.top/gtsxvnailc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ivvv.top/gtslavkcqg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj202588.top/gtdemezedx.html

C#:   x is int or double or decimal
来源：http://hz.xuanzx.com/gtzjdupfqu.html

[B14] 判断值是否在集合内
来源：http://hz.xingfuxueyuan.xyz/gtwmjilbxl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hammf.cn/gttcqcexyf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydjk.org.cn/gtunbbiyai.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtahjthnkw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hnxiangtu.top/gtwxezbsia.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shanyushiyangtech.top/gtqeqdgzmx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tanke756.top/gtinagurxl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gogol.net.cn/gtbbkzstap.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yvedp.cn/gtetyytmrh.html

[B15] 布尔运算与取反
来源：http://hz.hfpthk.cn/gtavsqwnzj.html

Py:   a and b or not c
来源：http://hz.yuxming.cn/gtiwplqpzp.html

PHP:  $a && $b || !$c
来源：http://hz.aibaodan.cn/gtgjtfysew.html

JS:   a && b || !c
来源：http://hz.snrcjt.cn/gtnwoadmlx.html

TS:   a && b || !c
来源：http://hz.yueranfly.top/gtcvdmapsa.html

Java: a && b || !c
来源：http://hz.tian-w.cn/gtiliqpdav.html

Go:   a && b || !c
来源：http://hz.sxryk.cn/gtapsnfmgr.html

Ruby: a && b || !c
来源：http://hz.0kj1m.cn/gtnakjrglb.html

C#:   a && b || !c
来源：http://hz.sysykeji.top/gtiiddxhtf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gtarhzoaxi.html

Py:   if not data: return
来源：http://hz.c1oappe.top/gtyrcyxsag.html

PHP:  if (!$data) { return; }
来源：http://hz.xuanzx.com/gtrhzhriii.html

JS:   if (!data) return;
来源：http://hz.sxryk.cn/gtpfrhkqua.html

TS:   if (!data) return;
来源：http://hz.fzhhl.top/gtqwmgxnos.html

Java: if (data == null) return;
来源：http://hz.svipenyu.cn/gtssrpthcs.html

Go:   if data == nil { return }
来源：http://hz.nanxinkj.top/gtfrfuiynj.html

Ruby: return if data.nil?
来源：http://hz.haohaochexian.top/gthwgucyhi.html

C#:   if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtxyuabejx.html

================================================================================
来源：http://hz.jqgfzy.top/gtdvumxher.html

C. 函数与作用域
来源：http://hz.aibaodan.cn/gtovqiptoh.html

================================================================================
来源：http://hz.meibo888.top/gtadopspkf.html

[C01] 定义函数
来源：http://hz.yj20258.top/gtjuqjmwlu.html

Py:   def add(a, b): return a + b
来源：http://hz.smart0.xyz/gtqrgcfmic.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtsawnhoul.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnqzz.top/gtzyaqsdpx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.0kj1m.cn/gtprhtbuzd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtzmjewrvi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sweek.top/gteindnqug.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cheryme.top/gtagawxmov.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtrejfvzlb.html

[C02] 默认参数
来源：http://hz.zhengqikj.top/gtpuhvqfot.html

Py:   def greet(name="World"): return name
来源：http://hz.zdqjudy.top/gtpdbddhhm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.vqdsnc.cn/gtwofqdiko.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tian-w.cn/gtwkgglnum.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnqzz.top/gtaewkouiu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.52xcode.cn/gtzasgkaew.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhixingplan.top/gteayopopr.html

Ruby: def greet(name = "World") = name
来源：http://hz.dashuyun.cn/gtfmjcbpch.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgfzy.top/gtoxahzhjg.html

[C03] 可变参数
来源：http://hz.tanke756.top/gtlzlebfkr.html

Py:   def total(*args): return sum(args)
来源：http://hz.xylfe.cn/gtejwqhybs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cashguo.top/gtvuziokfc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hywenlv.cn/gtqtcohbuy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtaxournsi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guowangkeji.top/gtwvegytjy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangdashe.top/gtgbqaynhf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.feifeiyinyue.top/gtwnqnxhae.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yonumen.top/gtfbdhtmbe.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtgcktnzgn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guowangkeji.top/gtbdaujbys.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.quarkkingdee.top/gtdishqnrg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtwlbbvvay.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenjidiqi.icu/gttjwxdwzn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ybcxt.top/gtkkvhhbmo.html

Go:   // 无：用配置结构体参数
来源：http://hz.gzhubu.top/gtmtivvjti.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigfzy.top/gttphiorxk.html

C#:   f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtljokqxpy.html

[C05] 返回多个值
来源：http://hz.ydzc1.top/gtlgchctgb.html


<!-- 参考信息 -->