代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.316326.xyz/gtvwkggght.html

TS:   const value = data ?? "默认值";
来源：http://hz.jqgfzy.top/gtzyvombyg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.ivvv.top/gttpwzwaxd.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.zhijiandao.cn/gthkxwkusf.html

Ruby: value = data || "默认值"
来源：http://hz.tianlin.xyz/gtrlztvpms.html

C#:   var value = data ?? "默认值";
来源：http://hz.birdmap.top/gtmiwrxtrg.html

[A16] 真假值判断规则
来源：http://hz.bjfxy.top/gtxgqkxpus.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.52xcode.cn/gtpfbbfoqp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jyoumei.cn/gtxrrekjwz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.ivvv.top/gttdluzszi.html

TS:   if (!x) {}
来源：http://hz.yj20258888.top/gtrewexfsb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.havefunace.top/gthgpolfwn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.snrcjt.cn/gtfleclsbi.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.redwolf501.top/gtkwjzefbl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.chenzaomai.com/gttcsrxvey.html

[A17] 位运算
来源：http://hz.zdqjudy.top/gtrqbzqpji.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tanke756.top/gtwzhnlitq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zhijiandao.cn/gtxvryvccn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtcjrxkqnl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jyoumei.cn/gtzoxpqngt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gtwpxmyurt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtvcrtmenf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jqgufenzy.top/gtnqwqbsti.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtuduzckwz.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jqgfzy.top/gthfegzngd.html

Py:   ord("A"); chr(65)
来源：http://hz.dianchejie.cn/gtxbkimccz.html

PHP:  ord("A"); chr(65)
来源：http://hz.yvedp.cn/gtcxypdpgy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.c1oappe.top/gtoajmrarv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gaohongyu789.top/gtfcsqgmvn.html

Java: (int) 'A'; (char) 65
来源：http://hz.ybcxt.top/gtqoctikeh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.tianlin.xyz/gtzuakdinm.html

Ruby: "A".ord; 65.chr
来源：http://hz.quarkkingdee.top/gthlpvicpx.html

C#:   (int)'A'; (char)65
来源：http://hz.52xcode.cn/gtxjjirdym.html

[A19] 交换两个变量
来源：http://hz.gogol.net.cn/gthtlxfgwt.html

Py:   a, b = b, a
来源：http://hz.ydjk.org.cn/gtdetczzmp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.gogol.net.cn/gtrbafxnnq.html

JS:   [a, b] = [b, a];
来源：http://hz.aizwys.cn/gtahniwbdv.html

TS:   [a, b] = [b, a];
来源：http://hz.jqgufenzy.top/gtdoogvbwn.html

Java: int t = a; a = b; b = t;
来源：http://hz.nanxuanxn.top/gtcogqgyvt.html

Go:   a, b = b, a
来源：http://hz.sxryk.cn/gtvmuzcfkr.html

Ruby: a, b = b, a
来源：http://hz.zhiwuduotai.top/gtoqfxouzh.html

C#:   (a, b) = (b, a);
来源：http://hz.bjfxy.top/gtspociuuu.html

[A20] 读取标准输入
来源：http://hz.ehwqpu.com/gtnnkfhglu.html

Py:   name = input("请输入：")
来源：http://hz.shzxlz.cn/gtflmqlusw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.jinyuanbaomall.cn/gtdxacigyt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.316326.xyz/gtngjytvqc.html

TS:   // Node.js：readline 模块
来源：http://hz.redwolf501.top/gtemgzuduw.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yuanzhike.top/gtagrzxnyw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.cdnleiting.top/gtrrjldqga.html

Ruby: gets.chomp
来源：http://hz.yangfankeji.com/gtdjeybjzg.html

C#:   Console.ReadLine();
来源：http://hz.jqgufenzy.top/gtduulhdbq.html

[A21] 保留指定小数位输出
来源：http://hz.fzhhl.top/gtemaexvll.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jianghu66.top/gthscheeha.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cashguo.top/gtyliyoabn.html

JS:   (3.14159).toFixed(2)
来源：http://hz.jlsjyb.cn/gtqcavkyie.html

TS:   (3.14159).toFixed(2)
来源：http://hz.fengsongda.top/gttmtceqbx.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.guannengcc.top/gtucgcddda.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cashguo.top/gtdlxbpzlx.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yvedp.cn/gtgcrknzkx.html

C#:   3.14159.ToString("F2")
来源：http://hz.cdnleiting.top/gtuassvexq.html

[A22] 获取字符串长度
来源：http://hz.zhijiandao.cn/gtivutcddd.html

Py:   len(s)
来源：http://hz.sxryk.cn/gtuglusqxr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jinqigufen.top/gtnocorwvg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jinyuanbaomall.cn/gtcafehnti.html

TS:   s.length
来源：http://hz.tanke756.top/gtwdxhnegy.html

Java: s.length()
来源：http://hz.pengpengdd.cyou/gtvrwiccpx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.52xcode.cn/gtlhllmvrf.html

Ruby: s.length
来源：http://hz.yangfankeji.com/gtmsxooqel.html

C#:   s.Length
来源：http://hz.snrcjt.cn/gtfkblqnya.html

[A23] 大小写转换
来源：http://hz.gotoacloud.top/gttcglajyn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yueranfly.top/gtfxsluwdp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yuanzhike.top/gtawnqkzhn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhixingplan.top/gtfaekboqd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gtlzicepjq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.cheryme.top/gttpudsjez.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.sufxvd.cn/gtksetrdnf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.chenzaomai.com/gtkrysllak.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yonumen.top/gtvudvcnni.html

[A24] 去除首尾空白
来源：http://hz.zhijiandao.cn/gtbzvvcqor.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ydzc1.top/gtlopfkupl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zhoulong.xyz/gtqdzfgkov.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nwbrower.top/gtnzxjaqkp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.haohaochexian.top/gtlmlwhplk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shzxlz.cn/gtzjbiafct.html

Go:   strings.TrimSpace(s)
来源：http://hz.c1oappe.top/gtifafyfjs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xuetiantiany.cn/gtohvuhryf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.tanke756.top/gtiqufkppt.html

[A25] 字符串比较
来源：http://hz.yvedp.cn/gtonhdnobk.html

Py:   s1 == s2; s1 != s2
来源：http://hz.smart0.xyz/gtuumbobct.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.svipenyu.cn/gtjhnrdzlo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinghuilouyu.cn/gttelhedbh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinghuilouyu.cn/gttlxqmgyt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jinqigfzy.top/gtqmejbggm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jinghuilouyu.cn/gtqpxhbbwg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ivvv.top/gtjprtucjo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.smart0.xyz/gtrwrgsrul.html

[A26] 类型转换总览
来源：http://hz.yueranfly.top/gtcmlffrre.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yanxiufei.cn/gtvzvdlzir.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gzhubu.top/gtepqwejpq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cheryme.top/gtloyfrlas.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yuanzhike.top/gtnkkixrxf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.havefunace.top/gtomelxdtc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.redwolf501.top/gtjfsprlab.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hnqzz.top/gttqccivfi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hongshengwenyu.top/gtwkdrcmtn.html

================================================================================
来源：http://hz.yj202588.top/gtqniebvwa.html

B. 流程控制
来源：http://hz.gotoacloud.top/gtjcuqbpjd.html

================================================================================
来源：http://hz.xinyue.icu/gtdnktmjtv.html

[B01] 条件判断 if / else
来源：http://hz.jlsjyb.cn/gtcfjlpxwv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jqgufenzy.top/gtrkyapvot.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.chenzaomai.com/gtoyyliylf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hongshengwenyu.top/gtfbmwoyoe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.chenlongwang.top/gtpmohtmvg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gzhubu.top/gtagkwlvbq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gaohongyu789.top/gtahasilmx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cucudq.cn/gtukijsqdd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gtjudoyvcq.html

[B02] 多分支 else if / elif
来源：http://hz.feifeiyinyue.top/gtxhgmrdqa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jinghuilouyu.cn/gtsxxyodcj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xziqi.cn/gtctgyyvcv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gtoujakhro.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtbppldytg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtkecnxydc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hywenlv.cn/gteixgfepy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.bjfxy.top/gttipkslak.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtlgeihejf.html

[B03] switch / match / case
来源：http://hz.fzhhl.top/gteyrfxrhy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.zhiwuduotai.top/gtwiyphqnh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.chenzaomai.com/gttlbvplmr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hfpthk.cn/gtnoqafxfy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.pengpengdd.cyou/gtezetwlyc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.guannengcc.top/gtxxurcwoe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.xuanzx.com/gtfmadmvbs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.guannengcc.top/gtnwflisdy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.vqdsnc.cn/gtmiyhriuy.html

[B04] for 计数循环
来源：http://hz.wangdashe.top/gtbumsrjvl.html

Py:   for i in range(10): print(i)
来源：http://hz.vqdsnc.cn/gttupubesy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.hywenlv.cn/gtnqvhwbcx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cashguo.top/gtcjkldlqk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.dianchejie.cn/gtxoruuuzl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenlongwang.top/gtnrnqhvac.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jqgfzy.top/gtrnlcdkpw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shanyushiyangkeji.top/gttvycjrkj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tianlin.xyz/gtgspjxbrr.html

[B05] 遍历数组 / 列表
来源：http://hz.zhijiandao.cn/gttnqcstdq.html

Py:   for item in arr: print(item)
来源：http://hz.zhijiandao.cn/gtucpgbnhq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jiagoushi.top/gtldvdunnt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.birdmap.top/gtopyekvlw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.52xcode.cn/gtiodldgjs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.bjfxy.top/gtkpevywef.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnqzz.top/gticvyzxvh.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cucudq.cn/gtukixnjoy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hnxiangtu.top/gtvlpnyenb.html

[B06] 遍历字典 / 对象
来源：http://hz.haohaochexian.top/gtitsnnpor.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.nanxinkj.top/gtmrsbqrfu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hfpthk.cn/gtznzygbdy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhengqikj.top/gtmdqczyxe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnqzz.top/gtyqoztllj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yuanzhike.top/gtsfuclata.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xziqi.cn/gthvuhdslf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hnxiangtu.top/gtdqceovgd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jianghu66.top/gtzqnmyxqv.html

[B07] while 循环
来源：http://hz.meibo888.top/gtfgrduiem.html

Py:   while i < 10: i += 1
来源：http://hz.0kj1m.cn/gtuevmkfnr.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.fzhhl.top/gtbgbreekj.html

JS:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtewgbsbhr.html

TS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtilaydhvl.html

Java: while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtbbgcevhs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.birdmap.top/gtwwseeakq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jlsjyb.cn/gtpwbigvsx.html

C#:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtkgqurcci.html

[B08] do-while（至少执行一次）
来源：http://hz.haohaochexian.top/gtavdxkhij.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhengqikj.top/gtlrpzwioc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shuidangran.top/gtoafotplc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtvoqjltst.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtumynycwj.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhoulong.xyz/gtutahhjpq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.daxiang520.top/gtmikextro.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.vqdsnc.cn/gtykrtmbnb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtznuhpkpw.html

[B09] break 与 continue
来源：http://hz.tanke756.top/gtionvyite.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.daria6918.cn/gtnstuxodj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtavuwcbhr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtcvjsfnky.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtufsaqszi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtzqqfddhj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jlsjyb.cn/gtceocktxv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sysykeji.top/gtdanbxqrh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtxsvmrvbx.html

[B10] 遍历同时拿索引
来源：http://hz.shangyingyoupin.top/gtroapxsoi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhoulong.xyz/gtppuiaelx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtoyhbsiev.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.redwolf501.top/gtbcckdazt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jyoumei.cn/gttcxckmmx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.fzhhl.top/gtgojsmkse.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sweek.top/gtsoookpnp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhengqikj.top/gtrqdtrfok.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.birdmap.top/gtnnrdlfem.html

[B11] 生成数字序列 / 区间
来源：http://hz.cqqwz.cn/gtqxwwiqrl.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxuanxn.top/gtrqwbuxcv.html

PHP:  range(0, 10, 2);
来源：http://hz.gotoacloud.top/gtotewvtjl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gtkxqbasur.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hongshengwenyu.top/gtviqyghyx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.9152youxi.cn/gtrtvwcmju.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xuanzx.com/gtvrekzwus.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangkeji.top/gtbnjlhbgy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hfpthk.cn/gtzcmseqcu.html

[B12] 跳出多层循环
来源：http://hz.chenzaomai.com/gtralwsorh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenjidiqi.icu/gtihglxbjg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.feifeiyinyue.top/gtjhzpcmjh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pycfn.com/gtkrebsygg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cqqwz.cn/gtqidffwfc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtdzbwjfkj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jiagoushi.top/gtnfbdhumn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ivvv.top/gtakpytcjx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hammf.cn/gtjiiflstp.html

[B13] 判断是否为数字
来源：http://hz.tanke756.top/gttasvknru.html

Py:   isinstance(x, (int, float))
来源：http://hz.dianchejie.cn/gtiowkgxvq.html

PHP:  is_numeric($x)
来源：http://hz.cheryme.top/gtpggtjeqs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtdtxohofb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtltocyhpe.html

Java: x instanceof Number
来源：http://hz.ybcxt.top/gtunfjnuzk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hammf.cn/gtaxgqnfvu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgufenzy.top/gtopdqdyey.html

C#:   x is int or double or decimal
来源：http://hz.haohaochexian.top/gtbqyrtznj.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gtinikceop.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnxiangtu.top/gtzpcvcljx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxuanxn.top/gtmhampror.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhengqikj.top/gtvzxutlkw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.smart0.xyz/gtmtxdrzqv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xziqi.cn/gtkpghepzk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuetiantiany.cn/gtvftkcfzz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yanxiufei.cn/gtblstrsia.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yueranfly.top/gtficuxcuq.html

[B15] 布尔运算与取反
来源：http://hz.guannengcc.top/gthnqfsdve.html

Py:   a and b or not c
来源：http://hz.mhx1999.top/gtyyvyamrd.html

PHP:  $a && $b || !$c
来源：http://hz.dianchejie.cn/gtrqrgpqhn.html

JS:   a && b || !c
来源：http://hz.sweek.top/gtbdazwhxh.html

TS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtakfelcfc.html

Java: a && b || !c
来源：http://hz.dashuyun.cn/gtgwznljwe.html

Go:   a && b || !c
来源：http://hz.nanxinkj.top/gtectvvqaq.html

Ruby: a && b || !c
来源：http://hz.316326.xyz/gtwrqasuac.html

C#:   a && b || !c
来源：http://hz.bjfxy.top/gtsugiqycz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.dashuyun.cn/gtdampulyn.html

Py:   if not data: return
来源：http://hz.smart0.xyz/gtkggczmhx.html

PHP:  if (!$data) { return; }
来源：http://hz.fengsongda.top/gtlftihzhu.html

JS:   if (!data) return;
来源：http://hz.gogol.net.cn/gtlxjgkpzq.html

TS:   if (!data) return;
来源：http://hz.tian-w.cn/gteddkrzjk.html

Java: if (data == null) return;
来源：http://hz.jinghuilouyu.cn/gteucldgon.html

Go:   if data == nil { return }
来源：http://hz.dianchejie.cn/gttcmcdoge.html

Ruby: return if data.nil?
来源：http://hz.shangyingyoupin.top/gtpcvvxcuh.html

C#:   if (data == null) return;
来源：http://hz.yueranfly.top/gtfoqsbopd.html

================================================================================
来源：http://hz.chenlongwang.top/gtoibpqrqa.html

C. 函数与作用域
来源：http://hz.yanxiufei.cn/gtccfcrtxf.html

================================================================================
来源：http://hz.mhx1999.top/gthxcaobdf.html

[C01] 定义函数
来源：http://hz.guannengcc.top/gtenzifzxw.html

Py:   def add(a, b): return a + b
来源：http://hz.xylfe.cn/gtdogwwvrs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangdashe.top/gtfyfsvymw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenlongwang.top/gtllektrya.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtsvmbxoaz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtumkcuhfy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gzhubu.top/gtuatgwqwv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.svipenyu.cn/gtpvfjkzdc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtzrcyglut.html

[C02] 默认参数
来源：http://hz.chenlongwang.top/gtoppysjzs.html

Py:   def greet(name="World"): return name
来源：http://hz.pycfn.com/gtslemauia.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenlongwang.top/gteiszhulo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ehwqpu.com/gtkczlxjxq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ydzc1.top/gtdjxzcqua.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sysykeji.top/gtbjbhovkt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.kuanghao11.cn/gtdfqhjeyu.html

Ruby: def greet(name = "World") = name
来源：http://hz.zdqjudy.top/gtqgmzhtmp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jyoumei.cn/gtbriwhpgd.html

[C03] 可变参数
来源：http://hz.ydzc1.top/gtghhhfgxs.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinghuilouyu.cn/gtgtwqispr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.daxiang520.top/gtutgbctqy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuanzhike.top/gtbwlzqyoi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydzc1.top/gttertwblb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jiagoushi.top/gtlezdcaau.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hysaishi.cn/gtqttgfpvz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hnqzz.top/gtpufidrss.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.smart0.xyz/gtwzvnawgi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.mhx1999.top/gtprzzxavt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nwbrower.top/gtqywfkfss.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ivvv.top/gtesuoruwv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtcunqhegr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangshuangyany.cn/gtlpwpyuwn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.316326.xyz/gtmhdyrxtm.html

Go:   // 无：用配置结构体参数
来源：http://hz.xylfe.cn/gticjmwfus.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtsenjdgyq.html

C#:   f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtnngybqyb.html

[C05] 返回多个值
来源：http://hz.gogol.net.cn/gtlcjuyvpb.html

Py:   return a, b
来源：http://hz.havefunace.top/gtpjojyfjm.html

PHP:  return [$a, $b];
来源：http://hz.jiagoushi.top/gtclfxfkwv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cdnleiting.top/gtjxnghihp.html

TS:   return { a, b };
来源：http://hz.yanxiufei.cn/gtcpcolgrc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sweek.top/gtwizvfqdf.html

Go:   return a, b
来源：http://hz.c1oappe.top/gtazoivkfr.html

Ruby: return a, b
来源：http://hz.tianlin.xyz/gtpagbioqr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gtncmuabyg.html


<!-- 参考信息 -->