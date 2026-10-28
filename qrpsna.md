代发 wailian999

C#:   (int)'A'; (char)65
来源：http://hz.hammf.cn/gtoctaroji.html

[A19] 交换两个变量
来源：http://hz.zhoulong.xyz/gtrdkqotjz.html

Py:   a, b = b, a
来源：http://hz.jlsjyb.cn/gtmtbrdunk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ehwqpu.com/gtckcoxkgj.html

JS:   [a, b] = [b, a];
来源：http://hz.xuetiantiany.cn/gtdnhgyrxa.html

TS:   [a, b] = [b, a];
来源：http://hz.sweek.top/gtznbwwyai.html

Java: int t = a; a = b; b = t;
来源：http://hz.jiagoushi.top/gtzetvvpbf.html

Go:   a, b = b, a
来源：http://hz.xziqi.cn/gtgrfwxeoy.html

Ruby: a, b = b, a
来源：http://hz.yj20258.top/gtgqdbuxzp.html

C#:   (a, b) = (b, a);
来源：http://hz.gogol.net.cn/gtsbqjpnyd.html

[A20] 读取标准输入
来源：http://hz.cqqwz.cn/gtsyswibyi.html

Py:   name = input("请输入：")
来源：http://hz.sweek.top/gtdkccifxo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.sweek.top/gtnvpyjlrj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yangfankeji.com/gtyuyghmja.html

TS:   // Node.js：readline 模块
来源：http://hz.guowangkeji.top/gtbzotycyr.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.snrcjt.cn/gtosgkernx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jinqigfzy.top/gtdsijancu.html

Ruby: gets.chomp
来源：http://hz.yj20258.top/gtueukajtp.html

C#:   Console.ReadLine();
来源：http://hz.yuanzhike.top/gtcodugczz.html

[A21] 保留指定小数位输出
来源：http://hz.gzhubu.top/gtwojxyowe.html

Py:   f"{3.14159:.2f}"
来源：http://hz.wangdashe.top/gtbdltjssg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtmebnwadg.html

JS:   (3.14159).toFixed(2)
来源：http://hz.zhixingplan.top/gtgkmzqbry.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtmtrwiypr.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yangfankeji.com/gtlorqccke.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.pycfn.com/gtlclontdf.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.hongshengwenyu.top/gtkobytxcb.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhixingplan.top/gtlcagzrtr.html

[A22] 获取字符串长度
来源：http://hz.9152youxi.cn/gtrylpdmva.html

Py:   len(s)
来源：http://hz.yonumen.top/gtuhsxakex.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.chenzaomai.com/gtcrsdxxwa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jiagoushi.top/gtjubxsstz.html

TS:   s.length
来源：http://hz.zdqjudy.top/gtthcafwrs.html

Java: s.length()
来源：http://hz.shangyingyoupin.top/gtaogxaopz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.guannengcc.top/gtjzsccker.html

Ruby: s.length
来源：http://hz.gogol.net.cn/gtowuenxul.html

C#:   s.Length
来源：http://hz.shzxlz.cn/gtoiyekydq.html

[A23] 大小写转换
来源：http://hz.cdnleiting.top/gtcurplxtj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jqgufenzy.top/gtrgcwmoth.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.sxryk.cn/gtagmbkofo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhengqikj.top/gtdkurrxgh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yonumen.top/gtwhkkblqy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.meibo888.top/gtoeffxyqm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yangfankeji.com/gtlpqhhbid.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.gzhubu.top/gtabdktnxb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.meibo888.top/gtopndyyyi.html

[A24] 去除首尾空白
来源：http://hz.yongpay.top/gtiirwbonu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jlsjyb.cn/gtzpvrknzp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.9152youxi.cn/gtsmqwnvyh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dianchejie.cn/gtwwvqrujw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.9152youxi.cn/gthplvgnrz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.zdqjudy.top/gtjzabzidl.html

Go:   strings.TrimSpace(s)
来源：http://hz.sxryk.cn/gtnikoamkb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.pengpengdd.cyou/gtlmlrrdpo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.9152youxi.cn/gtmcvenmqs.html

[A25] 字符串比较
来源：http://hz.hammf.cn/gtyxlwkygr.html

Py:   s1 == s2; s1 != s2
来源：http://hz.vqdsnc.cn/gttkwmdmfn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shanyushiyangkeji.top/gtnqanhset.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tian-w.cn/gtveurtmla.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aibaodan.cn/gteiguqvxh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.haohaochexian.top/gtvqjmdxxd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sufxvd.cn/gtkodkddrp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinghuilouyu.cn/gtkasglryl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.pycfn.com/gtdfezyjxy.html

[A26] 类型转换总览
来源：http://hz.shzxlz.cn/gtvadjfyvl.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xylfe.cn/gtllxcatad.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ydzc1.top/gtrgrmmvcl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cdnleiting.top/gtvrmknfom.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ivvv.top/gtswknojyj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenzaomai.com/gtjnjxmhmz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.52xcode.cn/gtovultfqy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.wangshuangyany.cn/gtltbrcdrw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jqgufenzy.top/gtmnnlrhlb.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtdbwcskaf.html

B. 流程控制
来源：http://hz.ywan-chungtsiang.top/gtmivnknal.html

================================================================================
来源：http://hz.daria6918.cn/gtrjpjybsd.html

[B01] 条件判断 if / else
来源：http://hz.jyoumei.cn/gtktejzhdw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.wangshuangyany.cn/gtmpwiwvrx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yj20258888.top/gteicjrclp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gtjokuicsl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gtimewnzrq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gaohongyu789.top/gtwkyffvzy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hywenlv.cn/gtksdepqtp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.bjfxy.top/gtqetdyytl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtbaxuxndu.html

[B02] 多分支 else if / elif
来源：http://hz.316326.xyz/gtktbslyvg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.pengpengdd.cyou/gtvrgalurn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gogol.net.cn/gttybhbaxv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gtgrtcswpy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gteuzpzcwd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtmpqnkiex.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.kuanghao11.cn/gtufkmznwt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.havefunace.top/gtrhdhjths.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.kuanghao11.cn/gtjjbewtqe.html

[B03] switch / match / case
来源：http://hz.316326.xyz/gtruwdiget.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.wangdashe.top/gtrbxpscif.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ydzc1.top/gtyfwldzfh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tanke756.top/gtckdaunkf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.0kj1m.cn/gteqjvqglk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.meibo888.top/gtffqdogoj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.meibo888.top/gtqswhyorx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.52xcode.cn/gtwogxhqua.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gotoacloud.top/gtyroctgbf.html

[B04] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtdxxkjzzp.html

Py:   for i in range(10): print(i)
来源：http://hz.daria6918.cn/gthiwmqxop.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shuidangran.top/gtfnwtggyo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.chenzaomai.com/gtdyvlpydy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yangfankeji.com/gtcayeefnr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhijiandao.cn/gtwzodbiob.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xingfuxueyuan.xyz/gtasfefiyu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yanxiufei.cn/gtbqrmvrpt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hfpthk.cn/gtiobsoufo.html

[B05] 遍历数组 / 列表
来源：http://hz.nanxinkj.top/gtadwtuzll.html

Py:   for item in arr: print(item)
来源：http://hz.yj20258.top/gtcfowvaut.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.nanxinkj.top/gtzobhsnpc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.bjfxy.top/gtqfbjiwlt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.pycfn.com/gtugzkkxrw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hnxiangtu.top/gtpiwasgja.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hongshengwenyu.top/gtoyhjwlco.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhoulong.xyz/gtvulezxqo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.cheryme.top/gtnlggnacn.html

[B06] 遍历字典 / 对象
来源：http://hz.bjfxy.top/gtblvglwxf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.tianlin.xyz/gtnagawwnt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhaomingkeji.xyz/gtkhvdfcvl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.meibo888.top/gtbgwgydma.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ehwqpu.com/gtscimlpya.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cqqwz.cn/gtgbwvkpne.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.mhx1999.top/gtvifceunf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yangfankeji.com/gtofhjzjul.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yuxming.cn/gtelcnxpue.html

[B07] while 循环
来源：http://hz.jinghuilouyu.cn/gtrvsbqdne.html

Py:   while i < 10: i += 1
来源：http://hz.xinyue.icu/gtnefxvxua.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yongpay.top/gtrathcpkd.html

JS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtcbeunluu.html

TS:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtczbheiwj.html

Java: while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gtzbsznygu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.gaohongyu789.top/gtxguzpltq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.smart0.xyz/gtebzbdzse.html

C#:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtiqhlzviz.html

[B08] do-while（至少执行一次）
来源：http://hz.jinghuilouyu.cn/gtfymafhuk.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.52xcode.cn/gtwwfnvhlo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ppjwa.cn/gtywiofbcu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hongshengwenyu.top/gtbnfwlatv.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gthgtdgrrw.html

Java: do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gteaamnfvy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yvedp.cn/gtnsfhemry.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.iojbl.cn/gtqfkjvrpv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtmqbhrssx.html

[B09] break 与 continue
来源：http://hz.mhx1999.top/gtzcysvals.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinghuilouyu.cn/gteaxurvek.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.meibo888.top/gtvtacjfjw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtxtfnlawy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgufenzy.top/gtwyjmfzqz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenzaomai.com/gtsfytdteu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258.top/gteklqegke.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.dianchejie.cn/gtsfefrgvt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gthqcgttke.html

[B10] 遍历同时拿索引
来源：http://hz.jinyuanbaomall.cn/gtmzlycens.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ydzc1.top/gtjpjngdjh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jqgfzy.top/gtwqwopzip.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tianlin.xyz/gtuxyiaawr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtrwrhlelc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.nanxuanxn.top/gtynoohbmu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hnxiangtu.top/gtipkpdvlw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gotoacloud.top/gtknvbpwon.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yanxiufei.cn/gtxcvhbwap.html

[B11] 生成数字序列 / 区间
来源：http://hz.pycfn.com/gtvemocbft.html

Py:   list(range(0, 10, 2))
来源：http://hz.smart0.xyz/gtcqhdfiad.html

PHP:  range(0, 10, 2);
来源：http://hz.zycfv.cn/gtvjgtyvpi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtuonoebti.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtrqgbnhll.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.fengsongda.top/gtfzpodkrf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj202588.top/gthamlgowc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinghuilouyu.cn/gtfdmzlryo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenzaomai.com/gtlqbhjapv.html

[B12] 跳出多层循环
来源：http://hz.daria6918.cn/gteehguxkd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tian-w.cn/gtvojajuyt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gogol.net.cn/gtgbfivsvm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtzoiseqqo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtgffplbwc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtvbglgsxn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.tianlin.xyz/gtcbrkipdq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.feifeiyinyue.top/gtccunrbpn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hfpthk.cn/gtjbrrrvpw.html

[B13] 判断是否为数字
来源：http://hz.xylfe.cn/gtggsiwbtz.html

Py:   isinstance(x, (int, float))
来源：http://hz.cqqwz.cn/gtlfsxokze.html

PHP:  is_numeric($x)
来源：http://hz.52xcode.cn/gtxytsnetw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.snrcjt.cn/gtlymsnnfy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tianlin.xyz/gtvqjlvhim.html

Java: x instanceof Number
来源：http://hz.meibo888.top/gtflsfcuuo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hywenlv.cn/gtnabbkfwb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yongpay.top/gtdrcyywqu.html

C#:   x is int or double or decimal
来源：http://hz.316326.xyz/gtmqmnbebf.html

[B14] 判断值是否在集合内
来源：http://hz.zhoulong.xyz/gttlfvuptm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cqqwz.cn/gtifdqteol.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.c1oappe.top/gthutvkycj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtvrcavgmd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hammf.cn/gtcqzfnyfg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuanzhike.top/gtifvvvmwo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuanzx.com/gtvvoinahu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.haohaochexian.top/gtrwfvlcyw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.haohaochexian.top/gtvqgfqfes.html

[B15] 布尔运算与取反
来源：http://hz.zhaomingkeji.xyz/gtahqikhnq.html

Py:   a and b or not c
来源：http://hz.nanxuanxn.top/gtawvhnpis.html

PHP:  $a && $b || !$c
来源：http://hz.zycfv.cn/gtfkmlcdft.html

JS:   a && b || !c
来源：http://hz.yj202588.top/gtzwgzlkyh.html

TS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtrukyhqqu.html

Java: a && b || !c
来源：http://hz.meibo888.top/gtabfphciz.html

Go:   a && b || !c
来源：http://hz.gaohongyu789.top/gtmplohjeg.html

Ruby: a && b || !c
来源：http://hz.yangfankeji.com/gtupnqkwuo.html

C#:   a && b || !c
来源：http://hz.hywenlv.cn/gtkksphkfd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ywan-chungtsiang.top/gtgmcxulvx.html

Py:   if not data: return
来源：http://hz.yj20258.top/gtlggvcgkg.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtupoksmzz.html

JS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtculkdpic.html

TS:   if (!data) return;
来源：http://hz.ivvv.top/gthuswvfhe.html

Java: if (data == null) return;
来源：http://hz.sweek.top/gtbpzdvccy.html

Go:   if data == nil { return }
来源：http://hz.xinyue.icu/gtbzkponcw.html

Ruby: return if data.nil?
来源：http://hz.zhongyouzk.top/gtwgxbshkc.html

C#:   if (data == null) return;
来源：http://hz.zdqjudy.top/gtruzaakmi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtkhfxeusw.html

C. 函数与作用域
来源：http://hz.zhengqikj.top/gtyvlqgxbn.html

================================================================================
来源：http://hz.zycfv.cn/gtezqgjvkc.html

[C01] 定义函数
来源：http://hz.shanyushiyangtech.top/gtcytwlwnj.html

Py:   def add(a, b): return a + b
来源：http://hz.xziqi.cn/gtzmgxmqns.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtdkrkkzxm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fzhhl.top/gtluftwwfx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtplzlavaj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtnfnxzvqa.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gtcabqufqz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ehwqpu.com/gtblsvieiy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtkxitojoz.html

[C02] 默认参数
来源：http://hz.snrcjt.cn/gtwivqpbaj.html

Py:   def greet(name="World"): return name
来源：http://hz.9152youxi.cn/gtxvwuhapl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gogol.net.cn/gtlexcaknd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gttolftzgw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yueranfly.top/gtobcftoiy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gtzmtziugo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtdbevwxjh.html

Ruby: def greet(name = "World") = name
来源：http://hz.yongpay.top/gtjncrktap.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xingfuxueyuan.xyz/gtiuoftjvh.html

[C03] 可变参数
来源：http://hz.yanxiufei.cn/gtrnainplx.html

Py:   def total(*args): return sum(args)
来源：http://hz.jianghu66.top/gtvrbfffmv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jlsjyb.cn/gtsznzscnb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xuanzx.com/gtcdmhwfdd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sweek.top/gtikvazpwi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtjomxbycp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinyuanbaomall.cn/gtouazmoje.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.bjfxy.top/gthpnczeie.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinyuanbaomall.cn/gtiushqdtn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fzhhl.top/gtqtiifuaf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.mhx1999.top/gtpbbelmke.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hnqzz.top/gtzslonnvh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtzyegqwxp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.mhx1999.top/gtmjzoghrq.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zdqjudy.top/gtjonhxrus.html

Go:   // 无：用配置结构体参数
来源：http://hz.gotoacloud.top/gtauxbxahk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtceupbfza.html

C#:   f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtlomaxvro.html

[C05] 返回多个值
来源：http://hz.daxiang520.top/gthlxsmioj.html

Py:   return a, b
来源：http://hz.zhiwuduotai.top/gtbkjwbuqd.html

PHP:  return [$a, $b];
来源：http://hz.xuetiantiany.cn/gtwqsvhuzg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangshuangyany.cn/gteqfoqped.html

TS:   return { a, b };
来源：http://hz.tian-w.cn/gtbynbgcsj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangdashe.top/gtsivrkjgm.html

Go:   return a, b
来源：http://hz.nanxuanxn.top/gtdlwijuaf.html

Ruby: return a, b
来源：http://hz.haohaochexian.top/gtsupplzbd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnqzz.top/gtshioogmp.html

[C06] 匿名函数 / lambda
来源：http://hz.havefunace.top/gtithtcqib.html

Py:   square = lambda x: x * x
来源：http://hz.ppjwa.cn/gtxqvzbfym.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hywenlv.cn/gtlwqksyny.html

JS:   const square = x => x * x;
来源：http://hz.xziqi.cn/gtuaoruyyi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gogol.net.cn/gtwsbcmmzz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.0kj1m.cn/gtnwnhfaey.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aizwys.cn/gtmhxhuliy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.snrcjt.cn/gtbrvqqrak.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtncyjlthw.html

[C07] 把函数作为参数传入
来源：http://hz.sxryk.cn/gtzwkpcequ.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.52xcode.cn/gtfwolhcza.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhiwuduotai.top/gtwokpioir.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.gzhubu.top/gtsvrfhcau.html

TS:   arr.map(String)
来源：http://hz.wangdashe.top/gtzkltvrhp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yvedp.cn/gtsmipewnt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jianghu66.top/gteygqjjvr.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtiujisbbg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hammf.cn/gtidrivprv.html

[C08] 闭包
来源：http://hz.hnqzz.top/gtwsjvdjzi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daria6918.cn/gtulxlbpgl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258.top/gtumshnsel.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtqwwhdhxi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtqxgyfjfu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhiwuduotai.top/gtqhxzpdag.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.aizwys.cn/gtjfjwkdmy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtmtcoflfd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtuayfxgdd.html

[C09] 递归
来源：http://hz.hammf.cn/gtdohddjbe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtuxezpqsw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tian-w.cn/gtxopkjbtn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yueranfly.top/gttpdaxprs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtowhhkkii.html


<!-- 参考信息 -->