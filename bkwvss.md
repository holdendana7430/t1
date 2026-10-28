代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxinkj.top/gtfukdscol.html

Java: (int) 'A'; (char) 65
来源：http://hz.pengpengdd.cyou/gtgmpwmrtu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.nanxinkj.top/gtrzdmxldj.html

Ruby: "A".ord; 65.chr
来源：http://hz.meibo888.top/gtegofvges.html

C#:   (int)'A'; (char)65
来源：http://hz.daxiang520.top/gtsgtbfqlv.html

[A19] 交换两个变量
来源：http://hz.yvedp.cn/gtuotpcofw.html

Py:   a, b = b, a
来源：http://hz.sweek.top/gthzczgale.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.pycfn.com/gtvzdgxafe.html

JS:   [a, b] = [b, a];
来源：http://hz.cqqwz.cn/gtxwnocfgn.html

TS:   [a, b] = [b, a];
来源：http://hz.zhixingplan.top/gtsyaqymbm.html

Java: int t = a; a = b; b = t;
来源：http://hz.xinyue.icu/gtfwitqfkd.html

Go:   a, b = b, a
来源：http://hz.xziqi.cn/gtyvjxutrl.html

Ruby: a, b = b, a
来源：http://hz.zdqjudy.top/gtmztaabqr.html

C#:   (a, b) = (b, a);
来源：http://hz.zhengqikj.top/gttmqhzokb.html

[A20] 读取标准输入
来源：http://hz.chenjidiqi.icu/gtaywwluzh.html

Py:   name = input("请输入：")
来源：http://hz.nanxinkj.top/gtujadyqgi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.mhx1999.top/gtzrycapjr.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.sweek.top/gtgdnnnmnr.html

TS:   // Node.js：readline 模块
来源：http://hz.hnqzz.top/gttrlxzhlx.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.hysaishi.cn/gtnmurress.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.aizwys.cn/gtnosftrkj.html

Ruby: gets.chomp
来源：http://hz.yj20258888.top/gtjxeupbag.html

C#:   Console.ReadLine();
来源：http://hz.cucudq.cn/gtlszpxqxl.html

[A21] 保留指定小数位输出
来源：http://hz.xuanzx.com/gthbfuhsje.html

Py:   f"{3.14159:.2f}"
来源：http://hz.daxiang520.top/gtiumkqqqd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.hnqzz.top/gtokybzajt.html

JS:   (3.14159).toFixed(2)
来源：http://hz.birdmap.top/gthqaiksml.html

TS:   (3.14159).toFixed(2)
来源：http://hz.nanxuanxn.top/gtupsxefhn.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.dashuyun.cn/gtmwmnrghb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shanyushiyangtech.top/gtodgeqlgi.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.andypj.xyz/gtxjlrqetb.html

C#:   3.14159.ToString("F2")
来源：http://hz.316326.xyz/gtvoeawcmp.html

[A22] 获取字符串长度
来源：http://hz.jinyuanbaomall.cn/gtvmhbxeqc.html

Py:   len(s)
来源：http://hz.316326.xyz/gtweytxkml.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yj20258.top/gtevntvquc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.cqqwz.cn/gtyxeyulwb.html

TS:   s.length
来源：http://hz.ivvv.top/gtseslclgb.html

Java: s.length()
来源：http://hz.aibaodan.cn/gtusstxmoi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yangfankeji.com/gtnlkkoggu.html

Ruby: s.length
来源：http://hz.zhengqikj.top/gtcgjytbgk.html

C#:   s.Length
来源：http://hz.sufxvd.cn/gtaatgpoyt.html

[A23] 大小写转换
来源：http://hz.quarkkingdee.top/gtymvgkqyy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.birdmap.top/gttuebmqtw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.shanyushiyangtech.top/gtomvgdakq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigfzy.top/gtbwmnmkib.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.nanxuanxn.top/gtdjsxuirj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.guowangkeji.top/gtydfojyqq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.dashuyun.cn/gtepnpeaga.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinyuanbaomall.cn/gtgeihqylc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jinyuanbaomall.cn/gtsyynscbd.html

[A24] 去除首尾空白
来源：http://hz.sweek.top/gtaleulffi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.hfpthk.cn/gtmdjbqzqm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yuxming.cn/gtsxtygupk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ydzc1.top/gtboukemwu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhijiandao.cn/gtrarmfjzw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.birdmap.top/gtmyfdsbce.html

Go:   strings.TrimSpace(s)
来源：http://hz.yanxiufei.cn/gtdcutktqi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhengqikj.top/gtgvdscyvx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cheryme.top/gtnzitdseo.html

[A25] 字符串比较
来源：http://hz.hysaishi.cn/gtfffdnyjd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.tianlin.xyz/gtzlvhmejg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.chenjidiqi.icu/gtoygogihd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.guannengcc.top/gtcacebzbf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigufen.top/gtsjskpvso.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.gzhubu.top/gtkvkbfboi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shanyushiyangkeji.top/gtlqkbgdlj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xuetiantiany.cn/gtyrrrmwim.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.316326.xyz/gtkvqmxaoy.html

[A26] 类型转换总览
来源：http://hz.xinyue.icu/gtajxvychy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.pengpengdd.cyou/gtztsudngu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cheryme.top/gtuekruehe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yonumen.top/gtjatoelhw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ivvv.top/gtzpumaint.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yuxming.cn/gtgxtjbqqz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yanxiufei.cn/gtaioyoimy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jlsjyb.cn/gtuzaqjyzc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jqgufenzy.top/gtbugzncvg.html

================================================================================
来源：http://hz.nanxinkj.top/gtxyyfvfua.html

B. 流程控制
来源：http://hz.aibaodan.cn/gtrslxazee.html

================================================================================
来源：http://hz.shuidangran.top/gtvzolrmkc.html

[B01] 条件判断 if / else
来源：http://hz.daria6918.cn/gtvyiyjesu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shzxlz.cn/gtmrotwekr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhoulong.xyz/gtolxpdqho.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangtech.top/gteielbdxe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtejaecheh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtqhuugrhy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.snrcjt.cn/gtwimanqsk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhiwuduotai.top/gththxrliu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtehulgxvy.html

[B02] 多分支 else if / elif
来源：http://hz.tanke756.top/gtyhkifnmv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yonumen.top/gtczmrtqyp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xinyue.icu/gttqxletcz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtlunuxcos.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtfbrqbprz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenzaomai.com/gtykiacdeq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.vqdsnc.cn/gtmezelrsb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sxryk.cn/gtnxrqsalf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtkpyigpwb.html

[B03] switch / match / case
来源：http://hz.9152youxi.cn/gtnewliwgg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sxryk.cn/gtiatgkgig.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xuetiantiany.cn/gtkhpialyt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.iojbl.cn/gtwqtigfav.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jianghu66.top/gtsrzlswpy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hywenlv.cn/gtyxobizae.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zycfv.cn/gtikilbtzo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jlsjyb.cn/gtsuobzwnu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.chenlongwang.top/gtupkytbog.html

[B04] for 计数循环
来源：http://hz.zhoulong.xyz/gttycltuad.html

Py:   for i in range(10): print(i)
来源：http://hz.316326.xyz/gtjamxahod.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yongpay.top/gthbwdwagk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yvedp.cn/gtdbeelujp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.316326.xyz/gtwpiqfnnq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.daxiang520.top/gtoklsuyzj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yj20258.top/gtkrqujfhr.html

Ruby: 10.times { |i| puts i }
来源：http://hz.gzhubu.top/gtdjlpllag.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tian-w.cn/gtbrnldrgw.html

[B05] 遍历数组 / 列表
来源：http://hz.ehwqpu.com/gtlhmehsud.html

Py:   for item in arr: print(item)
来源：http://hz.yuanzhike.top/gtdwsmkdgj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.tian-w.cn/gtjgrjrksm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yueranfly.top/gtrsyetzdd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sysykeji.top/gtlsgmttni.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gotoacloud.top/gtvguxgyla.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jyoumei.cn/gtvtpzlxck.html

Ruby: arr.each { |item| puts item }
来源：http://hz.aizwys.cn/gtntwwqzko.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gogol.net.cn/gtzshaadoi.html

[B06] 遍历字典 / 对象
来源：http://hz.cdnleiting.top/gtefiuoeit.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.aibaodan.cn/gthlunbzfi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ydjk.org.cn/gtnbkdxslx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.quarkkingdee.top/gtlhzrkxfw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.redwolf501.top/gtdlcgjnov.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shuidangran.top/gtrgedqptb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.tian-w.cn/gtlvocyyts.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.cdnleiting.top/gtnzhmndgc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.daxiang520.top/gtsynxrqqh.html

[B07] while 循环
来源：http://hz.yuxming.cn/gtbzjaeztu.html

Py:   while i < 10: i += 1
来源：http://hz.zhengqikj.top/gtufqtjjvz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xuanzx.com/gtvffcxfyv.html

JS:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtezkofimm.html

TS:   while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtvfncoefe.html

Java: while (i < 10) { i++; }
来源：http://hz.xylfe.cn/gthpiqblvo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.feifeiyinyue.top/gtfnflwyil.html

Ruby: while i < 10; i += 1; end
来源：http://hz.sxryk.cn/gtahgpbtnj.html

C#:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtdykitqpl.html

[B08] do-while（至少执行一次）
来源：http://hz.vqdsnc.cn/gtltonklhd.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.daxiang520.top/gtwobjvbwj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.dashuyun.cn/gtonnyasqn.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gtugicurzy.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hysaishi.cn/gteseswnqi.html

Java: do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gttfxyswqo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cdnleiting.top/gtgzirdfdt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yanxiufei.cn/gtbqkvujet.html

C#:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtmgsvqwck.html

[B09] break 与 continue
来源：http://hz.yuanzhike.top/gtoewzsnio.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hfpthk.cn/gtqqghirzr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhoulong.xyz/gtvoujbnzy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtbouepqrk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtjwrocjyu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gttfwixwai.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgfzy.top/gtuvikehpv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zycfv.cn/gtpzvludfm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtkojxzbux.html

[B10] 遍历同时拿索引
来源：http://hz.yj202588.top/gtpzkzkxfr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sufxvd.cn/gtzqtiqxzq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sweek.top/gtvsolhrfw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ybcxt.top/gtetawibwh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dianchejie.cn/gtpllulfxe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.quarkkingdee.top/gtnfbcikvk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.nanxuanxn.top/gtpdprougq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gaohongyu789.top/gtfjiukouf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sweek.top/gtbzphucxd.html

[B11] 生成数字序列 / 区间
来源：http://hz.vqdsnc.cn/gtjmbwwxop.html

Py:   list(range(0, 10, 2))
来源：http://hz.redwolf501.top/gtnxfuierl.html

PHP:  range(0, 10, 2);
来源：http://hz.aibaodan.cn/gttcujkcqp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gtbkgzqarm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtweuooshu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenjidiqi.icu/gtopkhabdn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ydzc1.top/gtmlaudorp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jiagoushi.top/gtarzbwdhw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ywan-chungtsiang.top/gtgfktwjkp.html

[B12] 跳出多层循环
来源：http://hz.svipenyu.cn/gtvqilmgsj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhijiandao.cn/gtsvjyoqfs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zycfv.cn/gtgachvpzh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtfsvxqdif.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtoomqqhid.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtdyzefigj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xingfuxueyuan.xyz/gtlsitdkzf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guowangkeji.top/gtcnfphgvp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hywenlv.cn/gtmfslvpjy.html

[B13] 判断是否为数字
来源：http://hz.yueranfly.top/gtywmjphmq.html

Py:   isinstance(x, (int, float))
来源：http://hz.cashguo.top/gtntjsxfkg.html

PHP:  is_numeric($x)
来源：http://hz.sweek.top/gtwtjuwzvo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yanxiufei.cn/gtnkiswvcu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtjlmwxobq.html

Java: x instanceof Number
来源：http://hz.havefunace.top/gtvmozpvkr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cashguo.top/gtmgkejqxc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cdnleiting.top/gtfldkgofp.html

C#:   x is int or double or decimal
来源：http://hz.52xcode.cn/gthpawzwic.html

[B14] 判断值是否在集合内
来源：http://hz.chenlongwang.top/gthcklcmcz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cdnleiting.top/gtmfntwqvg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxuanxn.top/gthvxelsml.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtdfjbzfnl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.haohaochexian.top/gtlnucadaw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.c1oappe.top/gtnaxrovlz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dianchejie.cn/gtfwoaylhk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.redwolf501.top/gtmhgrvjra.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shangyingyoupin.top/gtbftfijep.html

[B15] 布尔运算与取反
来源：http://hz.xinyue.icu/gturzkjtfz.html

Py:   a and b or not c
来源：http://hz.ehwqpu.com/gtxxoislzk.html

PHP:  $a && $b || !$c
来源：http://hz.ehwqpu.com/gtcasmloyd.html

JS:   a && b || !c
来源：http://hz.daxiang520.top/gtshgzhwko.html

TS:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtqnipsygj.html

Java: a && b || !c
来源：http://hz.yueranfly.top/gtpgoilisd.html

Go:   a && b || !c
来源：http://hz.xziqi.cn/gtjxqurzay.html

Ruby: a && b || !c
来源：http://hz.aizwys.cn/gtotzksfns.html

C#:   a && b || !c
来源：http://hz.xylfe.cn/gtgzmqknpa.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.9152youxi.cn/gtcfjyzgai.html

Py:   if not data: return
来源：http://hz.xuetiantiany.cn/gtoadrohqn.html

PHP:  if (!$data) { return; }
来源：http://hz.xylfe.cn/gtttyypvgy.html

JS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtwochwdmr.html

TS:   if (!data) return;
来源：http://hz.daxiang520.top/gtfsahlxpt.html

Java: if (data == null) return;
来源：http://hz.kuanghao11.cn/gtqmfdneav.html

Go:   if data == nil { return }
来源：http://hz.quarkkingdee.top/gtbtxdrekl.html

Ruby: return if data.nil?
来源：http://hz.yj20258.top/gtglqljpta.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtgwkdamrq.html

================================================================================
来源：http://hz.nwbrower.top/gtkfoqsodh.html

C. 函数与作用域
来源：http://hz.jinqigfzy.top/gtgxxyksue.html

================================================================================
来源：http://hz.daxiang520.top/gtdxvudzah.html

[C01] 定义函数
来源：http://hz.wangshuangyany.cn/gtvqjstlsm.html

Py:   def add(a, b): return a + b
来源：http://hz.xuanzx.com/gtkfjkwpaw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtqazlqhkq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtyywoqauv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gtqoiqnyoj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtfrrwtlyj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtkvtfuckq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daria6918.cn/gtptwtkspn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tianlin.xyz/gtccukoayw.html

[C02] 默认参数
来源：http://hz.xingfuxueyuan.xyz/gthaaplthj.html

Py:   def greet(name="World"): return name
来源：http://hz.jinqigufen.top/gtmgmeiruc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.wangshuangyany.cn/gtmmjbgazj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tianlin.xyz/gtmaoexuqc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinghuilouyu.cn/gtyitbebav.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.meibo888.top/gtbzuiuvrt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.haohaochexian.top/gtnktfvrcn.html

Ruby: def greet(name = "World") = name
来源：http://hz.ydjk.org.cn/gtdgjnttjj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xingfuxueyuan.xyz/gtkovgjogn.html

[C03] 可变参数
来源：http://hz.jyoumei.cn/gtssebqhqa.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258888.top/gtwuobkkhi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cashguo.top/gtfzirngpw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gthxlsnnvi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ywan-chungtsiang.top/gtqqozgwoj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.316326.xyz/gtwkwzmalm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgfzy.top/gtznzrfitt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cashguo.top/gtwnuoyctr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gogol.net.cn/gtxtailitu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xinyue.icu/gtdyadytlv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hysaishi.cn/gtqwtrqiyy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.9152youxi.cn/gtownspkhn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ppjwa.cn/gtmpwiftys.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shangyingyoupin.top/gtdqfigyce.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinyuanbaomall.cn/gtlhiiipej.html

Go:   // 无：用配置结构体参数
来源：http://hz.cheryme.top/gtsaphtnyz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gtpxiyjgbf.html

C#:   f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gtmvqieajg.html

[C05] 返回多个值
来源：http://hz.tian-w.cn/gtgqgewlyi.html

Py:   return a, b
来源：http://hz.fzhhl.top/gtnwjobujn.html

PHP:  return [$a, $b];
来源：http://hz.zdqjudy.top/gtrxecgans.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnxiangtu.top/gtmausilqn.html

TS:   return { a, b };
来源：http://hz.dianchejie.cn/gtgjkbqkmk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258888.top/gtjlxjigct.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtdpzynuwh.html

Ruby: return a, b
来源：http://hz.sysykeji.top/gtheaoyvie.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj202588.top/gtkhuyvqyt.html

[C06] 匿名函数 / lambda
来源：http://hz.fzhhl.top/gtijxyubci.html

Py:   square = lambda x: x * x
来源：http://hz.316326.xyz/gtfpcznloa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xinyue.icu/gtrwpesrwy.html

JS:   const square = x => x * x;
来源：http://hz.yuxming.cn/gtnvgofbuk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guowangkeji.top/gtaamefysr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangdashe.top/gtvrysuzon.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.meibo888.top/gteqscwxwu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj202588.top/gttxkgpucz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yueranfly.top/gtcfnjglla.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtyyruvmsh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.9152youxi.cn/gtbelrqwkt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ybcxt.top/gtvtzdwbni.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.bjfxy.top/gtwjggdprv.html

TS:   arr.map(String)
来源：http://hz.jlsjyb.cn/gtvigmbrtc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.bjfxy.top/gtcouabkmj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sweek.top/gthztzdbkc.html

Ruby: arr.map(&:upcase)
来源：http://hz.mhx1999.top/gtujikpnjr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.316326.xyz/gtrjmevdkf.html

[C08] 闭包
来源：http://hz.jianghu66.top/gtvhpxafrb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jqgfzy.top/gtuivrcudb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tianlin.xyz/gtyelwbtng.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtfjxfpgbx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtooqyzvaz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.pycfn.com/gthibxpsoj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangtech.top/gtlqxydxrj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.andypj.xyz/gtttkbwirr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtuhpjrzvw.html

[C09] 递归
来源：http://hz.birdmap.top/gtgawjdawj.html


<!-- 参考信息 -->