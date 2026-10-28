代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.quarkkingdee.top/gtawoaqlsn.html

TS:   const value = data ?? "默认值";
来源：http://hz.0kj1m.cn/gtibcvadxr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.cashguo.top/gtgqubmoia.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.smart0.xyz/gtgyztpgij.html

Ruby: value = data || "默认值"
来源：http://hz.xylfe.cn/gtpparrdek.html

C#:   var value = data ?? "默认值";
来源：http://hz.316326.xyz/gtfmxnfazl.html

[A16] 真假值判断规则
来源：http://hz.quarkkingdee.top/gthxrhagpn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yueranfly.top/gtybqpqxrt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.yj202588.top/gtotwmapxq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hnxiangtu.top/gtbbcfayex.html

TS:   if (!x) {}
来源：http://hz.ppjwa.cn/gtksyorpxd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.52xcode.cn/gtvdhascwq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jyoumei.cn/gtqcyuksim.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.xingfuxueyuan.xyz/gtdtqkuyhg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yongpay.top/gtnngaqsfd.html

[A17] 位运算
来源：http://hz.yangfankeji.com/gtqrykrkgi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtlcbbujnd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zycfv.cn/gtdnzmsfar.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258888.top/gtjrlnjzhg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.shuidangran.top/gtqikukhhr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258888.top/gtptxovwfp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gttleyntgg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sysykeji.top/gtrptftwyp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtxtzfzafu.html

[A18] 字符与 ASCII 码互转
来源：http://hz.iojbl.cn/gtwdnobqgm.html

Py:   ord("A"); chr(65)
来源：http://hz.iojbl.cn/gtledupkkn.html

PHP:  ord("A"); chr(65)
来源：http://hz.yongpay.top/gtmaejhclu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinyuanbaomall.cn/gtixrpqqhk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hysaishi.cn/gtbpocjvnx.html

Java: (int) 'A'; (char) 65
来源：http://hz.dianchejie.cn/gtwwhbbqtp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.quarkkingdee.top/gtvsxaddza.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhongyouzk.top/gtscxfzksx.html

C#:   (int)'A'; (char)65
来源：http://hz.gzhubu.top/gtkezqylxc.html

[A19] 交换两个变量
来源：http://hz.yj20258.top/gteybigwjz.html

Py:   a, b = b, a
来源：http://hz.c1oappe.top/gtkuvwudxt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.zhoulong.xyz/gtzioppvqs.html

JS:   [a, b] = [b, a];
来源：http://hz.yangfankeji.com/gtephzjsjw.html

TS:   [a, b] = [b, a];
来源：http://hz.birdmap.top/gtlkauxecq.html

Java: int t = a; a = b; b = t;
来源：http://hz.xuetiantiany.cn/gtmndqthda.html

Go:   a, b = b, a
来源：http://hz.daxiang520.top/gtkjotgdhp.html

Ruby: a, b = b, a
来源：http://hz.chenzaomai.com/gtzeiyzzkr.html

C#:   (a, b) = (b, a);
来源：http://hz.feifeiyinyue.top/gtsrfritjz.html

[A20] 读取标准输入
来源：http://hz.zhoulong.xyz/gtzbpsgffp.html

Py:   name = input("请输入：")
来源：http://hz.kuanghao11.cn/gttbuopcie.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cheryme.top/gtopvbvnrx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.9152youxi.cn/gtcthbpwzm.html

TS:   // Node.js：readline 模块
来源：http://hz.chenzaomai.com/gtcwvpocyh.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.ydjk.org.cn/gtvrczedga.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xylfe.cn/gtwbevzzll.html

Ruby: gets.chomp
来源：http://hz.pengpengdd.cyou/gtuyfdmgrt.html

C#:   Console.ReadLine();
来源：http://hz.jqgfzy.top/gtdtyzxoav.html

[A21] 保留指定小数位输出
来源：http://hz.nanxuanxn.top/gtydgcqaom.html

Py:   f"{3.14159:.2f}"
来源：http://hz.guannengcc.top/gtxmtmrgqp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.kuanghao11.cn/gtbgvdfisr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.andypj.xyz/gtewkxkacv.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jinqigufen.top/gtvmntxkei.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtupbqinqq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.svipenyu.cn/gtchxqxidr.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.9152youxi.cn/gtfirxsdjp.html

C#:   3.14159.ToString("F2")
来源：http://hz.ybcxt.top/gtqghwuiyo.html

[A22] 获取字符串长度
来源：http://hz.smart0.xyz/gthzbdudsp.html

Py:   len(s)
来源：http://hz.shzxlz.cn/gtewjscfty.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zhiwuduotai.top/gtabkfndyv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.tanke756.top/gtuyzqczvo.html

TS:   s.length
来源：http://hz.aibaodan.cn/gtwkfgltdy.html

Java: s.length()
来源：http://hz.birdmap.top/gtxeffqafq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jianghu66.top/gtrfjkcpvr.html

Ruby: s.length
来源：http://hz.gaohongyu789.top/gthrrzutxm.html

C#:   s.Length
来源：http://hz.ydzc1.top/gtmtzrivvq.html

[A23] 大小写转换
来源：http://hz.zycfv.cn/gtnbvubeaz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.sxryk.cn/gtrstfywcd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.sweek.top/gtbblvtplr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.havefunace.top/gtqxelbupw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.meibo888.top/gtvstcqpvr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinghuilouyu.cn/gtgybnzrfr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.shuidangran.top/gtowlabsim.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xuanzx.com/gtxhyxdbdo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.havefunace.top/gtnpxruevc.html

[A24] 去除首尾空白
来源：http://hz.shuidangran.top/gtcvottosk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.hongshengwenyu.top/gtvdjewrfu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hongshengwenyu.top/gtubmnsuei.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.quarkkingdee.top/gtuxmnicjd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yuxming.cn/gtcpoazbau.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yuanzhike.top/gtbhsbkwjs.html

Go:   strings.TrimSpace(s)
来源：http://hz.jlsjyb.cn/gtyemuuckg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.sxryk.cn/gtqyotleox.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.aizwys.cn/gtwvsatdsd.html

[A25] 字符串比较
来源：http://hz.aibaodan.cn/gtemcrgmzb.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhongyouzk.top/gtqwjyybnv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shzxlz.cn/gtpqoxyxim.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sysykeji.top/gtcespzmmi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yueranfly.top/gtkzfjvgmr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.sufxvd.cn/gtsqhbumlv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.redwolf501.top/gtjdnamwxl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sufxvd.cn/gtqyhvqfgk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yongpay.top/gtsapseclm.html

[A26] 类型转换总览
来源：http://hz.zycfv.cn/gtekssrcon.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.snrcjt.cn/gtpkbziicf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.feifeiyinyue.top/gtkqbbblnv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hysaishi.cn/gtrpzmhkwo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.andypj.xyz/gtruxvylst.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.nanxuanxn.top/gtvobhebxz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.shanyushiyangtech.top/gtigbqijzi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hywenlv.cn/gtviwlhlgr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jianghu66.top/gtavpxvjxc.html

================================================================================
来源：http://hz.andypj.xyz/gteevatwie.html

B. 流程控制
来源：http://hz.xylfe.cn/gtuzpztyas.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfqxlufzs.html

[B01] 条件判断 if / else
来源：http://hz.cdnleiting.top/gtwoffygcs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shangyingyoupin.top/gtpcbrwywz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yonumen.top/gtcbwiwxjn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtwzsdcktw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangkeji.top/gtrcdhheeq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.cucudq.cn/gtaqbmanif.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.c1oappe.top/gtvylnqrwc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.dashuyun.cn/gtfrnjgbqw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yuxming.cn/gtnzkjkhgf.html

[B02] 多分支 else if / elif
来源：http://hz.zhoulong.xyz/gtwobmfhbn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhiwuduotai.top/gtaoogqgzu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhoulong.xyz/gtlkydlzxa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.andypj.xyz/gttsxmhpzu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtrxhodnrk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxinkj.top/gtxuldsgii.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.fzhhl.top/gtqktojhlv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hnqzz.top/gtdmivzpdu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtninutzre.html

[B03] switch / match / case
来源：http://hz.jinyuanbaomall.cn/gtfstksdrv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.daxiang520.top/gtuamzvgmw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xylfe.cn/gtzihrjbfg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.redwolf501.top/gtrsscbiet.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hysaishi.cn/gtaehjstcm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jqgufenzy.top/gtdzptqolu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cqqwz.cn/gtghbyplog.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhijiandao.cn/gthitolsjx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ydjk.org.cn/gtmrodlscj.html

[B04] for 计数循环
来源：http://hz.dianchejie.cn/gtgcwqelso.html

Py:   for i in range(10): print(i)
来源：http://hz.daxiang520.top/gtuzbxqyfu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.tian-w.cn/gtpyxtubvp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sxryk.cn/gtvjdtuubc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.0kj1m.cn/gtphvbukoi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zycfv.cn/gtjlthksal.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.pycfn.com/gtcuokuozn.html

Ruby: 10.times { |i| puts i }
来源：http://hz.wangdashe.top/gtntsnwucm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.kuanghao11.cn/gtawvdbuxv.html

[B05] 遍历数组 / 列表
来源：http://hz.jinghuilouyu.cn/gtakknjwlt.html

Py:   for item in arr: print(item)
来源：http://hz.shanyushiyangtech.top/gtqgdkfgzn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.haohaochexian.top/gtjynvjwsl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yonumen.top/gtmwmowybm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.svipenyu.cn/gtwqmrcodh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zycfv.cn/gtdpjpqtau.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhixingplan.top/gtnmhjphsr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.xingfuxueyuan.xyz/gturxvtpqu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ydzc1.top/gtrqylwver.html

[B06] 遍历字典 / 对象
来源：http://hz.gotoacloud.top/gtsxbryejr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.feifeiyinyue.top/gtvxvdjnsi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.tianlin.xyz/gtvyvhuckr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yangfankeji.com/gtgpsdxugu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tianlin.xyz/gtctotfdic.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shanyushiyangtech.top/gtkickjrcv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nwbrower.top/gtmrhcbtzx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhixingplan.top/gtczaptsso.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.nanxinkj.top/gtocfawhqd.html

[B07] while 循环
来源：http://hz.jqgufenzy.top/gtapjdzfbq.html

Py:   while i < 10: i += 1
来源：http://hz.xingfuxueyuan.xyz/gtgofrhzal.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gzhubu.top/gtymgomleg.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gttkolrwvg.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gttgaqmtkv.html

Java: while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtykdkwrpq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shanyushiyangtech.top/gtyodbaoap.html

Ruby: while i < 10; i += 1; end
来源：http://hz.meibo888.top/gtkzfbilxa.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gtjtwftxcq.html

[B08] do-while（至少执行一次）
来源：http://hz.xinyue.icu/gtmucinxga.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.kuanghao11.cn/gtjzddngvn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258.top/gtioruwijz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtzwicbxdv.html

TS:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtwjbnrqlx.html

Java: do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtifmswccl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xylfe.cn/gtpyujrmux.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.andypj.xyz/gtqatiyeys.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtmmnrlquc.html

[B09] break 与 continue
来源：http://hz.zycfv.cn/gthqbqehlh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.wangdashe.top/gtgwjxvixt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtayiisrkw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtflkfgkhb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtaquhbryh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtvvhglmhi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.andypj.xyz/gtyxmfugiw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sufxvd.cn/gtrbodzhfv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtyllsqecl.html

[B10] 遍历同时拿索引
来源：http://hz.tian-w.cn/gtotjlhjjw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.smart0.xyz/gtzkoakfaa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cdnleiting.top/gthcjruirs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gtkvioggpz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gtvrgmnvfo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yj20258.top/gtcwfobzvo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xingfuxueyuan.xyz/gtyatepzuv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gaohongyu789.top/gthymdjcus.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ppjwa.cn/gtbihvlamc.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinghuilouyu.cn/gthwilmdrf.html

Py:   list(range(0, 10, 2))
来源：http://hz.cucudq.cn/gtylwtrlsd.html

PHP:  range(0, 10, 2);
来源：http://hz.haohaochexian.top/gtolojcavs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtplmhlgjz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.kuanghao11.cn/gthfdwbkot.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtonnedkpb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yuxming.cn/gtzqbpkcvt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinyuanbaomall.cn/gthtkbynfx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.aizwys.cn/gttthcjupg.html

[B12] 跳出多层循环
来源：http://hz.quarkkingdee.top/gtyzlcmqph.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ydzc1.top/gtfjudvghd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.0kj1m.cn/gtpiqygucc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gtobbadvuv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sweek.top/gtwqxgxyaq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gthgemfxyl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.haohaochexian.top/gtbamsjvbk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhengqikj.top/gthkrkslgx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gaohongyu789.top/gtlnzrkuzx.html

[B13] 判断是否为数字
来源：http://hz.cqqwz.cn/gtyxyvfaai.html

Py:   isinstance(x, (int, float))
来源：http://hz.cqqwz.cn/gtezfllcpa.html

PHP:  is_numeric($x)
来源：http://hz.nanxinkj.top/gtciqauzbu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtfudtdkip.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhengqikj.top/gtsfjkazkh.html

Java: x instanceof Number
来源：http://hz.haohaochexian.top/gtyarfkstt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ydzc1.top/gtqoegfldd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nanxinkj.top/gtxzqdymzl.html

C#:   x is int or double or decimal
来源：http://hz.redwolf501.top/gtwuuskkpz.html

[B14] 判断值是否在集合内
来源：http://hz.yuxming.cn/gtnqynfbod.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.iojbl.cn/gtiukvisph.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xinyue.icu/gtwhlwuges.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shangyingyoupin.top/gtaufrwpak.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtmpplharg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hywenlv.cn/gttqwxgcrn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.9152youxi.cn/gtbbtjgbpc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jqgfzy.top/gtofhjdeuc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.birdmap.top/gthmyvovgu.html

[B15] 布尔运算与取反
来源：http://hz.yonumen.top/gtaxvexvtv.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtoupbfppa.html

PHP:  $a && $b || !$c
来源：http://hz.feifeiyinyue.top/gtgswhsfyq.html

JS:   a && b || !c
来源：http://hz.ybcxt.top/gtzykmimsi.html

TS:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtsduwbwxi.html

Java: a && b || !c
来源：http://hz.iojbl.cn/gtfafsticd.html

Go:   a && b || !c
来源：http://hz.jianghu66.top/gtpowhpcvh.html

Ruby: a && b || !c
来源：http://hz.yangfankeji.com/gtwwkyjbew.html

C#:   a && b || !c
来源：http://hz.gotoacloud.top/gthouwdxux.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.haohaochexian.top/gtzgrvlndu.html

Py:   if not data: return
来源：http://hz.yueranfly.top/gtbebbmhdn.html

PHP:  if (!$data) { return; }
来源：http://hz.zhijiandao.cn/gteelstsji.html

JS:   if (!data) return;
来源：http://hz.shzxlz.cn/gtiomtkemm.html

TS:   if (!data) return;
来源：http://hz.yj202588.top/gtakzmutcx.html

Java: if (data == null) return;
来源：http://hz.mhx1999.top/gtvaqjzsup.html

Go:   if data == nil { return }
来源：http://hz.hnxiangtu.top/gtzizjowyk.html

Ruby: return if data.nil?
来源：http://hz.nanxinkj.top/gtcshxqkcv.html

C#:   if (data == null) return;
来源：http://hz.zhijiandao.cn/gtpyexnpat.html

================================================================================
来源：http://hz.jlsjyb.cn/gtrlgpwyai.html

C. 函数与作用域
来源：http://hz.jianghu66.top/gtgftxcglw.html

================================================================================
来源：http://hz.fzhhl.top/gtgpiwswvb.html

[C01] 定义函数
来源：http://hz.iojbl.cn/gtaksxvuiq.html

Py:   def add(a, b): return a + b
来源：http://hz.sweek.top/gtctxrzaxi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtzbpbopnr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtwnjhibqu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.redwolf501.top/gtalvffwnp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtgjevrcjl.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sxryk.cn/gtcqakowav.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tanke756.top/gtmgtmpsad.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtozepmtkp.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtadonvcdn.html

Py:   def greet(name="World"): return name
来源：http://hz.sysykeji.top/gtdoapoixz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yvedp.cn/gtkzwkjroc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cashguo.top/gtomdqmydh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.feifeiyinyue.top/gtfnupgkgm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xziqi.cn/gtvqdtfdkn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.meibo888.top/gtetpomiiq.html

Ruby: def greet(name = "World") = name
来源：http://hz.jiagoushi.top/gthxtxjsqv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tian-w.cn/gtpgsieekl.html

[C03] 可变参数
来源：http://hz.svipenyu.cn/gtaqmnpzbr.html

Py:   def total(*args): return sum(args)
来源：http://hz.pycfn.com/gtqyckqzwf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sxryk.cn/gtvwalvkle.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtxexjsstf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtcgeoqekk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.dianchejie.cn/gtcotbjahe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigufen.top/gtfyagxdsw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtibwngsyj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.0kj1m.cn/gtqumpabvd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gtmarleizk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.dianchejie.cn/gtzgfewxso.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhijiandao.cn/gtaqmlvtaj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sweek.top/gtlbrdjotp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenjidiqi.icu/gtryeavzwc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ppjwa.cn/gtemecqwnf.html

Go:   // 无：用配置结构体参数
来源：http://hz.dashuyun.cn/gtqqpozdrt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gttlidpmxr.html

C#:   f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtberteqlm.html

[C05] 返回多个值
来源：http://hz.haohaochexian.top/gtxqgabyar.html

Py:   return a, b
来源：http://hz.wangshuangyany.cn/gtnqkdgecj.html

PHP:  return [$a, $b];
来源：http://hz.sxryk.cn/gtszkdctjv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sweek.top/gtqnioepch.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtscqqlwul.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tianlin.xyz/gtmldckbtf.html

Go:   return a, b
来源：http://hz.hnxiangtu.top/gtfbvqjwuj.html

Ruby: return a, b
来源：http://hz.quarkkingdee.top/gttodvmgsr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.redwolf501.top/gtbdkcacyl.html


<!-- 参考信息 -->