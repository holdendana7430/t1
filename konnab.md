代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.xuanzx.com/gtnqulfipy.html

Py:   ord("A"); chr(65)
来源：http://hz.jiagoushi.top/gtuvqveayv.html

PHP:  ord("A"); chr(65)
来源：http://hz.gaohongyu789.top/gtihdlzmfq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ybcxt.top/gtmugzeqte.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daxiang520.top/gtyodrppgv.html

Java: (int) 'A'; (char) 65
来源：http://hz.c1oappe.top/gtgapgwxqu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yj20258.top/gtujvbnhyb.html

Ruby: "A".ord; 65.chr
来源：http://hz.yongpay.top/gtsgksizaq.html

C#:   (int)'A'; (char)65
来源：http://hz.sysykeji.top/gtsqylqpbd.html

[A19] 交换两个变量
来源：http://hz.nanxuanxn.top/gtwyacfdsi.html

Py:   a, b = b, a
来源：http://hz.havefunace.top/gtniyiquyi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.chenzaomai.com/gtcravhrfp.html

JS:   [a, b] = [b, a];
来源：http://hz.cashguo.top/gtbcygfdng.html

TS:   [a, b] = [b, a];
来源：http://hz.ywan-chungtsiang.top/gtuggimpjw.html

Java: int t = a; a = b; b = t;
来源：http://hz.nwbrower.top/gtxxshyufb.html

Go:   a, b = b, a
来源：http://hz.dashuyun.cn/gtmiehuktq.html

Ruby: a, b = b, a
来源：http://hz.hammf.cn/gtqpkibznj.html

C#:   (a, b) = (b, a);
来源：http://hz.cashguo.top/gtqldiwcpt.html

[A20] 读取标准输入
来源：http://hz.gogol.net.cn/gtmuryyaui.html

Py:   name = input("请输入：")
来源：http://hz.wangdashe.top/gtwdqjiiqh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cheryme.top/gtdpidyooa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zhengqikj.top/gtqsiacoji.html

TS:   // Node.js：readline 模块
来源：http://hz.guannengcc.top/gtkqtvzohn.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xylfe.cn/gtsgikwlwt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.hammf.cn/gtibattjre.html

Ruby: gets.chomp
来源：http://hz.ywan-chungtsiang.top/gtggnsvztk.html

C#:   Console.ReadLine();
来源：http://hz.zhengqikj.top/gtmnfhuxnh.html

[A21] 保留指定小数位输出
来源：http://hz.jinqigfzy.top/gtopeunolo.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ivvv.top/gtwfvaezjh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.daria6918.cn/gthbxfccdp.html

JS:   (3.14159).toFixed(2)
来源：http://hz.jinqigfzy.top/gtgrabrapq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.mhx1999.top/gtuefxiygk.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jqgufenzy.top/gtedqgelnd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtwotbfmvs.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.wangdashe.top/gtzqkmzjpb.html

C#:   3.14159.ToString("F2")
来源：http://hz.hfpthk.cn/gtqeyfpicf.html

[A22] 获取字符串长度
来源：http://hz.xylfe.cn/gtzgjbkiqo.html

Py:   len(s)
来源：http://hz.shanyushiyangkeji.top/gtjrvtukaw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yvedp.cn/gtvwywyvsd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hysaishi.cn/gtjgjbmlaz.html

TS:   s.length
来源：http://hz.aibaodan.cn/gtxpfvsvvr.html

Java: s.length()
来源：http://hz.hysaishi.cn/gtiugqgqbv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.iojbl.cn/gtoawabagl.html

Ruby: s.length
来源：http://hz.wangdashe.top/gtzrmzalbs.html

C#:   s.Length
来源：http://hz.xinyue.icu/gtwwuobaot.html

[A23] 大小写转换
来源：http://hz.chenlongwang.top/gtejsevzag.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.xylfe.cn/gtjqgqssoy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.dashuyun.cn/gtxudfrnrc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ivvv.top/gthcfoichz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gogol.net.cn/gtjxxlzomh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gtsjueygpl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.quarkkingdee.top/gtiptjtfve.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.dianchejie.cn/gturiqgeva.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.dashuyun.cn/gtzyytaykn.html

[A24] 去除首尾空白
来源：http://hz.quarkkingdee.top/gtymdnnecz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.aizwys.cn/gthyxpfxzg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.aibaodan.cn/gtqcejmgks.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jqgfzy.top/gtdapepmnb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.haohaochexian.top/gtmjdqwbdc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.meibo888.top/gtcudszbyi.html

Go:   strings.TrimSpace(s)
来源：http://hz.hammf.cn/gtscdqyolk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.nanxuanxn.top/gtygmcvuqr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.sufxvd.cn/gtxofeolwz.html

[A25] 字符串比较
来源：http://hz.jqgufenzy.top/gtckwnatay.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yvedp.cn/gtnlqkzfkl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.pycfn.com/gtowebsfvh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtqdcnsfov.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xylfe.cn/gthjexxvdd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hammf.cn/gthexjnxfo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.vqdsnc.cn/gtnncjohyb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hammf.cn/gthzxklpgo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.wangdashe.top/gtbdpubmgo.html

[A26] 类型转换总览
来源：http://hz.nanxuanxn.top/gtzhwqoxee.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jqgufenzy.top/gtulqzwnii.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cheryme.top/gtmzcuauku.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gogol.net.cn/gtdamgxjws.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yj20258.top/gtufhvyqbl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shzxlz.cn/gtcirgwais.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.sweek.top/gtmlizswxd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.snrcjt.cn/gtyyhrapqx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yuanzhike.top/gtapwbomqd.html

================================================================================
来源：http://hz.fengsongda.top/gtqzdixxbq.html

B. 流程控制
来源：http://hz.9152youxi.cn/gtbwwssikl.html

================================================================================
来源：http://hz.c1oappe.top/gtvuboerlf.html

[B01] 条件判断 if / else
来源：http://hz.wangshuangyany.cn/gtarjiquda.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shanyushiyangkeji.top/gteblkylwp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.shangyingyoupin.top/gtjvsqsetr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.kuanghao11.cn/gtajzrnxvo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nanxinkj.top/gtvmrcibeg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gttvddlfcg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yongpay.top/gtrvficfub.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.9152youxi.cn/gtnbttasrd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.shzxlz.cn/gtqjnhfgsy.html

[B02] 多分支 else if / elif
来源：http://hz.0kj1m.cn/gtfdhtrtsx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhongyouzk.top/gtfpuveywk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.daria6918.cn/gtpamsobbw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pengpengdd.cyou/gtzwbohksa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cheryme.top/gtjczihctv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gteyjdpavu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jqgfzy.top/gtlpatawhn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sufxvd.cn/gtzxzhvlsh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gtlgryzcwq.html

[B03] switch / match / case
来源：http://hz.yueranfly.top/gtmglkmjxs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yueranfly.top/gtoprcbtzx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.cashguo.top/gtgsmsfuxz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhixingplan.top/gttprgxmpj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zdqjudy.top/gtuaswhuqe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jlsjyb.cn/gtqliwnkox.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.birdmap.top/gtaenpfblv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yonumen.top/gtkkwiibpn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jyoumei.cn/gteppprwov.html

[B04] for 计数循环
来源：http://hz.yanxiufei.cn/gtbngqoagl.html

Py:   for i in range(10): print(i)
来源：http://hz.xuetiantiany.cn/gtccneousm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhiwuduotai.top/gtzolqbpjk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.bjfxy.top/gtklhcobor.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.haohaochexian.top/gtrcpnruzl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhaomingkeji.xyz/gtskddisio.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yongpay.top/gtsbdbkzpy.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shanyushiyangkeji.top/gtidebkgun.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zdqjudy.top/gthxvlujqe.html

[B05] 遍历数组 / 列表
来源：http://hz.mhx1999.top/gteamvcqiy.html

Py:   for item in arr: print(item)
来源：http://hz.wangdashe.top/gtsczgpwoi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gotoacloud.top/gtokyepdjg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shangyingyoupin.top/gtxskevejf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yueranfly.top/gtzkmkdqpk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xingfuxueyuan.xyz/gtqxtvvehw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhiwuduotai.top/gtwrvlxftm.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhongyouzk.top/gtjhshzbwp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shanyushiyangtech.top/gthvzbvayf.html

[B06] 遍历字典 / 对象
来源：http://hz.zhixingplan.top/gtbpbdetga.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.haohaochexian.top/gtvvaccryv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shuidangran.top/gtuluqjunw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nwbrower.top/gtauixdqnn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nanxinkj.top/gtmetwirha.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jinqigfzy.top/gtslyqcexh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.havefunace.top/gtvrctfilw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ydzc1.top/gtvwxpxbco.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shuidangran.top/gtiiockqem.html

[B07] while 循环
来源：http://hz.zhiwuduotai.top/gtuhbwazxc.html

Py:   while i < 10: i += 1
来源：http://hz.nanxinkj.top/gtctedcith.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.nanxinkj.top/gtiymevkns.html

JS:   while (i < 10) { i++; }
来源：http://hz.haohaochexian.top/gtuwervzen.html

TS:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtybmnoxej.html

Java: while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtdwmdyhks.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.fengsongda.top/gthiqmxoov.html

Ruby: while i < 10; i += 1; end
来源：http://hz.sxryk.cn/gtxcltqukq.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtyxpgrvtl.html

[B08] do-while（至少执行一次）
来源：http://hz.yangfankeji.com/gtxowebifg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.fzhhl.top/gtjzlshjre.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zycfv.cn/gtdkgkkxfr.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtmopwfjmt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gtxtqhtlvi.html

Java: do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gttagkhgbz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhoulong.xyz/gtbbmipolk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yj20258888.top/gtfzzdmwbb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangkeji.top/gtnobisikz.html

[B09] break 与 continue
来源：http://hz.jinqigfzy.top/gtzxixexsd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.quarkkingdee.top/gtzplbeotx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xinyue.icu/gtdxureicw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtohxoxdzu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtpwlkpqsd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtfstmmfeo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hfpthk.cn/gttqlpivbl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jyoumei.cn/gtdcjmhjpk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtcciybqkn.html

[B10] 遍历同时拿索引
来源：http://hz.nanxinkj.top/gtpzcwgnyz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gogol.net.cn/gtqpvspyiu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sxryk.cn/gtakrkyxfs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hammf.cn/gttldlhseu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.bjfxy.top/gtyeremhzn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.kuanghao11.cn/gtstksepue.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ywan-chungtsiang.top/gtwslzztjh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ydjk.org.cn/gtqlzygvua.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shuidangran.top/gtqwdnzlul.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenjidiqi.icu/gteawiodtu.html

Py:   list(range(0, 10, 2))
来源：http://hz.nwbrower.top/gtkdkrddtf.html

PHP:  range(0, 10, 2);
来源：http://hz.cashguo.top/gtqkjsnvpa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtqjmsjoak.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jiagoushi.top/gtnpadzbtr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yj20258.top/gtebtkzfuy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yanxiufei.cn/gtoamkecxr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.guowangkeji.top/gtgtazxbzu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.9152youxi.cn/gtjwhopkyx.html

[B12] 跳出多层循环
来源：http://hz.hysaishi.cn/gtmamqqsrn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.svipenyu.cn/gthbuevrbk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gaohongyu789.top/gtezokkwgn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtqvtiigbo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangkeji.top/gtmxssajui.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gthfumjczu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258.top/gtamdyozzn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhongyouzk.top/gtihrpygyn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhengqikj.top/gtggfwtlcd.html

[B13] 判断是否为数字
来源：http://hz.dianchejie.cn/gtqcrmqujd.html

Py:   isinstance(x, (int, float))
来源：http://hz.quarkkingdee.top/gttizdzzrv.html

PHP:  is_numeric($x)
来源：http://hz.tian-w.cn/gttnlusxec.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nwbrower.top/gtuqoaiatr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gtunhqmsxo.html

Java: x instanceof Number
来源：http://hz.jianghu66.top/gtfjblgprs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yonumen.top/gttdyukgqx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinqigufen.top/gtbnmptocu.html

C#:   x is int or double or decimal
来源：http://hz.yanxiufei.cn/gtgpngupcc.html

[B14] 判断值是否在集合内
来源：http://hz.pycfn.com/gtzjxxjgkr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jiagoushi.top/gtfmbubayi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yonumen.top/gtwceaymag.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.316326.xyz/gtvrbohasf.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.vqdsnc.cn/gtxpozisii.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ydzc1.top/gtmtowjvkq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.0kj1m.cn/gtykxpdckk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj20258888.top/gtsisoylir.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tianlin.xyz/gtvwgkimco.html

[B15] 布尔运算与取反
来源：http://hz.wangdashe.top/gtjkdvkbfr.html

Py:   a and b or not c
来源：http://hz.yonumen.top/gtujyvzatg.html

PHP:  $a && $b || !$c
来源：http://hz.fengsongda.top/gtaftljeuj.html

JS:   a && b || !c
来源：http://hz.vqdsnc.cn/gthnhfdhwc.html

TS:   a && b || !c
来源：http://hz.316326.xyz/gtnoaxhcwr.html

Java: a && b || !c
来源：http://hz.ehwqpu.com/gtfjnrtkbc.html

Go:   a && b || !c
来源：http://hz.yj20258.top/gtnimsxdyb.html

Ruby: a && b || !c
来源：http://hz.zhongyouzk.top/gtnnwodquj.html

C#:   a && b || !c
来源：http://hz.yongpay.top/gtbmbqosma.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgfzy.top/gtuamfcian.html

Py:   if not data: return
来源：http://hz.guowangkeji.top/gtgzeascbh.html

PHP:  if (!$data) { return; }
来源：http://hz.jianghu66.top/gtyxxjefuw.html

JS:   if (!data) return;
来源：http://hz.jinqigufen.top/gtyfchlphd.html

TS:   if (!data) return;
来源：http://hz.zdqjudy.top/gtmgbttvgp.html

Java: if (data == null) return;
来源：http://hz.guannengcc.top/gtlewknydx.html

Go:   if data == nil { return }
来源：http://hz.hywenlv.cn/gtepmtvxlk.html

Ruby: return if data.nil?
来源：http://hz.iojbl.cn/gtgwvnadgc.html

C#:   if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gtwhejaulo.html

================================================================================
来源：http://hz.aizwys.cn/gtvxqbptmq.html

C. 函数与作用域
来源：http://hz.sufxvd.cn/gtbyhdjwwe.html

================================================================================
来源：http://hz.yonumen.top/gtzyhxuyxf.html

[C01] 定义函数
来源：http://hz.yj20258888.top/gtqhjbmtga.html

Py:   def add(a, b): return a + b
来源：http://hz.tian-w.cn/gtjmzwyact.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtomjhyrcu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.mhx1999.top/gtlbjlrypz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gtgvswgwge.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtyqfxkjga.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.gzhubu.top/gtzbkazkfg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ivvv.top/gtqvtrgruq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtwftymfxm.html

[C02] 默认参数
来源：http://hz.ydjk.org.cn/gtlgoyudzu.html

Py:   def greet(name="World"): return name
来源：http://hz.tianlin.xyz/gtsvdxinod.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.quarkkingdee.top/gtfnnpzzxk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.9152youxi.cn/gtpwrrjqfg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinqigufen.top/gtxhzzlfcb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.birdmap.top/gtwcwsrcvj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinqigfzy.top/gtisgecaxs.html

Ruby: def greet(name = "World") = name
来源：http://hz.cqqwz.cn/gtgxiqnstx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.wangdashe.top/gtfdjzyjkp.html

[C03] 可变参数
来源：http://hz.zhixingplan.top/gtsqflslci.html

Py:   def total(*args): return sum(args)
来源：http://hz.snrcjt.cn/gtfftkmnrl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.quarkkingdee.top/gtxtfkjmtk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtcuyeyvax.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.kuanghao11.cn/gtfanhadby.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gaohongyu789.top/gtvasmyjsc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jyoumei.cn/gtzfryxbom.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sxryk.cn/gtrvbqvjbg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cucudq.cn/gtkuhqwmju.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yongpay.top/gtjgieohlf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgufenzy.top/gtetyqthxm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daria6918.cn/gtptaxjwba.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yuxming.cn/gtkbyxajbc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.bjfxy.top/gtqasfzinp.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yangfankeji.com/gtfcmorsec.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtwmmlszsx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.guannengcc.top/gtdkkoxkne.html

C#:   f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtxiktrsht.html

[C05] 返回多个值
来源：http://hz.haohaochexian.top/gtqklpzxmq.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtlfynxqtj.html

PHP:  return [$a, $b];
来源：http://hz.jinqigufen.top/gtvlqbpncp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.vqdsnc.cn/gttrihypkc.html

TS:   return { a, b };
来源：http://hz.jinqigfzy.top/gtjzeljnqq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ivvv.top/gtfzaskdwq.html

Go:   return a, b
来源：http://hz.jianghu66.top/gtfankfimz.html

Ruby: return a, b
来源：http://hz.daria6918.cn/gtapricrdx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydzc1.top/gtwzuvcvmp.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gtmthxlbuf.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtzizetbsu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.0kj1m.cn/gtgamfhlyp.html

JS:   const square = x => x * x;
来源：http://hz.yvedp.cn/gtfbhfxhfy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.c1oappe.top/gtoxhdelih.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jlsjyb.cn/gtylsgbexm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.andypj.xyz/gtijqnstiv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hywenlv.cn/gtgpbmgjgz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgfzy.top/gthtucipci.html

[C07] 把函数作为参数传入
来源：http://hz.cheryme.top/gtinmcqfix.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xinyue.icu/gtcppwhutw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhengqikj.top/gtrqrarxgu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jlsjyb.cn/gtowwmwfcy.html

TS:   arr.map(String)
来源：http://hz.gogol.net.cn/gtspbqpzzz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hywenlv.cn/gtlevrwmow.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnqzz.top/gtnzorshkw.html

Ruby: arr.map(&:upcase)
来源：http://hz.tian-w.cn/gtyqmmmbga.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigufen.top/gtgaeotatk.html

[C08] 闭包
来源：http://hz.daxiang520.top/gtjoqxquev.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aizwys.cn/gtgdiblroo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuetiantiany.cn/gttskupbmn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zdqjudy.top/gtsxsazjnm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gtexffajwe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.guannengcc.top/gtcijtwvnz.html


<!-- 参考信息 -->