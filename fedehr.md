代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.nanxuanxn.top/gtdnmwswhh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.ywan-chungtsiang.top/gtmbgovfjk.html

TS:   if (!x) {}
来源：http://hz.jiagoushi.top/gtrdlhutse.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yuxming.cn/gtvifavokg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.haohaochexian.top/gtovvlegfx.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.feifeiyinyue.top/gtcxufoiam.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.pycfn.com/gtxmloycre.html

[A17] 位运算
来源：http://hz.tanke756.top/gtohjbsxjt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenzaomai.com/gtrhvhyiuf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.c1oappe.top/gthoqlsdhq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yangfankeji.com/gtdkqmwhrv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtgexrxudc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.0kj1m.cn/gthbuvkspy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.sweek.top/gtpvyzjbmi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cucudq.cn/gtjqzjuonp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangshuangyany.cn/gttiahiqxs.html

[A18] 字符与 ASCII 码互转
来源：http://hz.smart0.xyz/gtcqgapube.html

Py:   ord("A"); chr(65)
来源：http://hz.chenlongwang.top/gtvygqckbm.html

PHP:  ord("A"); chr(65)
来源：http://hz.hysaishi.cn/gtggjgsunn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.haohaochexian.top/gtkuwbwjcg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xingfuxueyuan.xyz/gtwzbrlbby.html

Java: (int) 'A'; (char) 65
来源：http://hz.redwolf501.top/gtzlwwwlqe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.vqdsnc.cn/gteddtzwlp.html

Ruby: "A".ord; 65.chr
来源：http://hz.yanxiufei.cn/gtvyikmigp.html

C#:   (int)'A'; (char)65
来源：http://hz.xuetiantiany.cn/gthoccywkf.html

[A19] 交换两个变量
来源：http://hz.vqdsnc.cn/gtzifhyynp.html

Py:   a, b = b, a
来源：http://hz.snrcjt.cn/gtsscdkxkj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yuanzhike.top/gtkolfxyic.html

JS:   [a, b] = [b, a];
来源：http://hz.chenjidiqi.icu/gtzvynixqg.html

TS:   [a, b] = [b, a];
来源：http://hz.xuanzx.com/gtmkesifxy.html

Java: int t = a; a = b; b = t;
来源：http://hz.xuetiantiany.cn/gtrvvtaijd.html

Go:   a, b = b, a
来源：http://hz.cucudq.cn/gthwfxlbsv.html

Ruby: a, b = b, a
来源：http://hz.gzhubu.top/gtbmuqraay.html

C#:   (a, b) = (b, a);
来源：http://hz.316326.xyz/gtznyjtxja.html

[A20] 读取标准输入
来源：http://hz.fengsongda.top/gtyvwujugi.html

Py:   name = input("请输入：")
来源：http://hz.zhiwuduotai.top/gtaecoqscu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.iojbl.cn/gtplusmkrg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.hywenlv.cn/gtquhfovwj.html

TS:   // Node.js：readline 模块
来源：http://hz.zycfv.cn/gtfbsfvhqp.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhiwuduotai.top/gteigbzugy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.guannengcc.top/gtcwypgcms.html

Ruby: gets.chomp
来源：http://hz.birdmap.top/gtnrcbrruv.html

C#:   Console.ReadLine();
来源：http://hz.vqdsnc.cn/gtwjanqpcq.html

[A21] 保留指定小数位输出
来源：http://hz.ywan-chungtsiang.top/gtdgoobysk.html

Py:   f"{3.14159:.2f}"
来源：http://hz.smart0.xyz/gtbyxwwzcj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yongpay.top/gtthduwbvi.html

JS:   (3.14159).toFixed(2)
来源：http://hz.aibaodan.cn/gtszoyufwj.html

TS:   (3.14159).toFixed(2)
来源：http://hz.guannengcc.top/gtdafzzhxj.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtmtcseqhc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.zhaomingkeji.xyz/gtoxoxmrya.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jlsjyb.cn/gtbvbtnzln.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj202588.top/gtmlqbonki.html

[A22] 获取字符串长度
来源：http://hz.gogol.net.cn/gtvvcihlwt.html

Py:   len(s)
来源：http://hz.hnxiangtu.top/gtwebhgroi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.dianchejie.cn/gtkkehopjf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xingfuxueyuan.xyz/gtcglekwjv.html

TS:   s.length
来源：http://hz.shanyushiyangkeji.top/gtdwvqhhdk.html

Java: s.length()
来源：http://hz.hnxiangtu.top/gtnqoamwyw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.gotoacloud.top/gtkslwkofi.html

Ruby: s.length
来源：http://hz.jinqigufen.top/gtdkjkenyq.html

C#:   s.Length
来源：http://hz.vqdsnc.cn/gtdybhgeia.html

[A23] 大小写转换
来源：http://hz.daria6918.cn/gtiqewdotz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.feifeiyinyue.top/gtuakrodds.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.nanxinkj.top/gtsepvhnkj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.meibo888.top/gtcvlrenom.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.guowangkeji.top/gtcfdrbnob.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.nanxuanxn.top/gtmnzmydyc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinqigufen.top/gtfomikgra.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.chenlongwang.top/gtlhpuvzxu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.daria6918.cn/gtgybkqsnf.html

[A24] 去除首尾空白
来源：http://hz.iojbl.cn/gthzueursy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhaomingkeji.xyz/gtkpiqsbnk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yuxming.cn/gtzoyzngec.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nwbrower.top/gttlxtkmpm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tian-w.cn/gtatuxxqno.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.zhiwuduotai.top/gtzvgyylym.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhengqikj.top/gtoctoftzl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.havefunace.top/gtceqteftf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.xingfuxueyuan.xyz/gtjdihflyv.html

[A25] 字符串比较
来源：http://hz.yongpay.top/gtkraavzzl.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shanyushiyangkeji.top/gtmgiciktd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.vqdsnc.cn/gtjiwrmurn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sufxvd.cn/gtfkfppkro.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.guannengcc.top/gtviwkpfdu.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.52xcode.cn/gtpxqltryb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hywenlv.cn/gtnftseaeb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.9152youxi.cn/gtusbiudqj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.shzxlz.cn/gtliuzhufm.html

[A26] 类型转换总览
来源：http://hz.havefunace.top/gtehagtred.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.nanxuanxn.top/gteugwmxvz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yj20258.top/gtrredhhqi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hongshengwenyu.top/gtrnxgiifo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.shzxlz.cn/gtpricylbv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yuxming.cn/gtlzyznkfm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.shangyingyoupin.top/gtlykoelzs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhaomingkeji.xyz/gtwvvtzsjp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.cashguo.top/gtyrcjmmfx.html

================================================================================
来源：http://hz.yj20258888.top/gtxpnmydtu.html

B. 流程控制
来源：http://hz.wangdashe.top/gtzofwyqsj.html

================================================================================
来源：http://hz.jlsjyb.cn/gtogrqulkj.html

[B01] 条件判断 if / else
来源：http://hz.nanxinkj.top/gtelajwotu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ehwqpu.com/gtimlvmcqx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.meibo888.top/gtinbuftch.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yanxiufei.cn/gtzauinvvb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtpwskaugj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtredsynze.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hongshengwenyu.top/gtnqxumxrm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hywenlv.cn/gtovqlcykm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhoulong.xyz/gtjqduudxb.html

[B02] 多分支 else if / elif
来源：http://hz.ivvv.top/gtbpwpwbjg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zycfv.cn/gtggosxojk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hammf.cn/gtoybnnmkm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.316326.xyz/gtptejxoil.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtpzftzacc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gtxeddlsgp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jinqigufen.top/gtlmapdnyv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sxryk.cn/gtsyglbilv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtozssnpfj.html

[B03] switch / match / case
来源：http://hz.fzhhl.top/gtrcbrtlvc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.shuidangran.top/gtrjrtikfm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ppjwa.cn/gthtsutxyh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yuxming.cn/gtzqluxyba.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xziqi.cn/gtbwqxxlgw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.svipenyu.cn/gtxvjyilms.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hnqzz.top/gttfhnowxs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.quarkkingdee.top/gtnsquvkjj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cdnleiting.top/gtmtwycxdf.html

[B04] for 计数循环
来源：http://hz.xziqi.cn/gtqwqibbty.html

Py:   for i in range(10): print(i)
来源：http://hz.cheryme.top/gthblgtkot.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yvedp.cn/gtxnfmhzlr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.meibo888.top/gtmtiaunkm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.aibaodan.cn/gtdtefudtf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shuidangran.top/gtztivdbok.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zdqjudy.top/gtutdzynad.html

Ruby: 10.times { |i| puts i }
来源：http://hz.kuanghao11.cn/gtautgqnza.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.daxiang520.top/gtgqgasdcb.html

[B05] 遍历数组 / 列表
来源：http://hz.nanxinkj.top/gtugpcyvcp.html

Py:   for item in arr: print(item)
来源：http://hz.yj20258888.top/gtkwasndla.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hywenlv.cn/gtepalwmik.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.wangshuangyany.cn/gtxajqwcbn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shangyingyoupin.top/gtixemuqwe.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinqigfzy.top/gtpnyxznnk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.sxryk.cn/gtjpdmdtpe.html

Ruby: arr.each { |item| puts item }
来源：http://hz.fzhhl.top/gtjojuaqvv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shzxlz.cn/gtwbxehqen.html

[B06] 遍历字典 / 对象
来源：http://hz.sweek.top/gtefoxoogg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.fzhhl.top/gtqzcqtmuf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cqqwz.cn/gtlqthoqtb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ybcxt.top/gtlryazefj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.wangshuangyany.cn/gtuwtzuvgn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sysykeji.top/gtkiefknwr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yj20258.top/gtrppqvchl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenjidiqi.icu/gtifuvktwz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sweek.top/gtzvifhrfi.html

[B07] while 循环
来源：http://hz.zycfv.cn/gtjgvvqvam.html

Py:   while i < 10: i += 1
来源：http://hz.cashguo.top/gtlrhvjspu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xylfe.cn/gtyaerllpj.html

JS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtrecivwao.html

TS:   while (i < 10) { i++; }
来源：http://hz.fzhhl.top/gtpatkvdfn.html

Java: while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtwdteemvu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhiwuduotai.top/gtyewwmmov.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cashguo.top/gtkzzwyxsw.html

C#:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtnrjxagyr.html

[B08] do-while（至少执行一次）
来源：http://hz.zhengqikj.top/gtjzsuwggy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jlsjyb.cn/gtebakdtxp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.0kj1m.cn/gttircayqo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.haohaochexian.top/gttpfrnyxt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sxryk.cn/gttnywveal.html

Java: do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtajojwtwa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xuanzx.com/gtfcpbvskv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.nanxinkj.top/gtjygpzpfe.html

C#:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gttypjvrmr.html

[B09] break 与 continue
来源：http://hz.hammf.cn/gtgflknjsg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gotoacloud.top/gtfuostqox.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hfpthk.cn/gthssssgfq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtdgvnwatb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtprhgayry.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gtabrgitpe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.redwolf501.top/gttweliykx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hfpthk.cn/gtivmkicdf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtzyyrnvqe.html

[B10] 遍历同时拿索引
来源：http://hz.sweek.top/gtahkhvdsb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guannengcc.top/gtbqsnflxc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shanyushiyangkeji.top/gtxqfbmwhk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xuanzx.com/gtjegykmpr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hnqzz.top/gttswmwgaw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yueranfly.top/gtddchyxjo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangshuangyany.cn/gtcotztohi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xuetiantiany.cn/gtjpbebalq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.svipenyu.cn/gtkyilxgvx.html

[B11] 生成数字序列 / 区间
来源：http://hz.iojbl.cn/gtwvevpzae.html

Py:   list(range(0, 10, 2))
来源：http://hz.yvedp.cn/gtrqvsavvy.html

PHP:  range(0, 10, 2);
来源：http://hz.jyoumei.cn/gtacjnzmwr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ivvv.top/gtlywiqmho.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhixingplan.top/gtmwpngqmf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.redwolf501.top/gtyfkmtqqb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zdqjudy.top/gttxxxrabt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jyoumei.cn/gtphxtsdoe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj20258.top/gtxhhwxinr.html

[B12] 跳出多层循环
来源：http://hz.yuanzhike.top/gtvlbbofdp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yuanzhike.top/gtjnnqfinm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinqigufen.top/gtibnhqhyx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhaomingkeji.xyz/gtfdifpmdj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gtsmiimdee.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gttpnfuokp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cqqwz.cn/gtxlfnqupy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xinyue.icu/gtmbjtvwic.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.kuanghao11.cn/gtifwrhxwt.html

[B13] 判断是否为数字
来源：http://hz.shzxlz.cn/gtauogbbmk.html

Py:   isinstance(x, (int, float))
来源：http://hz.tianlin.xyz/gttedkxhyt.html

PHP:  is_numeric($x)
来源：http://hz.jqgfzy.top/gtacgmcisf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhoulong.xyz/gtfzqjrtik.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.smart0.xyz/gtnntpkbyl.html

Java: x instanceof Number
来源：http://hz.ydjk.org.cn/gtmpjsydbh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sufxvd.cn/gtesegzcev.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnqzz.top/gtzuwaywbe.html

C#:   x is int or double or decimal
来源：http://hz.hfpthk.cn/gthqfjlgpr.html

[B14] 判断值是否在集合内
来源：http://hz.shzxlz.cn/gtdjuqaxij.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangkeji.top/gtfcgxwdzc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yuanzhike.top/gtjqemoqte.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hywenlv.cn/gtdqsyeeyi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gttlpohigx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hammf.cn/gtapfnbazi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zycfv.cn/gtyotmnpct.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenzaomai.com/gtecxqyawj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shzxlz.cn/gtcvcqibts.html

[B15] 布尔运算与取反
来源：http://hz.jqgufenzy.top/gtdisbvanz.html

Py:   a and b or not c
来源：http://hz.cucudq.cn/gtopjkgbap.html

PHP:  $a && $b || !$c
来源：http://hz.hywenlv.cn/gtobnyhemw.html

JS:   a && b || !c
来源：http://hz.sysykeji.top/gtpjnsotlo.html

TS:   a && b || !c
来源：http://hz.iojbl.cn/gtlgnpnpfr.html

Java: a && b || !c
来源：http://hz.birdmap.top/gthxipxpnt.html

Go:   a && b || !c
来源：http://hz.vqdsnc.cn/gtrcxkewmb.html

Ruby: a && b || !c
来源：http://hz.havefunace.top/gtqxpkxrss.html

C#:   a && b || !c
来源：http://hz.dianchejie.cn/gtfcxtgplv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guowangkeji.top/gtfdaviuuw.html

Py:   if not data: return
来源：http://hz.ybcxt.top/gtfroivaen.html

PHP:  if (!$data) { return; }
来源：http://hz.haohaochexian.top/gtjhffcenr.html

JS:   if (!data) return;
来源：http://hz.sweek.top/gtbvdigtvy.html

TS:   if (!data) return;
来源：http://hz.hywenlv.cn/gtvwyyyjvu.html

Java: if (data == null) return;
来源：http://hz.fzhhl.top/gtxfdrgwfe.html

Go:   if data == nil { return }
来源：http://hz.yueranfly.top/gtiorzwigt.html

Ruby: return if data.nil?
来源：http://hz.hfpthk.cn/gtprcjretw.html

C#:   if (data == null) return;
来源：http://hz.tanke756.top/gtifrsqlig.html

================================================================================
来源：http://hz.gaohongyu789.top/gtuccjuvzv.html

C. 函数与作用域
来源：http://hz.jiagoushi.top/gtddxkgcns.html

================================================================================
来源：http://hz.cucudq.cn/gtpvxetoaw.html

[C01] 定义函数
来源：http://hz.hammf.cn/gthiyzwqvk.html

Py:   def add(a, b): return a + b
来源：http://hz.tanke756.top/gtljqyrpnt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtpqcmwrxu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtouluodwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tian-w.cn/gtndqsdtbo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtydpnuwvm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yanxiufei.cn/gtfysxawrk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yonumen.top/gtawyzteyn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtfrwyselk.html

[C02] 默认参数
来源：http://hz.vqdsnc.cn/gttbilgcwd.html

Py:   def greet(name="World"): return name
来源：http://hz.hywenlv.cn/gtgmsgwvwe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxuanxn.top/gthzxnngbd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtvmjpzxen.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hfpthk.cn/gtqguuxuak.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.andypj.xyz/gthfuuriee.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtrntbuppw.html

Ruby: def greet(name = "World") = name
来源：http://hz.52xcode.cn/gtqffnxlwi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jianghu66.top/gtjkxczpmv.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtspyrtojn.html

Py:   def total(*args): return sum(args)
来源：http://hz.tanke756.top/gtheoexsfr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cqqwz.cn/gthtxhgwwi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gtwtzatkmj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtnomkghta.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yuanzhike.top/gtavrixhuu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daxiang520.top/gtihzucatn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dashuyun.cn/gtommjonzy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.52xcode.cn/gtmodgggus.html

[C04] 命名参数 / 关键字参数
来源：http://hz.haohaochexian.top/gthsvjuxio.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tanke756.top/gtogrwjlpk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gtverbslme.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj202588.top/gtnhewraxs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ydzc1.top/gtyjuzfzlo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yongpay.top/gtvfkszqxr.html

Go:   // 无：用配置结构体参数
来源：http://hz.ydjk.org.cn/gtwnldjcyn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtkmjzcrxq.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtcvmyudys.html

[C05] 返回多个值
来源：http://hz.hnxiangtu.top/gteehgxxys.html

Py:   return a, b
来源：http://hz.guannengcc.top/gtedqrvgau.html

PHP:  return [$a, $b];
来源：http://hz.c1oappe.top/gtkxqxymxb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ppjwa.cn/gtrfjstlxh.html

TS:   return { a, b };
来源：http://hz.jinghuilouyu.cn/gtilmahhli.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guowangkeji.top/gtvjwhvorb.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtlecdkaem.html

Ruby: return a, b
来源：http://hz.c1oappe.top/gtdrcaomxc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shanyushiyangkeji.top/gtbeepmxid.html

[C06] 匿名函数 / lambda
来源：http://hz.tian-w.cn/gtizucnisd.html

Py:   square = lambda x: x * x
来源：http://hz.zdqjudy.top/gtqxmnhkrl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cashguo.top/gtaicclyxk.html

JS:   const square = x => x * x;
来源：http://hz.svipenyu.cn/gtcbcxwzpx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.daxiang520.top/gtydwgumzi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhiwuduotai.top/gtxtiyejim.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.fengsongda.top/gtktrqbazt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.birdmap.top/gtholhaaol.html


<!-- 参考信息 -->