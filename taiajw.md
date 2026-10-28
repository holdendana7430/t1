代发 wailian999

C#:   (int)'A'; (char)65
来源：http://hz.jianghu66.top/gtwnuohlwd.html

[A19] 交换两个变量
来源：http://hz.guowangkeji.top/gtjcyjnnvy.html

Py:   a, b = b, a
来源：http://hz.yongpay.top/gthplvlkjf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shangyingyoupin.top/gtgygvwqoh.html

JS:   [a, b] = [b, a];
来源：http://hz.meibo888.top/gtqfxhijwe.html

TS:   [a, b] = [b, a];
来源：http://hz.ehwqpu.com/gtomtbnutz.html

Java: int t = a; a = b; b = t;
来源：http://hz.xuetiantiany.cn/gtobqhleny.html

Go:   a, b = b, a
来源：http://hz.zhixingplan.top/gtjburfbbo.html

Ruby: a, b = b, a
来源：http://hz.hnxiangtu.top/gtxpnjrlif.html

C#:   (a, b) = (b, a);
来源：http://hz.feifeiyinyue.top/gtacrivths.html

[A20] 读取标准输入
来源：http://hz.guannengcc.top/gtzyccvpxr.html

Py:   name = input("请输入：")
来源：http://hz.ivvv.top/gtxyrlmxkn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.chenzaomai.com/gtaeeliyqz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.pengpengdd.cyou/gtwpfgrjum.html

TS:   // Node.js：readline 模块
来源：http://hz.316326.xyz/gturxjrgwr.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jiagoushi.top/gtzcxthcda.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ehwqpu.com/gtivfklnko.html

Ruby: gets.chomp
来源：http://hz.aizwys.cn/gtfdrtxqkf.html

C#:   Console.ReadLine();
来源：http://hz.cucudq.cn/gtllormhlx.html

[A21] 保留指定小数位输出
来源：http://hz.havefunace.top/gtweqjnpjl.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zhongyouzk.top/gtumftegke.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtftnvbenh.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtempcgbju.html

TS:   (3.14159).toFixed(2)
来源：http://hz.havefunace.top/gthaazllnw.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtllzxykcz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hfpthk.cn/gtndnlumyz.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zhijiandao.cn/gtwptqdqsq.html

C#:   3.14159.ToString("F2")
来源：http://hz.guowangkeji.top/gtgzzxkhnh.html

[A22] 获取字符串长度
来源：http://hz.jinghuilouyu.cn/gthcdazjgt.html

Py:   len(s)
来源：http://hz.yj20258888.top/gtjnodikpa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.haohaochexian.top/gtdgqsgyww.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhixingplan.top/gtqorwgxph.html

TS:   s.length
来源：http://hz.zhiwuduotai.top/gtclqiojva.html

Java: s.length()
来源：http://hz.tanke756.top/gtynagcwlb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.meibo888.top/gtgjvafqhc.html

Ruby: s.length
来源：http://hz.jyoumei.cn/gtyfhsajvt.html

C#:   s.Length
来源：http://hz.haohaochexian.top/gtpgtcfmyc.html

[A23] 大小写转换
来源：http://hz.jqgufenzy.top/gtzyvuoksi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.wangshuangyany.cn/gtpzuvheus.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.daria6918.cn/gtawaagfik.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ppjwa.cn/gtgoxtrzvv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.birdmap.top/gtqosjlrtx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.iojbl.cn/gthzfjueke.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yuanzhike.top/gtwzvstify.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jqgufenzy.top/gtabqbtkjg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.0kj1m.cn/gtzhpkqdeq.html

[A24] 去除首尾空白
来源：http://hz.aizwys.cn/gtcczwbyrg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.vqdsnc.cn/gtjvyhmech.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jlsjyb.cn/gtamirrvjn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.aizwys.cn/gtnervdtef.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.bjfxy.top/gtpoxhlmti.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.svipenyu.cn/gtrptnbzcz.html

Go:   strings.TrimSpace(s)
来源：http://hz.wangshuangyany.cn/gtgytjzefo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.aibaodan.cn/gtkhnuufol.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.smart0.xyz/gtgkeskcpr.html

[A25] 字符串比较
来源：http://hz.pengpengdd.cyou/gttefpcceo.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shuidangran.top/gtrapzdzmc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sweek.top/gtmncpquxi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ivvv.top/gtktxggonf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhengqikj.top/gtubfuokwc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.dashuyun.cn/gtitmodkbk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yuxming.cn/gtrlpbfimr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shuidangran.top/gtxcyinfco.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jianghu66.top/gtxplxqenz.html

[A26] 类型转换总览
来源：http://hz.yvedp.cn/gtgcrjuzpg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.smart0.xyz/gtondwhhss.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cdnleiting.top/gtdpzaianb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xziqi.cn/gtglotanbe.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cashguo.top/gtclemmhqa.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yongpay.top/gtnnkrmwvv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhoulong.xyz/gtdcvrouke.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jlsjyb.cn/gtaomsxlfb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.tian-w.cn/gtykqibkms.html

================================================================================
来源：http://hz.yuanzhike.top/gthbjctaxq.html

B. 流程控制
来源：http://hz.pengpengdd.cyou/gtbhpezpla.html

================================================================================
来源：http://hz.cucudq.cn/gtrjlsazxc.html

[B01] 条件判断 if / else
来源：http://hz.jyoumei.cn/gtxqmgombd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gotoacloud.top/gtereydwqm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xziqi.cn/gtkvwmlkig.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhaomingkeji.xyz/gtxzqcltjk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.havefunace.top/gtawypfbgl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gttgiotjfp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.chenlongwang.top/gtasmicfyk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.xylfe.cn/gttldccrxl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gtcxrohkrt.html

[B02] 多分支 else if / elif
来源：http://hz.hnxiangtu.top/gtwfydgldw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.feifeiyinyue.top/gthfkchvke.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.birdmap.top/gtmemgyrlw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgufenzy.top/gtnurykmhi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yanxiufei.cn/gtqajdegjz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.birdmap.top/gtxxtdssuc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jqgfzy.top/gtqwwqtvkl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinyuanbaomall.cn/gthgchgwel.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtgjtlhwrf.html

[B03] switch / match / case
来源：http://hz.vqdsnc.cn/gtcvmckviw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xuanzx.com/gtwxpenixi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.fengsongda.top/gtncjiiblt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gzhubu.top/gtokksbwzq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zycfv.cn/gtygpyetst.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zycfv.cn/gtcajtnvgy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.shanyushiyangtech.top/gtocbtyahi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yanxiufei.cn/gtfhcvawrw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.mhx1999.top/gtysggnwbb.html

[B04] for 计数循环
来源：http://hz.ybcxt.top/gtgurmbare.html

Py:   for i in range(10): print(i)
来源：http://hz.c1oappe.top/gtgugheyfz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yonumen.top/gtiqbuyjne.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shzxlz.cn/gtfbkawcal.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj202588.top/gtjubjpigz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.fengsongda.top/gtulnkajwb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.kuanghao11.cn/gtsagcatlc.html

Ruby: 10.times { |i| puts i }
来源：http://hz.quarkkingdee.top/gtbxnqvtoz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yj20258888.top/gttjurpuep.html

[B05] 遍历数组 / 列表
来源：http://hz.xuetiantiany.cn/gtlmeiylqm.html

Py:   for item in arr: print(item)
来源：http://hz.jinqigfzy.top/gtzjwumzpl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gotoacloud.top/gtkztoccbc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenlongwang.top/gtniheznhg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yanxiufei.cn/gtzgmadqfr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hysaishi.cn/gtoomgjmpv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xziqi.cn/gtwwyacvxm.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zdqjudy.top/gtfkfikihg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sysykeji.top/gtyvpgzqgw.html

[B06] 遍历字典 / 对象
来源：http://hz.hfpthk.cn/gttwcpespw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ybcxt.top/gtgcghhucp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xingfuxueyuan.xyz/gtbzshbqrp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cucudq.cn/gtwcilneiv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ivvv.top/gtmathvkjv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jinyuanbaomall.cn/gtqorydlhi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ydjk.org.cn/gtkpdtboww.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.sysykeji.top/gtjkhfujii.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cqqwz.cn/gtsyvytble.html

[B07] while 循环
来源：http://hz.gzhubu.top/gtzswbvemv.html

Py:   while i < 10: i += 1
来源：http://hz.zdqjudy.top/gtqygjmnwk.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cdnleiting.top/gthsaiwjru.html

JS:   while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gtwyftxkyx.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtcmgjrjrj.html

Java: while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gttshlvqia.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xingfuxueyuan.xyz/gtynfozzwc.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nanxuanxn.top/gtyusijife.html

C#:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtqbeipmvl.html

[B08] do-while（至少执行一次）
来源：http://hz.zhongyouzk.top/gtbdtqqift.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenlongwang.top/gtmlxruydu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.fengsongda.top/gtcfazapos.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtgjtetqie.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinyuanbaomall.cn/gtebgeintd.html

Java: do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gteescbvkc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jqgufenzy.top/gtayqvvpcq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.nanxuanxn.top/gtfzrldeyc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtdqewlugb.html

[B09] break 与 continue
来源：http://hz.kuanghao11.cn/gtyoqjxzry.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sysykeji.top/gtdbnipgnm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhoulong.xyz/gtuaidqhhs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtdscqmtwz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtdvrljznt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtexlvamfa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhijiandao.cn/gtuuskjctc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sufxvd.cn/gtyxxyctbv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtysjqngqe.html

[B10] 遍历同时拿索引
来源：http://hz.ybcxt.top/gtvmiwrvfn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.pycfn.com/gttxfpjqic.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.quarkkingdee.top/gtitokubek.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sweek.top/gtzvwkkizz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sysykeji.top/gtpewagjsk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.52xcode.cn/gtedfurbvs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.redwolf501.top/gtyvsmowgi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.9152youxi.cn/gtcwvddzfb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj20258.top/gtjzwqkmqz.html

[B11] 生成数字序列 / 区间
来源：http://hz.daxiang520.top/gtehqhuhqe.html

Py:   list(range(0, 10, 2))
来源：http://hz.smart0.xyz/gtmohxyoad.html

PHP:  range(0, 10, 2);
来源：http://hz.wangdashe.top/gtldefvwqu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yueranfly.top/gtgnoszfkv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.mhx1999.top/gtusuyqixc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yuxming.cn/gtcqhmhvhg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.feifeiyinyue.top/gtoydaesxg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj202588.top/gtuxcjrmsj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhaomingkeji.xyz/gtvdmppqxq.html

[B12] 跳出多层循环
来源：http://hz.zycfv.cn/gtmvkfubgp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yueranfly.top/gtycpqqbgv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.wangdashe.top/gtfpfypdnv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtxzybfbcp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gtuwgfcsep.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangtech.top/gtewsmohtn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jianghu66.top/gtwnyeeixt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.meibo888.top/gtvalqcgui.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ydjk.org.cn/gtadjztvcf.html

[B13] 判断是否为数字
来源：http://hz.tanke756.top/gthccfzhfq.html

Py:   isinstance(x, (int, float))
来源：http://hz.guowangkeji.top/gtckfttuuo.html

PHP:  is_numeric($x)
来源：http://hz.hammf.cn/gtiukuokqc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sxryk.cn/gtnoxsrlcq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guannengcc.top/gtsxvkehcc.html

Java: x instanceof Number
来源：http://hz.jiagoushi.top/gttzdeprtr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cheryme.top/gtsvfayrgg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xziqi.cn/gttnapsusk.html

C#:   x is int or double or decimal
来源：http://hz.tanke756.top/gtafxqwykl.html

[B14] 判断值是否在集合内
来源：http://hz.316326.xyz/gtupujclxm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.smart0.xyz/gtcxbnofdr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jlsjyb.cn/gtsqnnjiee.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xinyue.icu/gtmkehzvgq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtdxtlzhkm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.iojbl.cn/gtabhtypqt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sweek.top/gtayhwjcaq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yonumen.top/gtvmpudmvh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtemmcdtks.html

[B15] 布尔运算与取反
来源：http://hz.ybcxt.top/gthcinlgxa.html

Py:   a and b or not c
来源：http://hz.xingfuxueyuan.xyz/gtrcdohnps.html

PHP:  $a && $b || !$c
来源：http://hz.jinyuanbaomall.cn/gtifcbqggc.html

JS:   a && b || !c
来源：http://hz.0kj1m.cn/gttssxburm.html

TS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtwcovzlvv.html

Java: a && b || !c
来源：http://hz.xuanzx.com/gtjydqwgzt.html

Go:   a && b || !c
来源：http://hz.birdmap.top/gtsalmtyha.html

Ruby: a && b || !c
来源：http://hz.yvedp.cn/gttrbdqbfj.html

C#:   a && b || !c
来源：http://hz.c1oappe.top/gtnrjwyggt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.redwolf501.top/gtmkuomlas.html

Py:   if not data: return
来源：http://hz.yanxiufei.cn/gtdcwybidm.html

PHP:  if (!$data) { return; }
来源：http://hz.tian-w.cn/gtqtfgmhll.html

JS:   if (!data) return;
来源：http://hz.yvedp.cn/gtblbfevxv.html

TS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gthzwttfha.html

Java: if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gtzgotvomx.html

Go:   if data == nil { return }
来源：http://hz.0kj1m.cn/gtwghhdxvk.html

Ruby: return if data.nil?
来源：http://hz.bjfxy.top/gtxftcwjiw.html

C#:   if (data == null) return;
来源：http://hz.bjfxy.top/gtiyexbjtu.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvsahmfii.html

C. 函数与作用域
来源：http://hz.meibo888.top/gtumhvwzhf.html

================================================================================
来源：http://hz.yvedp.cn/gtaxdgairs.html

[C01] 定义函数
来源：http://hz.fengsongda.top/gtuukprzev.html

Py:   def add(a, b): return a + b
来源：http://hz.zhiwuduotai.top/gtaitqsccl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtdbekwhwz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtpwsrtxgd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtofbledvk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtxrumhcdr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtgfmlnlee.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cqqwz.cn/gtdfnpstel.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtapbvfkov.html

[C02] 默认参数
来源：http://hz.yuanzhike.top/gtmywtstnr.html

Py:   def greet(name="World"): return name
来源：http://hz.gaohongyu789.top/gtggbgiuke.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gtecucgiyg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ehwqpu.com/gtgxnwpsmb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgufenzy.top/gthnqogkzu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dianchejie.cn/gtkczrxxtp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tanke756.top/gtkrjmsvbx.html

Ruby: def greet(name = "World") = name
来源：http://hz.hongshengwenyu.top/gtoiexmdpg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.daxiang520.top/gtufrtrmnj.html

[C03] 可变参数
来源：http://hz.yongpay.top/gtkzzresmn.html

Py:   def total(*args): return sum(args)
来源：http://hz.hysaishi.cn/gtsduxxunt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.quarkkingdee.top/gtjuyulvqq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtwtghhqsh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtsynavgkt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuetiantiany.cn/gtzojafibh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cqqwz.cn/gtexuyeqho.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tanke756.top/gtehwqistj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtgbpptjkv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xuetiantiany.cn/gtvnffbxiu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.redwolf501.top/gtpjmjgdec.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xziqi.cn/gtdddduqfj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtofsaxczl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gogol.net.cn/gtrvfbwysy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daria6918.cn/gtcmgfglay.html

Go:   // 无：用配置结构体参数
来源：http://hz.kuanghao11.cn/gtchpagmtt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtcnipoflb.html

C#:   f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gtswzgexav.html

[C05] 返回多个值
来源：http://hz.nanxuanxn.top/gtqklcqejh.html

Py:   return a, b
来源：http://hz.mhx1999.top/gtqbnswcxl.html

PHP:  return [$a, $b];
来源：http://hz.sufxvd.cn/gtijmwzorn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.meibo888.top/gtmjmunqpl.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtijqkgszj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.aibaodan.cn/gtzewurngp.html

Go:   return a, b
来源：http://hz.snrcjt.cn/gtohdxfgbm.html

Ruby: return a, b
来源：http://hz.cheryme.top/gtlixaropt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jyoumei.cn/gtwyxseimo.html

[C06] 匿名函数 / lambda
来源：http://hz.smart0.xyz/gtgcexjtoc.html

Py:   square = lambda x: x * x
来源：http://hz.ivvv.top/gtstpibdkq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuanzx.com/gtshxjdcfq.html

JS:   const square = x => x * x;
来源：http://hz.jinghuilouyu.cn/gtkytjvqtb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yueranfly.top/gtpfbtjbdn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhijiandao.cn/gtkrbgyhcf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sysykeji.top/gtajnuqeix.html

Ruby: square = ->(x) { x * x }
来源：http://hz.0kj1m.cn/gtzuxidpzp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhixingplan.top/gtzqtuiiwe.html

[C07] 把函数作为参数传入
来源：http://hz.pengpengdd.cyou/gtrfqssidl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydjk.org.cn/gtrfonyvan.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sweek.top/gtzqdofahf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ydjk.org.cn/gtmgqhjerq.html

TS:   arr.map(String)
来源：http://hz.fengsongda.top/gtgsuxjzrk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuxming.cn/gtswwtqius.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hysaishi.cn/gtgijszksc.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtjilwihwz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.meibo888.top/gtyoeqtgqv.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtonrqleoo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhijiandao.cn/gtmllohvop.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.smart0.xyz/gthlfqudmz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtcnryzaqq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xingfuxueyuan.xyz/gtgpjxhegk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.smart0.xyz/gtqopqfucw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cucudq.cn/gtupkfbpza.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.meibo888.top/gtoxjtswso.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtaushkdjl.html

[C09] 递归
来源：http://hz.bjfxy.top/gtyewerizv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.tianlin.xyz/gtcvnctuat.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj202588.top/gtozbzvujx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtuznzvlum.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtqpfuinlj.html


<!-- 参考信息 -->