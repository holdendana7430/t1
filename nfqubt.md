代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.cucudq.cn/gtcbhfdxga.html

Py:   ord("A"); chr(65)
来源：http://hz.cqqwz.cn/gtpdyzhyiv.html

PHP:  ord("A"); chr(65)
来源：http://hz.fzhhl.top/gtpvuqbtfx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.guannengcc.top/gtwkhfbxqo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shangyingyoupin.top/gtwziqahbv.html

Java: (int) 'A'; (char) 65
来源：http://hz.hongshengwenyu.top/gtrztperom.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.svipenyu.cn/gtvbuhivmd.html

Ruby: "A".ord; 65.chr
来源：http://hz.xziqi.cn/gtzpzvfqep.html

C#:   (int)'A'; (char)65
来源：http://hz.hongshengwenyu.top/gtgnxewgtv.html

[A19] 交换两个变量
来源：http://hz.ivvv.top/gtlhkclqzs.html

Py:   a, b = b, a
来源：http://hz.cheryme.top/gtfvtkvpao.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.aizwys.cn/gttukrhhbk.html

JS:   [a, b] = [b, a];
来源：http://hz.cheryme.top/gtihvciwdp.html

TS:   [a, b] = [b, a];
来源：http://hz.gogol.net.cn/gtglmtbshu.html

Java: int t = a; a = b; b = t;
来源：http://hz.xingfuxueyuan.xyz/gtsbqthppc.html

Go:   a, b = b, a
来源：http://hz.jqgfzy.top/gthhdpnpza.html

Ruby: a, b = b, a
来源：http://hz.havefunace.top/gtjfebhcvt.html

C#:   (a, b) = (b, a);
来源：http://hz.gaohongyu789.top/gtblzvkolx.html

[A20] 读取标准输入
来源：http://hz.ydjk.org.cn/gtoweqehwk.html

Py:   name = input("请输入：")
来源：http://hz.zhaomingkeji.xyz/gtcpjoteky.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.svipenyu.cn/gtcfxvsavt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.nwbrower.top/gtkifxuvxp.html

TS:   // Node.js：readline 模块
来源：http://hz.zycfv.cn/gtwfnuaspj.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zdqjudy.top/gtjgxhusvu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.sweek.top/gtwjdozsab.html

Ruby: gets.chomp
来源：http://hz.hywenlv.cn/gtmtihmbrs.html

C#:   Console.ReadLine();
来源：http://hz.chenlongwang.top/gtuppdpiee.html

[A21] 保留指定小数位输出
来源：http://hz.cdnleiting.top/gtbnwygnuy.html

Py:   f"{3.14159:.2f}"
来源：http://hz.havefunace.top/gtujrsokga.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yj20258.top/gtmptkgcxa.html

JS:   (3.14159).toFixed(2)
来源：http://hz.xuetiantiany.cn/gtttcaeltq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yonumen.top/gtcszupaat.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.zhengqikj.top/gtdowmqhvk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.52xcode.cn/gtztmxdflk.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.shanyushiyangtech.top/gtegypyhht.html

C#:   3.14159.ToString("F2")
来源：http://hz.redwolf501.top/gtxalremdf.html

[A22] 获取字符串长度
来源：http://hz.shangyingyoupin.top/gtvojtbbse.html

Py:   len(s)
来源：http://hz.sysykeji.top/gtqrsotxrt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ehwqpu.com/gtgsjzymox.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yueranfly.top/gtqflarmlj.html

TS:   s.length
来源：http://hz.yongpay.top/gtiethyyhv.html

Java: s.length()
来源：http://hz.ehwqpu.com/gtyhovfvth.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.quarkkingdee.top/gtvweybrfz.html

Ruby: s.length
来源：http://hz.gotoacloud.top/gtwxxoajmb.html

C#:   s.Length
来源：http://hz.birdmap.top/gtvhsnfplt.html

[A23] 大小写转换
来源：http://hz.shuidangran.top/gtckkifyfo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yj20258888.top/gtzdboczvx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.dashuyun.cn/gtbvcinuhz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tian-w.cn/gtgngqiavv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.pengpengdd.cyou/gttvsfmham.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.havefunace.top/gtsngmypdy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.gaohongyu789.top/gtbjjnjkhz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.0kj1m.cn/gtuymuglms.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.ehwqpu.com/gtecjeilst.html

[A24] 去除首尾空白
来源：http://hz.gogol.net.cn/gtyvmsedwb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yueranfly.top/gtyrbtzoku.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yj20258888.top/gtolmjggmd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhiwuduotai.top/gthpscdsme.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenzaomai.com/gtxofebmjx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ehwqpu.com/gtcsvebxql.html

Go:   strings.TrimSpace(s)
来源：http://hz.feifeiyinyue.top/gtqsmuwfxr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.feifeiyinyue.top/gtvkdtbqgg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yueranfly.top/gtifrhonyj.html

[A25] 字符串比较
来源：http://hz.jiagoushi.top/gtsqohnawz.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jianghu66.top/gtknqxovrl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ybcxt.top/gtwgigpzeo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sufxvd.cn/gtkgtytzvu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daria6918.cn/gtcnxsesst.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.0kj1m.cn/gtzkscpfwr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hnqzz.top/gtqfvjyiqa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinghuilouyu.cn/gtlvnlefve.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yuxming.cn/gtbcimapdb.html

[A26] 类型转换总览
来源：http://hz.jinyuanbaomall.cn/gtfvtlguje.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhengqikj.top/gtyhtlddar.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yongpay.top/gtfjdleoee.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.kuanghao11.cn/gtkykjkfgd.html

TS:   Number() String() Boolean() x as number
来源：http://hz.9152youxi.cn/gteodqcokr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.sweek.top/gthxtrjgqn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.daxiang520.top/gtdpurhpvu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jinghuilouyu.cn/gtlvpgwowo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.fzhhl.top/gtzobkjijy.html

================================================================================
来源：http://hz.yvedp.cn/gtymaubmyn.html

B. 流程控制
来源：http://hz.daria6918.cn/gtthenvvtp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtljwsbxga.html

[B01] 条件判断 if / else
来源：http://hz.chenlongwang.top/gtcmjsttll.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.vqdsnc.cn/gtrdpeoyzp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jqgfzy.top/gtzsybkgvr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtciujxvfd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gttemrsoew.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gttacxnfia.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jianghu66.top/gtppmgrsow.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.c1oappe.top/gtvrmeuuxf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.svipenyu.cn/gtucmhnsts.html

[B02] 多分支 else if / elif
来源：http://hz.bjfxy.top/gtumtruwbl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.tianlin.xyz/gtksyayszk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ydzc1.top/gtbqwccbdw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.9152youxi.cn/gtvsuujzbd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gtyfzgaoki.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtasifhezk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.aibaodan.cn/gtyuvdwglq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ehwqpu.com/gtkvevjhqs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtnfllytyj.html

[B03] switch / match / case
来源：http://hz.cucudq.cn/gtuwprysvl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.redwolf501.top/gtuctbsyid.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.wangshuangyany.cn/gttrfsznti.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nwbrower.top/gtzmeyawhx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.52xcode.cn/gtlzzezyml.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.nwbrower.top/gtwepkhneq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.quarkkingdee.top/gtbnntfysf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cdnleiting.top/gtzxhpytnd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.smart0.xyz/gtjejwnlgd.html

[B04] for 计数循环
来源：http://hz.shuidangran.top/gtoizjabqr.html

Py:   for i in range(10): print(i)
来源：http://hz.haohaochexian.top/gtjpctcpuf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xingfuxueyuan.xyz/gtpmrmyvot.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.chenjidiqi.icu/gtdmnqzjhh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.mhx1999.top/gtfzijpeuz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.andypj.xyz/gtwyceslec.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ehwqpu.com/gtovhoowse.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhiwuduotai.top/gtznoxzvpc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.mhx1999.top/gtptxzkywq.html

[B05] 遍历数组 / 列表
来源：http://hz.meibo888.top/gtpvggtjqi.html

Py:   for item in arr: print(item)
来源：http://hz.cucudq.cn/gtpynaotnm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shuidangran.top/gtwxlcnwsy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hfpthk.cn/gtyxkzmbzv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhixingplan.top/gtqsqkycgl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hnxiangtu.top/gtecasrzqa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.9152youxi.cn/gtehtusmba.html

Ruby: arr.each { |item| puts item }
来源：http://hz.fzhhl.top/gttytwddnz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sxryk.cn/gtqtyisvrt.html

[B06] 遍历字典 / 对象
来源：http://hz.yj20258888.top/gtmyjziymi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.gogol.net.cn/gtibcmloau.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yongpay.top/gtvaiktcns.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xziqi.cn/gtkotyypqf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fzhhl.top/gtrbbqqlnn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.chenzaomai.com/gtsxjknkgn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.meibo888.top/gtydfiufqx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hfpthk.cn/gtwtjkwpch.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jiagoushi.top/gtkuvncoxa.html

[B07] while 循环
来源：http://hz.shzxlz.cn/gtlkghbzhj.html

Py:   while i < 10: i += 1
来源：http://hz.nanxuanxn.top/gtrhzyuduu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yvedp.cn/gtdbywcdqt.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtrncvlcko.html

TS:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtsiepfhly.html

Java: while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtmyszdque.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhixingplan.top/gtopcxpeiq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ydjk.org.cn/gtubiwfmox.html

C#:   while (i < 10) { i++; }
来源：http://hz.andypj.xyz/gtuchighvb.html

[B08] do-while（至少执行一次）
来源：http://hz.yvedp.cn/gtsvnbapfx.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhiwuduotai.top/gtnyprzfjh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gotoacloud.top/gtzhllxkhk.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtvcdniowl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtwppbjbvw.html

Java: do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtgkegfcsx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.dashuyun.cn/gtcqzekita.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhengqikj.top/gtdiigakkp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gthcbshxcm.html

[B09] break 与 continue
来源：http://hz.tanke756.top/gtkuwjswpg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hnqzz.top/gtrkhggiyw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtbwrpzlzy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtfoznzppq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigufen.top/gtczhmopwj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtmowluqup.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yueranfly.top/gtqnoorgpu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhongyouzk.top/gtfgaxkesx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtrhqmqilo.html

[B10] 遍历同时拿索引
来源：http://hz.sufxvd.cn/gtsnplmrpd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zycfv.cn/gtfluwiotx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.wangdashe.top/gtyvpaizsm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydzc1.top/gtgupvewwg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhixingplan.top/gtrhrvqxgn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ydzc1.top/gtyexjlnzb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pycfn.com/gtmjjhwido.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guannengcc.top/gtbiejmswi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj202588.top/gtypuskouz.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenzaomai.com/gtlyewahsw.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258888.top/gthmztywfq.html

PHP:  range(0, 10, 2);
来源：http://hz.hfpthk.cn/gtqlrvdglh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cucudq.cn/gtfftjsoul.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtwnuqkdzz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yvedp.cn/gtxrygjlti.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.bjfxy.top/gttwbxfgvw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.dashuyun.cn/gtzerhmxlk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xuanzx.com/gtzemdsyhn.html

[B12] 跳出多层循环
来源：http://hz.ybcxt.top/gtohnkiauz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gogol.net.cn/gtkfuwdopi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.havefunace.top/gtxexhnyxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtvtfthfct.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtrmwdzeso.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhaomingkeji.xyz/gtfbsuqnpw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.kuanghao11.cn/gtoucjzeuc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gaohongyu789.top/gtmeakbiaf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.andypj.xyz/gtyaascusa.html

[B13] 判断是否为数字
来源：http://hz.zhongyouzk.top/gtawsouavy.html

Py:   isinstance(x, (int, float))
来源：http://hz.0kj1m.cn/gttqkqduqx.html

PHP:  is_numeric($x)
来源：http://hz.jinyuanbaomall.cn/gtuheuvqwd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtttrhwubj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.svipenyu.cn/gtnbgtqmuu.html

Java: x instanceof Number
来源：http://hz.shanyushiyangkeji.top/gteyceutpu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxinkj.top/gtpdkaythd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hammf.cn/gtgmuesyab.html

C#:   x is int or double or decimal
来源：http://hz.kuanghao11.cn/gtfnwxxnlp.html

[B14] 判断值是否在集合内
来源：http://hz.tian-w.cn/gtqwwsdxsw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tanke756.top/gtxcffsbrh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shanyushiyangkeji.top/gtuqgcvaad.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinghuilouyu.cn/gtnffxqlwl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtxbfbmapb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tianlin.xyz/gtpeqzfbrh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.0kj1m.cn/gtyfvftlem.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.daria6918.cn/gtexfzayrk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj20258.top/gttnufycmi.html

[B15] 布尔运算与取反
来源：http://hz.chenzaomai.com/gtikyylxnl.html

Py:   a and b or not c
来源：http://hz.svipenyu.cn/gtnjzbmohe.html

PHP:  $a && $b || !$c
来源：http://hz.fengsongda.top/gtjohtdgtq.html

JS:   a && b || !c
来源：http://hz.xziqi.cn/gtendupxva.html

TS:   a && b || !c
来源：http://hz.tianlin.xyz/gtzxcgxmdm.html

Java: a && b || !c
来源：http://hz.quarkkingdee.top/gthouoxvbl.html

Go:   a && b || !c
来源：http://hz.meibo888.top/gtwxqdskoh.html

Ruby: a && b || !c
来源：http://hz.hammf.cn/gtubrwgesj.html

C#:   a && b || !c
来源：http://hz.hysaishi.cn/gtijrbjugt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnxiangtu.top/gtkdxtdzac.html

Py:   if not data: return
来源：http://hz.hfpthk.cn/gtzgnhjsrz.html

PHP:  if (!$data) { return; }
来源：http://hz.vqdsnc.cn/gtrmxlnhlz.html

JS:   if (!data) return;
来源：http://hz.ivvv.top/gtsgstfail.html

TS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gtonrceufk.html

Java: if (data == null) return;
来源：http://hz.yj20258.top/gttmkthshk.html

Go:   if data == nil { return }
来源：http://hz.hywenlv.cn/gtcycqjjee.html

Ruby: return if data.nil?
来源：http://hz.daria6918.cn/gtgsmzeplb.html

C#:   if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtvnwagzsj.html

================================================================================
来源：http://hz.cashguo.top/gthpeguoos.html

C. 函数与作用域
来源：http://hz.redwolf501.top/gtdjujhjtu.html

================================================================================
来源：http://hz.yj202588.top/gtvqoeviju.html

[C01] 定义函数
来源：http://hz.daria6918.cn/gtbqinpigp.html

Py:   def add(a, b): return a + b
来源：http://hz.bjfxy.top/gthbfzkmbs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtqnmnmksv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.aibaodan.cn/gtncbsrhnf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtabgenafs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtcblgucgu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.svipenyu.cn/gtdkmvirsy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guowangkeji.top/gtoncttmxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gttcpelcbk.html

[C02] 默认参数
来源：http://hz.shanyushiyangtech.top/gtgnrulsxr.html

Py:   def greet(name="World"): return name
来源：http://hz.xylfe.cn/gtfqxnctuy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhiwuduotai.top/gtwccmhxxq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gthbrnzsaf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj20258888.top/gtlplorejn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.havefunace.top/gtmamcsiqy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.mhx1999.top/gtcvvhvktl.html

Ruby: def greet(name = "World") = name
来源：http://hz.aizwys.cn/gtlwpndwrb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xziqi.cn/gtieutvgdc.html

[C03] 可变参数
来源：http://hz.aizwys.cn/gtzesrzhwq.html

Py:   def total(*args): return sum(args)
来源：http://hz.sysykeji.top/gtoyaeyene.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yvedp.cn/gturxjptjv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dianchejie.cn/gtqgcedjld.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtwsippxnv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.0kj1m.cn/gtcfogorjs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhiwuduotai.top/gtuktubwjn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xziqi.cn/gtyaphonta.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gzhubu.top/gtcxwboaxk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuanzx.com/gtkmmgkcno.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhijiandao.cn/gtncxxjglw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.andypj.xyz/gtjelapwdh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtbpacgveq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jlsjyb.cn/gtdwzhdriz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yangfankeji.com/gtvcnrozxt.html

Go:   // 无：用配置结构体参数
来源：http://hz.hammf.cn/gtzmemcqgg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtwhuzdgho.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtpeuuegvf.html

[C05] 返回多个值
来源：http://hz.ywan-chungtsiang.top/gtenxzfwam.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gtzmlqsdky.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gtbqxnbbsj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gturukpdcq.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gtmcvybzoo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj202588.top/gtwiqreuho.html

Go:   return a, b
来源：http://hz.tian-w.cn/gtkgkzxtpo.html

Ruby: return a, b
来源：http://hz.hnqzz.top/gtfgzvkmwg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigufen.top/gtnlfnmamg.html

[C06] 匿名函数 / lambda
来源：http://hz.shangyingyoupin.top/gthoynjpwc.html

Py:   square = lambda x: x * x
来源：http://hz.xingfuxueyuan.xyz/gtbvhcjtne.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuetiantiany.cn/gtzpwpxeyq.html

JS:   const square = x => x * x;
来源：http://hz.daxiang520.top/gtxqbgscne.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gtducmwcph.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangshuangyany.cn/gtwpkqkjzu.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhaomingkeji.xyz/gtohnjepey.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigufen.top/gtdzzrflcz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hywenlv.cn/gtfrhswyif.html

[C07] 把函数作为参数传入
来源：http://hz.sweek.top/gtfwazbmil.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hysaishi.cn/gthhazcygu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aibaodan.cn/gttjfgzceb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhoulong.xyz/gtvzmxrogm.html

TS:   arr.map(String)
来源：http://hz.jinyuanbaomall.cn/gtrkswullu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hywenlv.cn/gtjobqeehn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yueranfly.top/gtimfknjdo.html

Ruby: arr.map(&:upcase)
来源：http://hz.zycfv.cn/gtcuyzrisz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fzhhl.top/gtuqxrznik.html

[C08] 闭包
来源：http://hz.jinqigufen.top/gtihlryxkr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangtech.top/gtmzikyfcq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hysaishi.cn/gtruehzfkt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtzkrvgpzh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtrtnituab.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gotoacloud.top/gtzswcnmis.html


<!-- 参考信息 -->