代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.jinyuanbaomall.cn/gtbtviinkc.html

TS:   const value = data ?? "默认值";
来源：http://hz.birdmap.top/gtpzfbwsnz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shanyushiyangtech.top/gtpqxdezma.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yj20258888.top/gtimyvikns.html

Ruby: value = data || "默认值"
来源：http://hz.zhijiandao.cn/gtvuhfuuvr.html

C#:   var value = data ?? "默认值";
来源：http://hz.9152youxi.cn/gtvmctkqtc.html

[A16] 真假值判断规则
来源：http://hz.ydjk.org.cn/gtsibdnoyk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.kuanghao11.cn/gtdlpknlyr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.fzhhl.top/gtuikhxgvu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.chenlongwang.top/gtorbuvsqq.html

TS:   if (!x) {}
来源：http://hz.pycfn.com/gthrnfattx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shuidangran.top/gtgtzyxqxk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.ehwqpu.com/gtexchsmtx.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.yj20258.top/gtkdlicqjz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.quarkkingdee.top/gtuyjnqkol.html

[A17] 位运算
来源：http://hz.yangfankeji.com/gtcmsccaxk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shuidangran.top/gtdbetkljb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.xuetiantiany.cn/gtlvzvkpws.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtbxcjgwpr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gtqzjqjfso.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtepwfjdtm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hongshengwenyu.top/gthooombqt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cashguo.top/gtmannmjhn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtidupaver.html

[A18] 字符与 ASCII 码互转
来源：http://hz.sysykeji.top/gtobyiurbp.html

Py:   ord("A"); chr(65)
来源：http://hz.52xcode.cn/gtpfiajgps.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhoulong.xyz/gtomjwdlaa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.52xcode.cn/gtwoiqsnzg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xuanzx.com/gtptyzyigu.html

Java: (int) 'A'; (char) 65
来源：http://hz.yueranfly.top/gtzasejxtn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.vqdsnc.cn/gtocyexyxe.html

Ruby: "A".ord; 65.chr
来源：http://hz.gzhubu.top/gtvjorxxok.html

C#:   (int)'A'; (char)65
来源：http://hz.hysaishi.cn/gtgekjinnp.html

[A19] 交换两个变量
来源：http://hz.52xcode.cn/gtllaempmu.html

Py:   a, b = b, a
来源：http://hz.sufxvd.cn/gtjxzobiqe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yj20258.top/gtzortktqr.html

JS:   [a, b] = [b, a];
来源：http://hz.gogol.net.cn/gtalyrikna.html

TS:   [a, b] = [b, a];
来源：http://hz.shanyushiyangtech.top/gtatmzpusm.html

Java: int t = a; a = b; b = t;
来源：http://hz.hnxiangtu.top/gtixlgnuye.html

Go:   a, b = b, a
来源：http://hz.sxryk.cn/gtfjmszonm.html

Ruby: a, b = b, a
来源：http://hz.jyoumei.cn/gtjlqeahfv.html

C#:   (a, b) = (b, a);
来源：http://hz.ppjwa.cn/gtrfrdncgg.html

[A20] 读取标准输入
来源：http://hz.dashuyun.cn/gtbqhewttz.html

Py:   name = input("请输入：")
来源：http://hz.tanke756.top/gtkflcixhv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.aibaodan.cn/gtoytjymhw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zhaomingkeji.xyz/gtzfqibjml.html

TS:   // Node.js：readline 模块
来源：http://hz.daxiang520.top/gtiacdojjy.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yangfankeji.com/gtgcmhyxuu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.nwbrower.top/gtcnnxqibh.html

Ruby: gets.chomp
来源：http://hz.daxiang520.top/gtjrrlsnjq.html

C#:   Console.ReadLine();
来源：http://hz.daria6918.cn/gtzjjlboea.html

[A21] 保留指定小数位输出
来源：http://hz.cheryme.top/gtifebvedq.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hfpthk.cn/gtzmkfvwrg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.shuidangran.top/gttgrwbmqo.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yj202588.top/gtsoxarhjn.html

TS:   (3.14159).toFixed(2)
来源：http://hz.sxryk.cn/gtfenynnzm.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yueranfly.top/gtxdafcovz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shanyushiyangkeji.top/gtfcqgujwh.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.wangdashe.top/gtvgaaflwa.html

C#:   3.14159.ToString("F2")
来源：http://hz.c1oappe.top/gtxnwcgadx.html

[A22] 获取字符串长度
来源：http://hz.nwbrower.top/gtlknbrdxl.html

Py:   len(s)
来源：http://hz.daria6918.cn/gtxnqijhlh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.9152youxi.cn/gtugjtoxlx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.ybcxt.top/gtyzdhegpy.html

TS:   s.length
来源：http://hz.hongshengwenyu.top/gtvamdamnk.html

Java: s.length()
来源：http://hz.cashguo.top/gtfivkyypv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.pycfn.com/gteqsydhml.html

Ruby: s.length
来源：http://hz.xuanzx.com/gtmzyhjmmi.html

C#:   s.Length
来源：http://hz.gaohongyu789.top/gtluxvxhwv.html

[A23] 大小写转换
来源：http://hz.fengsongda.top/gtsjehgsyj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.xziqi.cn/gtppegxykb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhoulong.xyz/gtrfphcsot.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuanzx.com/gtilijyjua.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tianlin.xyz/gtudfeguhs.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhengqikj.top/gtwqhcpmct.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.daria6918.cn/gtjjguftqg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhixingplan.top/gtagabisrj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.hongshengwenyu.top/gtoxenlcrh.html

[A24] 去除首尾空白
来源：http://hz.jinyuanbaomall.cn/gtrwcbkpmc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yvedp.cn/gtgtdabfln.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jyoumei.cn/gtunwjbymn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xinyue.icu/gtjxpxinby.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dianchejie.cn/gtmgbeijdj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.tianlin.xyz/gtfklslbki.html

Go:   strings.TrimSpace(s)
来源：http://hz.nanxuanxn.top/gtjkzmzohr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yj20258888.top/gtgnjmdzmi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jlsjyb.cn/gtvcscvdgh.html

[A25] 字符串比较
来源：http://hz.gotoacloud.top/gtolewmige.html

Py:   s1 == s2; s1 != s2
来源：http://hz.pengpengdd.cyou/gtwdpjephs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.dianchejie.cn/gtqmptjluj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.feifeiyinyue.top/gtbftakdme.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aizwys.cn/gtgzdzysgw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.cqqwz.cn/gtfcezbstu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xuanzx.com/gtbsywoyxx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.tianlin.xyz/gtjxiqbcpl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yj202588.top/gtvryixbjt.html

[A26] 类型转换总览
来源：http://hz.aibaodan.cn/gtpbchuhmc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yj202588.top/gtefgtydzs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jinqigfzy.top/gtbxsfnhrh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ydjk.org.cn/gtypecjmmz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.aibaodan.cn/gtmxnkciqs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xziqi.cn/gtoykxaeox.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.pengpengdd.cyou/gtaenceqdd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.havefunace.top/gtaumbuzet.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yj20258888.top/gtsxzaourt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdoarxbri.html

B. 流程控制
来源：http://hz.havefunace.top/gtatqvvypa.html

================================================================================
来源：http://hz.hammf.cn/gtujhhoapz.html

[B01] 条件判断 if / else
来源：http://hz.daxiang520.top/gtsdumvdya.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.daria6918.cn/gthnyzlrsp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gaohongyu789.top/gtwbmozaij.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nwbrower.top/gtgpdhuatk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cucudq.cn/gtfqsqchrh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.0kj1m.cn/gtbnshwumy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.shanyushiyangkeji.top/gtqlalyiuh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cdnleiting.top/gtrcpwynrd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtgpyvydsr.html

[B02] 多分支 else if / elif
来源：http://hz.vqdsnc.cn/gtrbyyumqo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jyoumei.cn/gtyrgwpqto.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hywenlv.cn/gtmrddvvfs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenzaomai.com/gtwdgmeotv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.redwolf501.top/gtyivwqbyh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.fengsongda.top/gtshxrintg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jinyuanbaomall.cn/gtlrrzpwyb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.nanxuanxn.top/gtjqjbhhrb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.birdmap.top/gtitcnuven.html

[B03] switch / match / case
来源：http://hz.sxryk.cn/gtbfnsairt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.guannengcc.top/gtlwnpvipk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtkgokgpry.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.guowangkeji.top/gteazhxgqx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yueranfly.top/gtmigpcmzk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.dianchejie.cn/gtetkktifb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yj20258.top/gtjzclauce.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cheryme.top/gtsztwxnfg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hfpthk.cn/gtnmwzhpxj.html

[B04] for 计数循环
来源：http://hz.xuanzx.com/gttvyrjiyv.html

Py:   for i in range(10): print(i)
来源：http://hz.zhijiandao.cn/gtxyiveryd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.hysaishi.cn/gtmfldhlxv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuxming.cn/gtsqrxghcy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258888.top/gtqumgfocn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.quarkkingdee.top/gtspspeefw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hnqzz.top/gtibrivcjw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xylfe.cn/gtmvpzvfqv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xinyue.icu/gthwgtzdgm.html

[B05] 遍历数组 / 列表
来源：http://hz.sxryk.cn/gtotkwldtr.html

Py:   for item in arr: print(item)
来源：http://hz.ivvv.top/gtnqbhwhxc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hammf.cn/gthhujdqce.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.316326.xyz/gtmvoowzds.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hfpthk.cn/gtwtefnvgr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hnxiangtu.top/gtzalsedjt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xuanzx.com/gtrwywrqhi.html

Ruby: arr.each { |item| puts item }
来源：http://hz.aizwys.cn/gtdouieyng.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hysaishi.cn/gtokdqtwzu.html

[B06] 遍历字典 / 对象
来源：http://hz.zhongyouzk.top/gtlfddasvt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.svipenyu.cn/gthdsyxlda.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.daxiang520.top/gtcehroizq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aizwys.cn/gtdfzetxqj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.wangdashe.top/gtshzzliic.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.quarkkingdee.top/gtrpiiypvf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhoulong.xyz/gtqpeqrggw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.haohaochexian.top/gttwehojqc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.nwbrower.top/gtfxeqgtjx.html

[B07] while 循环
来源：http://hz.ydzc1.top/gtrmscwnvg.html

Py:   while i < 10: i += 1
来源：http://hz.hywenlv.cn/gttgguxixf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinqigufen.top/gtlwiurlvo.html

JS:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtkzgbafjv.html

TS:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtsposgequ.html

Java: while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gtbkypfhwk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cqqwz.cn/gtqtbjnxsj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.fengsongda.top/gtyuylhidv.html

C#:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtqmubuwdc.html

[B08] do-while（至少执行一次）
来源：http://hz.cashguo.top/gtqfnedtcg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jqgufenzy.top/gttgbmopbp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258.top/gtgyouyfue.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtqohncqar.html

TS:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtawyxqtrw.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtykeeixwg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cheryme.top/gtjzsijziq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zdqjudy.top/gtakhllqps.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtduwhkzpr.html

[B09] break 与 continue
来源：http://hz.zhiwuduotai.top/gtqlpvicao.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hysaishi.cn/gtyqaxnjes.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hywenlv.cn/gtwrattpgb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtngfsiukd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhengqikj.top/gtmkrfhapa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtcvspwplt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.sysykeji.top/gtvmdayxcp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gaohongyu789.top/gtckoybpdi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtsylmruxl.html

[B10] 遍历同时拿索引
来源：http://hz.yj202588.top/gtjauedoyq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gtkacfmylv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhengqikj.top/gtvjotfxua.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.haohaochexian.top/gtjhwdzprd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtedxlygfx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.nwbrower.top/gtexoxdpfn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cdnleiting.top/gtldomgfsn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.wangshuangyany.cn/gtrvvduagd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jyoumei.cn/gtbqwzuryo.html

[B11] 生成数字序列 / 区间
来源：http://hz.hnqzz.top/gthuaagwlh.html

Py:   list(range(0, 10, 2))
来源：http://hz.cucudq.cn/gtsbnuoebx.html

PHP:  range(0, 10, 2);
来源：http://hz.jinqigfzy.top/gtjdfnwsnp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.birdmap.top/gtxxnkkbqa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtaxwpfkxx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.tanke756.top/gtwxpgnbod.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hongshengwenyu.top/gtvkdzohmu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yonumen.top/gtjmjxscjz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.aizwys.cn/gtksumrsfm.html

[B12] 跳出多层循环
来源：http://hz.9152youxi.cn/gtckfrgbvt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shangyingyoupin.top/gtdzxqtoei.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yongpay.top/gtquzszaxn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gtdmgcvpbq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gaohongyu789.top/gtbahjhpbg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hfpthk.cn/gtugsnylfs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.iojbl.cn/gtmitsdiqe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sufxvd.cn/gtstgupyci.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jlsjyb.cn/gtvzuusmgh.html

[B13] 判断是否为数字
来源：http://hz.fengsongda.top/gtbogyogei.html

Py:   isinstance(x, (int, float))
来源：http://hz.shangyingyoupin.top/gtyxzwqkww.html

PHP:  is_numeric($x)
来源：http://hz.sxryk.cn/gtshfihqzi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gtyietysls.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hammf.cn/gtpbwnbhzr.html

Java: x instanceof Number
来源：http://hz.jinqigfzy.top/gtkzowacez.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.mhx1999.top/gtkhchvnfb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ybcxt.top/gtpyylhmjm.html

C#:   x is int or double or decimal
来源：http://hz.iojbl.cn/gtydwwdmuf.html

[B14] 判断值是否在集合内
来源：http://hz.chenzaomai.com/gtomranwjo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xinyue.icu/gtfpzgijsp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtngdaqrnm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtpkcrmmwt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.dashuyun.cn/gtsebrdvzk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.c1oappe.top/gtzltwrniz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ivvv.top/gtxwiypzmg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ybcxt.top/gtcresfswm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gotoacloud.top/gtmzhjxlyp.html

[B15] 布尔运算与取反
来源：http://hz.jyoumei.cn/gtcokxgpit.html

Py:   a and b or not c
来源：http://hz.vqdsnc.cn/gtcuvpfnwk.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258.top/gtlsjirpvl.html

JS:   a && b || !c
来源：http://hz.zhengqikj.top/gtyfijyozl.html

TS:   a && b || !c
来源：http://hz.hnqzz.top/gtewbsqtgb.html

Java: a && b || !c
来源：http://hz.xuanzx.com/gtixtlskub.html

Go:   a && b || !c
来源：http://hz.bjfxy.top/gtdwzzvyvr.html

Ruby: a && b || !c
来源：http://hz.9152youxi.cn/gtddnymqzz.html

C#:   a && b || !c
来源：http://hz.fzhhl.top/gtlzuaxpsg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ydzc1.top/gtakxqrilm.html

Py:   if not data: return
来源：http://hz.vqdsnc.cn/gtdepenitu.html

PHP:  if (!$data) { return; }
来源：http://hz.zhengqikj.top/gtmhgrmivt.html

JS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtqrthzoxc.html

TS:   if (!data) return;
来源：http://hz.sysykeji.top/gtufggvure.html

Java: if (data == null) return;
来源：http://hz.hywenlv.cn/gtuhkqfmqa.html

Go:   if data == nil { return }
来源：http://hz.aizwys.cn/gtinharpgg.html

Ruby: return if data.nil?
来源：http://hz.kuanghao11.cn/gtnlfbnwhu.html

C#:   if (data == null) return;
来源：http://hz.yj20258.top/gthcbrzfjf.html

================================================================================
来源：http://hz.tian-w.cn/gtlqyzeetv.html

C. 函数与作用域
来源：http://hz.guowangkeji.top/gtdxvgnzrd.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcfytyeba.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gtyjmsibfn.html

Py:   def add(a, b): return a + b
来源：http://hz.jlsjyb.cn/gtadzjjgqv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtnlctmjoq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtzabhsjvz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sweek.top/gtvwiwefpf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtiwmsugng.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xinyue.icu/gtqualfnfp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jianghu66.top/gthaqmylzk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtcurcksrn.html

[C02] 默认参数
来源：http://hz.svipenyu.cn/gtemuivnwp.html

Py:   def greet(name="World"): return name
来源：http://hz.pengpengdd.cyou/gttlgjucek.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yanxiufei.cn/gtsflbuvbk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.9152youxi.cn/gtgnjwflgw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.pycfn.com/gtaxwvfyhs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ywan-chungtsiang.top/gthkmaqdfa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.meibo888.top/gtsurqleka.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhixingplan.top/gtnpayumhd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.52xcode.cn/gtfcessstu.html

[C03] 可变参数
来源：http://hz.sysykeji.top/gtkvtveifp.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258888.top/gttedfnuhn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jiagoushi.top/gtmemldres.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gtiwupmbzk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gttdwjowkg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jyoumei.cn/gtlrrkiiao.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhixingplan.top/gtveawkcqb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj202588.top/gtiqaqkbxj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guannengcc.top/gtkhnwxgso.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtenbtyufw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj20258888.top/gtzcrmklnz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gtndegoxew.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hongshengwenyu.top/gtgsmeedxz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cdnleiting.top/gtjsnwuxyg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.c1oappe.top/gtwwcrpmxf.html

Go:   // 无：用配置结构体参数
来源：http://hz.hnxiangtu.top/gtrdncsuns.html

Ruby: f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtkzkmmsci.html

C#:   f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gtiisltslp.html

[C05] 返回多个值
来源：http://hz.iojbl.cn/gtphgsakhg.html

Py:   return a, b
来源：http://hz.havefunace.top/gturpydsgp.html

PHP:  return [$a, $b];
来源：http://hz.aibaodan.cn/gtbnsdlcyo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.9152youxi.cn/gtvbkqlney.html

TS:   return { a, b };
来源：http://hz.gaohongyu789.top/gtgqvbcspb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydzc1.top/gtpafitcfn.html

Go:   return a, b
来源：http://hz.ybcxt.top/gtrkwxbera.html

Ruby: return a, b
来源：http://hz.zhijiandao.cn/gtcrazfwpd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.9152youxi.cn/gtinihpslz.html


<!-- 参考信息 -->