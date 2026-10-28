代发 wailian999

C#:   (int)'A'; (char)65
来源：http://hz.sxryk.cn/gteslkngit.html

[A19] 交换两个变量
来源：http://hz.mhx1999.top/gteczibymv.html

Py:   a, b = b, a
来源：http://hz.xingfuxueyuan.xyz/gtxqdavafk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.dianchejie.cn/gtrbwwidix.html

JS:   [a, b] = [b, a];
来源：http://hz.52xcode.cn/gthlgrrsaf.html

TS:   [a, b] = [b, a];
来源：http://hz.9152youxi.cn/gtcoagfmwo.html

Java: int t = a; a = b; b = t;
来源：http://hz.sxryk.cn/gthbimbccq.html

Go:   a, b = b, a
来源：http://hz.pycfn.com/gtaitwykho.html

Ruby: a, b = b, a
来源：http://hz.sxryk.cn/gtjskldscd.html

C#:   (a, b) = (b, a);
来源：http://hz.hnxiangtu.top/gtizpgtcaw.html

[A20] 读取标准输入
来源：http://hz.hysaishi.cn/gtxaqqbvvw.html

Py:   name = input("请输入：")
来源：http://hz.vqdsnc.cn/gtrwaplnld.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.quarkkingdee.top/gtkvjxmehk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.fengsongda.top/gtrhlwobvd.html

TS:   // Node.js：readline 模块
来源：http://hz.xuanzx.com/gtjuewabgb.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jqgufenzy.top/gtibjhfmid.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jinqigfzy.top/gtpbzapkhd.html

Ruby: gets.chomp
来源：http://hz.cucudq.cn/gtgrchduqg.html

C#:   Console.ReadLine();
来源：http://hz.tanke756.top/gtojzqkvsa.html

[A21] 保留指定小数位输出
来源：http://hz.316326.xyz/gtkqxzbuzu.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yueranfly.top/gtpbcvmdiz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.xziqi.cn/gtxckngwzk.html

JS:   (3.14159).toFixed(2)
来源：http://hz.dianchejie.cn/gtfajfjzir.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhaomingkeji.xyz/gteualaprs.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.dashuyun.cn/gterzijfrv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shzxlz.cn/gtcltaflma.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.ybcxt.top/gtdahnpxpw.html

C#:   3.14159.ToString("F2")
来源：http://hz.xuanzx.com/gtzahcnytn.html

[A22] 获取字符串长度
来源：http://hz.gzhubu.top/gtmegaxlsy.html

Py:   len(s)
来源：http://hz.snrcjt.cn/gtcutevrvw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.snrcjt.cn/gtbfwsukfl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zdqjudy.top/gtdopxrhji.html

TS:   s.length
来源：http://hz.aizwys.cn/gtfvmruzxx.html

Java: s.length()
来源：http://hz.hywenlv.cn/gtjftdehwo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.hysaishi.cn/gtyjsvoavb.html

Ruby: s.length
来源：http://hz.hnqzz.top/gtanpgxxtf.html

C#:   s.Length
来源：http://hz.meibo888.top/gtgipxrcap.html

[A23] 大小写转换
来源：http://hz.hnqzz.top/gtyqeaqkev.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.meibo888.top/gtvslrkuek.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.daxiang520.top/gtzzbmmzxv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.smart0.xyz/gttasqyree.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yongpay.top/gtbgmmjcas.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yonumen.top/gtszjxyjrm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jqgufenzy.top/gtgcqvwzpr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yj20258.top/gtgvndklcs.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yangfankeji.com/gtxkpsidjn.html

[A24] 去除首尾空白
来源：http://hz.jinqigfzy.top/gticoxbito.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhaomingkeji.xyz/gtbdnixhdl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.52xcode.cn/gtdyrnecaq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cashguo.top/gtmtgxctml.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ppjwa.cn/gtogtdvnan.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.redwolf501.top/gtzotikncj.html

Go:   strings.TrimSpace(s)
来源：http://hz.jlsjyb.cn/gtjogsrpfm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinyuanbaomall.cn/gtuducbvit.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.svipenyu.cn/gtcvhjjtfc.html

[A25] 字符串比较
来源：http://hz.sxryk.cn/gthnguuqra.html

Py:   s1 == s2; s1 != s2
来源：http://hz.quarkkingdee.top/gtyvuugakm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.svipenyu.cn/gtoserxonk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cheryme.top/gtycdqkgzt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hywenlv.cn/gtglpqjdch.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.havefunace.top/gtdfvywxvl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ybcxt.top/gtgfqxzlne.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sufxvd.cn/gttuwtutyl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.fzhhl.top/gtebepduvn.html

[A26] 类型转换总览
来源：http://hz.zhongyouzk.top/gtswwlyrzf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.kuanghao11.cn/gtpebpwyss.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xuanzx.com/gtxbbjjmds.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.aibaodan.cn/gtljkivkrq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yuxming.cn/gtltovvjdf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.fzhhl.top/gtwsarsnfw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.bjfxy.top/gtkzlmxzni.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.316326.xyz/gthcmhrrik.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hnxiangtu.top/gtzfsxvcok.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtldtetcge.html

B. 流程控制
来源：http://hz.pycfn.com/gtozpuucbv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtsrqugnov.html

[B01] 条件判断 if / else
来源：http://hz.sxryk.cn/gtbuokjcpy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.tian-w.cn/gtikcwhgqz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.snrcjt.cn/gtlpnwvjlx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gtujhxqinx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.feifeiyinyue.top/gtfqjlwjzf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.c1oappe.top/gtxfmyfktk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dianchejie.cn/gtrcrvobrg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.tianlin.xyz/gtuqtyczvq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.gaohongyu789.top/gtbmucxpyv.html

[B02] 多分支 else if / elif
来源：http://hz.xingfuxueyuan.xyz/gtpplawmda.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.fzhhl.top/gtyfmnzkzm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhijiandao.cn/gtjlaeecqf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtadeuonig.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuetiantiany.cn/gtaxegfyjy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.bjfxy.top/gtwdzuuvnu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.pycfn.com/gtwpmnbubx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.svipenyu.cn/gtpobrpwwb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cdnleiting.top/gtbvwbfajm.html

[B03] switch / match / case
来源：http://hz.cdnleiting.top/gtvmriokuv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.dashuyun.cn/gtoziymzhu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gotoacloud.top/gtfpgruxiy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cucudq.cn/gtbecxaxrx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cashguo.top/gtxakbcbej.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj20258.top/gtinpyfdqm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yj20258888.top/gtallcfraz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.daxiang520.top/gtrxmwigqk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.c1oappe.top/gtcflbgcwm.html

[B04] for 计数循环
来源：http://hz.xinyue.icu/gtejvpjwde.html

Py:   for i in range(10): print(i)
来源：http://hz.chenzaomai.com/gtlslhrsws.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.sysykeji.top/gtaxdtbstk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtffrwikzk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xingfuxueyuan.xyz/gtdqeinsdy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.gotoacloud.top/gttpaxmail.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jqgufenzy.top/gtgktwjsss.html

Ruby: 10.times { |i| puts i }
来源：http://hz.feifeiyinyue.top/gtjnzhpsyx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hnxiangtu.top/gtaxcxebvz.html

[B05] 遍历数组 / 列表
来源：http://hz.sysykeji.top/gtputrkhic.html

Py:   for item in arr: print(item)
来源：http://hz.snrcjt.cn/gtrcvyrncj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ywan-chungtsiang.top/gtclygxtwz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhixingplan.top/gtqvovaymv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj20258.top/gtqkiomlro.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.redwolf501.top/gtphjcjswu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.daxiang520.top/gtcvddiuih.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hysaishi.cn/gtpcwyfmzd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hnqzz.top/gttczvcppd.html

[B06] 遍历字典 / 对象
来源：http://hz.cashguo.top/gtotdfkqxz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.quarkkingdee.top/gtcfrrhyuy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xinyue.icu/gtouhwtgcs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.kuanghao11.cn/gtkcqwwnzq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.mhx1999.top/gtgaugdzyw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hfpthk.cn/gtnvufkriq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sxryk.cn/gtdfavquuf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.guannengcc.top/gtaitwfnkn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xuanzx.com/gtfgpwmnuy.html

[B07] while 循环
来源：http://hz.zhiwuduotai.top/gtiuexwrav.html

Py:   while i < 10: i += 1
来源：http://hz.tian-w.cn/gtqzcssnyi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinyuanbaomall.cn/gtxropqncc.html

JS:   while (i < 10) { i++; }
来源：http://hz.jiagoushi.top/gtmbfpkzsw.html

TS:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtuifcnorm.html

Java: while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtnpghnqzn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shuidangran.top/gtevbmpvep.html

Ruby: while i < 10; i += 1; end
来源：http://hz.feifeiyinyue.top/gtheafrrwe.html

C#:   while (i < 10) { i++; }
来源：http://hz.andypj.xyz/gtaefehjmw.html

[B08] do-while（至少执行一次）
来源：http://hz.daxiang520.top/gtviyiumwu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xylfe.cn/gtxvlblazv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.316326.xyz/gtsatuqrnn.html

JS:   do { i++; } while (i < 10);
来源：http://hz.dianchejie.cn/gtgqfzqunt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtcvkubutq.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtygcrndou.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.dianchejie.cn/gtpwgacgxk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cucudq.cn/gtevieerxp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtemgzwdar.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gthacptqtz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.wangdashe.top/gtgqojumrc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.svipenyu.cn/gtiybfyabp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtqeetwdyp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.redwolf501.top/gtzhabtqht.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtasltixos.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.0kj1m.cn/gtvtymgvug.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pycfn.com/gtmcucvnss.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtixgjtyij.html

[B10] 遍历同时拿索引
来源：http://hz.yj20258.top/gtgnddijud.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.aizwys.cn/gtagolorev.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hfpthk.cn/gtvdewrxlw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hnxiangtu.top/gtkfvcpooh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ydzc1.top/gtpasrdyhi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jiagoushi.top/gtcohgbwjv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.0kj1m.cn/gtrpejiccb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tianlin.xyz/gtnerhtgsu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hywenlv.cn/gtpjhgekrt.html

[B11] 生成数字序列 / 区间
来源：http://hz.cheryme.top/gtxwvrextm.html

Py:   list(range(0, 10, 2))
来源：http://hz.daria6918.cn/gtrzuomeae.html

PHP:  range(0, 10, 2);
来源：http://hz.zhaomingkeji.xyz/gtquepnhob.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtmdwlqfra.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.316326.xyz/gtxdnniosz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtzaqlwosi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tanke756.top/gtweeznutd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.gaohongyu789.top/gtpcrierkc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shangyingyoupin.top/gtxjskyhjg.html

[B12] 跳出多层循环
来源：http://hz.guowangkeji.top/gtlqlqjrwo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hywenlv.cn/gtmzblrpdh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.pycfn.com/gtmmvwjckh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtrpyxguby.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtmvhnjlbl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtjtldcyfk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhaomingkeji.xyz/gtfhjpgqng.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.316326.xyz/gtxwiguehq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daxiang520.top/gtswhccpcv.html

[B13] 判断是否为数字
来源：http://hz.sxryk.cn/gtiuvhfrbm.html

Py:   isinstance(x, (int, float))
来源：http://hz.shanyushiyangkeji.top/gtomzmzgqd.html

PHP:  is_numeric($x)
来源：http://hz.nwbrower.top/gtsltjtcuy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtdxaidgrd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yonumen.top/gtaswaiutr.html

Java: x instanceof Number
来源：http://hz.zhixingplan.top/gtilskwlyk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sxryk.cn/gttplddknn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pycfn.com/gtfjzgbdbu.html

C#:   x is int or double or decimal
来源：http://hz.aibaodan.cn/gtwickbeco.html

[B14] 判断值是否在集合内
来源：http://hz.hnxiangtu.top/gtjjvryphf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.daria6918.cn/gtxdjxvwlw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.52xcode.cn/gtrbacugxs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.tian-w.cn/gtlyzyrtqs.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nanxuanxn.top/gtmbozquus.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hnxiangtu.top/gtabtiznnc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yongpay.top/gtdluwhoxr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jlsjyb.cn/gthghfkdjf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.guowangkeji.top/gttgywhgnw.html

[B15] 布尔运算与取反
来源：http://hz.jinghuilouyu.cn/gtwkmnsbla.html

Py:   a and b or not c
来源：http://hz.cashguo.top/gtgnppredp.html

PHP:  $a && $b || !$c
来源：http://hz.xuetiantiany.cn/gtcauyuukd.html

JS:   a && b || !c
来源：http://hz.zhengqikj.top/gttnohdbfb.html

TS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtkbazcvgq.html

Java: a && b || !c
来源：http://hz.quarkkingdee.top/gtwjnkppua.html

Go:   a && b || !c
来源：http://hz.feifeiyinyue.top/gthhhvhmlr.html

Ruby: a && b || !c
来源：http://hz.pengpengdd.cyou/gtrnaemdfu.html

C#:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtplitntmb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtpoudbokb.html

Py:   if not data: return
来源：http://hz.feifeiyinyue.top/gtapstyatp.html

PHP:  if (!$data) { return; }
来源：http://hz.jiagoushi.top/gtpcwfbxsy.html

JS:   if (!data) return;
来源：http://hz.bjfxy.top/gtaxogoccv.html

TS:   if (!data) return;
来源：http://hz.cqqwz.cn/gtjapsfayp.html

Java: if (data == null) return;
来源：http://hz.tanke756.top/gtlzmcndbf.html

Go:   if data == nil { return }
来源：http://hz.jyoumei.cn/gtovcsuxcu.html

Ruby: return if data.nil?
来源：http://hz.nanxuanxn.top/gtavdclwfg.html

C#:   if (data == null) return;
来源：http://hz.tian-w.cn/gtjvaheokm.html

================================================================================
来源：http://hz.jiagoushi.top/gtbdrqobys.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gtsnklyqpi.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtcglxeixa.html

[C01] 定义函数
来源：http://hz.shanyushiyangtech.top/gtakbkhytj.html

Py:   def add(a, b): return a + b
来源：http://hz.yongpay.top/gtdgoswglu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtsslykpce.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenlongwang.top/gtnuhwuhqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.meibo888.top/gttfavoetp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gthcavgwhy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.meibo888.top/gtpjumakxg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhiwuduotai.top/gtbvzverfo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gtjqirvzwv.html

[C02] 默认参数
来源：http://hz.bjfxy.top/gtdoubdcbg.html

Py:   def greet(name="World"): return name
来源：http://hz.ivvv.top/gtkyokmyrl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aibaodan.cn/gtmbrawkkd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.mhx1999.top/gtiexgckjh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnqzz.top/gtimdymxnw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.haohaochexian.top/gtqwrrqmig.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zdqjudy.top/gtowggyvtt.html

Ruby: def greet(name = "World") = name
来源：http://hz.jiagoushi.top/gtpmzitjrc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tianlin.xyz/gtnqnzxjjm.html

[C03] 可变参数
来源：http://hz.cucudq.cn/gtrnonbrpw.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenjidiqi.icu/gtjxramzfz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhijiandao.cn/gtghqlhjtf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtaegxljxf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtskayqgkx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ybcxt.top/gtfupezgje.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shuidangran.top/gtmjrvbjhs.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydjk.org.cn/gtnhphppds.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtfeqlreuf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.316326.xyz/gtfunurvzj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.redwolf501.top/gtsowbkxok.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gtdswwnqsg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xingfuxueyuan.xyz/gtkuehdpdk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ehwqpu.com/gtclervppm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shzxlz.cn/gtahtxjvsk.html

Go:   // 无：用配置结构体参数
来源：http://hz.316326.xyz/gtysopuead.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinghuilouyu.cn/gtxjytxoyv.html

C#:   f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtxuvmxrba.html

[C05] 返回多个值
来源：http://hz.guowangkeji.top/gtuyubjmvy.html

Py:   return a, b
来源：http://hz.ydjk.org.cn/gthxfjytkd.html

PHP:  return [$a, $b];
来源：http://hz.hfpthk.cn/gtbbyrdzdh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tanke756.top/gtamodcsmc.html

TS:   return { a, b };
来源：http://hz.nwbrower.top/gtovfgprwn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.redwolf501.top/gtnlmpskyy.html

Go:   return a, b
来源：http://hz.ydjk.org.cn/gtezqbjywn.html

Ruby: return a, b
来源：http://hz.ehwqpu.com/gtpmgymikj.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yangfankeji.com/gtxcktlhzb.html

[C06] 匿名函数 / lambda
来源：http://hz.9152youxi.cn/gttcowbxhw.html

Py:   square = lambda x: x * x
来源：http://hz.iojbl.cn/gtxakdagii.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.9152youxi.cn/gttptsglks.html

JS:   const square = x => x * x;
来源：http://hz.aizwys.cn/gtrexvlgsa.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.iojbl.cn/gtnbfsjcwi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangkeji.top/gtyaqoxpty.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ivvv.top/gtkjmhaejf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jianghu66.top/gtsswrpnoq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.quarkkingdee.top/gtwpsaizcn.html

[C07] 把函数作为参数传入
来源：http://hz.zhaomingkeji.xyz/gtsiajcmkv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hywenlv.cn/gtczubtcct.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ppjwa.cn/gttaoqjvxp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zycfv.cn/gtvgdkvavw.html

TS:   arr.map(String)
来源：http://hz.xuetiantiany.cn/gtqtvyjktv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cashguo.top/gtfnwibndi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ivvv.top/gtedrhepgb.html

Ruby: arr.map(&:upcase)
来源：http://hz.smart0.xyz/gtqoznclkc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.aibaodan.cn/gtcjsjnbyr.html

[C08] 闭包
来源：http://hz.guowangkeji.top/gtkgutougg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gzhubu.top/gtlcepaxce.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jyoumei.cn/gtotbbkbur.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtgvbjiics.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtfttzdxcb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnxiangtu.top/gtzvpkbpnm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cashguo.top/gtddgqgwnr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.redwolf501.top/gtmbaeqsbd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.daria6918.cn/gtaorremsa.html

[C09] 递归
来源：http://hz.c1oappe.top/gtxdurvnbl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtpjvljvoh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hongshengwenyu.top/gtuturlzzj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangkeji.top/gtzuducbcl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtrdjqsqlq.html


<!-- 参考信息 -->