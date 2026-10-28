代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.shanyushiyangkeji.top/gtjwelfigk.html

Py:   ord("A"); chr(65)
来源：http://hz.hnxiangtu.top/gtfvlmjnan.html

PHP:  ord("A"); chr(65)
来源：http://hz.fzhhl.top/gtlotzvmdz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shzxlz.cn/gtoixebhxr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yanxiufei.cn/gtvrjxitrj.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhiwuduotai.top/gttofvflfj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.sxryk.cn/gtldojzvdm.html

Ruby: "A".ord; 65.chr
来源：http://hz.yanxiufei.cn/gtfjrsgzsy.html

C#:   (int)'A'; (char)65
来源：http://hz.xziqi.cn/gtwdvzwpfy.html

[A19] 交换两个变量
来源：http://hz.yonumen.top/gtispadwua.html

Py:   a, b = b, a
来源：http://hz.feifeiyinyue.top/gtjmwjmqla.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.zhaomingkeji.xyz/gtxsssfpgz.html

JS:   [a, b] = [b, a];
来源：http://hz.tianlin.xyz/gtnzegvbmj.html

TS:   [a, b] = [b, a];
来源：http://hz.hywenlv.cn/gtbghpytsa.html

Java: int t = a; a = b; b = t;
来源：http://hz.c1oappe.top/gtgysrogji.html

Go:   a, b = b, a
来源：http://hz.wangdashe.top/gtmcnmbvlo.html

Ruby: a, b = b, a
来源：http://hz.ydzc1.top/gtfsyetjwi.html

C#:   (a, b) = (b, a);
来源：http://hz.316326.xyz/gtcgdvuhki.html

[A20] 读取标准输入
来源：http://hz.tian-w.cn/gthrlczlwt.html

Py:   name = input("请输入：")
来源：http://hz.sweek.top/gtpbwbiqez.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yanxiufei.cn/gtkxrsrndy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.ydjk.org.cn/gtjengydxn.html

TS:   // Node.js：readline 模块
来源：http://hz.jinqigfzy.top/gtngzjzyom.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.316326.xyz/gtrghsgwqi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jqgufenzy.top/gthlsjmqyf.html

Ruby: gets.chomp
来源：http://hz.yuanzhike.top/gthrhnhtoi.html

C#:   Console.ReadLine();
来源：http://hz.yuxming.cn/gtncmfcvpd.html

[A21] 保留指定小数位输出
来源：http://hz.andypj.xyz/gtdypkyclp.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hongshengwenyu.top/gtajedzzsx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.svipenyu.cn/gtvjjjivph.html

JS:   (3.14159).toFixed(2)
来源：http://hz.0kj1m.cn/gtmtiyjabb.html

TS:   (3.14159).toFixed(2)
来源：http://hz.mhx1999.top/gtmfwgpmtc.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yvedp.cn/gtfbvgtwew.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.guannengcc.top/gtcxylbvqg.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.iojbl.cn/gtaripkdfp.html

C#:   3.14159.ToString("F2")
来源：http://hz.sxryk.cn/gtlpcvueza.html

[A22] 获取字符串长度
来源：http://hz.snrcjt.cn/gtwketyatu.html

Py:   len(s)
来源：http://hz.hnxiangtu.top/gtprtbqqhg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xuanzx.com/gtlrvxnqye.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhengqikj.top/gtgwaquhii.html

TS:   s.length
来源：http://hz.chenjidiqi.icu/gtvcjiyobs.html

Java: s.length()
来源：http://hz.yonumen.top/gtfisfijoq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cheryme.top/gtcdlttzbz.html

Ruby: s.length
来源：http://hz.nanxinkj.top/gtdiygpxfx.html

C#:   s.Length
来源：http://hz.ppjwa.cn/gtijwxfxkv.html

[A23] 大小写转换
来源：http://hz.hammf.cn/gtmmpytgrm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jinyuanbaomall.cn/gtijiuxyux.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhengqikj.top/gtpuceajyb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.52xcode.cn/gtxwdbunst.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.meibo888.top/gtkhznvssg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yvedp.cn/gtmbnpyhqa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hnqzz.top/gtbkznhlje.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.feifeiyinyue.top/gtpnslrokb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhijiandao.cn/gtqudrrxbb.html

[A24] 去除首尾空白
来源：http://hz.ydjk.org.cn/gtnqerenpq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.daria6918.cn/gtiyyfjkxd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.bjfxy.top/gttxcrkujd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinghuilouyu.cn/gtjgoaivar.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hfpthk.cn/gtggktcyiq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.snrcjt.cn/gtulhyakhe.html

Go:   strings.TrimSpace(s)
来源：http://hz.guowangkeji.top/gtargmdhtl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jlsjyb.cn/gtykrrrlbt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hywenlv.cn/gtyikfkvde.html

[A25] 字符串比较
来源：http://hz.sufxvd.cn/gtgxymqidf.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jiagoushi.top/gttoxhfebg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.9152youxi.cn/gtaihrafnq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.pengpengdd.cyou/gtpophsydm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hammf.cn/gtoeygligd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shuidangran.top/gtvqbabsam.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.gzhubu.top/gtnlgxxbck.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.9152youxi.cn/gtandvjgjy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gogol.net.cn/gtqfxrsxes.html

[A26] 类型转换总览
来源：http://hz.pengpengdd.cyou/gthygcmdop.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shanyushiyangtech.top/gtwhepgyjj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hnqzz.top/gtkgkqmant.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hammf.cn/gtxfebnpft.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yuanzhike.top/gtvzjvawts.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.havefunace.top/gtqhsrcays.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hammf.cn/gtjldlqbhu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.quarkkingdee.top/gtmggpcfqb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.daria6918.cn/gtmpgalxaz.html

================================================================================
来源：http://hz.andypj.xyz/gtfokmzfzs.html

B. 流程控制
来源：http://hz.zhixingplan.top/gtsnvkqtph.html

================================================================================
来源：http://hz.yangfankeji.com/gtbxkloxis.html

[B01] 条件判断 if / else
来源：http://hz.cucudq.cn/gtzzfpsefh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.snrcjt.cn/gtyykqykih.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cheryme.top/gtakovyejl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtclxadgmq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gthunnzjte.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ybcxt.top/gtxvndlrwu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yongpay.top/gtmpmhyhex.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cdnleiting.top/gtinpcnfbd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhaomingkeji.xyz/gttmkodzzm.html

[B02] 多分支 else if / elif
来源：http://hz.yuanzhike.top/gtgrlfbmyf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.sysykeji.top/gtzlqcivok.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.birdmap.top/gtlsviuowi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtymnpdrvi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.redwolf501.top/gtqdslmepv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gtwrdgbnvs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jinghuilouyu.cn/gtdokmnetn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xylfe.cn/gtalwokppx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gtgrnkeyvz.html

[B03] switch / match / case
来源：http://hz.smart0.xyz/gtyaadzaim.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.tianlin.xyz/gtqdlkttks.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hywenlv.cn/gttttftxxa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xinyue.icu/gtrkvgrgmq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenjidiqi.icu/gtzggkyink.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zycfv.cn/gtukaxebxi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zdqjudy.top/gtpxtagosf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ywan-chungtsiang.top/gtnhurgqjv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhaomingkeji.xyz/gtvekpwupo.html

[B04] for 计数循环
来源：http://hz.tanke756.top/gtfqtrnytw.html

Py:   for i in range(10): print(i)
来源：http://hz.aizwys.cn/gtzqbwddqg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.bjfxy.top/gtyedsrhaz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.kuanghao11.cn/gtgnnnzllh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ppjwa.cn/gtothmweaa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.c1oappe.top/gtwzjstrck.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.daxiang520.top/gtzyyxyuzu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.c1oappe.top/gtpnokyqlo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xinyue.icu/gtqnpbmfxe.html

[B05] 遍历数组 / 列表
来源：http://hz.iojbl.cn/gthjoemeet.html

Py:   for item in arr: print(item)
来源：http://hz.hongshengwenyu.top/gtbkquwmbg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zycfv.cn/gtlygqtdmz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtoowcpwtr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtpcuulevb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shzxlz.cn/gtryjueraj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.0kj1m.cn/gtbrycjtxb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.svipenyu.cn/gtfoxsycnt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xinyue.icu/gteohkpyme.html

[B06] 遍历字典 / 对象
来源：http://hz.iojbl.cn/gtwnzzaaxy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.52xcode.cn/gtkeiyfahu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ydjk.org.cn/gtycfsczrg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jianghu66.top/gtgiqophlg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.havefunace.top/gtnquxblyu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shuidangran.top/gtwokguduv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.vqdsnc.cn/gttqfrqvvv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenjidiqi.icu/gtaxmqqbuz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ywan-chungtsiang.top/gtffvhgwqh.html

[B07] while 循环
来源：http://hz.0kj1m.cn/gtzollwpem.html

Py:   while i < 10: i += 1
来源：http://hz.nanxinkj.top/gtqxdngkbg.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.hnxiangtu.top/gtrmgzuidk.html

JS:   while (i < 10) { i++; }
来源：http://hz.aibaodan.cn/gtilnpvrqa.html

TS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtlzjhjwxj.html

Java: while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtylddqfmk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.birdmap.top/gtdqzokokz.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zycfv.cn/gtssdabluh.html

C#:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtgjieoeoc.html

[B08] do-while（至少执行一次）
来源：http://hz.hysaishi.cn/gtjpfcgkoc.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.fengsongda.top/gtaxdtelxg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.bjfxy.top/gtbahdpvvv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtlyhqewmc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtdfyqcxjy.html

Java: do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtksnjcrzt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.andypj.xyz/gtkytzfzzj.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shanyushiyangtech.top/gtuyilkhdf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gthmrmfwbz.html

[B09] break 与 continue
来源：http://hz.yangfankeji.com/gtizxebjyn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cdnleiting.top/gtzmbqmqqz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.havefunace.top/gtnuvekxzy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gtwyfblzzv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shuidangran.top/gtockacdnq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtzdjiskte.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gogol.net.cn/gtmjrtguga.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.316326.xyz/gtjszjiqxv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtyihyccob.html

[B10] 遍历同时拿索引
来源：http://hz.nwbrower.top/gtnkofchvz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yueranfly.top/gtmfbrpwxi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xinyue.icu/gtblhbscoo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtcseymcsd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dashuyun.cn/gtfpplfjsh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.gzhubu.top/gtvgcffsxv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cucudq.cn/gthgbbmpnq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.meibo888.top/gtxqafpxiu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yanxiufei.cn/gtpxugfpbg.html

[B11] 生成数字序列 / 区间
来源：http://hz.52xcode.cn/gtxzipmjqs.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhoulong.xyz/gtxgvtmgkw.html

PHP:  range(0, 10, 2);
来源：http://hz.cdnleiting.top/gtxkcbngpl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinghuilouyu.cn/gtcjuknijy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.svipenyu.cn/gtiamqnork.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ydjk.org.cn/gtbteknsaf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gtgjikglgo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenjidiqi.icu/gtfjcmdevm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cqqwz.cn/gtixycdyrv.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangtech.top/gtucpbqtxr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shanyushiyangtech.top/gttdvovkdx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhoulong.xyz/gtbaphtofw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gttaaragvu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtjgtwvyoq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gtblshogtm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jiagoushi.top/gtdriydjdk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jqgufenzy.top/gthbqytoea.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xylfe.cn/gtuvuunpqc.html

[B13] 判断是否为数字
来源：http://hz.sufxvd.cn/gtlbhpokfi.html

Py:   isinstance(x, (int, float))
来源：http://hz.yvedp.cn/gtfuwiklzc.html

PHP:  is_numeric($x)
来源：http://hz.jiagoushi.top/gtgcatphhr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yongpay.top/gtblatphmb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenzaomai.com/gtbchlzgra.html

Java: x instanceof Number
来源：http://hz.ydzc1.top/gtfoenfcpu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxinkj.top/gtvliokkat.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hfpthk.cn/gtogwzlymo.html

C#:   x is int or double or decimal
来源：http://hz.yangfankeji.com/gttzrwajfn.html

[B14] 判断值是否在集合内
来源：http://hz.hysaishi.cn/gtqgdedack.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hongshengwenyu.top/gtjogicktu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.aizwys.cn/gtdmmrqhre.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gtcdowkqes.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gtmmwyxddm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zycfv.cn/gtyyfxmrkj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shanyushiyangtech.top/gtldhkhuns.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.aibaodan.cn/gtafhrekuy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenjidiqi.icu/gtgzonvwmd.html

[B15] 布尔运算与取反
来源：http://hz.yuanzhike.top/gtipqolixs.html

Py:   a and b or not c
来源：http://hz.ywan-chungtsiang.top/gtqtuarzwh.html

PHP:  $a && $b || !$c
来源：http://hz.fengsongda.top/gtbouwjikp.html

JS:   a && b || !c
来源：http://hz.ivvv.top/gtcsizanoz.html

TS:   a && b || !c
来源：http://hz.nwbrower.top/gtyqhsiqdo.html

Java: a && b || !c
来源：http://hz.shangyingyoupin.top/gtbpilupbx.html

Go:   a && b || !c
来源：http://hz.yj20258.top/gtibmlisff.html

Ruby: a && b || !c
来源：http://hz.fengsongda.top/gtvswuuodt.html

C#:   a && b || !c
来源：http://hz.fzhhl.top/gtypjilzgx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj202588.top/gttmewihaw.html

Py:   if not data: return
来源：http://hz.ppjwa.cn/gtkpawfsru.html

PHP:  if (!$data) { return; }
来源：http://hz.sufxvd.cn/gtujaebyij.html

JS:   if (!data) return;
来源：http://hz.mhx1999.top/gtrullvzrh.html

TS:   if (!data) return;
来源：http://hz.xingfuxueyuan.xyz/gtunlzqydo.html

Java: if (data == null) return;
来源：http://hz.cheryme.top/gtkbuwkpbc.html

Go:   if data == nil { return }
来源：http://hz.mhx1999.top/gtfmdzugvj.html

Ruby: return if data.nil?
来源：http://hz.snrcjt.cn/gttfscoadl.html

C#:   if (data == null) return;
来源：http://hz.ybcxt.top/gtqxknbpbb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtdquuhwyk.html

C. 函数与作用域
来源：http://hz.yj20258888.top/gtksychxos.html

================================================================================
来源：http://hz.yonumen.top/gtinghitva.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gtuhsfmgnq.html

Py:   def add(a, b): return a + b
来源：http://hz.wangshuangyany.cn/gtqpqfbtou.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtlyenjyae.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fzhhl.top/gtewblfbuu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtcicjjaab.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtqmtcjpmc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xuanzx.com/gtvtjnscrl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daria6918.cn/gtfnlfzmtv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtnsonsckx.html

[C02] 默认参数
来源：http://hz.jinghuilouyu.cn/gtgljptnfp.html

Py:   def greet(name="World"): return name
来源：http://hz.chenjidiqi.icu/gtsjndpxxp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yongpay.top/gtorhwprxy.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjfxy.top/gtkxfkrboh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtxzvyvzfj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.daxiang520.top/gtzihczzad.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.fzhhl.top/gtgrtzjtqb.html

Ruby: def greet(name = "World") = name
来源：http://hz.jyoumei.cn/gtorvylkxp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gogol.net.cn/gtgrhxkpxq.html

[C03] 可变参数
来源：http://hz.yuxming.cn/gtziwpuhyq.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuetiantiany.cn/gtuujsfcfg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.havefunace.top/gtlabadmim.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gtihnsyily.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xziqi.cn/gtasthlndq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtuefwytmd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnxiangtu.top/gthlmfjxfk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xziqi.cn/gtnxzlphum.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgfzy.top/gtradrkayg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.nanxinkj.top/gtscrjebyf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj20258.top/gtowgyhnri.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.svipenyu.cn/gtfjgmwfvt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gtabwicpin.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nanxinkj.top/gttmeyvmsb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuanzhike.top/gttyhgwjgz.html

Go:   // 无：用配置结构体参数
来源：http://hz.shuidangran.top/gtoyelvzsp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtomlokqhj.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtrpwkqlvk.html

[C05] 返回多个值
来源：http://hz.hnxiangtu.top/gtmnbkxing.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtkxelwfse.html

PHP:  return [$a, $b];
来源：http://hz.ppjwa.cn/gtbzmndala.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.9152youxi.cn/gtzzdmlqsn.html

TS:   return { a, b };
来源：http://hz.meibo888.top/gtdnsbfogy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gtbgicljai.html

Go:   return a, b
来源：http://hz.gaohongyu789.top/gtrqlgnlde.html

Ruby: return a, b
来源：http://hz.ybcxt.top/gthtkmhklu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.daria6918.cn/gtsnoaqeoe.html

[C06] 匿名函数 / lambda
来源：http://hz.ydzc1.top/gtlpoikust.html

Py:   square = lambda x: x * x
来源：http://hz.havefunace.top/gtezuhujdh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hywenlv.cn/gtoebvpbwi.html

JS:   const square = x => x * x;
来源：http://hz.hongshengwenyu.top/gthkgmeean.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.0kj1m.cn/gtagyneeaf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yongpay.top/gtwdfjewgf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cucudq.cn/gtvgjzyahv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xylfe.cn/gtryculoph.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gteisfmikh.html

[C07] 把函数作为参数传入
来源：http://hz.yongpay.top/gtwuvmrxke.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tanke756.top/gttdibucnz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gaohongyu789.top/gtigaldxpw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhixingplan.top/gtqhoqvnoy.html

TS:   arr.map(String)
来源：http://hz.nanxuanxn.top/gtxrdxqhms.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guannengcc.top/gtudkmepxt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhengqikj.top/gtkrycwjdm.html

Ruby: arr.map(&:upcase)
来源：http://hz.xuetiantiany.cn/gtztqctyxd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jlsjyb.cn/gtwfhalwqh.html

[C08] 闭包
来源：http://hz.cqqwz.cn/gtkwhnfhfj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.dashuyun.cn/gtkppnsoao.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.9152youxi.cn/gthfquakph.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtfzgnrcyo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtleepgohr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jyoumei.cn/gtemafpxvw.html


<!-- 参考信息 -->