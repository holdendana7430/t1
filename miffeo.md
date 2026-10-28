代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.yangfankeji.com/gteezhuhtl.html

[A15] 空值判断与默认值
来源：http://hz.bjfxy.top/gtijounzmt.html

Py:   value = data or "默认值"
来源：http://hz.yonumen.top/gthtbxlyyz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.yj202588.top/gtmehfirux.html

JS:   const value = data ?? "默认值";
来源：http://hz.gzhubu.top/gtpwhxqaqw.html

TS:   const value = data ?? "默认值";
来源：http://hz.aibaodan.cn/gtjflhcnlc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.cucudq.cn/gtmmawippi.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.316326.xyz/gtkpjmycxc.html

Ruby: value = data || "默认值"
来源：http://hz.yongpay.top/gtsldwrfvr.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinqigfzy.top/gtwfahihqh.html

[A16] 真假值判断规则
来源：http://hz.yongpay.top/gtowyuvert.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.chenjidiqi.icu/gtlnhfgixn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yueranfly.top/gtkctvgbtx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jinyuanbaomall.cn/gtxxacjkjv.html

TS:   if (!x) {}
来源：http://hz.wangshuangyany.cn/gtifyewhtu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.c1oappe.top/gtcgklclma.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zhixingplan.top/gtxerwgoow.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.sysykeji.top/gtnvwxreup.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.fengsongda.top/gttxymkeib.html

[A17] 位运算
来源：http://hz.cdnleiting.top/gtmvvlbzdg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zycfv.cn/gtuaogtkkw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yueranfly.top/gterrluwbg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj202588.top/gtczgigquc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.nwbrower.top/gtnlklyndi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtzfwrchzc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yj20258888.top/gtwfogjlpn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hnqzz.top/gtlkoygvfv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtlzkfbmju.html

[A18] 字符与 ASCII 码互转
来源：http://hz.bjfxy.top/gtloiopohg.html

Py:   ord("A"); chr(65)
来源：http://hz.aibaodan.cn/gtfflqrdcc.html

PHP:  ord("A"); chr(65)
来源：http://hz.feifeiyinyue.top/gtvyuzfhbh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.vqdsnc.cn/gtoctceknu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gotoacloud.top/gtwnozrsrq.html

Java: (int) 'A'; (char) 65
来源：http://hz.9152youxi.cn/gtydziyhed.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.0kj1m.cn/gtjfanikgy.html

Ruby: "A".ord; 65.chr
来源：http://hz.jinghuilouyu.cn/gtqdefsbcp.html

C#:   (int)'A'; (char)65
来源：http://hz.bjfxy.top/gtfmafwhnp.html

[A19] 交换两个变量
来源：http://hz.ehwqpu.com/gtzskiefct.html

Py:   a, b = b, a
来源：http://hz.zhaomingkeji.xyz/gtkyekafsr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.316326.xyz/gtyhkacccl.html

JS:   [a, b] = [b, a];
来源：http://hz.hnqzz.top/gtnptbdmmk.html

TS:   [a, b] = [b, a];
来源：http://hz.bjfxy.top/gtugvyjryi.html

Java: int t = a; a = b; b = t;
来源：http://hz.pengpengdd.cyou/gtgyoivtnu.html

Go:   a, b = b, a
来源：http://hz.xuetiantiany.cn/gtayairumt.html

Ruby: a, b = b, a
来源：http://hz.yongpay.top/gtibvndqir.html

C#:   (a, b) = (b, a);
来源：http://hz.feifeiyinyue.top/gtvikvjsua.html

[A20] 读取标准输入
来源：http://hz.gotoacloud.top/gtzjpwxfcf.html

Py:   name = input("请输入：")
来源：http://hz.nwbrower.top/gtytsmttho.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yvedp.cn/gtpirpqcna.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.redwolf501.top/gtylyweydb.html

TS:   // Node.js：readline 模块
来源：http://hz.kuanghao11.cn/gttzxtsqid.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.cqqwz.cn/gtlvumhmrm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jiagoushi.top/gtaabwzmkj.html

Ruby: gets.chomp
来源：http://hz.zhixingplan.top/gtbcsofpxe.html

C#:   Console.ReadLine();
来源：http://hz.chenzaomai.com/gtnapbgjnf.html

[A21] 保留指定小数位输出
来源：http://hz.shanyushiyangtech.top/gtytbaxlol.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ybcxt.top/gtigfmfsdc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yangfankeji.com/gtkdetvweg.html

JS:   (3.14159).toFixed(2)
来源：http://hz.guannengcc.top/gtukydnxtz.html

TS:   (3.14159).toFixed(2)
来源：http://hz.xingfuxueyuan.xyz/gtetbnzril.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jinghuilouyu.cn/gtlhhwiuhe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.chenlongwang.top/gtcejmyrus.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yuanzhike.top/gtrzvwxkph.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhijiandao.cn/gtbpdusrqd.html

[A22] 获取字符串长度
来源：http://hz.gzhubu.top/gtsricugwh.html

Py:   len(s)
来源：http://hz.c1oappe.top/gtxutztqbr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.haohaochexian.top/gtlrbuemtc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.haohaochexian.top/gtnoggflqh.html

TS:   s.length
来源：http://hz.shangyingyoupin.top/gtwjuyndpk.html

Java: s.length()
来源：http://hz.jianghu66.top/gtdgircfcq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.gotoacloud.top/gtgmlhhreu.html

Ruby: s.length
来源：http://hz.iojbl.cn/gtgdxvidcb.html

C#:   s.Length
来源：http://hz.shuidangran.top/gtgtsukppe.html

[A23] 大小写转换
来源：http://hz.ydzc1.top/gtmeonbxrr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jinghuilouyu.cn/gtrtwyegje.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.tanke756.top/gtoplcstgp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yongpay.top/gtfdyprzlz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cdnleiting.top/gtvdxnwcoy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.tianlin.xyz/gtqdsinbes.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.xuanzx.com/gtemgkeubu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.nanxinkj.top/gttfpgunnz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.dianchejie.cn/gtlybdpvui.html

[A24] 去除首尾空白
来源：http://hz.gaohongyu789.top/gtbyttdbdb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.sufxvd.cn/gtgpkffbua.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.birdmap.top/gtukxdfouy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zdqjudy.top/gtfsjvcute.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenlongwang.top/gttqwqrwrg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.chenlongwang.top/gtajlspywk.html

Go:   strings.TrimSpace(s)
来源：http://hz.cqqwz.cn/gtqvlbsjlq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jqgfzy.top/gtxrwhatmc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.wangshuangyany.cn/gtoftmrmwe.html

[A25] 字符串比较
来源：http://hz.havefunace.top/gthklidcrp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.aizwys.cn/gtnduznqew.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.wangshuangyany.cn/gtcxfbzyxb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hnqzz.top/gtydzbabek.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgfzy.top/gteeefmfrc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.wangdashe.top/gtiaxxtuao.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ppjwa.cn/gtesujgqjm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhengqikj.top/gtxlehtvxe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gzhubu.top/gtdvsfulpc.html

[A26] 类型转换总览
来源：http://hz.gaohongyu789.top/gtaachapaj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sysykeji.top/gtjrpbqfuo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.iojbl.cn/gtngzmqrdb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yanxiufei.cn/gtedpovrva.html

TS:   Number() String() Boolean() x as number
来源：http://hz.mhx1999.top/gtkwkfovcs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.feifeiyinyue.top/gtnlkxtinq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.tianlin.xyz/gtlrvksboh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.nanxuanxn.top/gtcnwpcfyz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zycfv.cn/gtphltdvow.html

================================================================================
来源：http://hz.cucudq.cn/gtcsiwllho.html

B. 流程控制
来源：http://hz.aizwys.cn/gtglacpamp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdxhnmbkf.html

[B01] 条件判断 if / else
来源：http://hz.wangdashe.top/gtbnxwcitj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.birdmap.top/gtkfpcichx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hnqzz.top/gtdpljsych.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.andypj.xyz/gtghtinnkk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtrfxbuqbj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gaohongyu789.top/gtfxwixtui.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.chenzaomai.com/gtxbevzbiz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jqgufenzy.top/gtfudkyxue.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtneydaqur.html

[B02] 多分支 else if / elif
来源：http://hz.ydjk.org.cn/gtyzqetahm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.xziqi.cn/gtleatjdqm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ehwqpu.com/gtrpasqfzv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.9152youxi.cn/gtmompyoii.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gtiolfjzhq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtzxgujhnp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shanyushiyangkeji.top/gtyckarsde.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hnxiangtu.top/gtzsizqznb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtwavaezjt.html

[B03] switch / match / case
来源：http://hz.yuxming.cn/gtbovphkls.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hywenlv.cn/gtrvctwnon.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gogol.net.cn/gtqovixvtv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aizwys.cn/gtjvxciowm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sufxvd.cn/gtlhptrglh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.316326.xyz/gtkmczlbjb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.c1oappe.top/gtuthjppvn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.9152youxi.cn/gtngyeeerc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.snrcjt.cn/gtiofvnyfs.html

[B04] for 计数循环
来源：http://hz.hywenlv.cn/gtasuyngwl.html

Py:   for i in range(10): print(i)
来源：http://hz.nwbrower.top/gtaoxkntla.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ybcxt.top/gtgxlvmgqi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtrzusryxu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhengqikj.top/gtdioragzx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jinyuanbaomall.cn/gtokemvjhr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hywenlv.cn/gtmndkgork.html

Ruby: 10.times { |i| puts i }
来源：http://hz.feifeiyinyue.top/gtepmsogfv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jinyuanbaomall.cn/gtrtodxecv.html

[B05] 遍历数组 / 列表
来源：http://hz.yj20258.top/gtntcvyzos.html

Py:   for item in arr: print(item)
来源：http://hz.yvedp.cn/gtqlhogxzm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.iojbl.cn/gtudskgeoa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.iojbl.cn/gtcbpvimwg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.nanxinkj.top/gtifhtncsr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.daria6918.cn/gttcxoxqds.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.wangdashe.top/gtlirlzyqj.html

Ruby: arr.each { |item| puts item }
来源：http://hz.chenlongwang.top/gtywgnfynk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.cdnleiting.top/gtaxykimjh.html

[B06] 遍历字典 / 对象
来源：http://hz.0kj1m.cn/gtxswdsbxw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuxming.cn/gtlywlstbe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.guannengcc.top/gtzjxgbpqi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj202588.top/gtkanbthyh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yanxiufei.cn/gtswwtybmy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xuanzx.com/gtlsvmmgwe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sufxvd.cn/gtrspmcslz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zycfv.cn/gtuupymiie.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cheryme.top/gtvbnklrac.html

[B07] while 循环
来源：http://hz.ydjk.org.cn/gtmvlmirbb.html

Py:   while i < 10: i += 1
来源：http://hz.c1oappe.top/gtkvfsymnc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhoulong.xyz/gtpqcgdwxt.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtiltkxzgq.html

TS:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtzlcdbxyc.html

Java: while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtkjsscmxf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinyuanbaomall.cn/gtjvrohhvi.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xziqi.cn/gtsbzkopnp.html

C#:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtwdfuytfm.html

[B08] do-while（至少执行一次）
来源：http://hz.hongshengwenyu.top/gtovxkglez.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jqgufenzy.top/gtzkvqphow.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.svipenyu.cn/gtwmlprdhf.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtyzitfutw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gtiafsxdrj.html

Java: do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtoliindok.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.daria6918.cn/gtaqipzirp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jqgufenzy.top/gtjtjggthv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtwwurvuvm.html

[B09] break 与 continue
来源：http://hz.nwbrower.top/gtcbelpypg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shzxlz.cn/gtdocyfcgd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hfpthk.cn/gtafckoetf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtdzswligv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtvmazicjq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtvlecydvl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.mhx1999.top/gtmhmvlgwl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gotoacloud.top/gtdpqewevo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtsjfvznwu.html

[B10] 遍历同时拿索引
来源：http://hz.nwbrower.top/gtgphcbzio.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dianchejie.cn/gtqdkfnpiw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.pengpengdd.cyou/gtxssuynnm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zdqjudy.top/gtzcxqgepd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yj20258888.top/gtmxtlzdra.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sweek.top/gtvigsqaea.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.nwbrower.top/gtnpjgipdp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ybcxt.top/gtbovexvtd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cqqwz.cn/gtlsetloyv.html

[B11] 生成数字序列 / 区间
来源：http://hz.yonumen.top/gtzbgweorv.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258.top/gtvttwponj.html

PHP:  range(0, 10, 2);
来源：http://hz.xuanzx.com/gtaiuxisft.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtpblfaszc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtrmvcwtqn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.tianlin.xyz/gtqgwwkbvv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tian-w.cn/gtvchzizsk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangkeji.top/gtmgwoplzt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.9152youxi.cn/gtytgvtckn.html

[B12] 跳出多层循环
来源：http://hz.shuidangran.top/gtxacwtgdb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ydjk.org.cn/gtiahavmvd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhengqikj.top/gtvwagznwk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtjidhdvui.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtfasqhxgn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gtxgkbuctz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ydzc1.top/gtrhqgxotu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.wangshuangyany.cn/gtjojrdkvv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhijiandao.cn/gtymeqgyqy.html

[B13] 判断是否为数字
来源：http://hz.xinyue.icu/gtqxlyowti.html

Py:   isinstance(x, (int, float))
来源：http://hz.sxryk.cn/gtiyregdpm.html

PHP:  is_numeric($x)
来源：http://hz.yonumen.top/gtmzrwnixs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinyuanbaomall.cn/gtgpinlpzm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.svipenyu.cn/gtbxalwgak.html

Java: x instanceof Number
来源：http://hz.zhiwuduotai.top/gtwdxfpmpq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhixingplan.top/gtbotivtii.html

Ruby: x.is_a?(Numeric)
来源：http://hz.quarkkingdee.top/gtqwwfmrjr.html

C#:   x is int or double or decimal
来源：http://hz.hnqzz.top/gtdhhtrxmu.html

[B14] 判断值是否在集合内
来源：http://hz.jyoumei.cn/gtvbicxmuw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhiwuduotai.top/gthmmtrwey.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydzc1.top/gtoayzxrfd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtpwtuyndk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gtzpqzsmqf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhaomingkeji.xyz/gtyxwexkwq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cdnleiting.top/gtxzhqvpdv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tanke756.top/gtdcxfvnwe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ybcxt.top/gtjhpwrtjl.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangtech.top/gtpndrxgng.html

Py:   a and b or not c
来源：http://hz.xingfuxueyuan.xyz/gtzqjusxqg.html

PHP:  $a && $b || !$c
来源：http://hz.ybcxt.top/gtftitbifd.html

JS:   a && b || !c
来源：http://hz.zhijiandao.cn/gtnuertzbm.html

TS:   a && b || !c
来源：http://hz.yvedp.cn/gtkqbslejw.html

Java: a && b || !c
来源：http://hz.zhoulong.xyz/gtfmjjetcf.html

Go:   a && b || !c
来源：http://hz.zdqjudy.top/gttxsdvmcx.html

Ruby: a && b || !c
来源：http://hz.guannengcc.top/gtufkldumf.html

C#:   a && b || !c
来源：http://hz.fengsongda.top/gtdtceycpp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shanyushiyangkeji.top/gtvkclmpea.html

Py:   if not data: return
来源：http://hz.tian-w.cn/gtyajdkqtu.html

PHP:  if (!$data) { return; }
来源：http://hz.mhx1999.top/gtpdizfygz.html

JS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtkvwtnsgz.html

TS:   if (!data) return;
来源：http://hz.xuanzx.com/gtzyjxzscm.html

Java: if (data == null) return;
来源：http://hz.wangdashe.top/gtncjfamnw.html

Go:   if data == nil { return }
来源：http://hz.ydjk.org.cn/gtcbxnlpbf.html

Ruby: return if data.nil?
来源：http://hz.pycfn.com/gtdcqxpfis.html

C#:   if (data == null) return;
来源：http://hz.wangdashe.top/gtrntwiqor.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqmiftrls.html

C. 函数与作用域
来源：http://hz.zhengqikj.top/gtdqpflpby.html

================================================================================
来源：http://hz.tian-w.cn/gtmwatjika.html

[C01] 定义函数
来源：http://hz.xuetiantiany.cn/gtiokzcpzg.html

Py:   def add(a, b): return a + b
来源：http://hz.cdnleiting.top/gtuqfbgqmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtninwxhpu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtchocdeav.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtdqurrklb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtmffijpaz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgufenzy.top/gttwwgskam.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj20258888.top/gtcyjzwpge.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtmszqtxux.html

[C02] 默认参数
来源：http://hz.cqqwz.cn/gtpdshfryh.html

Py:   def greet(name="World"): return name
来源：http://hz.pengpengdd.cyou/gtolozusjf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yonumen.top/gtjlemruvt.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cqqwz.cn/gtsfvkdqdv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtouwmryjx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hywenlv.cn/gtaztgxump.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtlclyjiwb.html

Ruby: def greet(name = "World") = name
来源：http://hz.yanxiufei.cn/gtvzdbogfs.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnqzz.top/gtwhwcniyp.html

[C03] 可变参数
来源：http://hz.zdqjudy.top/gtcxxdplfv.html

Py:   def total(*args): return sum(args)
来源：http://hz.52xcode.cn/gtvpruyuce.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtmjkgktaw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtjhyavnbk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtvniblfom.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj20258.top/gtqrdwhpht.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangshuangyany.cn/gtpsiwbixm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuetiantiany.cn/gtpfmgnxox.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.vqdsnc.cn/gtaqqrdogj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shuidangran.top/gtvplobypr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.aibaodan.cn/gtateiehrn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yueranfly.top/gtqktybidc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtvfhtnuzg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yuanzhike.top/gtmwnmxqdo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hammf.cn/gtpheulfjb.html

Go:   // 无：用配置结构体参数
来源：http://hz.aibaodan.cn/gtfaqtmaxx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtxvuteuhb.html

C#:   f(a: 1, b: 2)
来源：http://hz.gzhubu.top/gtgadryzxj.html

[C05] 返回多个值
来源：http://hz.haohaochexian.top/gtgcaztuxp.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtemmkalgr.html

PHP:  return [$a, $b];
来源：http://hz.cqqwz.cn/gthsyhgdjh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hongshengwenyu.top/gtwyichhhp.html

TS:   return { a, b };
来源：http://hz.meibo888.top/gtmaxcfcgr.html


<!-- 参考信息 -->