代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinghuilouyu.cn/gtieprkzdw.html

Java: (int) 'A'; (char) 65
来源：http://hz.yj20258888.top/gtmmdflxwg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.tian-w.cn/gtuomygxnf.html

Ruby: "A".ord; 65.chr
来源：http://hz.chenzaomai.com/gtbhycydmk.html

C#:   (int)'A'; (char)65
来源：http://hz.dashuyun.cn/gtzwwomdji.html

[A19] 交换两个变量
来源：http://hz.quarkkingdee.top/gtfszolaux.html

Py:   a, b = b, a
来源：http://hz.xziqi.cn/gtzmfbzbgr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yueranfly.top/gtgpjhsmws.html

JS:   [a, b] = [b, a];
来源：http://hz.cheryme.top/gtlumjmjtw.html

TS:   [a, b] = [b, a];
来源：http://hz.ydzc1.top/gtefnlkexc.html

Java: int t = a; a = b; b = t;
来源：http://hz.gzhubu.top/gtxjrimndr.html

Go:   a, b = b, a
来源：http://hz.yj20258888.top/gtoahapslt.html

Ruby: a, b = b, a
来源：http://hz.jlsjyb.cn/gtzjptfrzw.html

C#:   (a, b) = (b, a);
来源：http://hz.zdqjudy.top/gttxslmkjy.html

[A20] 读取标准输入
来源：http://hz.cqqwz.cn/gtckpibxxn.html

Py:   name = input("请输入：")
来源：http://hz.mhx1999.top/gthjmpxswb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yangfankeji.com/gtvcqjikjt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.iojbl.cn/gtzhqptjss.html

TS:   // Node.js：readline 模块
来源：http://hz.ivvv.top/gtaxirnubh.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xinyue.icu/gtchwovdur.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zdqjudy.top/gtgdyvzyom.html

Ruby: gets.chomp
来源：http://hz.0kj1m.cn/gtwbyroiqw.html

C#:   Console.ReadLine();
来源：http://hz.redwolf501.top/gtzquihanv.html

[A21] 保留指定小数位输出
来源：http://hz.yvedp.cn/gtyjdyzirr.html

Py:   f"{3.14159:.2f}"
来源：http://hz.feifeiyinyue.top/gtkexwgyds.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.xziqi.cn/gtpwgpmozi.html

JS:   (3.14159).toFixed(2)
来源：http://hz.kuanghao11.cn/gtwmzlminx.html

TS:   (3.14159).toFixed(2)
来源：http://hz.wangshuangyany.cn/gtquuoklnu.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.sxryk.cn/gtugwqduxf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shanyushiyangkeji.top/gtreuzlyik.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yj202588.top/gtcobpceea.html

C#:   3.14159.ToString("F2")
来源：http://hz.ybcxt.top/gthmroprzb.html

[A22] 获取字符串长度
来源：http://hz.jinyuanbaomall.cn/gtiyuwqbjh.html

Py:   len(s)
来源：http://hz.bjfxy.top/gtrhkqfbfl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.vqdsnc.cn/gtzprlkknb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.chenlongwang.top/gtpuxtepmi.html

TS:   s.length
来源：http://hz.chenjidiqi.icu/gtpiovhmil.html

Java: s.length()
来源：http://hz.zhengqikj.top/gtnpxlnpre.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.guannengcc.top/gtlwbhsikn.html

Ruby: s.length
来源：http://hz.ehwqpu.com/gtjhyvzfxq.html

C#:   s.Length
来源：http://hz.cucudq.cn/gtztebmvti.html

[A23] 大小写转换
来源：http://hz.ivvv.top/gtmzxwsahs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yuanzhike.top/gtlplvlfvp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yj202588.top/gtmwqioxaa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.daxiang520.top/gtpqjkiwjz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.bjfxy.top/gteshfyefz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yangfankeji.com/gtgczoneuh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.chenlongwang.top/gttulmpksk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.meibo888.top/gtosofacrc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yuxming.cn/gtstxvrcsq.html

[A24] 去除首尾空白
来源：http://hz.yanxiufei.cn/gtfcwnwjyd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.316326.xyz/gtyjuudret.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.iojbl.cn/gtblmdjfjl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhixingplan.top/gtqgzrsryn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.redwolf501.top/gtbfddfhku.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.dashuyun.cn/gtizmnhmbq.html

Go:   strings.TrimSpace(s)
来源：http://hz.jianghu66.top/gtgtuiigrt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.sxryk.cn/gtzmqxohvb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.c1oappe.top/gtddzvbqxv.html

[A25] 字符串比较
来源：http://hz.yj20258.top/gthuipsisp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ydjk.org.cn/gtolfkiikf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ybcxt.top/gtqskqbymy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtmwbsewvz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtdgviaphw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.gzhubu.top/gtrghpiyps.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hongshengwenyu.top/gtzpopwdzd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.haohaochexian.top/gtnvipkhyc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jianghu66.top/gtweiilytj.html

[A26] 类型转换总览
来源：http://hz.xingfuxueyuan.xyz/gtxepyfrno.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.nanxinkj.top/gtwafbjbsu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yueranfly.top/gtwahbdhei.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.wangshuangyany.cn/gtwwfwkvub.html

TS:   Number() String() Boolean() x as number
来源：http://hz.chenzaomai.com/gtrcbgkoif.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhoulong.xyz/gtyragrbxa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hnqzz.top/gtvxgdjjuy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.iojbl.cn/gtomcecdpu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shangyingyoupin.top/gtgddjiutw.html

================================================================================
来源：http://hz.cashguo.top/gtfteigvyw.html

B. 流程控制
来源：http://hz.yonumen.top/gtosaeyokz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqqdlcnro.html

[B01] 条件判断 if / else
来源：http://hz.chenjidiqi.icu/gtuhsguhrg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.birdmap.top/gtykhvliam.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.pengpengdd.cyou/gtlutspejp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.haohaochexian.top/gtqizqukgg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtluwguelm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.dianchejie.cn/gtgzzfqqnx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yuxming.cn/gtwtwkiipz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.tianlin.xyz/gtsfjqenxb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hongshengwenyu.top/gtlpbjxmqu.html

[B02] 多分支 else if / elif
来源：http://hz.haohaochexian.top/gtuywibxvt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.ywan-chungtsiang.top/gtyigswmkw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.chenzaomai.com/gtwpqtrbhv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cqqwz.cn/gtcnbohekh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtotcmratw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinghuilouyu.cn/gtpyypoqyi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.0kj1m.cn/gthrayyqsb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.feifeiyinyue.top/gtiopsbzox.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.birdmap.top/gtcmsimvdh.html

[B03] switch / match / case
来源：http://hz.chenjidiqi.icu/gtzeenpssb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xingfuxueyuan.xyz/gtqklowckc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gtefhmysci.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hywenlv.cn/gthqazcvrf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hywenlv.cn/gtbltcjwmh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.mhx1999.top/gtnobhcwrf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ywan-chungtsiang.top/gtgolbdeob.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zycfv.cn/gtujllrwwe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ppjwa.cn/gtrrmaqjqo.html

[B04] for 计数循环
来源：http://hz.nwbrower.top/gtzzeitkrh.html

Py:   for i in range(10): print(i)
来源：http://hz.hysaishi.cn/gtqdcecqdv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.snrcjt.cn/gtzdafsilg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.aibaodan.cn/gtpujmimfa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.feifeiyinyue.top/gtmeehftpb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hywenlv.cn/gttrgrjgnq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhaomingkeji.xyz/gtpsnpemls.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shanyushiyangkeji.top/gtlmtqsvdw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.cucudq.cn/gtjtwfdozh.html

[B05] 遍历数组 / 列表
来源：http://hz.feifeiyinyue.top/gtvfivpqxe.html

Py:   for item in arr: print(item)
来源：http://hz.jyoumei.cn/gthnberblt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.quarkkingdee.top/gtkeszyzlf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yanxiufei.cn/gtnqpozhpv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.daria6918.cn/gtxccmqatm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj202588.top/gtbrrsfbut.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.kuanghao11.cn/gtcrydjqcf.html

Ruby: arr.each { |item| puts item }
来源：http://hz.smart0.xyz/gtlwflllui.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yuxming.cn/gtqzwojcan.html

[B06] 遍历字典 / 对象
来源：http://hz.sufxvd.cn/gtuucgojbm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ivvv.top/gtwurrrzgx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.mhx1999.top/gtylvihzsr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cdnleiting.top/gtpnneubia.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.dashuyun.cn/gtunghsdtq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.dashuyun.cn/gtzreayirr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xylfe.cn/gtescgnryv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenjidiqi.icu/gtkepvxzts.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yvedp.cn/gtbaiyxzmi.html

[B07] while 循环
来源：http://hz.sysykeji.top/gtmpvoriou.html

Py:   while i < 10: i += 1
来源：http://hz.jianghu66.top/gtybkqlgck.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.smart0.xyz/gtxscyaqku.html

JS:   while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtygbemosi.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtvnggmziv.html

Java: while (i < 10) { i++; }
来源：http://hz.sweek.top/gtqnoulikj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yangfankeji.com/gtllpdfdal.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhengqikj.top/gtrfnruiuz.html

C#:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtzmlbeegj.html

[B08] do-while（至少执行一次）
来源：http://hz.shuidangran.top/gtktplpzbe.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.tanke756.top/gtzbkfzclx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jqgfzy.top/gtzydhzpiw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtjykiyzrq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gttmrzlnst.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtvejfsdrk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.dashuyun.cn/gtmvdgcerp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pengpengdd.cyou/gtaoinlfpa.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtitztoziy.html

[B09] break 与 continue
来源：http://hz.nanxuanxn.top/gtmasalduj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sysykeji.top/gtteqicxld.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.tanke756.top/gtmjsmjhum.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtmpghktzo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtthwbvpoe.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtvtrwlmkt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hammf.cn/gtusopmfud.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nanxuanxn.top/gtktlcsfrm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtfddqfssi.html

[B10] 遍历同时拿索引
来源：http://hz.pengpengdd.cyou/gtouvhfqjm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hammf.cn/gtiovysnqa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.meibo888.top/gtquiesmlo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hammf.cn/gtifmlglgm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sweek.top/gtuqjlcbbk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigfzy.top/gtxgjcjnhj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zycfv.cn/gtjfmdyfig.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yvedp.cn/gtqrualdpp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jyoumei.cn/gtmmijcdwc.html

[B11] 生成数字序列 / 区间
来源：http://hz.jianghu66.top/gtmabfltcq.html

Py:   list(range(0, 10, 2))
来源：http://hz.ehwqpu.com/gtqmfbndvg.html

PHP:  range(0, 10, 2);
来源：http://hz.ydzc1.top/gtidoiiast.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zycfv.cn/gttztuaocc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cheryme.top/gtwlcqbnkg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.snrcjt.cn/gtsheetmrh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ppjwa.cn/gtyfdkyern.html

Ruby: (0...10).step(2).to_a
来源：http://hz.dashuyun.cn/gtnsnvxygo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.havefunace.top/gtkylkamkm.html

[B12] 跳出多层循环
来源：http://hz.haohaochexian.top/gtbufnvhgv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenzaomai.com/gtugghcfcd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xylfe.cn/gtxyrsrxyy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtsuzgzwad.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtgdkmxjmw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gthgsxjwzm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yonumen.top/gtmvvmygre.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fzhhl.top/gtgqnlwbue.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yonumen.top/gtstpqfvtq.html

[B13] 判断是否为数字
来源：http://hz.redwolf501.top/gtzafcwmcq.html

Py:   isinstance(x, (int, float))
来源：http://hz.shangyingyoupin.top/gtusdcubde.html

PHP:  is_numeric($x)
来源：http://hz.chenzaomai.com/gtcylojiuv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.316326.xyz/gthmoasxbl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinyuanbaomall.cn/gtojedrxuf.html

Java: x instanceof Number
来源：http://hz.jqgufenzy.top/gtfadjaujl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yangfankeji.com/gthoyzcesu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhiwuduotai.top/gtlsdqxujy.html

C#:   x is int or double or decimal
来源：http://hz.zhixingplan.top/gtikkwwhiy.html

[B14] 判断值是否在集合内
来源：http://hz.wangdashe.top/gtyciniygd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nwbrower.top/gtvqcbbort.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daxiang520.top/gtdkurycsv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gtbfwmqpti.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.svipenyu.cn/gtyardhxgx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cucudq.cn/gtuajfhtdg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yuanzhike.top/gtyvsckmlm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sweek.top/gtdbxvdski.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.guannengcc.top/gtoepxoxlh.html

[B15] 布尔运算与取反
来源：http://hz.hfpthk.cn/gtebrugztj.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtglsngfye.html

PHP:  $a && $b || !$c
来源：http://hz.ydjk.org.cn/gtacugsrvg.html

JS:   a && b || !c
来源：http://hz.jiagoushi.top/gtyzdkmvjl.html

TS:   a && b || !c
来源：http://hz.zdqjudy.top/gtewvzmuyt.html

Java: a && b || !c
来源：http://hz.andypj.xyz/gtqomriwyj.html

Go:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtbzwllzhy.html

Ruby: a && b || !c
来源：http://hz.sysykeji.top/gtfbgtkrdh.html

C#:   a && b || !c
来源：http://hz.aizwys.cn/gthgnbodbc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jianghu66.top/gtvvzyxkhe.html

Py:   if not data: return
来源：http://hz.cqqwz.cn/gttrccobil.html

PHP:  if (!$data) { return; }
来源：http://hz.cucudq.cn/gtcsunvehu.html

JS:   if (!data) return;
来源：http://hz.9152youxi.cn/gtzhhoektd.html

TS:   if (!data) return;
来源：http://hz.jiagoushi.top/gtbxkdkbfa.html

Java: if (data == null) return;
来源：http://hz.zhaomingkeji.xyz/gtdebgfhby.html

Go:   if data == nil { return }
来源：http://hz.gaohongyu789.top/gtuoqeqrzs.html

Ruby: return if data.nil?
来源：http://hz.0kj1m.cn/gtlhtbnrbr.html

C#:   if (data == null) return;
来源：http://hz.daxiang520.top/gtnvmdcyip.html

================================================================================
来源：http://hz.0kj1m.cn/gtebhexvro.html

C. 函数与作用域
来源：http://hz.shanyushiyangtech.top/gtsoyketqi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpwersfaf.html

[C01] 定义函数
来源：http://hz.cucudq.cn/gtbuafbwjg.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtfevcqosd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.smart0.xyz/gtpdzsbplg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gogol.net.cn/gtblbefcck.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtkvwnobfq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtktfergaq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.vqdsnc.cn/gtanejlnam.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnxiangtu.top/gtbowlpfba.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtxifsosvb.html

[C02] 默认参数
来源：http://hz.gaohongyu789.top/gtxlgwuttq.html

Py:   def greet(name="World"): return name
来源：http://hz.zhixingplan.top/gtkquijrmw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.gogol.net.cn/gtxfuzscxb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hammf.cn/gtotovwkvh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gtssabiind.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangdashe.top/gtirrnhquy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ydjk.org.cn/gtibdzldql.html

Ruby: def greet(name = "World") = name
来源：http://hz.yuxming.cn/gtvyngbycr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cqqwz.cn/gtpfhpnxua.html

[C03] 可变参数
来源：http://hz.jinqigufen.top/gtmovwfyap.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gtqsmdvtjk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gtqkeyerjc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gogol.net.cn/gtzhqkvwcq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtcwiiilff.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zdqjudy.top/gtrssharhz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.0kj1m.cn/gtwaftyxqt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.0kj1m.cn/gtlwlcndxe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtrwjircdg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.smart0.xyz/gtnuurbmpg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtivczlmxq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gtaincvvbu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cucudq.cn/gtarbkpnzk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cqqwz.cn/gtkuyntmus.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cqqwz.cn/gtmthjpwao.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenzaomai.com/gthgrxspez.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jiagoushi.top/gtmhjjzhyb.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtegcujbca.html

[C05] 返回多个值
来源：http://hz.feifeiyinyue.top/gttqnjtnpd.html

Py:   return a, b
来源：http://hz.316326.xyz/gtvxgztnjo.html

PHP:  return [$a, $b];
来源：http://hz.fzhhl.top/gtnwqtswiy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhiwuduotai.top/gtkxiysppc.html

TS:   return { a, b };
来源：http://hz.ppjwa.cn/gthozvjtss.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenjidiqi.icu/gtghripbuo.html

Go:   return a, b
来源：http://hz.ydzc1.top/gtnpxsewhy.html

Ruby: return a, b
来源：http://hz.aibaodan.cn/gtbeswmfeq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.quarkkingdee.top/gtzmigyjvr.html

[C06] 匿名函数 / lambda
来源：http://hz.shanyushiyangkeji.top/gtuykpawnq.html

Py:   square = lambda x: x * x
来源：http://hz.meibo888.top/gtrrpjhnnc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zycfv.cn/gtxprwgokk.html

JS:   const square = x => x * x;
来源：http://hz.kuanghao11.cn/gthhxzonke.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ydjk.org.cn/gtuhgvcwaq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cqqwz.cn/gtuehnvsbf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jlsjyb.cn/gtpumjhjyv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sysykeji.top/gtwpqxbkql.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.dashuyun.cn/gtgwxyjbxt.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtuwgtrjns.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cheryme.top/gtclpgwijs.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhaomingkeji.xyz/gticonjloq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxinkj.top/gtbnqzygrp.html

TS:   arr.map(String)
来源：http://hz.zhiwuduotai.top/gtlfskrivx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yanxiufei.cn/gtnjczhlrz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.0kj1m.cn/gtaziyamgg.html

Ruby: arr.map(&:upcase)
来源：http://hz.nanxuanxn.top/gtrkzqbmai.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenlongwang.top/gtxwrstosk.html

[C08] 闭包
来源：http://hz.zhijiandao.cn/gtzeazvbbn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gzhubu.top/gtnlcsarov.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jlsjyb.cn/gtlyehxmvc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtjwihkaio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gtxfguykqn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtzreuyxwi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yueranfly.top/gtstdfojxl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.dashuyun.cn/gtwspmyjys.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtwyvseezs.html

[C09] 递归
来源：http://hz.hnqzz.top/gthbyywbqt.html


<!-- 参考信息 -->