代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.jinyuanbaomall.cn/gthaibupql.html

Py:   ord("A"); chr(65)
来源：http://hz.nanxinkj.top/gtwklbwwzj.html

PHP:  ord("A"); chr(65)
来源：http://hz.chenjidiqi.icu/gtyzccxwoz.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hfpthk.cn/gtwdjaxbmp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ywan-chungtsiang.top/gtyyiqhyem.html

Java: (int) 'A'; (char) 65
来源：http://hz.yj202588.top/gtweeukkqj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.xinyue.icu/gtzxjwunnu.html

Ruby: "A".ord; 65.chr
来源：http://hz.hywenlv.cn/gttmqlacww.html

C#:   (int)'A'; (char)65
来源：http://hz.dashuyun.cn/gtfgdmgaxq.html

[A19] 交换两个变量
来源：http://hz.cashguo.top/gtmdveyphg.html

Py:   a, b = b, a
来源：http://hz.hnxiangtu.top/gtuztchtqh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shuidangran.top/gtcestavfn.html

JS:   [a, b] = [b, a];
来源：http://hz.jiagoushi.top/gtrtsvnzad.html

TS:   [a, b] = [b, a];
来源：http://hz.nwbrower.top/gtnouyvehl.html

Java: int t = a; a = b; b = t;
来源：http://hz.jinyuanbaomall.cn/gtzcobgpwn.html

Go:   a, b = b, a
来源：http://hz.yueranfly.top/gtcxlbkusf.html

Ruby: a, b = b, a
来源：http://hz.zhixingplan.top/gtiyfkkmci.html

C#:   (a, b) = (b, a);
来源：http://hz.sweek.top/gtkwtnvomx.html

[A20] 读取标准输入
来源：http://hz.ydjk.org.cn/gtfiijkkqa.html

Py:   name = input("请输入：")
来源：http://hz.guowangkeji.top/gtbxhrcljv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.zycfv.cn/gtypmlnece.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xziqi.cn/gtmidjbvow.html

TS:   // Node.js：readline 模块
来源：http://hz.ivvv.top/gtsxiriphu.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.havefunace.top/gteeewjqae.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.gogol.net.cn/gtumsfcvjz.html

Ruby: gets.chomp
来源：http://hz.shanyushiyangtech.top/gtkyysiahw.html

C#:   Console.ReadLine();
来源：http://hz.guannengcc.top/gtgbsbqmuc.html

[A21] 保留指定小数位输出
来源：http://hz.sufxvd.cn/gtjapyfxei.html

Py:   f"{3.14159:.2f}"
来源：http://hz.daxiang520.top/gtgelegzub.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zhaomingkeji.xyz/gtectgslqx.html

JS:   (3.14159).toFixed(2)
来源：http://hz.xuanzx.com/gtmjdrkjec.html

TS:   (3.14159).toFixed(2)
来源：http://hz.hnqzz.top/gthvqznsdf.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.haohaochexian.top/gtyotznjwf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hfpthk.cn/gtdfinpxyg.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtvthasmtt.html

C#:   3.14159.ToString("F2")
来源：http://hz.hywenlv.cn/gtcfwtygvq.html

[A22] 获取字符串长度
来源：http://hz.pycfn.com/gtsqsugrao.html

Py:   len(s)
来源：http://hz.cucudq.cn/gtkmakihqd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xuetiantiany.cn/gtkaxwjmjr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhengqikj.top/gtyyejhlfc.html

TS:   s.length
来源：http://hz.jianghu66.top/gtmzemnzun.html

Java: s.length()
来源：http://hz.yongpay.top/gtpaisurgn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.shzxlz.cn/gtnsnqqdgw.html

Ruby: s.length
来源：http://hz.havefunace.top/gtcrohsekm.html

C#:   s.Length
来源：http://hz.zhaomingkeji.xyz/gtqclttsix.html

[A23] 大小写转换
来源：http://hz.tianlin.xyz/gtcrnhqcph.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zhoulong.xyz/gtqbxxhxqm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.kuanghao11.cn/gtrzgbpwpo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.wangshuangyany.cn/gtnxczqygr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.9152youxi.cn/gtjxjjubke.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.ehwqpu.com/gthynjzkfc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ivvv.top/gtppxumykh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.wangdashe.top/gtrgmetupa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yvedp.cn/gtmycamygf.html

[A24] 去除首尾空白
来源：http://hz.cqqwz.cn/gtoyikgswt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.guannengcc.top/gtfucsppml.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ivvv.top/gtmqklnbdz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.bjfxy.top/gtxlwovysv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gzhubu.top/gtlljiatll.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.cheryme.top/gtxotasvzj.html

Go:   strings.TrimSpace(s)
来源：http://hz.svipenyu.cn/gtwownfkjt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.pycfn.com/gtdxyzxpaj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.nanxuanxn.top/gtxlhewjhp.html

[A25] 字符串比较
来源：http://hz.gaohongyu789.top/gtljohtbka.html

Py:   s1 == s2; s1 != s2
来源：http://hz.guannengcc.top/gtotnywrni.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.quarkkingdee.top/gtdkbidsev.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hywenlv.cn/gtweuapuyp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sysykeji.top/gtifsjzfll.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yuxming.cn/gthuclqtrj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.chenjidiqi.icu/gtludamyhz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.nanxuanxn.top/gtwnnyanch.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.daxiang520.top/gtnvphdtee.html

[A26] 类型转换总览
来源：http://hz.svipenyu.cn/gtpzdeggfj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hnxiangtu.top/gtqnwwveiw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.redwolf501.top/gttqzbhyyu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xylfe.cn/gtxersslvy.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sufxvd.cn/gtaecpuxir.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ydjk.org.cn/gttjzokejl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.svipenyu.cn/gtumykigks.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jqgfzy.top/gtyeprxgxo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.andypj.xyz/gtkfmhohcb.html

================================================================================
来源：http://hz.jianghu66.top/gteabsckmk.html

B. 流程控制
来源：http://hz.quarkkingdee.top/gtzmfvqyrt.html

================================================================================
来源：http://hz.zhongyouzk.top/gtevsknzxo.html

[B01] 条件判断 if / else
来源：http://hz.zhengqikj.top/gtixzehuco.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ywan-chungtsiang.top/gtktibtamq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ppjwa.cn/gtdvuutujw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fengsongda.top/gtaqrvutso.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cucudq.cn/gtwcyebnsq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xziqi.cn/gtiuswwdyt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.pycfn.com/gtitphfnbo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yueranfly.top/gtydamlpbj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hysaishi.cn/gtqyhogzmx.html

[B02] 多分支 else if / elif
来源：http://hz.aizwys.cn/gtcqhxqbzk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.pengpengdd.cyou/gtzcumapgi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xuetiantiany.cn/gtijcceyxs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gtzjhfrwzm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtzkjdvmhf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghu66.top/gtluugjdnm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ydjk.org.cn/gtndslyjng.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yonumen.top/gthxaehthw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jyoumei.cn/gtpfmewdbg.html

[B03] switch / match / case
来源：http://hz.tianlin.xyz/gthoxilzzd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.shzxlz.cn/gtbscppcoo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jlsjyb.cn/gtdrhagtdf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jiagoushi.top/gtfkapkcrc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daxiang520.top/gtcizlvswf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cucudq.cn/gtwclpmqjh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.xinyue.icu/gtqlucvmym.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenlongwang.top/gtkyjhqeab.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.guannengcc.top/gtzwrhchrq.html

[B04] for 计数循环
来源：http://hz.yj20258888.top/gtwintvrif.html

Py:   for i in range(10): print(i)
来源：http://hz.kuanghao11.cn/gtmbxnlniw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yonumen.top/gtdpemitrv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xylfe.cn/gthvlimzbw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.snrcjt.cn/gtjnlfyvuq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yj202588.top/gtuovtpqjd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.sufxvd.cn/gtvvxoinli.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhixingplan.top/gtyakzxide.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.sysykeji.top/gtgqkgguyo.html

[B05] 遍历数组 / 列表
来源：http://hz.hongshengwenyu.top/gtufcczmyn.html

Py:   for item in arr: print(item)
来源：http://hz.yuanzhike.top/gtlsuzskzq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jianghu66.top/gtobwfwzrk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj20258888.top/gtcpilnfkw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.c1oappe.top/gtvmsriozi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.kuanghao11.cn/gtqkhpvcks.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cheryme.top/gtlcnvinuj.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yuxming.cn/gtefgsfjap.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gogol.net.cn/gtqgucuxio.html

[B06] 遍历字典 / 对象
来源：http://hz.cashguo.top/gtdgosqqzl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.meibo888.top/gtzpxtbyum.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinqigfzy.top/gtnfhrzodm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fengsongda.top/gttzjqfser.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuetiantiany.cn/gtgawkyzvd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.svipenyu.cn/gthffkuvcf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sxryk.cn/gtzevkqkya.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.andypj.xyz/gtiryboqsh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hongshengwenyu.top/gtmlmluvcz.html

[B07] while 循环
来源：http://hz.xylfe.cn/gtrtowvjhp.html

Py:   while i < 10: i += 1
来源：http://hz.hammf.cn/gtlgoxxcll.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jlsjyb.cn/gtmlwpeexf.html

JS:   while (i < 10) { i++; }
来源：http://hz.dashuyun.cn/gtrdxwkmsa.html

TS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gttvnheucv.html

Java: while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtipvlmzmm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tianlin.xyz/gtwfyqmuhl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.sxryk.cn/gtyigczlfh.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtruydlflo.html

[B08] do-while（至少执行一次）
来源：http://hz.hywenlv.cn/gttieuhsrq.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj20258888.top/gttcxzoduu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yuanzhike.top/gtjjbxdfzj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtwnmmqnjd.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtqbnfebhp.html

Java: do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gtmcfepbfv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.havefunace.top/gtryicapfd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.dianchejie.cn/gtsugilpzp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtdenqnyts.html

[B09] break 与 continue
来源：http://hz.zhoulong.xyz/gtcegkdfwe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xylfe.cn/gtzcvnqfpg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hammf.cn/gtpooewtpr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtgjmcyrmb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtyqcesirq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtkfyfflmf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.52xcode.cn/gtxpwvyluy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cdnleiting.top/gtmsnrtxpg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtelyhfyua.html

[B10] 遍历同时拿索引
来源：http://hz.sweek.top/gteuwfckvj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jlsjyb.cn/gtjuqbqkzx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.birdmap.top/gtxfzznfct.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hnqzz.top/gtbfuweeyr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtbixngxku.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hywenlv.cn/gtujfgapft.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yangfankeji.com/gtjtnemgnj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.svipenyu.cn/gtblrrsrsq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.mhx1999.top/gtylicadli.html

[B11] 生成数字序列 / 区间
来源：http://hz.dashuyun.cn/gtxyobmdsy.html

Py:   list(range(0, 10, 2))
来源：http://hz.cheryme.top/gtisyhvxqv.html

PHP:  range(0, 10, 2);
来源：http://hz.yuanzhike.top/gtwospowhu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zycfv.cn/gtlhddutjv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj202588.top/gtqkalvvfv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenzaomai.com/gtdipaxymi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinyuanbaomall.cn/gtsjlowufl.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangtech.top/gtldotaohv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.pengpengdd.cyou/gtsvywzvbp.html

[B12] 跳出多层循环
来源：http://hz.haohaochexian.top/gtoiloajwf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.aibaodan.cn/gtdlearnmp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guannengcc.top/gtuddoaigz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtzugkkowb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhaomingkeji.xyz/gtivfmxbec.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gttutxuhhv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.wangdashe.top/gtjxbpasmy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zdqjudy.top/gtdawfdryz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gotoacloud.top/gtwgywzntz.html

[B13] 判断是否为数字
来源：http://hz.gogol.net.cn/gtqdhayfth.html

Py:   isinstance(x, (int, float))
来源：http://hz.guowangkeji.top/gtknoofcoo.html

PHP:  is_numeric($x)
来源：http://hz.xziqi.cn/gtbxbxsphb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhiwuduotai.top/gtcipidcrr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xinyue.icu/gtcitnrqpb.html

Java: x instanceof Number
来源：http://hz.aibaodan.cn/gtdxvzqmik.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hammf.cn/gtzhjelmoq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnxiangtu.top/gtoevsozbc.html

C#:   x is int or double or decimal
来源：http://hz.vqdsnc.cn/gtmrmzquht.html

[B14] 判断值是否在集合内
来源：http://hz.cqqwz.cn/gtlkdonrfc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.iojbl.cn/gthabafdhw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hysaishi.cn/gtbsewdcth.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.daria6918.cn/gtdjmejspg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtcmkvwdnk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gtgozwnqor.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gotoacloud.top/gtdkbyqgcs.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jqgufenzy.top/gtykszckji.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.mhx1999.top/gtalzrwnnj.html

[B15] 布尔运算与取反
来源：http://hz.ydjk.org.cn/gtzqpfhkbg.html

Py:   a and b or not c
来源：http://hz.cdnleiting.top/gtradpuijb.html

PHP:  $a && $b || !$c
来源：http://hz.yueranfly.top/gtzocripoj.html

JS:   a && b || !c
来源：http://hz.cdnleiting.top/gtsyijuqpm.html

TS:   a && b || !c
来源：http://hz.zhixingplan.top/gtsepvgojz.html

Java: a && b || !c
来源：http://hz.jlsjyb.cn/gtaxwnsvgb.html

Go:   a && b || !c
来源：http://hz.mhx1999.top/gteklkovtz.html

Ruby: a && b || !c
来源：http://hz.zhiwuduotai.top/gtpnceehns.html

C#:   a && b || !c
来源：http://hz.zhongyouzk.top/gtcjchkpso.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigufen.top/gtbsyqxrju.html

Py:   if not data: return
来源：http://hz.svipenyu.cn/gtpksvfgcg.html

PHP:  if (!$data) { return; }
来源：http://hz.daria6918.cn/gtrnzhqpth.html

JS:   if (!data) return;
来源：http://hz.jqgfzy.top/gtgieimlco.html

TS:   if (!data) return;
来源：http://hz.iojbl.cn/gtkqgfgcof.html

Java: if (data == null) return;
来源：http://hz.zhengqikj.top/gtiouqebfy.html

Go:   if data == nil { return }
来源：http://hz.shanyushiyangtech.top/gtsfghfhsw.html

Ruby: return if data.nil?
来源：http://hz.sufxvd.cn/gtbqptbdeo.html

C#:   if (data == null) return;
来源：http://hz.gotoacloud.top/gtqcoabksk.html

================================================================================
来源：http://hz.yuanzhike.top/gttceaklvp.html

C. 函数与作用域
来源：http://hz.zhoulong.xyz/gteoanqsvx.html

================================================================================
来源：http://hz.aibaodan.cn/gtgqdjoibl.html

[C01] 定义函数
来源：http://hz.fzhhl.top/gtdqeifzmw.html

Py:   def add(a, b): return a + b
来源：http://hz.sxryk.cn/gtogykogtf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtyswofuyd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.0kj1m.cn/gtbtryrvsu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtdsjpqzov.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gteggkedjg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gtcwmhnyiq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cdnleiting.top/gtgpcgofmc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtmqwpqztt.html

[C02] 默认参数
来源：http://hz.shangyingyoupin.top/gtadezjoce.html

Py:   def greet(name="World"): return name
来源：http://hz.tanke756.top/gtgxiiadkr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ppjwa.cn/gtgbbbeiyk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuanzx.com/gtzvefzval.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.wangdashe.top/gtzhgphpgi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.mhx1999.top/gtrnjstssz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xziqi.cn/gtduqfmsgr.html

Ruby: def greet(name = "World") = name
来源：http://hz.daxiang520.top/gtzavnkubx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dashuyun.cn/gtgbnackjr.html

[C03] 可变参数
来源：http://hz.yonumen.top/gtlnuzfzrs.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinqigfzy.top/gtrhsygbdd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenlongwang.top/gtevlanwze.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gogol.net.cn/gtvxkuwjqx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yueranfly.top/gtrayidmly.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.pycfn.com/gtywqeobbp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.snrcjt.cn/gtzdcygowg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hnxiangtu.top/gtpgagtvaz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yongpay.top/gtufrjwdop.html

[C04] 命名参数 / 关键字参数
来源：http://hz.meibo888.top/gtufbdszpc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.smart0.xyz/gtufowxcvo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj20258888.top/gtahoyuemd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtwrxfmfef.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.redwolf501.top/gtvlrgcdhg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.meibo888.top/gtwnqirxik.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gtttiqesbo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sweek.top/gtexsolwnf.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtglryvolv.html

[C05] 返回多个值
来源：http://hz.52xcode.cn/gtijbjgyxe.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtkvgdvlrf.html

PHP:  return [$a, $b];
来源：http://hz.chenjidiqi.icu/gtqugczxzr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sysykeji.top/gtopmqhjva.html

TS:   return { a, b };
来源：http://hz.ivvv.top/gtuutwqwun.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yanxiufei.cn/gtslglvtyz.html

Go:   return a, b
来源：http://hz.9152youxi.cn/gtulsjzvuc.html

Ruby: return a, b
来源：http://hz.guowangkeji.top/gtcwqemusu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtqpwjxzmy.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigufen.top/gtrbhwjehm.html

Py:   square = lambda x: x * x
来源：http://hz.shangyingyoupin.top/gtoggvzutx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.fzhhl.top/gtxajbuycb.html

JS:   const square = x => x * x;
来源：http://hz.yj20258.top/gtvqimdmgr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtipddalfa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtcojpkbvo.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.birdmap.top/gtscecioqy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtcwidfcpy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuanzx.com/gtohfmanko.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gturbstmqm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yongpay.top/gtpllvdzac.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tianlin.xyz/gtirvmzfye.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj202588.top/gtodrqmykc.html

TS:   arr.map(String)
来源：http://hz.aibaodan.cn/gtwrhldtpg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ywan-chungtsiang.top/gtamzjkgfp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hammf.cn/gtyuiebatv.html

Ruby: arr.map(&:upcase)
来源：http://hz.zycfv.cn/gtlcqicoqy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jlsjyb.cn/gtwxhaglao.html

[C08] 闭包
来源：http://hz.iojbl.cn/gtubezjzlm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gtotgrpbct.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.kuanghao11.cn/gtxmdwhola.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtgyuscnqx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtwkukwbrk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuetiantiany.cn/gtmhpdkhuc.html


<!-- 参考信息 -->