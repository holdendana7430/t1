代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.ppjwa.cn/gtwxlldaph.html

C#:   var value = data ?? "默认值";
来源：http://hz.hysaishi.cn/gtgmarjtih.html

[A16] 真假值判断规则
来源：http://hz.zhixingplan.top/gtahupuqdt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.sysykeji.top/gtldkmsset.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.zhixingplan.top/gtlziklxfw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.aizwys.cn/gtrrcrmanf.html

TS:   if (!x) {}
来源：http://hz.shuidangran.top/gtsveiktfu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.smart0.xyz/gtluophkut.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.bjfxy.top/gtknwyueud.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.xuanzx.com/gtwuarsruz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.mhx1999.top/gtgnabckdp.html

[A17] 位运算
来源：http://hz.jinqigfzy.top/gtvdfglmxp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.haohaochexian.top/gtthkmocop.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.c1oappe.top/gtqsksehep.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtpxhimhmj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.havefunace.top/gtpumqdhet.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cucudq.cn/gtifgadbxu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.cheryme.top/gtywdreqkg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cqqwz.cn/gthzkbsuuk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtethwwbqb.html

[A18] 字符与 ASCII 码互转
来源：http://hz.svipenyu.cn/gtefuehqly.html

Py:   ord("A"); chr(65)
来源：http://hz.dashuyun.cn/gtxkvurugd.html

PHP:  ord("A"); chr(65)
来源：http://hz.mhx1999.top/gtiirtiiga.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gotoacloud.top/gtzeyknhsr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cqqwz.cn/gtzfoggasq.html

Java: (int) 'A'; (char) 65
来源：http://hz.shanyushiyangtech.top/gtksjjoaay.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.meibo888.top/gtrradimnz.html

Ruby: "A".ord; 65.chr
来源：http://hz.chenjidiqi.icu/gtfkumnpzb.html

C#:   (int)'A'; (char)65
来源：http://hz.sxryk.cn/gtjrzezhzr.html

[A19] 交换两个变量
来源：http://hz.jqgfzy.top/gtwoxvdogz.html

Py:   a, b = b, a
来源：http://hz.dianchejie.cn/gtwlifqyiz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yonumen.top/gtskazatqq.html

JS:   [a, b] = [b, a];
来源：http://hz.c1oappe.top/gtfpflkewl.html

TS:   [a, b] = [b, a];
来源：http://hz.cqqwz.cn/gtkrvsihrr.html

Java: int t = a; a = b; b = t;
来源：http://hz.tian-w.cn/gtvdvtysmk.html

Go:   a, b = b, a
来源：http://hz.zhengqikj.top/gtjmtxweuy.html

Ruby: a, b = b, a
来源：http://hz.yongpay.top/gtzhggvlqx.html

C#:   (a, b) = (b, a);
来源：http://hz.mhx1999.top/gtjclsejjb.html

[A20] 读取标准输入
来源：http://hz.fzhhl.top/gtmrcxgthu.html

Py:   name = input("请输入：")
来源：http://hz.tian-w.cn/gthdzxcicz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.zhaomingkeji.xyz/gtrsrexwzx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.wangshuangyany.cn/gtvhxidtip.html

TS:   // Node.js：readline 模块
来源：http://hz.fzhhl.top/gtzkmtfwvi.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.ywan-chungtsiang.top/gtogoehzzj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.0kj1m.cn/gtwhhxafuu.html

Ruby: gets.chomp
来源：http://hz.jqgufenzy.top/gtyppkcudn.html

C#:   Console.ReadLine();
来源：http://hz.dashuyun.cn/gtrscezcsj.html

[A21] 保留指定小数位输出
来源：http://hz.ywan-chungtsiang.top/gtrmjqydwn.html

Py:   f"{3.14159:.2f}"
来源：http://hz.sysykeji.top/gtenvanmxx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zhongyouzk.top/gtfdqlgirr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sufxvd.cn/gtibmtblbi.html

TS:   (3.14159).toFixed(2)
来源：http://hz.cheryme.top/gtpvhvnhjb.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.feifeiyinyue.top/gtfepejbkb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.nwbrower.top/gtvedjyxmq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.chenjidiqi.icu/gtcbzhcspw.html

C#:   3.14159.ToString("F2")
来源：http://hz.ppjwa.cn/gttpyyflhn.html

[A22] 获取字符串长度
来源：http://hz.yueranfly.top/gteabgylye.html

Py:   len(s)
来源：http://hz.fengsongda.top/gttlkrjtjw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ppjwa.cn/gtysfluvyt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yj202588.top/gtcxwoezwe.html

TS:   s.length
来源：http://hz.guowangkeji.top/gtmnkdsvor.html

Java: s.length()
来源：http://hz.xuetiantiany.cn/gtbsnolvjs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.sweek.top/gtheeoiehw.html

Ruby: s.length
来源：http://hz.jinyuanbaomall.cn/gtuyalrody.html

C#:   s.Length
来源：http://hz.9152youxi.cn/gtouziohrf.html

[A23] 大小写转换
来源：http://hz.smart0.xyz/gtacegusdd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.0kj1m.cn/gtwdywhkhg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cheryme.top/gtbvjixpog.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xylfe.cn/gthwvgegai.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cashguo.top/gtndveqcda.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigfzy.top/gtitbzrmil.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.xuetiantiany.cn/gtjmrpabse.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yuanzhike.top/gtdvpwyuhf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yj20258.top/gthgawkpra.html

[A24] 去除首尾空白
来源：http://hz.nwbrower.top/gtwnakgrgi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shanyushiyangkeji.top/gtgwqhyuvq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.mhx1999.top/gtgmdvcsif.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigfzy.top/gteonommhk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhoulong.xyz/gtbhrdbflv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.daria6918.cn/gtgzatmmcs.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhixingplan.top/gtzqxjjciu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cqqwz.cn/gtuwvtqbgl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.dashuyun.cn/gtzskrewsv.html

[A25] 字符串比较
来源：http://hz.cucudq.cn/gtwazukgxr.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xylfe.cn/gtquzhbsxr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yonumen.top/gtpjgghxdy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yuxming.cn/gtziemiyfd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydjk.org.cn/gtbwyzyugl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yangfankeji.com/gtlnftseoy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.svipenyu.cn/gtsjykxqtt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xylfe.cn/gtyclktkrj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jinqigfzy.top/gtrhbnzzox.html

[A26] 类型转换总览
来源：http://hz.sweek.top/gttuiqdzid.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sysykeji.top/gtferglvfv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.tianlin.xyz/gtyprtuvxr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinghuilouyu.cn/gtcwitwytn.html

TS:   Number() String() Boolean() x as number
来源：http://hz.birdmap.top/gtpjduyajf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.dashuyun.cn/gtvuflfmoj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhoulong.xyz/gtppfeyawi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hysaishi.cn/gtamrdoton.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.havefunace.top/gtbnwswclu.html

================================================================================
来源：http://hz.yangfankeji.com/gtdjznvnkp.html

B. 流程控制
来源：http://hz.redwolf501.top/gtxzpnktgi.html

================================================================================
来源：http://hz.yongpay.top/gtnsdihmxa.html

[B01] 条件判断 if / else
来源：http://hz.shanyushiyangtech.top/gttqspmqug.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.0kj1m.cn/gtpvibgbyo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jlsjyb.cn/gtiwqkekag.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ppjwa.cn/gteovzwniz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gtobrjxxsc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtimydmdef.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hnxiangtu.top/gtosewzuop.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhoulong.xyz/gtobvkinof.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.wangdashe.top/gtsqorvqlp.html

[B02] 多分支 else if / elif
来源：http://hz.cucudq.cn/gtltywxain.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.meibo888.top/gtfunkikvo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gzhubu.top/gtofxwhlod.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gtwkkmofin.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhaomingkeji.xyz/gtuuowfgpi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gtxysqklip.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.0kj1m.cn/gtjwytrrkc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yuxming.cn/gttfbamrgt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtrftkfsxe.html

[B03] switch / match / case
来源：http://hz.svipenyu.cn/gtfewacqui.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sxryk.cn/gtgxtsodhm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.cashguo.top/gtiulflhkq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhijiandao.cn/gtnjkatwmc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cheryme.top/gtcbdxgkip.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenlongwang.top/gtejsbnefu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.snrcjt.cn/gtxooaopgw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhijiandao.cn/gtbqmyeehx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.daria6918.cn/gtartelgjc.html

[B04] for 计数循环
来源：http://hz.kuanghao11.cn/gtoalocskt.html

Py:   for i in range(10): print(i)
来源：http://hz.jiagoushi.top/gtrtqasmbm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.quarkkingdee.top/gtugnwvmbh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ydzc1.top/gthkqllags.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangshuangyany.cn/gtxspylhqt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yvedp.cn/gtcchycddw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cucudq.cn/gtqobkdyjg.html

Ruby: 10.times { |i| puts i }
来源：http://hz.0kj1m.cn/gthmrdfran.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.gotoacloud.top/gtllitxtua.html

[B05] 遍历数组 / 列表
来源：http://hz.zhengqikj.top/gtoihpwkgw.html

Py:   for item in arr: print(item)
来源：http://hz.xingfuxueyuan.xyz/gtdttoiobf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hfpthk.cn/gtjpgofjik.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.pycfn.com/gtnjthyfrq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xuetiantiany.cn/gteeuzmaow.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhoulong.xyz/gtcqxfoxoq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.smart0.xyz/gtrjttgqjr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.havefunace.top/gtnzfjfxqr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhongyouzk.top/gtzwizhhpq.html

[B06] 遍历字典 / 对象
来源：http://hz.yongpay.top/gtpzamjsgc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.gotoacloud.top/gtupnqvshb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.quarkkingdee.top/gtvammdkrq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hongshengwenyu.top/gtgutkteyk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sxryk.cn/gtcvfkwfih.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jianghu66.top/gtplqpcife.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.aizwys.cn/gttzwycfzp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.tanke756.top/gtsqcaingh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhixingplan.top/gthwbuauvv.html

[B07] while 循环
来源：http://hz.shuidangran.top/gtatolmrce.html

Py:   while i < 10: i += 1
来源：http://hz.hfpthk.cn/gtpvqbwvxb.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xylfe.cn/gtgkvlbdju.html

JS:   while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtzardnlaz.html

TS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtxvtqklfa.html

Java: while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtiokyjbkw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.nanxinkj.top/gtmoyxqgjz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj20258888.top/gtbfidsohm.html

C#:   while (i < 10) { i++; }
来源：http://hz.haohaochexian.top/gtejrsyvaz.html

[B08] do-while（至少执行一次）
来源：http://hz.yongpay.top/gtrknpbgop.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cdnleiting.top/gtmmolxkdn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.snrcjt.cn/gtyoiegqrh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtkkeuszap.html

TS:   do { i++; } while (i < 10);
来源：http://hz.wangshuangyany.cn/gtwsmvfqil.html

Java: do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtnhggpbtv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.aibaodan.cn/gtualoafre.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ybcxt.top/gteiozvjjs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtnbjmobus.html

[B09] break 与 continue
来源：http://hz.xziqi.cn/gttnyllvje.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gaohongyu789.top/gtkmeqajdy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinqigfzy.top/gtmbwqmkob.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtzkscanco.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtxxlhiamc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jiagoushi.top/gtzhtxzewh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.0kj1m.cn/gtiuusxpkr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zdqjudy.top/gtfgusrjfw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dianchejie.cn/gtcfwkvabn.html

[B10] 遍历同时拿索引
来源：http://hz.cdnleiting.top/gtkxvsxmof.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hfpthk.cn/gtsoooksuq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yonumen.top/gtpwbkyglj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.chenlongwang.top/gtxbgvtrew.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yonumen.top/gtvhpgufrq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yonumen.top/gtmvfydqkk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.snrcjt.cn/gtiqhauhtd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj20258888.top/gtzivzhckq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sweek.top/gtuauyivqp.html

[B11] 生成数字序列 / 区间
来源：http://hz.nanxinkj.top/gtxlvrkpqf.html

Py:   list(range(0, 10, 2))
来源：http://hz.52xcode.cn/gthdoxajjq.html

PHP:  range(0, 10, 2);
来源：http://hz.dianchejie.cn/gtubjqtezr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtydnamrzl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.haohaochexian.top/gtlphmafki.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.sufxvd.cn/gtpybyyyzu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj202588.top/gttpyugpla.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ybcxt.top/gtwykuexgy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xuetiantiany.cn/gtqaogxrfu.html

[B12] 跳出多层循环
来源：http://hz.jinyuanbaomall.cn/gtsyglajsm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pengpengdd.cyou/gtsrgpdhwu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shangyingyoupin.top/gtkjahxykv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gtokviqhar.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtqqdocqqu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.sweek.top/gttfmorbmv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xziqi.cn/gtrnnuopnl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ydjk.org.cn/gtdwolvdnd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hongshengwenyu.top/gthdzyghrx.html

[B13] 判断是否为数字
来源：http://hz.hnqzz.top/gtteckrvtz.html

Py:   isinstance(x, (int, float))
来源：http://hz.sweek.top/gtnbvkiytw.html

PHP:  is_numeric($x)
来源：http://hz.zhoulong.xyz/gtgmmddchc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.andypj.xyz/gthlbusmaq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtzalwwijl.html

Java: x instanceof Number
来源：http://hz.xuanzx.com/gtzaydvwaz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zdqjudy.top/gtdrafhwdp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.havefunace.top/gteyqagtnr.html

C#:   x is int or double or decimal
来源：http://hz.sysykeji.top/gtocnqexuz.html

[B14] 判断值是否在集合内
来源：http://hz.havefunace.top/gthpiuuqso.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinqigufen.top/gtjmiscomp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daxiang520.top/gtvbizprun.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.smart0.xyz/gtwoiemxpj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenlongwang.top/gtryhfxntx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gtofwvanek.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.quarkkingdee.top/gtefddnicr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.redwolf501.top/gtfbvteiwn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.smart0.xyz/gtldlgmmdp.html

[B15] 布尔运算与取反
来源：http://hz.shangyingyoupin.top/gtozfyxkdr.html

Py:   a and b or not c
来源：http://hz.yuxming.cn/gtatnjxedg.html

PHP:  $a && $b || !$c
来源：http://hz.daxiang520.top/gtgufnoslx.html

JS:   a && b || !c
来源：http://hz.aibaodan.cn/gtnxkonazx.html

TS:   a && b || !c
来源：http://hz.gogol.net.cn/gtfdmlydvy.html

Java: a && b || !c
来源：http://hz.daxiang520.top/gtvgithhbh.html

Go:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtcdsjlssl.html

Ruby: a && b || !c
来源：http://hz.jqgufenzy.top/gtzdrmwqio.html

C#:   a && b || !c
来源：http://hz.zhoulong.xyz/gtmwabzsek.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.meibo888.top/gtmzqrpnyw.html

Py:   if not data: return
来源：http://hz.chenzaomai.com/gtacdamkwm.html

PHP:  if (!$data) { return; }
来源：http://hz.sysykeji.top/gtgglytmfl.html

JS:   if (!data) return;
来源：http://hz.daxiang520.top/gtkdnozilz.html

TS:   if (!data) return;
来源：http://hz.c1oappe.top/gtjcreyalm.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gtuvfijqpd.html

Go:   if data == nil { return }
来源：http://hz.cucudq.cn/gticnmmtci.html

Ruby: return if data.nil?
来源：http://hz.chenzaomai.com/gtpjxomflx.html

C#:   if (data == null) return;
来源：http://hz.yj20258.top/gtndqvpqex.html

================================================================================
来源：http://hz.jqgfzy.top/gtwdmovxkf.html

C. 函数与作用域
来源：http://hz.aibaodan.cn/gttojzroiu.html

================================================================================
来源：http://hz.hnqzz.top/gtwuxcqrdw.html

[C01] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtfbftilvp.html

Py:   def add(a, b): return a + b
来源：http://hz.0kj1m.cn/gtmgqjbbtw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtznbmbmao.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pycfn.com/gtlzonpguw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gtnglmbkgp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtvsjcpjsw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yonumen.top/gtzfdscekf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenjidiqi.icu/gtnogouyul.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtsiiksplq.html

[C02] 默认参数
来源：http://hz.haohaochexian.top/gtzmvxuius.html

Py:   def greet(name="World"): return name
来源：http://hz.jqgufenzy.top/gtmqzfafjd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jyoumei.cn/gthdbwncza.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tanke756.top/gtehsrhojr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.smart0.xyz/gtvborzfoc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnxiangtu.top/gtpsrrjokm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aizwys.cn/gthudlqmxm.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gtqbnjflul.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenlongwang.top/gtvqbjujeq.html

[C03] 可变参数
来源：http://hz.chenjidiqi.icu/gtfpgjjjlk.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenjidiqi.icu/gtxoflkaej.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xinyue.icu/gtdbmixacn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xuetiantiany.cn/gtcamvnnus.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtherxauhj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ywan-chungtsiang.top/gttoftuppw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangshuangyany.cn/gtlpktfgup.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.0kj1m.cn/gtljvmfuzp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gtxdczksyp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gogol.net.cn/gtesdbakgi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangtech.top/gtzdtvnjrt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.kuanghao11.cn/gtgyhwefxh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cashguo.top/gtndvsspjk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yongpay.top/gtzgbvrhuo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yangfankeji.com/gtfjyqnliq.html

Go:   // 无：用配置结构体参数
来源：http://hz.hammf.cn/gtobtxdcjj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtkpqpbqll.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtliqbggoo.html

[C05] 返回多个值
来源：http://hz.nanxuanxn.top/gtytqeykea.html

Py:   return a, b
来源：http://hz.zhongyouzk.top/gtnrhzipxr.html

PHP:  return [$a, $b];
来源：http://hz.havefunace.top/gtpmmirbdb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtkkpcgtly.html

TS:   return { a, b };
来源：http://hz.yj202588.top/gtcpmaqwhh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tianlin.xyz/gtvvchqvcy.html

Go:   return a, b
来源：http://hz.birdmap.top/gtcpplpljn.html

Ruby: return a, b
来源：http://hz.ehwqpu.com/gtqmhpioqu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jyoumei.cn/gtuhgnncne.html

[C06] 匿名函数 / lambda
来源：http://hz.kuanghao11.cn/gtuxkbejbm.html

Py:   square = lambda x: x * x
来源：http://hz.chenlongwang.top/gtowipndfl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhongyouzk.top/gticwvyqyv.html

JS:   const square = x => x * x;
来源：http://hz.jinghuilouyu.cn/gtypvomjuh.html


<!-- 参考信息 -->