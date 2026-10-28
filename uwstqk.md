代发 wailian999

[A22] 获取字符串长度
来源：http://hz.vqdsnc.cn/gtwqtvxdnp.html

Py:   len(s)
来源：http://hz.tianlin.xyz/gtytxhaqzv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.sysykeji.top/gtudblfsvp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.c1oappe.top/gtrydiyftj.html

TS:   s.length
来源：http://hz.yj20258.top/gtvhdnodec.html

Java: s.length()
来源：http://hz.shuidangran.top/gtkfwncsxk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.hfpthk.cn/gtmpdbzgan.html

Ruby: s.length
来源：http://hz.haohaochexian.top/gtenmhvkaa.html

C#:   s.Length
来源：http://hz.shuidangran.top/gtardsmxin.html

[A23] 大小写转换
来源：http://hz.jinyuanbaomall.cn/gtxmhlfual.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yvedp.cn/gtvdhxummn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.dashuyun.cn/gtwdrhjjoj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.c1oappe.top/gtygehzweb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hnxiangtu.top/gtfuomvlrc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shzxlz.cn/gtkbbqdluw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.andypj.xyz/gtgacbaxvr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ydzc1.top/gtexdpfrlv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zycfv.cn/gtlqwvuykr.html

[A24] 去除首尾空白
来源：http://hz.yongpay.top/gtjrisxaxs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ybcxt.top/gtossrvido.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.gotoacloud.top/gtdequxmzu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zdqjudy.top/gtzizhbbwk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ehwqpu.com/gtrcqtipve.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xziqi.cn/gtcedvjkcg.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhixingplan.top/gtovlhknxc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.mhx1999.top/gtjvaetsch.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hysaishi.cn/gtozuwbqif.html

[A25] 字符串比较
来源：http://hz.xinyue.icu/gttgatrbzf.html

Py:   s1 == s2; s1 != s2
来源：http://hz.mhx1999.top/gtuufsqwep.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.gogol.net.cn/gtiklmhifb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydjk.org.cn/gtskejfeaa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aizwys.cn/gtzfazovaa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shzxlz.cn/gtqyejqcoj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yueranfly.top/gttoowahfg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hywenlv.cn/gtkuvdfycs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gtvedwtymd.html

[A26] 类型转换总览
来源：http://hz.xylfe.cn/gtfshoxtmf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yvedp.cn/gtytgjqvnc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yuxming.cn/gtkgzrfydv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cdnleiting.top/gterlwtguo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.c1oappe.top/gttuzeyqea.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cdnleiting.top/gtgszjtjnx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.aibaodan.cn/gtgcbyquvz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.0kj1m.cn/gtushawaua.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zycfv.cn/gtlosxnmyt.html

================================================================================
来源：http://hz.0kj1m.cn/gtamgolcyv.html

B. 流程控制
来源：http://hz.sufxvd.cn/gtqxlharbi.html

================================================================================
来源：http://hz.52xcode.cn/gtndycpoly.html

[B01] 条件判断 if / else
来源：http://hz.xziqi.cn/gthrwxwsvs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhongyouzk.top/gtbxtthvri.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yvedp.cn/gttafmxrfp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtdmufrpfc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.chenlongwang.top/gtqxhndksb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yangfankeji.com/gtspzcoayr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yanxiufei.cn/gtxzaqxyzn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.wangdashe.top/gtncbnlymh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtoikopiwl.html

[B02] 多分支 else if / elif
来源：http://hz.9152youxi.cn/gtwuymufwd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.xingfuxueyuan.xyz/gtlozqlwvv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jinqigfzy.top/gtwuzozfpb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigfzy.top/gtgjpjcdxs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtmfikcskl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhixingplan.top/gtxzavmqqz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.havefunace.top/gttkktwplf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.cucudq.cn/gtwisuyigx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtfbptfwwi.html

[B03] switch / match / case
来源：http://hz.xinyue.icu/gtkrfosmef.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.0kj1m.cn/gtnzcjydfd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yongpay.top/gtjxginsdk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.kuanghao11.cn/gtuthowdwu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhixingplan.top/gtfncwfcjj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yonumen.top/gtcmcapjsr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.mhx1999.top/gtpopxihwr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.havefunace.top/gttizizvlv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yonumen.top/gtstzjnrnz.html

[B04] for 计数循环
来源：http://hz.cdnleiting.top/gtszepzzib.html

Py:   for i in range(10): print(i)
来源：http://hz.yuanzhike.top/gtyigkaoxn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.quarkkingdee.top/gtsxewdiqg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtcjevrrlh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.316326.xyz/gtikqwtgmq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhixingplan.top/gtjwturojj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.9152youxi.cn/gtbczgogal.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jyoumei.cn/gtiaxyxzwj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hongshengwenyu.top/gtzgwnfhtm.html

[B05] 遍历数组 / 列表
来源：http://hz.jiagoushi.top/gtnscsrtdy.html

Py:   for item in arr: print(item)
来源：http://hz.cashguo.top/gtakovwfzb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.snrcjt.cn/gtburajkce.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj20258.top/gtbixfmqli.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gteyadhebq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.svipenyu.cn/gtdkmjtgln.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xziqi.cn/gtejxpdqje.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shuidangran.top/gtipncsnik.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.fengsongda.top/gtomcwblob.html

[B06] 遍历字典 / 对象
来源：http://hz.sufxvd.cn/gtmrbvbphc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.tianlin.xyz/gtsuykpfwl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yongpay.top/gtdtfspkiy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yongpay.top/gtxrxhesxj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jlsjyb.cn/gtcefngdku.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cheryme.top/gtxyktfsns.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.svipenyu.cn/gtuxrnuczz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yuxming.cn/gtfnnsjrjz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xziqi.cn/gtekswiweh.html

[B07] while 循环
来源：http://hz.cucudq.cn/gttjrsboyl.html

Py:   while i < 10: i += 1
来源：http://hz.316326.xyz/gtnevttjvb.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.dianchejie.cn/gtphjhtidn.html

JS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtnidloxmo.html

TS:   while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtxpiwbvob.html

Java: while (i < 10) { i++; }
来源：http://hz.yonumen.top/gthsvayagl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jyoumei.cn/gtxporznhi.html

Ruby: while i < 10; i += 1; end
来源：http://hz.nwbrower.top/gtkfphvfdn.html

C#:   while (i < 10) { i++; }
来源：http://hz.bjfxy.top/gtqepuqovc.html

[B08] do-while（至少执行一次）
来源：http://hz.zhoulong.xyz/gtxlbcvvxy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jqgfzy.top/gtmdvrcbaw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yuanzhike.top/gtbxyzynra.html

JS:   do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtujuxkqbg.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtcfpjhnng.html

Java: do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gtlsygwevz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ppjwa.cn/gttiscavls.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hywenlv.cn/gtdwokbwhq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtawlvetky.html

[B09] break 与 continue
来源：http://hz.yangfankeji.com/gtooweiayk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gaohongyu789.top/gtyrvodmgn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhaomingkeji.xyz/gtgatfpdeu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhijiandao.cn/gtqrrmfqye.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtztltfvww.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtvkjgfvra.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nwbrower.top/gtaxhpcjsv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.tianlin.xyz/gtuxllxxxx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtxrgqefzy.html

[B10] 遍历同时拿索引
来源：http://hz.jinyuanbaomall.cn/gtehyzopas.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shanyushiyangkeji.top/gtgcmaifbt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ydjk.org.cn/gtmatcdkwi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.c1oappe.top/gtaquythfn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gtvxwdpqpr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.tanke756.top/gtmrnhcycw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xingfuxueyuan.xyz/gtnczkpvrf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yvedp.cn/gtprnecosl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.iojbl.cn/gtjfvqybae.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinqigfzy.top/gttlisryje.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgufenzy.top/gtqmqijlot.html

PHP:  range(0, 10, 2);
来源：http://hz.sysykeji.top/gtjjcvzjgy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhijiandao.cn/gtqfjyqqbp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jlsjyb.cn/gtltipevgh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hammf.cn/gtxfmwjgey.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.redwolf501.top/gttrwcytdn.html

Ruby: (0...10).step(2).to_a
来源：http://hz.0kj1m.cn/gtamfxjbqk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yueranfly.top/gttnykrkld.html

[B12] 跳出多层循环
来源：http://hz.fengsongda.top/gtycsaatsp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.andypj.xyz/gtmrjjhnog.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnqzz.top/gtsoemjxrv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fzhhl.top/gtxicqqjvw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtrmxmaota.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtudbzypyb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhijiandao.cn/gtublpzuxf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.daxiang520.top/gttesckttg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhixingplan.top/gtdiqwctar.html

[B13] 判断是否为数字
来源：http://hz.nanxuanxn.top/gthlhprxtr.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtnmkeqfgb.html

PHP:  is_numeric($x)
来源：http://hz.birdmap.top/gtrdttsjmo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhongyouzk.top/gtigbngqgy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtvjlaylsd.html

Java: x instanceof Number
来源：http://hz.dianchejie.cn/gtrmjajcha.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuetiantiany.cn/gtfnytthmp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ybcxt.top/gtkjivxlob.html

C#:   x is int or double or decimal
来源：http://hz.cashguo.top/gtwmscopgy.html

[B14] 判断值是否在集合内
来源：http://hz.yonumen.top/gtjhukuiok.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sysykeji.top/gtairyxcwd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.meibo888.top/gtqcnwgrrg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.pengpengdd.cyou/gttlkitxvh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtaatncard.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cqqwz.cn/gtczbnkqts.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.bjfxy.top/gtslqwtwhq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sxryk.cn/gtmuldyhvd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.andypj.xyz/gtfyskfevw.html

[B15] 布尔运算与取反
来源：http://hz.yueranfly.top/gtemxssnwo.html

Py:   a and b or not c
来源：http://hz.chenlongwang.top/gtwlcwgyon.html

PHP:  $a && $b || !$c
来源：http://hz.shzxlz.cn/gtrsrtuxzf.html

JS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtblbxtpva.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gtjyljgywi.html

Java: a && b || !c
来源：http://hz.dashuyun.cn/gteqjwtyoj.html

Go:   a && b || !c
来源：http://hz.ydjk.org.cn/gtjpzhgyde.html

Ruby: a && b || !c
来源：http://hz.yj20258.top/gtdfdqdsbw.html

C#:   a && b || !c
来源：http://hz.quarkkingdee.top/gtahykudul.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtbvpegfgq.html

Py:   if not data: return
来源：http://hz.tian-w.cn/gtmkwzzbwp.html

PHP:  if (!$data) { return; }
来源：http://hz.vqdsnc.cn/gtqvzvdfio.html

JS:   if (!data) return;
来源：http://hz.yueranfly.top/gtotwjxtpa.html

TS:   if (!data) return;
来源：http://hz.yj20258.top/gtyprxjulz.html

Java: if (data == null) return;
来源：http://hz.zdqjudy.top/gtdrmfnzaw.html

Go:   if data == nil { return }
来源：http://hz.cucudq.cn/gtklfsrmhn.html

Ruby: return if data.nil?
来源：http://hz.iojbl.cn/gtokkhygul.html

C#:   if (data == null) return;
来源：http://hz.yj20258888.top/gtvtfomncd.html

================================================================================
来源：http://hz.sufxvd.cn/gtlhrqrszf.html

C. 函数与作用域
来源：http://hz.sufxvd.cn/gtaogtzrxw.html

================================================================================
来源：http://hz.meibo888.top/gtcncvvewr.html

[C01] 定义函数
来源：http://hz.pengpengdd.cyou/gtxvjulcum.html

Py:   def add(a, b): return a + b
来源：http://hz.c1oappe.top/gtdqkpwpjf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtccmcusfe.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cashguo.top/gtgtpmgwsz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ivvv.top/gtteeytmkt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtrrhiyfee.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hfpthk.cn/gtlwnjveqh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.snrcjt.cn/gtfcxmotps.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtrgveeyyq.html

[C02] 默认参数
来源：http://hz.hywenlv.cn/gtdfvpfgbw.html

Py:   def greet(name="World"): return name
来源：http://hz.52xcode.cn/gtxlwsdixy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tian-w.cn/gtmfzzoehy.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gotoacloud.top/gtynxqejfw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ppjwa.cn/gtqynlpoon.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnxiangtu.top/gtqvgsuicl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guannengcc.top/gtwysskdev.html

Ruby: def greet(name = "World") = name
来源：http://hz.xuetiantiany.cn/gtjmfmbkgl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gtvszasmlh.html

[C03] 可变参数
来源：http://hz.hammf.cn/gtmfytfhxv.html

Py:   def total(*args): return sum(args)
来源：http://hz.gogol.net.cn/gthbxysrmf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhixingplan.top/gtearnigqu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gttrkmycmj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhijiandao.cn/gtsdwnfeoc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yuanzhike.top/gtsrvsfkuf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ybcxt.top/gttkijduug.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuanzx.com/gtprggoewp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtygpufoiw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj20258.top/gtbkmwnuxg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jyoumei.cn/gtckqznglw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yongpay.top/gtpzirrqta.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtcafaupni.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xziqi.cn/gtgczcyrxj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.wangshuangyany.cn/gtbjcaipwm.html

Go:   // 无：用配置结构体参数
来源：http://hz.daxiang520.top/gtrymelfzb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtbuftkbrp.html

C#:   f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtahzwmasm.html

[C05] 返回多个值
来源：http://hz.52xcode.cn/gtymsownup.html

Py:   return a, b
来源：http://hz.zhongyouzk.top/gtberxxntu.html

PHP:  return [$a, $b];
来源：http://hz.zhaomingkeji.xyz/gtuevirxmb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.kuanghao11.cn/gtcsqfxxdl.html

TS:   return { a, b };
来源：http://hz.tianlin.xyz/gtfzblinea.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtakvulwjz.html

Go:   return a, b
来源：http://hz.tian-w.cn/gtrpcsyadq.html

Ruby: return a, b
来源：http://hz.hongshengwenyu.top/gttxkuhwov.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yanxiufei.cn/gtlflxoyfy.html

[C06] 匿名函数 / lambda
来源：http://hz.gotoacloud.top/gtdgldcwxt.html

Py:   square = lambda x: x * x
来源：http://hz.0kj1m.cn/gtpmhuxpyf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.c1oappe.top/gtzzfvjboj.html

JS:   const square = x => x * x;
来源：http://hz.jinghuilouyu.cn/gtvfejopwa.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhengqikj.top/gtfkakvnwl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xingfuxueyuan.xyz/gtvwijgisf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.vqdsnc.cn/gtsrjlpajm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.wangshuangyany.cn/gtkhxhzpdt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ehwqpu.com/gtimmbumkd.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtznkzvinh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ivvv.top/gtqdwcvelw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ivvv.top/gtxplvyivg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yonumen.top/gtahngnrjo.html

TS:   arr.map(String)
来源：http://hz.guannengcc.top/gthuukcrux.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hysaishi.cn/gtwtfihwmm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aizwys.cn/gtrpwwebqv.html

Ruby: arr.map(&:upcase)
来源：http://hz.fengsongda.top/gtuzjwiezr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.0kj1m.cn/gtawhrdmsh.html

[C08] 闭包
来源：http://hz.jianghu66.top/gtcjpmnunh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.redwolf501.top/gtgtkxevhc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtuhncgmse.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xuanzx.com/gtxxqktdje.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtlblftetn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.guowangkeji.top/gtpcjnxoqr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhixingplan.top/gtpexzwjnu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.feifeiyinyue.top/gtmuafaueg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtdhjkwcem.html

[C09] 递归
来源：http://hz.gaohongyu789.top/gtkpclmhrk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhiwuduotai.top/gtsxdjzhgd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gotoacloud.top/gtgnlrayvj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangtech.top/gtbqqvxmaw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangshuangyany.cn/gtcsaqzyvb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hammf.cn/gtvsxomajj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jiagoushi.top/gtexzxsypl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtazbvylfj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.9152youxi.cn/gthrvolnsg.html

[C10] 变量作用域
来源：http://hz.andypj.xyz/gtuzihvube.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ppjwa.cn/gtydeepjuf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.feifeiyinyue.top/gtdmfrbwqd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cdnleiting.top/gtsttwwits.html

TS:   同 JS
来源：http://hz.gotoacloud.top/gtysyoklad.html

Java: 方法内为块级作用域
来源：http://hz.zycfv.cn/gttcfdpghb.html

Go:   花括号块级作用域
来源：http://hz.sysykeji.top/gtzppaotja.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.52xcode.cn/gtookbztyu.html

C#:   块级作用域
来源：http://hz.jlsjyb.cn/gtpipmyfuk.html

[C11] 模块导入与导出
来源：http://hz.xinyue.icu/gtvcluzpny.html

Py:   from module import func
来源：http://hz.shanyushiyangkeji.top/gtsoofdqhm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dianchejie.cn/gtfjkxasvw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuetiantiany.cn/gtwvluyfpd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ppjwa.cn/gtjuuyhynv.html

Java: import java.util.List;
来源：http://hz.gaohongyu789.top/gthrundupv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.feifeiyinyue.top/gtajgbrnwa.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gtotbemmsd.html

C#:   using System.Text;
来源：http://hz.sweek.top/gtqminefmi.html

[C12] 立即执行函数 IIFE
来源：http://hz.aizwys.cn/gtyqcmjuwc.html

Py:   (lambda: print("run"))()
来源：http://hz.0kj1m.cn/gthzelxhyl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.dianchejie.cn/gtjdqaiuaj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtdyomicuf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtlbgmkhyh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tianlin.xyz/gtptdoahap.html


<!-- 参考信息 -->