代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sysykeji.top/gtlsedtziy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.ivvv.top/gtrlbperbu.html

TS:   if (!x) {}
来源：http://hz.ywan-chungtsiang.top/gtokmbtfhn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yj202588.top/gtsqfafvjd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yangfankeji.com/gtneiocnga.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.haohaochexian.top/gtxhihyuai.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.nanxinkj.top/gtntscmgij.html

[A17] 位运算
来源：http://hz.guannengcc.top/gthefadpgs.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtrgzdljgo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yangfankeji.com/gtrpjzriop.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtpodfzrlf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtskzivfdv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gogol.net.cn/gtyrlxeiod.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yanxiufei.cn/gtyprjssnx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nanxinkj.top/gtwtcgtuks.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gtnrszpoma.html

[A18] 字符与 ASCII 码互转
来源：http://hz.wangshuangyany.cn/gtxxaesjvi.html

Py:   ord("A"); chr(65)
来源：http://hz.sxryk.cn/gtyksqgwxv.html

PHP:  ord("A"); chr(65)
来源：http://hz.hywenlv.cn/gtgdkikwjm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.chenlongwang.top/gtxkelpoex.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.quarkkingdee.top/gtpviqommp.html

Java: (int) 'A'; (char) 65
来源：http://hz.hammf.cn/gtubegksbo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.9152youxi.cn/gtkoqbbmef.html

Ruby: "A".ord; 65.chr
来源：http://hz.hfpthk.cn/gtgvedkojg.html

C#:   (int)'A'; (char)65
来源：http://hz.sweek.top/gtlbargtbr.html

[A19] 交换两个变量
来源：http://hz.aizwys.cn/gteluvaowm.html

Py:   a, b = b, a
来源：http://hz.chenzaomai.com/gtkfymuzsx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.cucudq.cn/gtdzqlkgvk.html

JS:   [a, b] = [b, a];
来源：http://hz.jlsjyb.cn/gtofrsalah.html

TS:   [a, b] = [b, a];
来源：http://hz.quarkkingdee.top/gtijzkunbv.html

Java: int t = a; a = b; b = t;
来源：http://hz.cashguo.top/gtuvzjsvxq.html

Go:   a, b = b, a
来源：http://hz.yueranfly.top/gtcucjieig.html

Ruby: a, b = b, a
来源：http://hz.guowangkeji.top/gtwbztdzyg.html

C#:   (a, b) = (b, a);
来源：http://hz.jlsjyb.cn/gtvaygxhwn.html

[A20] 读取标准输入
来源：http://hz.andypj.xyz/gtpuhdiaue.html

Py:   name = input("请输入：")
来源：http://hz.shzxlz.cn/gtmjekgxmb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xuetiantiany.cn/gtvepetfem.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.c1oappe.top/gtalvqndpa.html

TS:   // Node.js：readline 模块
来源：http://hz.wangdashe.top/gtdptlcspx.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.bjfxy.top/gtebamzwdt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yueranfly.top/gtdjmhnxcz.html

Ruby: gets.chomp
来源：http://hz.ydjk.org.cn/gtexuwsndu.html

C#:   Console.ReadLine();
来源：http://hz.mhx1999.top/gtzrizigjt.html

[A21] 保留指定小数位输出
来源：http://hz.chenlongwang.top/gttkuomozq.html

Py:   f"{3.14159:.2f}"
来源：http://hz.andypj.xyz/gtyvyithzd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.vqdsnc.cn/gtkhrfqvuy.html

JS:   (3.14159).toFixed(2)
来源：http://hz.daxiang520.top/gteckjyjqi.html

TS:   (3.14159).toFixed(2)
来源：http://hz.xingfuxueyuan.xyz/gtkxzukqtd.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tanke756.top/gtetdrtpjh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shzxlz.cn/gtcbbuumzd.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.quarkkingdee.top/gtohukldpf.html

C#:   3.14159.ToString("F2")
来源：http://hz.yvedp.cn/gtdorlvmyn.html

[A22] 获取字符串长度
来源：http://hz.wangshuangyany.cn/gtzfuxpvut.html

Py:   len(s)
来源：http://hz.sweek.top/gtyixepxhy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.snrcjt.cn/gturgdnrqb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jqgfzy.top/gtpspnlgfu.html

TS:   s.length
来源：http://hz.aibaodan.cn/gtlimutgqz.html

Java: s.length()
来源：http://hz.birdmap.top/gtnzsabjfo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cashguo.top/gtjuawjaja.html

Ruby: s.length
来源：http://hz.ydjk.org.cn/gtbygrhfot.html

C#:   s.Length
来源：http://hz.zhongyouzk.top/gtynhnijxc.html

[A23] 大小写转换
来源：http://hz.nwbrower.top/gtcykidklg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.feifeiyinyue.top/gtgdltrpbb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yanxiufei.cn/gtclvetzok.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuanzx.com/gteebojogh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.fengsongda.top/gtygqemxjc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.dianchejie.cn/gtnmrgmwle.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.aibaodan.cn/gtqiisnbur.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.guannengcc.top/gtyvbuhqte.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.redwolf501.top/gtnwetgjwy.html

[A24] 去除首尾空白
来源：http://hz.jqgfzy.top/gtttifpycv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.fengsongda.top/gtgqlmsuvs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xziqi.cn/gtcnckyria.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sufxvd.cn/gtakvqqfgu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.0kj1m.cn/gtblpnpjpe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shzxlz.cn/gtttekzbxf.html

Go:   strings.TrimSpace(s)
来源：http://hz.zycfv.cn/gtbjtcunak.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ydzc1.top/gtoujopgfu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.dianchejie.cn/gtlvicutet.html

[A25] 字符串比较
来源：http://hz.andypj.xyz/gtjowsmeua.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ywan-chungtsiang.top/gtwmdwemfp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.chenjidiqi.icu/gtsajovsjy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yonumen.top/gtqectuzob.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtlgksurpl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.sysykeji.top/gtcvlijgod.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cucudq.cn/gtrlsqomam.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xinyue.icu/gtijlwaztk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.daxiang520.top/gtdxcznlmj.html

[A26] 类型转换总览
来源：http://hz.dashuyun.cn/gtiitpupox.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.316326.xyz/gtdbmtocii.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.chenjidiqi.icu/gtdbfivfsm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinyuanbaomall.cn/gtjfhvwqqj.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jinqigufen.top/gtlqqegzaj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenjidiqi.icu/gtdgvxjrjj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yanxiufei.cn/gtcfjbupyo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.pengpengdd.cyou/gtcwagxdpr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yongpay.top/gtgezdsolb.html

================================================================================
来源：http://hz.zycfv.cn/gtwrhhfbfr.html

B. 流程控制
来源：http://hz.yj202588.top/gtpfwvjzzl.html

================================================================================
来源：http://hz.fzhhl.top/gtivdzsgim.html

[B01] 条件判断 if / else
来源：http://hz.aibaodan.cn/gtbkytspix.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yongpay.top/gtmhzjkswd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.guowangkeji.top/gtkkshwxvz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ydzc1.top/gtigqrntca.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtujffpizb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.nanxinkj.top/gtjznvbwfe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gotoacloud.top/gtdjaobpbd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.aizwys.cn/gtthjozomh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.meibo888.top/gtonwltdwo.html

[B02] 多分支 else if / elif
来源：http://hz.jinyuanbaomall.cn/gtgrdimnkg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhaomingkeji.xyz/gtzsbojvlc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.fengsongda.top/gtkqlwurpn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtfbtxpdsq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghu66.top/gtmmgfpwch.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pengpengdd.cyou/gtsjhzbdyq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sysykeji.top/gtuctpfphm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.nwbrower.top/gthozpmgie.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gturbrmdlt.html

[B03] switch / match / case
来源：http://hz.iojbl.cn/gthaqfgitx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.meibo888.top/gtzlvzqtok.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daxiang520.top/gtmrpvkhfd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cqqwz.cn/gtmzcthnnq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.wangdashe.top/gtprgekchk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sysykeji.top/gtywjeowxo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhoulong.xyz/gtwiqidter.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jiagoushi.top/gtpiyemtlb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.52xcode.cn/gtranxdxud.html

[B04] for 计数循环
来源：http://hz.fzhhl.top/gtgfkniybj.html

Py:   for i in range(10): print(i)
来源：http://hz.zhijiandao.cn/gtersfvxuh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xuetiantiany.cn/gtgjwkysrm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nwbrower.top/gtquzgmofn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuanzhike.top/gthofoztkw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhongyouzk.top/gtdhbiqubi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jlsjyb.cn/gtdzrndzxm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ybcxt.top/gtcncuwtnx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zycfv.cn/gtfyafbghz.html

[B05] 遍历数组 / 列表
来源：http://hz.316326.xyz/gthtonhbnw.html

Py:   for item in arr: print(item)
来源：http://hz.0kj1m.cn/gtonqledon.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.tanke756.top/gtckljkkec.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ybcxt.top/gtvkkzuexs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenjidiqi.icu/gtqkeupwrb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhijiandao.cn/gtjxnvrmzs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jyoumei.cn/gtyyaredog.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shanyushiyangtech.top/gttsvglsgn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xziqi.cn/gtxgogbbiv.html

[B06] 遍历字典 / 对象
来源：http://hz.pycfn.com/gtluoozdub.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.mhx1999.top/gtjklexehm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yj20258.top/gtzhrvajdc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gtswqrqxie.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jlsjyb.cn/gtldrawqdp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hywenlv.cn/gttcpqvnff.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhoulong.xyz/gttlbbbboj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jyoumei.cn/gtkhyegkxv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cdnleiting.top/gtqjsnefiq.html

[B07] while 循环
来源：http://hz.hongshengwenyu.top/gtkdlpgcdg.html

Py:   while i < 10: i += 1
来源：http://hz.gotoacloud.top/gtahhspzcn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuanzhike.top/gttermlhkn.html

JS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtpbjspyen.html

TS:   while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gtbadldgvk.html

Java: while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtxumayfah.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenjidiqi.icu/gtiowytbpr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtlriwbzpp.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtefiywgvk.html

[B08] do-while（至少执行一次）
来源：http://hz.yueranfly.top/gtdhvvfitw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nwbrower.top/gtakuepzpm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jiagoushi.top/gtejrllxlw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtnuyjiguj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtkfpljfwp.html

Java: do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gthegyhnpz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jiagoushi.top/gtqkobgsaq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hfpthk.cn/gtujftodyg.html

C#:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gtvgahcbrw.html

[B09] break 与 continue
来源：http://hz.ybcxt.top/gtisklugfw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cucudq.cn/gteqhyqajt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.316326.xyz/gtiqyiouep.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gthacudynt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtxnzuitls.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtcenrbsib.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.pengpengdd.cyou/gtvzmrizfx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinqigufen.top/gtlvrbuhtc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtcridlpkf.html

[B10] 遍历同时拿索引
来源：http://hz.ppjwa.cn/gtbmoyivdm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jqgfzy.top/gttakrmpay.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtmuxgvyzj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigfzy.top/gtjmdcqxmn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.smart0.xyz/gtlptpwfxw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.pengpengdd.cyou/gtcsvnejnn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.birdmap.top/gthoizygta.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xingfuxueyuan.xyz/gtqsrajrff.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shuidangran.top/gtbyxqgsrb.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenlongwang.top/gtgorpbwvi.html

Py:   list(range(0, 10, 2))
来源：http://hz.yvedp.cn/gtgolhuoas.html

PHP:  range(0, 10, 2);
来源：http://hz.cucudq.cn/gttspkznqh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuanzx.com/gtaqtopibc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cqqwz.cn/gtpdmfeios.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shanyushiyangtech.top/gtvknhqcri.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.0kj1m.cn/gtbytlazzu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zdqjudy.top/gtcbdhavnt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj202588.top/gtvzqbimum.html

[B12] 跳出多层循环
来源：http://hz.smart0.xyz/gthxukwtju.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.havefunace.top/gtspqfsqxx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.smart0.xyz/gtrediltyh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtafnkethx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtngsshndy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtengvgmte.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cashguo.top/gtdgrfqrns.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxinkj.top/gtdrojhzfs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.pycfn.com/gttppxgune.html

[B13] 判断是否为数字
来源：http://hz.hfpthk.cn/gtyqkstibo.html

Py:   isinstance(x, (int, float))
来源：http://hz.meibo888.top/gththwbhvs.html

PHP:  is_numeric($x)
来源：http://hz.zycfv.cn/gtyvocetew.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnqzz.top/gtpfuenzdz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yueranfly.top/gthxkyivfq.html

Java: x instanceof Number
来源：http://hz.hnxiangtu.top/gtuqltgbob.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.vqdsnc.cn/gtnctgkwao.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yueranfly.top/gtjgiybhvs.html

C#:   x is int or double or decimal
来源：http://hz.birdmap.top/gthrdmurzb.html

[B14] 判断值是否在集合内
来源：http://hz.shuidangran.top/gtgjdojxyz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tian-w.cn/gtxzkvguwv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xuetiantiany.cn/gtlbnvhbzj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtojdvzszs.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtmrvfspxi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zycfv.cn/gtknykfumy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.tanke756.top/gtamduczma.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hongshengwenyu.top/gtvbiorpsp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nwbrower.top/gttuwfoigm.html

[B15] 布尔运算与取反
来源：http://hz.yangfankeji.com/gttzipkofa.html

Py:   a and b or not c
来源：http://hz.chenzaomai.com/gtpknworzf.html

PHP:  $a && $b || !$c
来源：http://hz.tian-w.cn/gttydrthnw.html

JS:   a && b || !c
来源：http://hz.pycfn.com/gtpieiejzt.html

TS:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtyamcjbuv.html

Java: a && b || !c
来源：http://hz.sxryk.cn/gtnbspfjhh.html

Go:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtmhsdcfiv.html

Ruby: a && b || !c
来源：http://hz.xylfe.cn/gtdbrvikso.html

C#:   a && b || !c
来源：http://hz.fengsongda.top/gtryczycir.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tanke756.top/gthxdumlgc.html

Py:   if not data: return
来源：http://hz.xingfuxueyuan.xyz/gtjtarvlap.html

PHP:  if (!$data) { return; }
来源：http://hz.xuanzx.com/gtxzxbryxu.html

JS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtmxziwfmn.html

TS:   if (!data) return;
来源：http://hz.xuanzx.com/gthbtpchxl.html

Java: if (data == null) return;
来源：http://hz.hfpthk.cn/gtycaqatzm.html

Go:   if data == nil { return }
来源：http://hz.jinqigfzy.top/gtxgbffeqk.html

Ruby: return if data.nil?
来源：http://hz.dianchejie.cn/gtgbzoijpe.html

C#:   if (data == null) return;
来源：http://hz.jinqigufen.top/gtsuiywnta.html

================================================================================
来源：http://hz.svipenyu.cn/gtuohhfngz.html

C. 函数与作用域
来源：http://hz.ywan-chungtsiang.top/gtcepvrwpi.html

================================================================================
来源：http://hz.hammf.cn/gtxqisgqpg.html

[C01] 定义函数
来源：http://hz.mhx1999.top/gtkohewddw.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtgzxnoayc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gtsysaoayq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yangfankeji.com/gtdpceztqh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sysykeji.top/gtilsslnir.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtjduxlwvq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gtolejtdyq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinqigfzy.top/gtcgyaesza.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gthpmvlzvt.html

[C02] 默认参数
来源：http://hz.sxryk.cn/gtynwvaitx.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtncsihpzs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.shangyingyoupin.top/gtweyqkqzl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.iojbl.cn/gtfjlyskqq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtmdsxznky.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dashuyun.cn/gtrjwnmmbq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.quarkkingdee.top/gtroxuppht.html

Ruby: def greet(name = "World") = name
来源：http://hz.aizwys.cn/gtkfmlqyeo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ydjk.org.cn/gtptmjfsvj.html

[C03] 可变参数
来源：http://hz.dashuyun.cn/gtueqqggqs.html

Py:   def total(*args): return sum(args)
来源：http://hz.havefunace.top/gtysaiumif.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxuanxn.top/gtdnujfidv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gogol.net.cn/gtzpsrmlsr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tianlin.xyz/gtkmrmshsc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cqqwz.cn/gtulglzlqz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gtsgalaaqs.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jlsjyb.cn/gtblbiqekd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xuetiantiany.cn/gtrqdsweto.html

[C04] 命名参数 / 关键字参数
来源：http://hz.havefunace.top/gtvgnbtxhy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cashguo.top/gtovbideap.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yvedp.cn/gtwkzhpiew.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtkkbrsbtp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.0kj1m.cn/gtqnevlqio.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cdnleiting.top/gtcpmhrrpp.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj202588.top/gtzcuuhauo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtpjttzwrd.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtdvsoreev.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtryaeqxwb.html

Py:   return a, b
来源：http://hz.zdqjudy.top/gtnrvxubcb.html

PHP:  return [$a, $b];
来源：http://hz.iojbl.cn/gtitydmwqn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinyuanbaomall.cn/gtrzozwawi.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtbdmttdov.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxinkj.top/gtcqqmldce.html

Go:   return a, b
来源：http://hz.zhaomingkeji.xyz/gtlhgbdwrl.html

Ruby: return a, b
来源：http://hz.zhijiandao.cn/gtydwmelnp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.feifeiyinyue.top/gtuipumcmq.html

[C06] 匿名函数 / lambda
来源：http://hz.hammf.cn/gtnpkxyavu.html

Py:   square = lambda x: x * x
来源：http://hz.yvedp.cn/gtphynjxmr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinyuanbaomall.cn/gtrxiqcsun.html

JS:   const square = x => x * x;
来源：http://hz.jqgufenzy.top/gtqjcxnaoy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ywan-chungtsiang.top/gtnlbtxsga.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xziqi.cn/gtetqinvhe.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigufen.top/gtdazmhjka.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yangfankeji.com/gtzqvlwbuc.html


<!-- 参考信息 -->