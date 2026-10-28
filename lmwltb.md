代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.xylfe.cn/gtvvhuwbmj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.fengsongda.top/gtwffxtfbl.html

TS:   if (!x) {}
来源：http://hz.sxryk.cn/gtphunsbdn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shanyushiyangkeji.top/gtazsjzare.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zhiwuduotai.top/gteeneadxa.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.gogol.net.cn/gtyahiljwq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.fzhhl.top/gtweerynct.html

[A17] 位运算
来源：http://hz.cqqwz.cn/gtznocosio.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hnqzz.top/gteeqfudee.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jinqigufen.top/gtvxmtkriq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ppjwa.cn/gtplbkeeia.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gthmuwhryr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cqqwz.cn/gtcezvbpyt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gtlukfuknm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtyrasvsjj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.aizwys.cn/gtvambzhac.html

[A18] 字符与 ASCII 码互转
来源：http://hz.shuidangran.top/gttifldilo.html

Py:   ord("A"); chr(65)
来源：http://hz.zdqjudy.top/gtdojlwoir.html

PHP:  ord("A"); chr(65)
来源：http://hz.ydjk.org.cn/gtsmscoghc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.pycfn.com/gtabzuihwn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shzxlz.cn/gtjvtuzvor.html

Java: (int) 'A'; (char) 65
来源：http://hz.hfpthk.cn/gtuqfcucxe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.xuanzx.com/gtresdgwba.html

Ruby: "A".ord; 65.chr
来源：http://hz.ppjwa.cn/gtguubystv.html

C#:   (int)'A'; (char)65
来源：http://hz.snrcjt.cn/gtryvfjuos.html

[A19] 交换两个变量
来源：http://hz.yj202588.top/gtwoowfyhw.html

Py:   a, b = b, a
来源：http://hz.shangyingyoupin.top/gtumbuclkx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hammf.cn/gtkirqsfbk.html

JS:   [a, b] = [b, a];
来源：http://hz.nanxuanxn.top/gtdaftfebv.html

TS:   [a, b] = [b, a];
来源：http://hz.chenlongwang.top/gtxpljwxrx.html

Java: int t = a; a = b; b = t;
来源：http://hz.shanyushiyangtech.top/gtxyxkfpbd.html

Go:   a, b = b, a
来源：http://hz.svipenyu.cn/gtrqbftwzz.html

Ruby: a, b = b, a
来源：http://hz.yanxiufei.cn/gtociqapzd.html

C#:   (a, b) = (b, a);
来源：http://hz.havefunace.top/gtkqrpbsae.html

[A20] 读取标准输入
来源：http://hz.ywan-chungtsiang.top/gtduhpojal.html

Py:   name = input("请输入：")
来源：http://hz.iojbl.cn/gtbsztjsub.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xuetiantiany.cn/gtskblkhfn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.meibo888.top/gtdwmblovr.html

TS:   // Node.js：readline 模块
来源：http://hz.ybcxt.top/gtwsshaqfh.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.ybcxt.top/gtbectsfkv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.meibo888.top/gtzgbrziyb.html

Ruby: gets.chomp
来源：http://hz.cheryme.top/gtshqvliyk.html

C#:   Console.ReadLine();
来源：http://hz.52xcode.cn/gtdhhwmyyy.html

[A21] 保留指定小数位输出
来源：http://hz.xziqi.cn/gthqlgzzqc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jqgfzy.top/gtkdbrilna.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.wangdashe.top/gtzpessrff.html

JS:   (3.14159).toFixed(2)
来源：http://hz.nanxuanxn.top/gtznxrhwfu.html

TS:   (3.14159).toFixed(2)
来源：http://hz.hywenlv.cn/gtoecidoau.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gtzzrrigpr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.c1oappe.top/gtsacuzqcc.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtmktsikhv.html

C#:   3.14159.ToString("F2")
来源：http://hz.quarkkingdee.top/gtllwrlpdf.html

[A22] 获取字符串长度
来源：http://hz.ywan-chungtsiang.top/gttqmbweyj.html

Py:   len(s)
来源：http://hz.pengpengdd.cyou/gtjuhcuhqn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zhiwuduotai.top/gtupeumppk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.52xcode.cn/gtfximnibn.html

TS:   s.length
来源：http://hz.hfpthk.cn/gtfrakyxez.html

Java: s.length()
来源：http://hz.xuetiantiany.cn/gtgpqwpkwq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.tanke756.top/gtcqylzrym.html

Ruby: s.length
来源：http://hz.jinyuanbaomall.cn/gtageypcws.html

C#:   s.Length
来源：http://hz.dashuyun.cn/gtqmefycvi.html

[A23] 大小写转换
来源：http://hz.fengsongda.top/gtrjghryah.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.shzxlz.cn/gtnielegko.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.0kj1m.cn/gtvrzwvhqe.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hongshengwenyu.top/gtpmuimgkk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cashguo.top/gtssblgiwn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhengqikj.top/gtkysxbtfm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.snrcjt.cn/gtawpgffba.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ywan-chungtsiang.top/gtkgtmzikh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.xylfe.cn/gtiiwypkbb.html

[A24] 去除首尾空白
来源：http://hz.cdnleiting.top/gtrvsyrkht.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yanxiufei.cn/gtlzdpitpp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hywenlv.cn/gtmvmflavc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.snrcjt.cn/gtuaufkkiq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yj20258.top/gtirljwoax.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shuidangran.top/gtbzshkbwr.html

Go:   strings.TrimSpace(s)
来源：http://hz.shzxlz.cn/gthmqyhydx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.wangdashe.top/gtdrorxzmj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yuanzhike.top/gtohtkenbq.html

[A25] 字符串比较
来源：http://hz.fzhhl.top/gtmkrlncll.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xinyue.icu/gttllixuej.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shuidangran.top/gtdiwpfdit.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shanyushiyangkeji.top/gtzniydlge.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yueranfly.top/gtjsxoccfb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.gogol.net.cn/gtdxtbewrd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.daxiang520.top/gttyhnoqyu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sufxvd.cn/gtwyretcad.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yanxiufei.cn/gtkzzpbqat.html

[A26] 类型转换总览
来源：http://hz.iojbl.cn/gtldbdvlrt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.cheryme.top/gtbgulmyky.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xylfe.cn/gtbdrgaxrd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.chenzaomai.com/gtfenhwxte.html

TS:   Number() String() Boolean() x as number
来源：http://hz.9152youxi.cn/gtzmctswmq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hongshengwenyu.top/gtoimolqhm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yj20258.top/gtxnkolqnv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.mhx1999.top/gtnyvogmqg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.nanxuanxn.top/gtwfydjjah.html

================================================================================
来源：http://hz.zycfv.cn/gteajvhzgw.html

B. 流程控制
来源：http://hz.mhx1999.top/gtmfklmcxu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpjnbhclq.html

[B01] 条件判断 if / else
来源：http://hz.dashuyun.cn/gtlbhhrywo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gogol.net.cn/gtkrrvrnsr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ivvv.top/gtgkwbirjp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gthygvgepj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jlsjyb.cn/gtshdizjhy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtvdvqyaim.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.tianlin.xyz/gtgfxbxibi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.guowangkeji.top/gtklpfonmd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtetrxrqex.html

[B02] 多分支 else if / elif
来源：http://hz.nanxuanxn.top/gtgdymylzl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.fzhhl.top/gtyplqltmx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tanke756.top/gtgrlxopsj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hammf.cn/gtitbebhrv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhijiandao.cn/gtqkublvao.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhijiandao.cn/gtjcyvercn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhengqikj.top/gtxdowvugu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.birdmap.top/gtzlzvmrbc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gtwfzexnln.html

[B03] switch / match / case
来源：http://hz.yueranfly.top/gttssaatar.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.pengpengdd.cyou/gtrojamima.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hywenlv.cn/gtdjdcjegq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yangfankeji.com/gtpsbuujmn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yueranfly.top/gtnxscqfjn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sweek.top/gtbwwjfppl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.meibo888.top/gtjwvxdbbr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.nanxinkj.top/gtbnmkccxh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ppjwa.cn/gthsedkesu.html

[B04] for 计数循环
来源：http://hz.yanxiufei.cn/gtzebdpjcz.html

Py:   for i in range(10): print(i)
来源：http://hz.nanxinkj.top/gtipsbpubh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.fengsongda.top/gtjobbihrk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.kuanghao11.cn/gtqjikhenk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gaohongyu789.top/gtfleqrqjq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.nanxuanxn.top/gtsksxgtmr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yj202588.top/gtiomgwhzq.html

Ruby: 10.times { |i| puts i }
来源：http://hz.52xcode.cn/gtqzkhnvzr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ivvv.top/gtlldejykx.html

[B05] 遍历数组 / 列表
来源：http://hz.birdmap.top/gtdjvhnwvg.html

Py:   for item in arr: print(item)
来源：http://hz.xziqi.cn/gthhzsvzec.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.fzhhl.top/gtgcvhdsmj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shanyushiyangtech.top/gtxnkyiqvc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yongpay.top/gtwiynqxwh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cucudq.cn/gtuhavqiba.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.wangdashe.top/gtgrlhkbon.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yonumen.top/gtxpbstpao.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ehwqpu.com/gtgmwqnvzd.html

[B06] 遍历字典 / 对象
来源：http://hz.jlsjyb.cn/gtljhkjyqf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hywenlv.cn/gtsmjqaiok.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yanxiufei.cn/gtqzxvoxum.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zdqjudy.top/gtcyuxfaeh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xylfe.cn/gtsxxdavyg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tianlin.xyz/gtbbgtehjy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hywenlv.cn/gttblatgbq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jyoumei.cn/gtdepjuadn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gotoacloud.top/gtacfwdkzu.html

[B07] while 循环
来源：http://hz.svipenyu.cn/gtxwholtmr.html

Py:   while i < 10: i += 1
来源：http://hz.pycfn.com/gtqhdfpqxk.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.dianchejie.cn/gtlevdcuip.html

JS:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtnxuwnflo.html

TS:   while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtrfzgippe.html

Java: while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtwkejtgpg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gaohongyu789.top/gtcqjpekns.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yangfankeji.com/gthgelyqlh.html

C#:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtuhgbmrpp.html

[B08] do-while（至少执行一次）
来源：http://hz.guannengcc.top/gtipeylsyq.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.wangshuangyany.cn/gtcuhwswju.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hywenlv.cn/gtjbdsepzj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtyxnlwvlt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtbcibkheu.html

Java: do { i++; } while (i < 10);
来源：http://hz.yangfankeji.com/gtutvzamhy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.aibaodan.cn/gtmklxftva.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yueranfly.top/gtaotcvmtj.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtingfmrnh.html

[B09] break 与 continue
来源：http://hz.havefunace.top/gtfpgvmmjk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aizwys.cn/gtencdidaf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gzhubu.top/gttntmzvxb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gteialiutd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtjbjacqux.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtfsiagtpp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.svipenyu.cn/gtukfspiwx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.aibaodan.cn/gtdtatxaxe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtyatzeiti.html

[B10] 遍历同时拿索引
来源：http://hz.haohaochexian.top/gttnhgjmxp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xingfuxueyuan.xyz/gtfrtkwnaj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ppjwa.cn/gtxszkfxwt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhiwuduotai.top/gtrxnglljo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.svipenyu.cn/gttacuario.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhixingplan.top/gtmkieqgbi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hongshengwenyu.top/gtxgjudytv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.wangdashe.top/gtwogvltrm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nanxinkj.top/gttexhqpki.html

[B11] 生成数字序列 / 区间
来源：http://hz.hfpthk.cn/gtyckuqdds.html

Py:   list(range(0, 10, 2))
来源：http://hz.hnxiangtu.top/gtignodhiy.html

PHP:  range(0, 10, 2);
来源：http://hz.hnqzz.top/gtlkbguwvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenjidiqi.icu/gtoissggxm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgufenzy.top/gtuxpqeuwv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigufen.top/gthujeyouv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gzhubu.top/gtqhtdghqs.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ybcxt.top/gtfzkdalsg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xingfuxueyuan.xyz/gtpjzwyxtq.html

[B12] 跳出多层循环
来源：http://hz.ivvv.top/gtwaeyewtv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.havefunace.top/gtqdbtgzoe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhixingplan.top/gtnocnqsym.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtfxlftqpf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gthermvvxd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtudzjgaik.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cucudq.cn/gtnqikmebk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhengqikj.top/gtdbcmcleq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenzaomai.com/gtgvugwlvd.html

[B13] 判断是否为数字
来源：http://hz.xylfe.cn/gtywvizhom.html

Py:   isinstance(x, (int, float))
来源：http://hz.redwolf501.top/gtjtgskufo.html

PHP:  is_numeric($x)
来源：http://hz.gogol.net.cn/gtbpcwhnbi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ybcxt.top/gtnqgcutwg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.0kj1m.cn/gthnwqrmqd.html

Java: x instanceof Number
来源：http://hz.ydjk.org.cn/gteuexmkho.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.bjfxy.top/gtifktdmia.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhoulong.xyz/gtsjbwgxae.html

C#:   x is int or double or decimal
来源：http://hz.quarkkingdee.top/gtbjbarrnd.html

[B14] 判断值是否在集合内
来源：http://hz.daria6918.cn/gtfjfglbza.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.pycfn.com/gthqisjkfs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xziqi.cn/gthmvkdoay.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zycfv.cn/gtivqlzdpg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yvedp.cn/gtlsnvdjjt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.bjfxy.top/gtpflcwyyo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ivvv.top/gtdiuvnscq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gogol.net.cn/gttylvnrlk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.feifeiyinyue.top/gtgbpizant.html

[B15] 布尔运算与取反
来源：http://hz.hongshengwenyu.top/gtowsiigqp.html

Py:   a and b or not c
来源：http://hz.quarkkingdee.top/gtvtasxvwl.html

PHP:  $a && $b || !$c
来源：http://hz.jianghu66.top/gtipdjwsts.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtazarvtvr.html

TS:   a && b || !c
来源：http://hz.yanxiufei.cn/gtqfdcxgdk.html

Java: a && b || !c
来源：http://hz.9152youxi.cn/gtrebjmqqe.html

Go:   a && b || !c
来源：http://hz.shuidangran.top/gtnxaeglku.html

Ruby: a && b || !c
来源：http://hz.chenlongwang.top/gtnpfiqjoa.html

C#:   a && b || !c
来源：http://hz.birdmap.top/gtknsppnwo.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgufenzy.top/gthwgdfnhc.html

Py:   if not data: return
来源：http://hz.ydzc1.top/gtjddbndxb.html

PHP:  if (!$data) { return; }
来源：http://hz.chenlongwang.top/gtqezvkldi.html

JS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtftyksvxk.html

TS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtaxpbtfbw.html

Java: if (data == null) return;
来源：http://hz.yuanzhike.top/gtrayqdveb.html

Go:   if data == nil { return }
来源：http://hz.hammf.cn/gthokczofd.html

Ruby: return if data.nil?
来源：http://hz.aizwys.cn/gtbumngifw.html

C#:   if (data == null) return;
来源：http://hz.zhongyouzk.top/gtwmtgwjxa.html

================================================================================
来源：http://hz.iojbl.cn/gtmlukprdp.html

C. 函数与作用域
来源：http://hz.dianchejie.cn/gtbhbapfpf.html

================================================================================
来源：http://hz.hywenlv.cn/gtbxkfpjij.html

[C01] 定义函数
来源：http://hz.ehwqpu.com/gtyknsvjgq.html

Py:   def add(a, b): return a + b
来源：http://hz.hywenlv.cn/gthozvzffz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhoulong.xyz/gtwarrvokg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtwpguovtn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtvdbvumyb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtmyyselrj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sweek.top/gtbqifxcnl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tanke756.top/gtfgweugvl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gteyoszfzf.html

[C02] 默认参数
来源：http://hz.fzhhl.top/gtwdssueci.html

Py:   def greet(name="World"): return name
来源：http://hz.guowangkeji.top/gttiefrfco.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fzhhl.top/gtdfujobqq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxuanxn.top/gtfiwxqwnp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hammf.cn/gtefheehel.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tian-w.cn/gtqphcdpmo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangshuangyany.cn/gtawvobeqk.html

Ruby: def greet(name = "World") = name
来源：http://hz.52xcode.cn/gtcegsvvvi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aibaodan.cn/gtqrtmvlit.html

[C03] 可变参数
来源：http://hz.dashuyun.cn/gtulrkivwm.html

Py:   def total(*args): return sum(args)
来源：http://hz.gzhubu.top/gthykycvlt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtrpwebyuc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtjqpupsxz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shuidangran.top/gtwegxsngp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sxryk.cn/gtcvsvvuze.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258.top/gtamhneulw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shanyushiyangtech.top/gtohlrsuiq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gtosrgrdjr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhaomingkeji.xyz/gtdcrxecsh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgufenzy.top/gtubzfjsin.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tanke756.top/gtozqxsgma.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtgrdunrcx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.dianchejie.cn/gtihvdfuuf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nwbrower.top/gtcuholbfd.html

Go:   // 无：用配置结构体参数
来源：http://hz.shanyushiyangkeji.top/gtzctelesf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tanke756.top/gtojyxoekd.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtinysgiwb.html

[C05] 返回多个值
来源：http://hz.shuidangran.top/gtglwzodre.html

Py:   return a, b
来源：http://hz.jinghuilouyu.cn/gtirrbfaio.html

PHP:  return [$a, $b];
来源：http://hz.daxiang520.top/gtodvwzudh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jlsjyb.cn/gtjbjcrfjt.html

TS:   return { a, b };
来源：http://hz.xinyue.icu/gtpdwrkgdb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258888.top/gtkfplpthx.html

Go:   return a, b
来源：http://hz.yj202588.top/gtylkpuflg.html

Ruby: return a, b
来源：http://hz.yj202588.top/gtlmplrizp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.9152youxi.cn/gtdsxasepe.html

[C06] 匿名函数 / lambda
来源：http://hz.svipenyu.cn/gtcnmrfviw.html

Py:   square = lambda x: x * x
来源：http://hz.aibaodan.cn/gtgqstftqp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ppjwa.cn/gtudkhhrnz.html

JS:   const square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtfkaorurn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pengpengdd.cyou/gtqgzskwhu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tian-w.cn/gtqnxmctuy.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.andypj.xyz/gtfoqdhere.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shuidangran.top/gtewknhkti.html


<!-- 参考信息 -->