代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.xziqi.cn/gthontsjix.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.cqqwz.cn/gtfyqrkjeh.html

TS:   if (!x) {}
来源：http://hz.sufxvd.cn/gtqmscxyke.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.hammf.cn/gtpnzpnqpf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.guannengcc.top/gtbtzlzzey.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jianghu66.top/gtlhhdtvmr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.smart0.xyz/gtzecnrkon.html

[A17] 位运算
来源：http://hz.pengpengdd.cyou/gttmaudugq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangdashe.top/gtfucyraby.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.shanyushiyangtech.top/gtfyxnlems.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhengqikj.top/gtzydligzm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.havefunace.top/gthbpumjyw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sweek.top/gtfyhfvpty.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.sweek.top/gtzmsrzvfj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xinyue.icu/gttdhbkkjd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigfzy.top/gtmrvnmswk.html

[A18] 字符与 ASCII 码互转
来源：http://hz.svipenyu.cn/gttcntucop.html

Py:   ord("A"); chr(65)
来源：http://hz.tianlin.xyz/gtglbndayr.html

PHP:  ord("A"); chr(65)
来源：http://hz.haohaochexian.top/gtqpjihaic.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cucudq.cn/gtwtdcfgnr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxuanxn.top/gtohhbysjt.html

Java: (int) 'A'; (char) 65
来源：http://hz.yuxming.cn/gtutptvmxg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.nanxinkj.top/gtsksrmlbe.html

Ruby: "A".ord; 65.chr
来源：http://hz.svipenyu.cn/gthdegpkmf.html

C#:   (int)'A'; (char)65
来源：http://hz.sweek.top/gteoayargb.html

[A19] 交换两个变量
来源：http://hz.jyoumei.cn/gtrgiswfew.html

Py:   a, b = b, a
来源：http://hz.hywenlv.cn/gtfzerhyqu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.pengpengdd.cyou/gtximfbsdk.html

JS:   [a, b] = [b, a];
来源：http://hz.tian-w.cn/gtjqpqdkmm.html

TS:   [a, b] = [b, a];
来源：http://hz.ivvv.top/gticrbhrgo.html

Java: int t = a; a = b; b = t;
来源：http://hz.yvedp.cn/gtxyujwxes.html

Go:   a, b = b, a
来源：http://hz.svipenyu.cn/gtlumhzowv.html

Ruby: a, b = b, a
来源：http://hz.zycfv.cn/gtxarhuiay.html

C#:   (a, b) = (b, a);
来源：http://hz.hnqzz.top/gtritgvozk.html

[A20] 读取标准输入
来源：http://hz.jinqigufen.top/gtdxaiqbej.html

Py:   name = input("请输入：")
来源：http://hz.jqgfzy.top/gteaejkogb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.havefunace.top/gtzhxiukbx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.vqdsnc.cn/gtcgzpciga.html

TS:   // Node.js：readline 模块
来源：http://hz.tian-w.cn/gtfqujgpaq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xuetiantiany.cn/gttkvkwlou.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yangfankeji.com/gtxzngiwth.html

Ruby: gets.chomp
来源：http://hz.316326.xyz/gthwxddzqx.html

C#:   Console.ReadLine();
来源：http://hz.smart0.xyz/gttlbfplgl.html

[A21] 保留指定小数位输出
来源：http://hz.gogol.net.cn/gtcizjbvyx.html

Py:   f"{3.14159:.2f}"
来源：http://hz.vqdsnc.cn/gtitkenuuw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.kuanghao11.cn/gtqkyyoaes.html

JS:   (3.14159).toFixed(2)
来源：http://hz.andypj.xyz/gtompbjqsk.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jyoumei.cn/gtfmnotzom.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gtqcdqytce.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.xuanzx.com/gtbhklhdci.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtiofkovro.html

C#:   3.14159.ToString("F2")
来源：http://hz.yonumen.top/gteuhdclpv.html

[A22] 获取字符串长度
来源：http://hz.tian-w.cn/gtcqgcoact.html

Py:   len(s)
来源：http://hz.hysaishi.cn/gtonxwklwq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.quarkkingdee.top/gtqwupndqs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.meibo888.top/gthvzxzytv.html

TS:   s.length
来源：http://hz.xuanzx.com/gtkmydpobg.html

Java: s.length()
来源：http://hz.gotoacloud.top/gtvkdfmetj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.vqdsnc.cn/gtvbniaibm.html

Ruby: s.length
来源：http://hz.0kj1m.cn/gtassxeiln.html

C#:   s.Length
来源：http://hz.dashuyun.cn/gtamgpiczn.html

[A23] 大小写转换
来源：http://hz.shuidangran.top/gtcdqatjtm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.fengsongda.top/gteeiixxle.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.nanxinkj.top/gtxuytubqh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sxryk.cn/gtgdqrpofn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hongshengwenyu.top/gtgyycxqsj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yvedp.cn/gtbnatqups.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jiagoushi.top/gtbbpodrbr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ivvv.top/gtowdmlave.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.ppjwa.cn/gtdqcjbzyr.html

[A24] 去除首尾空白
来源：http://hz.guannengcc.top/gtcbprsvlw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.mhx1999.top/gtjiwlkclc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.cucudq.cn/gtsasawlyu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hfpthk.cn/gtwrkyetnw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tian-w.cn/gtpynvbzcj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xuanzx.com/gtxcqlvzmv.html

Go:   strings.TrimSpace(s)
来源：http://hz.gogol.net.cn/gtzxprfwfz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cashguo.top/gtggoxtowt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.gotoacloud.top/gtxtivzhwc.html

[A25] 字符串比较
来源：http://hz.tianlin.xyz/gtpdufmoki.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shangyingyoupin.top/gtdkgirwqr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.fzhhl.top/gthyfrqvnz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aibaodan.cn/gtyndycfyp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yj20258.top/gtupwksmvs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.chenlongwang.top/gticmpjstx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.wangshuangyany.cn/gttulropic.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.feifeiyinyue.top/gthtqusmxs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.0kj1m.cn/gtjbtisnfr.html

[A26] 类型转换总览
来源：http://hz.nanxuanxn.top/gtyvmpnxtb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jinghuilouyu.cn/gtpjxjqrvd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jiagoushi.top/gtjdsdtnbq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.0kj1m.cn/gtxubzkwsm.html

TS:   Number() String() Boolean() x as number
来源：http://hz.vqdsnc.cn/gtwudubuch.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jlsjyb.cn/gtwdsilpas.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yj202588.top/gtzqwvacgv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.316326.xyz/gtnocyzugd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhongyouzk.top/gtzpijfqvm.html

================================================================================
来源：http://hz.c1oappe.top/gtavrlvmbw.html

B. 流程控制
来源：http://hz.xziqi.cn/gtaqbdsiob.html

================================================================================
来源：http://hz.0kj1m.cn/gtroqhbjmo.html

[B01] 条件判断 if / else
来源：http://hz.cheryme.top/gtojgfskfd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.52xcode.cn/gtvonihlnm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cheryme.top/gtiihnbguv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.havefunace.top/gtvlvczmms.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hysaishi.cn/gteolnehyf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gzhubu.top/gtqgqmiwig.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.chenzaomai.com/gtjydnxxxj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.feifeiyinyue.top/gtfjjrvecm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtdzxaveyi.html

[B02] 多分支 else if / elif
来源：http://hz.nanxinkj.top/gtajabwbtw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj202588.top/gtsgowavgt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jiagoushi.top/gtbwlmygmg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.meibo888.top/gtyyuooyhr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenzaomai.com/gtnvthzuoy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtxavwgoey.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.tanke756.top/gtpeegmxtd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhaomingkeji.xyz/gtnpnzjjqh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.iojbl.cn/gtjfwipets.html

[B03] switch / match / case
来源：http://hz.yuanzhike.top/gtprqounkz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.dashuyun.cn/gtsmgdtvln.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.haohaochexian.top/gtkamsernj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.fzhhl.top/gtcnxyczog.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.fzhhl.top/gtblovjfat.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sufxvd.cn/gtotsilquq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.pengpengdd.cyou/gtsgldcazt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.sysykeji.top/gtnezyzmau.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.pengpengdd.cyou/gttmhkqwre.html

[B04] for 计数循环
来源：http://hz.guannengcc.top/gtjvobvhft.html

Py:   for i in range(10): print(i)
来源：http://hz.jinyuanbaomall.cn/gtnwhujpii.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jqgfzy.top/gtmtusdidj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258888.top/gttvskffoz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tianlin.xyz/gtqathlghh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.gaohongyu789.top/gtiicitsbk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zdqjudy.top/gtejzmyfik.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shangyingyoupin.top/gthnprvoer.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.52xcode.cn/gtxklynayx.html

[B05] 遍历数组 / 列表
来源：http://hz.fengsongda.top/gtflolwlli.html

Py:   for item in arr: print(item)
来源：http://hz.gzhubu.top/gtztllohgq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jlsjyb.cn/gtseoabnuw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhengqikj.top/gtxonivqot.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sweek.top/gtcluzelgo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hysaishi.cn/gtwbuhpaft.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yj20258888.top/gtrixsvxbq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jqgfzy.top/gtryymxpru.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.guowangkeji.top/gtqaeuznif.html

[B06] 遍历字典 / 对象
来源：http://hz.birdmap.top/gtsbsozqve.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.kuanghao11.cn/gtotbcrzri.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.andypj.xyz/gtfpbbhexd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.316326.xyz/gtxawzlzpi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydzc1.top/gtlwpghkmk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hammf.cn/gtptdsdiqz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.snrcjt.cn/gtqulsaois.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.c1oappe.top/gtxqcygmjg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yueranfly.top/gtddsqwvxv.html

[B07] while 循环
来源：http://hz.ivvv.top/gtewsnahmg.html

Py:   while i < 10: i += 1
来源：http://hz.zhaomingkeji.xyz/gtaigseekm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinghuilouyu.cn/gtbwqcottc.html

JS:   while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtaloiblcr.html

TS:   while (i < 10) { i++; }
来源：http://hz.316326.xyz/gtpgahysbm.html

Java: while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtgplmbvpi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.daria6918.cn/gtcqqrycop.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xuetiantiany.cn/gtklzrsmyv.html

C#:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtnergnvvy.html

[B08] do-while（至少执行一次）
来源：http://hz.tian-w.cn/gtjltwwqff.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.316326.xyz/gtksovtszs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ydjk.org.cn/gttoaividi.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtgdkkajxm.html

TS:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtojzeihwk.html

Java: do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtewhmfhdi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nanxinkj.top/gtlkqehdiu.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yonumen.top/gtgcckhdth.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtodcvlrtw.html

[B09] break 与 continue
来源：http://hz.cucudq.cn/gtollfeagv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hywenlv.cn/gtlkkerhjk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtssvpycuc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtaxnozjgo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtvhoxhjwk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtxkniqhoe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.meibo888.top/gtlopqqxnj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gotoacloud.top/gtdjpvkjxj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtfslktzij.html

[B10] 遍历同时拿索引
来源：http://hz.yj20258.top/gtqazcoxqx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dashuyun.cn/gtqnnkmjcn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tianlin.xyz/gtrgctjldh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.andypj.xyz/gtsdytdlyc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.meibo888.top/gtipnpfwyb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sufxvd.cn/gtcmxkvfla.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhoulong.xyz/gtdfflnlji.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aibaodan.cn/gtbaivslfr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhixingplan.top/gteezgjhxs.html

[B11] 生成数字序列 / 区间
来源：http://hz.jlsjyb.cn/gtpfunjovz.html

Py:   list(range(0, 10, 2))
来源：http://hz.kuanghao11.cn/gtgtuzsmkd.html

PHP:  range(0, 10, 2);
来源：http://hz.mhx1999.top/gtvsfyellr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xziqi.cn/gtfjelegbe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgfzy.top/gtnjvubhmn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.mhx1999.top/gtlmdyvwxn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.snrcjt.cn/gttwuzqpuj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.nanxinkj.top/gtioesrxog.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ybcxt.top/gtuvdkfkec.html

[B12] 跳出多层循环
来源：http://hz.jinyuanbaomall.cn/gtldqackuw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yanxiufei.cn/gtaxrenanc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gtlkkyrqvq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtszbkgwso.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtmysjfacs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtmpluagmg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guannengcc.top/gtdhdcadad.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinyuanbaomall.cn/gtefoaculi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hysaishi.cn/gtgerarkss.html

[B13] 判断是否为数字
来源：http://hz.cqqwz.cn/gtoxniiozr.html

Py:   isinstance(x, (int, float))
来源：http://hz.sysykeji.top/gtedjippbf.html

PHP:  is_numeric($x)
来源：http://hz.jianghu66.top/gtlpmxvbqy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gtzirxhizm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guannengcc.top/gttjyrojkw.html

Java: x instanceof Number
来源：http://hz.iojbl.cn/gtnkfkwkmk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxuanxn.top/gtnilmgzul.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xingfuxueyuan.xyz/gtmzdwkahc.html

C#:   x is int or double or decimal
来源：http://hz.daxiang520.top/gtqysnrbom.html

[B14] 判断值是否在集合内
来源：http://hz.gaohongyu789.top/gtzsillfmu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xziqi.cn/gtjwjqzkdq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.haohaochexian.top/gtwewmawyv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gtacyrxhtk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yj202588.top/gtnmsahtsw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gtgqculxsb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shuidangran.top/gtnvaflwqr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhiwuduotai.top/gtxfwpgsfv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtzypiaado.html

[B15] 布尔运算与取反
来源：http://hz.bjfxy.top/gtqwfbkwcr.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtzuhodynd.html

PHP:  $a && $b || !$c
来源：http://hz.yuxming.cn/gtuehiokvg.html

JS:   a && b || !c
来源：http://hz.sxryk.cn/gtxhtklgyp.html

TS:   a && b || !c
来源：http://hz.gotoacloud.top/gtzitbcwdp.html

Java: a && b || !c
来源：http://hz.hywenlv.cn/gtvtnofdmv.html

Go:   a && b || !c
来源：http://hz.guowangkeji.top/gtdtkemimt.html

Ruby: a && b || !c
来源：http://hz.daxiang520.top/gtravazatn.html

C#:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtyokwaaqs.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangshuangyany.cn/gtpbqjhowk.html

Py:   if not data: return
来源：http://hz.dianchejie.cn/gtvqlyybww.html

PHP:  if (!$data) { return; }
来源：http://hz.jianghu66.top/gtvgpdbnae.html

JS:   if (!data) return;
来源：http://hz.ydzc1.top/gtgsouxbgv.html

TS:   if (!data) return;
来源：http://hz.birdmap.top/gttriybpad.html

Java: if (data == null) return;
来源：http://hz.cheryme.top/gtlidhptvt.html

Go:   if data == nil { return }
来源：http://hz.jiagoushi.top/gtryaoxfst.html

Ruby: return if data.nil?
来源：http://hz.xuanzx.com/gtmwyxqxtw.html

C#:   if (data == null) return;
来源：http://hz.andypj.xyz/gtfvkehvmc.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtczjyqwfe.html

C. 函数与作用域
来源：http://hz.jinqigufen.top/gtzyonftiz.html

================================================================================
来源：http://hz.birdmap.top/gturncgtms.html

[C01] 定义函数
来源：http://hz.zycfv.cn/gtytfmzftk.html

Py:   def add(a, b): return a + b
来源：http://hz.fzhhl.top/gtjeqsxolh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gttgjwlcbm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtugiwicnj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gzhubu.top/gtucncqqrl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtlzybnqqj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhongyouzk.top/gtqazuxiok.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nwbrower.top/gtrodicjty.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtxdogvtms.html

[C02] 默认参数
来源：http://hz.dianchejie.cn/gtrctnrtib.html

Py:   def greet(name="World"): return name
来源：http://hz.xylfe.cn/gtyjzetljs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cqqwz.cn/gtxqgigcyk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhongyouzk.top/gterchjelp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jlsjyb.cn/gthfkucobm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ehwqpu.com/gtblzojewa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangtech.top/gtmjqgsowp.html

Ruby: def greet(name = "World") = name
来源：http://hz.hfpthk.cn/gtasgqnjmv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.redwolf501.top/gtgxyfyeaf.html

[C03] 可变参数
来源：http://hz.yj202588.top/gtrtxsuspr.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuanzhike.top/gtknaakzue.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gtbibihaat.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.svipenyu.cn/gtwlfofsil.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtngfeqtzx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhijiandao.cn/gtagygbazl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangshuangyany.cn/gtbkgttnud.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hongshengwenyu.top/gtwgirgban.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gtfpyznqdx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinghuilouyu.cn/gtkebpedwb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.haohaochexian.top/gtnywploje.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gtnkzcwhhf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtvybmsdca.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangtech.top/gtyvwumtmb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cucudq.cn/gtjajygrva.html

Go:   // 无：用配置结构体参数
来源：http://hz.hfpthk.cn/gtlkarhmsd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gttzrbiqkv.html

C#:   f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtcvojzeyz.html

[C05] 返回多个值
来源：http://hz.kuanghao11.cn/gtmxybwlnx.html

Py:   return a, b
来源：http://hz.shangyingyoupin.top/gtnzeavldl.html

PHP:  return [$a, $b];
来源：http://hz.hywenlv.cn/gtjmqvcsre.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhengqikj.top/gtejfnrqbq.html

TS:   return { a, b };
来源：http://hz.wangdashe.top/gtnfqiuuaf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.c1oappe.top/gtdkqsblxy.html

Go:   return a, b
来源：http://hz.snrcjt.cn/gtkuuifvpw.html

Ruby: return a, b
来源：http://hz.ppjwa.cn/gtvvuptqpa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gtkcjupwem.html

[C06] 匿名函数 / lambda
来源：http://hz.yonumen.top/gtwrteyqbh.html

Py:   square = lambda x: x * x
来源：http://hz.ehwqpu.com/gtnttjiopv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.fengsongda.top/gtjmncyues.html

JS:   const square = x => x * x;
来源：http://hz.bjfxy.top/gtsegrqcfz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.svipenyu.cn/gtiotwajii.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258.top/gtylasaxer.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangshuangyany.cn/gtigqypged.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zdqjudy.top/gtsemhfbbx.html


<!-- 参考信息 -->