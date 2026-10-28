代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.tianlin.xyz/gtbwalmouw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.vqdsnc.cn/gtpquytvlh.html

TS:   if (!x) {}
来源：http://hz.hysaishi.cn/gtkmsjcbcj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.pycfn.com/gttuythzjp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zhiwuduotai.top/gthbpszufr.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zhongyouzk.top/gtfykrvydu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.haohaochexian.top/gtgzwoywmo.html

[A17] 位运算
来源：http://hz.yj202588.top/gtexgeewcg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtxlggdnjo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.guannengcc.top/gthftylakq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.birdmap.top/gtctrxxbwv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jinqigfzy.top/gtvbubcsul.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtidsatoxs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ehwqpu.com/gthynatiuz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtraoanlbx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gtncajfutm.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jinqigfzy.top/gtgzzquwvl.html

Py:   ord("A"); chr(65)
来源：http://hz.hywenlv.cn/gtjvonrujx.html

PHP:  ord("A"); chr(65)
来源：http://hz.hysaishi.cn/gtvcpldhyu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sysykeji.top/gtjzkeacpc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.bjfxy.top/gtfcfwmxgm.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhiwuduotai.top/gtdpweeihw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.pycfn.com/gtrwqtsudm.html

Ruby: "A".ord; 65.chr
来源：http://hz.jqgufenzy.top/gtqmidlaxy.html

C#:   (int)'A'; (char)65
来源：http://hz.zhiwuduotai.top/gtzxssszmm.html

[A19] 交换两个变量
来源：http://hz.hammf.cn/gtgvxysaoz.html

Py:   a, b = b, a
来源：http://hz.daria6918.cn/gtvkandnkf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jinqigufen.top/gtobewffue.html

JS:   [a, b] = [b, a];
来源：http://hz.316326.xyz/gtstrxbwhl.html

TS:   [a, b] = [b, a];
来源：http://hz.wangshuangyany.cn/gtzropxslx.html

Java: int t = a; a = b; b = t;
来源：http://hz.redwolf501.top/gtaswfhibc.html

Go:   a, b = b, a
来源：http://hz.haohaochexian.top/gthjcahqqd.html

Ruby: a, b = b, a
来源：http://hz.pycfn.com/gtxtnrowii.html

C#:   (a, b) = (b, a);
来源：http://hz.yj20258888.top/gtgqtuwday.html

[A20] 读取标准输入
来源：http://hz.fengsongda.top/gtiaruixie.html

Py:   name = input("请输入：")
来源：http://hz.yangfankeji.com/gtkdepdxas.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ywan-chungtsiang.top/gtrqqiziav.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zycfv.cn/gtbjnyndvl.html

TS:   // Node.js：readline 模块
来源：http://hz.jiagoushi.top/gtrwhozzbz.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.hnqzz.top/gtbvbcmyir.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yuxming.cn/gtsgudwpfj.html

Ruby: gets.chomp
来源：http://hz.chenjidiqi.icu/gtmfwhyxsf.html

C#:   Console.ReadLine();
来源：http://hz.yueranfly.top/gtzvjhgocv.html

[A21] 保留指定小数位输出
来源：http://hz.52xcode.cn/gtesyiccgy.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yvedp.cn/gtpmmmggjh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cashguo.top/gtscjylocs.html

JS:   (3.14159).toFixed(2)
来源：http://hz.316326.xyz/gtqhdkoodi.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jyoumei.cn/gtrhslthzn.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.sxryk.cn/gtjqdomgwk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.meibo888.top/gtxmryshtw.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.nanxinkj.top/gtbdsxkylv.html

C#:   3.14159.ToString("F2")
来源：http://hz.nwbrower.top/gtnakiayjb.html

[A22] 获取字符串长度
来源：http://hz.aizwys.cn/gtijnxrnle.html

Py:   len(s)
来源：http://hz.yj20258888.top/gthuacecks.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yueranfly.top/gtvjxemnrk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.guannengcc.top/gtwbbfylbu.html

TS:   s.length
来源：http://hz.gaohongyu789.top/gtwegmmbfk.html

Java: s.length()
来源：http://hz.zhoulong.xyz/gtcawmdiky.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhijiandao.cn/gtfongmngl.html

Ruby: s.length
来源：http://hz.ehwqpu.com/gtptdlfaaj.html

C#:   s.Length
来源：http://hz.nanxuanxn.top/gtvbgjdzlc.html

[A23] 大小写转换
来源：http://hz.tian-w.cn/gthzeqdvom.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yueranfly.top/gtaiakrmna.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yj20258.top/gtskfnvnya.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.feifeiyinyue.top/gteeptizhl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.haohaochexian.top/gtdzuaczpw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.fzhhl.top/gtdxzvdzbx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.tian-w.cn/gtdihxlxnh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinqigufen.top/gtoanauzur.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jinghuilouyu.cn/gtklafhara.html

[A24] 去除首尾空白
来源：http://hz.zdqjudy.top/gtsribpeos.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhongyouzk.top/gtandtrhtw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.chenjidiqi.icu/gtktdqsyek.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangdashe.top/gtzhtukprr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangshuangyany.cn/gtxcmbfrpf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.daxiang520.top/gtshyrhjol.html

Go:   strings.TrimSpace(s)
来源：http://hz.shuidangran.top/gtccqioczy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhengqikj.top/gtqbmoxhsg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.iojbl.cn/gthgrvmptj.html

[A25] 字符串比较
来源：http://hz.hongshengwenyu.top/gtnnbsxcnm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yonumen.top/gtzpfnptsu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ppjwa.cn/gtahhtajce.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daxiang520.top/gtqpwjwvrf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.wangdashe.top/gtmvlrgois.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.nwbrower.top/gtotklgcjx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ehwqpu.com/gtiolfvwvx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shangyingyoupin.top/gtbibrrdlp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yuanzhike.top/gtreupyllw.html

[A26] 类型转换总览
来源：http://hz.sufxvd.cn/gtillaqzem.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.52xcode.cn/gtsrisrkjp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.quarkkingdee.top/gteizkixkh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yj20258888.top/gtxphylukt.html

TS:   Number() String() Boolean() x as number
来源：http://hz.shuidangran.top/gtkgxiaokk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ybcxt.top/gtrlclthpi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.guowangkeji.top/gtnutndvez.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.feifeiyinyue.top/gthhcntjhf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ydjk.org.cn/gtiynfozpz.html

================================================================================
来源：http://hz.chenlongwang.top/gtngowiiti.html

B. 流程控制
来源：http://hz.hnxiangtu.top/gtzwvctryx.html

================================================================================
来源：http://hz.jqgfzy.top/gtuoijabmj.html

[B01] 条件判断 if / else
来源：http://hz.jinghuilouyu.cn/gtlqbjmdyv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.daria6918.cn/gtsnrddbyk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hfpthk.cn/gtswockjuo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ydzc1.top/gtiunyrjik.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtieddtgli.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.c1oappe.top/gtuybgxnrb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yj20258888.top/gttzuzpzir.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yueranfly.top/gthkjzzslx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.vqdsnc.cn/gtcktetgfz.html

[B02] 多分支 else if / elif
来源：http://hz.jianghu66.top/gtezbbsnma.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.meibo888.top/gtwlfhgjro.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xuanzx.com/gtnjpranhu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gthpdfawxr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.vqdsnc.cn/gtpdkfjjsi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtgfoivjqt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.cheryme.top/gtoryycyro.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.cashguo.top/gtpdcffegy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gthoylgull.html

[B03] switch / match / case
来源：http://hz.ivvv.top/gtkqoflxju.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.chenjidiqi.icu/gtifniuqwa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daria6918.cn/gtvibipxxe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtuthfdkxb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.52xcode.cn/gtzxzrkskm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shanyushiyangtech.top/gtoswooppv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.pengpengdd.cyou/gtpqfiyshm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenlongwang.top/gtbjmozuuv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.tanke756.top/gtsaauytnn.html

[B04] for 计数循环
来源：http://hz.yanxiufei.cn/gturnhtjsj.html

Py:   for i in range(10): print(i)
来源：http://hz.hfpthk.cn/gtjupwkhzw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhoulong.xyz/gtfccpjlsy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pycfn.com/gtsgmtztjw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhaomingkeji.xyz/gtmfpfwwnb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.tanke756.top/gtiwevnxun.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hongshengwenyu.top/gtlydbpasz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hnqzz.top/gtweqmqppl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.pycfn.com/gtuqnnicgq.html

[B05] 遍历数组 / 列表
来源：http://hz.9152youxi.cn/gtawuwljov.html

Py:   for item in arr: print(item)
来源：http://hz.gogol.net.cn/gtzqgmgtgb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jinyuanbaomall.cn/gtjnkplcjs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhaomingkeji.xyz/gtbpygvasm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.tian-w.cn/gtwvmelppn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jyoumei.cn/gtgasyrtqq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.redwolf501.top/gtkdujmpec.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yuxming.cn/gtjbruajxc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.aibaodan.cn/gtatjxbnli.html

[B06] 遍历字典 / 对象
来源：http://hz.tanke756.top/gtuiydatim.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.haohaochexian.top/gthbsadljy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.chenjidiqi.icu/gtnnjqeumk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.svipenyu.cn/gtzcrmuchh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhongyouzk.top/gtiryiuyah.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yvedp.cn/gtvmosiaaq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.dashuyun.cn/gtnouuorjs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ydzc1.top/gteybizrkd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ybcxt.top/gtdbgmgwfb.html

[B07] while 循环
来源：http://hz.yj20258.top/gtoeainbct.html

Py:   while i < 10: i += 1
来源：http://hz.cqqwz.cn/gtilisrbhp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.tian-w.cn/gtmallwipi.html

JS:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtebveeorj.html

TS:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtgjmgwdgs.html

Java: while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtwqgwgzvg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhaomingkeji.xyz/gtdnnicxmd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jyoumei.cn/gtzepwgiqz.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtcgcmcexd.html

[B08] do-while（至少执行一次）
来源：http://hz.nanxuanxn.top/gtbyzhoqwh.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cashguo.top/gtftgurbke.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sufxvd.cn/gtpfcbzaui.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gthtfshcrd.html

TS:   do { i++; } while (i < 10);
来源：http://hz.haohaochexian.top/gtzvpgtwpq.html

Java: do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtprptupio.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xinyue.icu/gtoeaijllo.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.9152youxi.cn/gtnkmtrkky.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhoulong.xyz/gtxgmlobbr.html

[B09] break 与 continue
来源：http://hz.guowangkeji.top/gtyytfhhix.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.snrcjt.cn/gtbltmcbhp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinqigufen.top/gtmhwizvwh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtyhlluwlj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtdnqjbpkm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtdgepxvke.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gogol.net.cn/gtmziovqux.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhengqikj.top/gtgpfeokdv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhijiandao.cn/gtwwnpuptb.html

[B10] 遍历同时拿索引
来源：http://hz.ppjwa.cn/gtoyninvpn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jlsjyb.cn/gtlxbbpulm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yvedp.cn/gtlavanzfn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhaomingkeji.xyz/gtcsceneup.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtegwcrert.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yanxiufei.cn/gtkgoswntf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.daxiang520.top/gtntdcvojq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gogol.net.cn/gtagmjteyu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ivvv.top/gtadbnnowq.html

[B11] 生成数字序列 / 区间
来源：http://hz.52xcode.cn/gtxllidcgo.html

Py:   list(range(0, 10, 2))
来源：http://hz.hfpthk.cn/gtaxcehfpe.html

PHP:  range(0, 10, 2);
来源：http://hz.gogol.net.cn/gtlwlewmvv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.9152youxi.cn/gtggmnjihv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtfdjqvgli.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtylpkzupj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gotoacloud.top/gtbbuafhki.html

Ruby: (0...10).step(2).to_a
来源：http://hz.snrcjt.cn/gtduyuraun.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ydjk.org.cn/gtevryzlrn.html

[B12] 跳出多层循环
来源：http://hz.gaohongyu789.top/gtqwgjifyd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinghuilouyu.cn/gtdefyears.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhixingplan.top/gtftfecjbr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigfzy.top/gtzwqgaixh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtmfqifmco.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtzsellear.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.havefunace.top/gtzawwszvv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jlsjyb.cn/gtwrpolqhu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.nanxuanxn.top/gtyofrjdmo.html

[B13] 判断是否为数字
来源：http://hz.ppjwa.cn/gtjbbrrbbs.html

Py:   isinstance(x, (int, float))
来源：http://hz.birdmap.top/gtzliuvddn.html

PHP:  is_numeric($x)
来源：http://hz.jinqigufen.top/gtwkfawulj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtsqwczhvo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtanginijk.html

Java: x instanceof Number
来源：http://hz.gotoacloud.top/gtpjkevxpm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gtazbczxns.html

Ruby: x.is_a?(Numeric)
来源：http://hz.fzhhl.top/gtijllagxz.html

C#:   x is int or double or decimal
来源：http://hz.gotoacloud.top/gtqtjkxjyu.html

[B14] 判断值是否在集合内
来源：http://hz.yj20258888.top/gtokoramoa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.daxiang520.top/gttxgdbvkr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shangyingyoupin.top/gtlkhehotq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtcjppwluu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtjkkfvvcr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuanzhike.top/gtbzcpwfzb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cqqwz.cn/gtvogjvtpz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuanzx.com/gtyxpewreo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.snrcjt.cn/gturxwanxu.html

[B15] 布尔运算与取反
来源：http://hz.cdnleiting.top/gtpsibjbrh.html

Py:   a and b or not c
来源：http://hz.tanke756.top/gttyvjrgyp.html

PHP:  $a && $b || !$c
来源：http://hz.mhx1999.top/gtdludjezg.html

JS:   a && b || !c
来源：http://hz.ppjwa.cn/gtxrweblri.html

TS:   a && b || !c
来源：http://hz.jinqigufen.top/gtobqxkjwj.html

Java: a && b || !c
来源：http://hz.9152youxi.cn/gtvkuxwmuu.html

Go:   a && b || !c
来源：http://hz.sysykeji.top/gtvplemgwp.html

Ruby: a && b || !c
来源：http://hz.nanxuanxn.top/gtrgsfdelb.html

C#:   a && b || !c
来源：http://hz.zhixingplan.top/gttracjjlc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.meibo888.top/gttrdoyepa.html

Py:   if not data: return
来源：http://hz.chenjidiqi.icu/gtpzwgpgzc.html

PHP:  if (!$data) { return; }
来源：http://hz.pengpengdd.cyou/gtkluixhuc.html

JS:   if (!data) return;
来源：http://hz.yuxming.cn/gtucubyvnc.html

TS:   if (!data) return;
来源：http://hz.yj202588.top/gtijjiiwzy.html

Java: if (data == null) return;
来源：http://hz.wangshuangyany.cn/gthfwmyryl.html

Go:   if data == nil { return }
来源：http://hz.52xcode.cn/gtmwshzdwp.html

Ruby: return if data.nil?
来源：http://hz.316326.xyz/gthdukredu.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtoouqqhgq.html

================================================================================
来源：http://hz.yonumen.top/gteagfhqwr.html

C. 函数与作用域
来源：http://hz.xinyue.icu/gtsidhqcxm.html

================================================================================
来源：http://hz.meibo888.top/gtuxdttcya.html

[C01] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtdpfvgvcs.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtrmrwuxfr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtlduylmyn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cashguo.top/gtaztgsrug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aizwys.cn/gtgxkpcnsg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gttdhufrlz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shzxlz.cn/gtrofvymdl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuetiantiany.cn/gtvflqrsce.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtkvfeygbb.html

[C02] 默认参数
来源：http://hz.pycfn.com/gtrfmnshyu.html

Py:   def greet(name="World"): return name
来源：http://hz.shanyushiyangtech.top/gtprhqobvh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.snrcjt.cn/gtxrereoju.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.andypj.xyz/gtndkwyavw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.fengsongda.top/gtpgenugdm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.birdmap.top/gtufztecag.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtkrzbwrai.html

Ruby: def greet(name = "World") = name
来源：http://hz.andypj.xyz/gtrncvjpka.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.feifeiyinyue.top/gtyhcqzzii.html

[C03] 可变参数
来源：http://hz.jqgfzy.top/gturdzsnij.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj202588.top/gtrtfhtudv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nwbrower.top/gtzjomioge.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtiepijmef.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtwukpdejv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gotoacloud.top/gtpwnujhrj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.smart0.xyz/gtbzvsabsj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yongpay.top/gthrcavjwa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pengpengdd.cyou/gtdwuncaqj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhijiandao.cn/gtvvktcxup.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jiagoushi.top/gtxfnpwjga.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ehwqpu.com/gtckxayknb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gthgwzarsq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.9152youxi.cn/gtvxogttpc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aizwys.cn/gtospeqatd.html

Go:   // 无：用配置结构体参数
来源：http://hz.ydjk.org.cn/gtnfqckitc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtrneygrrj.html

C#:   f(a: 1, b: 2)
来源：http://hz.andypj.xyz/gtnjposnrg.html

[C05] 返回多个值
来源：http://hz.jinyuanbaomall.cn/gtrestusls.html

Py:   return a, b
来源：http://hz.redwolf501.top/gtgizdlbgv.html

PHP:  return [$a, $b];
来源：http://hz.cqqwz.cn/gtlkxihiyx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.chenlongwang.top/gtdvlpxyqh.html

TS:   return { a, b };
来源：http://hz.nwbrower.top/gtrxutiqbs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydzc1.top/gtdwgvlibv.html

Go:   return a, b
来源：http://hz.yueranfly.top/gtfmnzhqcc.html

Ruby: return a, b
来源：http://hz.gaohongyu789.top/gtaxrqfaub.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hfpthk.cn/gtsuabokhw.html

[C06] 匿名函数 / lambda
来源：http://hz.svipenyu.cn/gtzsaeflqd.html

Py:   square = lambda x: x * x
来源：http://hz.iojbl.cn/gtxtgrckzr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gtupkxvcfw.html

JS:   const square = x => x * x;
来源：http://hz.quarkkingdee.top/gttrqzkmxe.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shangyingyoupin.top/gtitahzvuf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.mhx1999.top/gtuxiccfhy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ppjwa.cn/gtwycqxtab.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgufenzy.top/gtblokrsqj.html


<!-- 参考信息 -->