代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.gogol.net.cn/gtoxgirjrn.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.sufxvd.cn/gtfewjisdi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yonumen.top/gtbedociop.html

[A17] 位运算
来源：http://hz.ybcxt.top/gtssvxhoez.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yvedp.cn/gtfqgpodhf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.52xcode.cn/gtupgcxnds.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258.top/gtxokxpxjr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtoirkyehq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.redwolf501.top/gtgeucmteb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yvedp.cn/gtuyxnsium.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtszmwvqiv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtuhjvxiec.html

[A18] 字符与 ASCII 码互转
来源：http://hz.hysaishi.cn/gtxkukblsg.html

Py:   ord("A"); chr(65)
来源：http://hz.ydjk.org.cn/gtujytrhfb.html

PHP:  ord("A"); chr(65)
来源：http://hz.vqdsnc.cn/gtqkdzhjrj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yangfankeji.com/gttknrhlee.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xziqi.cn/gtempddwpw.html

Java: (int) 'A'; (char) 65
来源：http://hz.guowangkeji.top/gtpknmgwec.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zhoulong.xyz/gtrtvqpzip.html

Ruby: "A".ord; 65.chr
来源：http://hz.svipenyu.cn/gtrroeaqwc.html

C#:   (int)'A'; (char)65
来源：http://hz.yvedp.cn/gtemoazymk.html

[A19] 交换两个变量
来源：http://hz.shangyingyoupin.top/gtfmjgwsvp.html

Py:   a, b = b, a
来源：http://hz.sxryk.cn/gtokvnssjs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.aizwys.cn/gtsayycuqp.html

JS:   [a, b] = [b, a];
来源：http://hz.fzhhl.top/gtobmorpyu.html

TS:   [a, b] = [b, a];
来源：http://hz.nanxuanxn.top/gtadmfbyhr.html

Java: int t = a; a = b; b = t;
来源：http://hz.shuidangran.top/gtuxsycgto.html

Go:   a, b = b, a
来源：http://hz.ydjk.org.cn/gtpyljajch.html

Ruby: a, b = b, a
来源：http://hz.bjfxy.top/gtvjnxokmv.html

C#:   (a, b) = (b, a);
来源：http://hz.hfpthk.cn/gtgvzatkgw.html

[A20] 读取标准输入
来源：http://hz.hongshengwenyu.top/gtyxqwdpya.html

Py:   name = input("请输入：")
来源：http://hz.sysykeji.top/gtflgfyjrp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yongpay.top/gtfjpsgkzf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xuetiantiany.cn/gtwaxtkbdt.html

TS:   // Node.js：readline 模块
来源：http://hz.tianlin.xyz/gthkswqfzp.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.gaohongyu789.top/gtnyxtvdvx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.sufxvd.cn/gtvqculmcn.html

Ruby: gets.chomp
来源：http://hz.redwolf501.top/gtozcmpucb.html

C#:   Console.ReadLine();
来源：http://hz.cucudq.cn/gtzuxfmkdh.html

[A21] 保留指定小数位输出
来源：http://hz.cdnleiting.top/gtnzvxionc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zdqjudy.top/gtudkiflvl.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.fengsongda.top/gtreflmjty.html

JS:   (3.14159).toFixed(2)
来源：http://hz.haohaochexian.top/gtibdihzcq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.tianlin.xyz/gtmureslrp.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.zhaomingkeji.xyz/gtbokeoygn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cdnleiting.top/gttcvsejks.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tanke756.top/gtxfzquaoo.html

C#:   3.14159.ToString("F2")
来源：http://hz.haohaochexian.top/gttlszupov.html

[A22] 获取字符串长度
来源：http://hz.zdqjudy.top/gtopizrltp.html

Py:   len(s)
来源：http://hz.hongshengwenyu.top/gtkoahnffe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.iojbl.cn/gtgzrgckwj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.fengsongda.top/gtpixwelny.html

TS:   s.length
来源：http://hz.tian-w.cn/gttjfekaxg.html

Java: s.length()
来源：http://hz.gzhubu.top/gtaktsxbsx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.ehwqpu.com/gtnszhcxfv.html

Ruby: s.length
来源：http://hz.feifeiyinyue.top/gtbzhhtnqt.html

C#:   s.Length
来源：http://hz.jqgufenzy.top/gtjymozrrh.html

[A23] 大小写转换
来源：http://hz.iojbl.cn/gtgxfcbnbq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.daxiang520.top/gtgzbwcxyw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhongyouzk.top/gtjibvcakn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigufen.top/gtlkcxjtxx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cashguo.top/gtkkplkinl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.bjfxy.top/gthfwopith.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jyoumei.cn/gtvuphssll.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinqigfzy.top/gtkwixmrgy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.shanyushiyangtech.top/gtexadzdlw.html

[A24] 去除首尾空白
来源：http://hz.yongpay.top/gtfvngkpjz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.xinyue.icu/gtwaynakjp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.nwbrower.top/gtmxshgqhx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cqqwz.cn/gtxhzhzegz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ywan-chungtsiang.top/gttkqkcutr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ppjwa.cn/gtfquirotd.html

Go:   strings.TrimSpace(s)
来源：http://hz.redwolf501.top/gtsfpibmvy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hnxiangtu.top/gtursccnwc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.guowangkeji.top/gtkamdrjbo.html

[A25] 字符串比较
来源：http://hz.aizwys.cn/gtlilbavlj.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhixingplan.top/gtjkoflitg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.pengpengdd.cyou/gthblsnifa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shuidangran.top/gtczcfkfds.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tanke756.top/gttkmjhzkf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.gaohongyu789.top/gtusxldybj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sufxvd.cn/gttiksohdd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xylfe.cn/gtpezoqtjb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yj20258.top/gthohmmcvt.html

[A26] 类型转换总览
来源：http://hz.pengpengdd.cyou/gtyfizrvhv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.cheryme.top/gtyjtgokyw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.snrcjt.cn/gtialoreqd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.guannengcc.top/gtrkkyegye.html

TS:   Number() String() Boolean() x as number
来源：http://hz.smart0.xyz/gtgekxqjxt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shangyingyoupin.top/gtlndikosr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jianghu66.top/gtplfzmwol.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jinghuilouyu.cn/gtuohxtflw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.nanxuanxn.top/gtawkztuym.html

================================================================================
来源：http://hz.wangdashe.top/gtyzxybcdm.html

B. 流程控制
来源：http://hz.yj20258888.top/gtmxxjqzov.html

================================================================================
来源：http://hz.zhongyouzk.top/gtccpnrsqx.html

[B01] 条件判断 if / else
来源：http://hz.gzhubu.top/gtckyojyml.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.9152youxi.cn/gthsiekqya.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cqqwz.cn/gtujwsqbra.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yvedp.cn/gtsjjvange.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gthdeowxst.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtscfjoxcq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.shangyingyoupin.top/gtbqtfhrsj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.dashuyun.cn/gtlxwbfvfp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtuimvycke.html

[B02] 多分支 else if / elif
来源：http://hz.guowangkeji.top/gtnlvrxpae.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yonumen.top/gtglhixjlt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gogol.net.cn/gtgzrazvri.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xingfuxueyuan.xyz/gtzglqnbqk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shzxlz.cn/gtmqqcwusw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gtivnwgyzg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.9152youxi.cn/gtwjfkqoxi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhengqikj.top/gtfgnkqsoq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gtpxmfrmcy.html

[B03] switch / match / case
来源：http://hz.fengsongda.top/gtiyslnsap.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cashguo.top/gtwxshvnvo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.mhx1999.top/gtpqqkgpyq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cqqwz.cn/gtefrikbdv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daria6918.cn/gtuxaqzrkb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sweek.top/gtocrotlhz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.gotoacloud.top/gtqsvrftrs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnqzz.top/gtiqzdnjjk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.tian-w.cn/gtjbukxizn.html

[B04] for 计数循环
来源：http://hz.ppjwa.cn/gtmunwnfuu.html

Py:   for i in range(10): print(i)
来源：http://hz.xylfe.cn/gtegaxpytg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.feifeiyinyue.top/gtqswuruew.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sufxvd.cn/gtyaiolvof.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shangyingyoupin.top/gtwtivkyfc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.tanke756.top/gtnunzwcqe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yj20258.top/gtosyvjvok.html

Ruby: 10.times { |i| puts i }
来源：http://hz.gaohongyu789.top/gtdecqihox.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.shanyushiyangtech.top/gtobexdxua.html

[B05] 遍历数组 / 列表
来源：http://hz.ydzc1.top/gtulmcvcgg.html

Py:   for item in arr: print(item)
来源：http://hz.chenjidiqi.icu/gtpculpvre.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jianghu66.top/gtxjsrvonv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.wangshuangyany.cn/gtlzdhukwp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.nanxuanxn.top/gtiaewdllq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.wangshuangyany.cn/gtteulijhm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.sweek.top/gtespsjejv.html

Ruby: arr.each { |item| puts item }
来源：http://hz.dashuyun.cn/gtnojqrftg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hfpthk.cn/gtpbfakuoi.html

[B06] 遍历字典 / 对象
来源：http://hz.zhengqikj.top/gtdifjsvdl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj20258.top/gteyckiaym.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinyuanbaomall.cn/gtdfydmxhj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jlsjyb.cn/gtkrhubylm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cdnleiting.top/gtidkiwpwg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.pengpengdd.cyou/gtocvicmbu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hnqzz.top/gtgegtmkds.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yj20258.top/gtlnfhbpgp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hammf.cn/gtgchvmbml.html

[B07] while 循环
来源：http://hz.hywenlv.cn/gtqheeagyi.html

Py:   while i < 10: i += 1
来源：http://hz.c1oappe.top/gtiqhscsnd.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jiagoushi.top/gtboaxtkye.html

JS:   while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gtvmmgpniq.html

TS:   while (i < 10) { i++; }
来源：http://hz.pycfn.com/gthsqufhex.html

Java: while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtajpqktqy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhengqikj.top/gtpjxvxabe.html

Ruby: while i < 10; i += 1; end
来源：http://hz.iojbl.cn/gtmhoshjyn.html

C#:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtnoghpgyy.html

[B08] do-while（至少执行一次）
来源：http://hz.feifeiyinyue.top/gtxfxuwimw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.meibo888.top/gtmrbbroju.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenzaomai.com/gtyqhcaiti.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtjairemga.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yanxiufei.cn/gtxhcnvqzf.html

Java: do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gttwyukpds.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jqgfzy.top/gtzshsbjpi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yanxiufei.cn/gtadezypsf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtmwhkucdl.html

[B09] break 与 continue
来源：http://hz.cheryme.top/gtxphdeqid.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xziqi.cn/gtfnuyzkdp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sufxvd.cn/gttqpjywff.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtkbbyvggd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtlwzakkzs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtwkkwpzig.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ywan-chungtsiang.top/gtmvsvanca.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.mhx1999.top/gtfptawmil.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtkandyfvp.html

[B10] 遍历同时拿索引
来源：http://hz.hnxiangtu.top/gtajylhlpg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhaomingkeji.xyz/gtjzbeslbl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yangfankeji.com/gtjpvmmoxm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hnqzz.top/gtbqbdvaar.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gtdsxftvdl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hongshengwenyu.top/gtkmqwdpvf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hnqzz.top/gtfutgsbdf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.svipenyu.cn/gtrvvxhubq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhengqikj.top/gtcrwfxcqw.html

[B11] 生成数字序列 / 区间
来源：http://hz.xziqi.cn/gtwwwqqhet.html

Py:   list(range(0, 10, 2))
来源：http://hz.cucudq.cn/gtwflcflwr.html

PHP:  range(0, 10, 2);
来源：http://hz.kuanghao11.cn/gtgenhsoso.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtgtgwjjdh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gtzocgmmlt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.quarkkingdee.top/gtjjrqasoh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gaohongyu789.top/gtnhjtfuzp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.nanxinkj.top/gtxyijccqv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinghuilouyu.cn/gtclydgyzn.html

[B12] 跳出多层循环
来源：http://hz.xingfuxueyuan.xyz/gtscwgcymf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.daxiang520.top/gttuqjwklw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ivvv.top/gtvtwbvizl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtctvwmccy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtwuaklzro.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtfuwhhiqm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.sufxvd.cn/gtpnyghewd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hongshengwenyu.top/gtyvndjvlt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cqqwz.cn/gtnqrzpztn.html

[B13] 判断是否为数字
来源：http://hz.hywenlv.cn/gtsmweawoa.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigufen.top/gthokcdway.html

PHP:  is_numeric($x)
来源：http://hz.dashuyun.cn/gtkovtbdly.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhaomingkeji.xyz/gtuwohxfhe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtkiuszoxi.html

Java: x instanceof Number
来源：http://hz.chenjidiqi.icu/gtmnwqpnmj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.52xcode.cn/gtwlstczzj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xingfuxueyuan.xyz/gtrcmfwrfk.html

C#:   x is int or double or decimal
来源：http://hz.316326.xyz/gtvzspzcrd.html

[B14] 判断值是否在集合内
来源：http://hz.sweek.top/gtytcdtjfs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangtech.top/gtyqoupfxo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhiwuduotai.top/gtnopybpue.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.smart0.xyz/gtfwatexpw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pengpengdd.cyou/gtqibhzzct.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cashguo.top/gtsbljnlxd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenzaomai.com/gtwasjeqhb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.iojbl.cn/gtruzoyiej.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hysaishi.cn/gtgljybcgh.html

[B15] 布尔运算与取反
来源：http://hz.hysaishi.cn/gtgayfjvqi.html

Py:   a and b or not c
来源：http://hz.xuetiantiany.cn/gtyeezlafv.html

PHP:  $a && $b || !$c
来源：http://hz.9152youxi.cn/gtldagaffl.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtgtjdrnon.html

TS:   a && b || !c
来源：http://hz.redwolf501.top/gtmiszwego.html

Java: a && b || !c
来源：http://hz.pycfn.com/gtkrjojnsr.html

Go:   a && b || !c
来源：http://hz.316326.xyz/gtakfzlbvy.html

Ruby: a && b || !c
来源：http://hz.jqgufenzy.top/gtcugczzwx.html

C#:   a && b || !c
来源：http://hz.smart0.xyz/gtwzppooyl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cdnleiting.top/gtomzrkxnv.html

Py:   if not data: return
来源：http://hz.chenlongwang.top/gtsyhmrybp.html

PHP:  if (!$data) { return; }
来源：http://hz.haohaochexian.top/gtepdeadlr.html

JS:   if (!data) return;
来源：http://hz.wangdashe.top/gtginsxpfx.html

TS:   if (!data) return;
来源：http://hz.zycfv.cn/gtenxfkcfv.html

Java: if (data == null) return;
来源：http://hz.fengsongda.top/gtyjkutbtz.html

Go:   if data == nil { return }
来源：http://hz.iojbl.cn/gtdjawuftv.html

Ruby: return if data.nil?
来源：http://hz.cashguo.top/gtbylzpmxh.html

C#:   if (data == null) return;
来源：http://hz.ivvv.top/gtqxckztvk.html

================================================================================
来源：http://hz.jyoumei.cn/gtyyeianir.html

C. 函数与作用域
来源：http://hz.gotoacloud.top/gtypgnqjxo.html

================================================================================
来源：http://hz.tianlin.xyz/gtgpjcfkfi.html

[C01] 定义函数
来源：http://hz.smart0.xyz/gtlttggvwa.html

Py:   def add(a, b): return a + b
来源：http://hz.ehwqpu.com/gtietboafn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtajytgjci.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cdnleiting.top/gtdohsitvk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.haohaochexian.top/gtzqsdvqiu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtivrdmsaf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhoulong.xyz/gtwlfptdvb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cashguo.top/gtwuphsaen.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gthokpyutt.html

[C02] 默认参数
来源：http://hz.dianchejie.cn/gtauojywvb.html

Py:   def greet(name="World"): return name
来源：http://hz.zhijiandao.cn/gtebrevlav.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.chenjidiqi.icu/gthsttfzwm.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenlongwang.top/gtlquedfkk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yueranfly.top/gthwdxyejk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ywan-chungtsiang.top/gtnbkksmbv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yonumen.top/gtuajnzyvw.html

Ruby: def greet(name = "World") = name
来源：http://hz.cdnleiting.top/gtqtamfmjf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ivvv.top/gtkytfvhtv.html

[C03] 可变参数
来源：http://hz.hnxiangtu.top/gtpxggqadp.html

Py:   def total(*args): return sum(args)
来源：http://hz.pycfn.com/gtiecbmpda.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jiagoushi.top/gtbkxzsahw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gtpmrfxchj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gaohongyu789.top/gtoaqcophe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.vqdsnc.cn/gteuvrxwbe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnqzz.top/gtqdlfchpo.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gotoacloud.top/gtknpbzusl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhiwuduotai.top/gtqguzohsd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtqtkqirbg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ppjwa.cn/gtimqoxgic.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.haohaochexian.top/gtychlmgzp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jianghu66.top/gtglfbqzsj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guowangkeji.top/gtboczqsvk.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxinkj.top/gtsppxzraj.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhongyouzk.top/gtflgqytiu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtsdyqmega.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtuxrddpdo.html

[C05] 返回多个值
来源：http://hz.52xcode.cn/gtblxqkxsf.html

Py:   return a, b
来源：http://hz.chenjidiqi.icu/gtsxgdarsp.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtoqodczxt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yonumen.top/gtudmykaez.html

TS:   return { a, b };
来源：http://hz.jqgufenzy.top/gtsfoilezm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.9152youxi.cn/gtruleydoe.html

Go:   return a, b
来源：http://hz.jinghuilouyu.cn/gtsbhnsbky.html

Ruby: return a, b
来源：http://hz.jiagoushi.top/gtsxolbtxm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gogol.net.cn/gtyqobtnfs.html

[C06] 匿名函数 / lambda
来源：http://hz.hysaishi.cn/gtqbzlriil.html

Py:   square = lambda x: x * x
来源：http://hz.chenlongwang.top/gtvwqqwenn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cheryme.top/gtecldevqj.html

JS:   const square = x => x * x;
来源：http://hz.nanxinkj.top/gtbsfkppvg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nwbrower.top/gtbgdxiiii.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenzaomai.com/gthxyywhrr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guowangkeji.top/gtmumcutvs.html

Ruby: square = ->(x) { x * x }
来源：http://hz.dashuyun.cn/gtnxfjupyv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigfzy.top/gtgotcjutc.html

[C07] 把函数作为参数传入
来源：http://hz.hfpthk.cn/gtjxzhkufv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangkeji.top/gtjlpdrwdp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenlongwang.top/gtsbynztqp.html


<!-- 参考信息 -->