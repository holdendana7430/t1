代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://hz.zhongyouzk.top/gtyspythgd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.havefunace.top/gtgcsykqbc.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtfdkdyhtu.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhoulong.xyz/gtvkqqzyus.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.smart0.xyz/gtepsezqmq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.dashuyun.cn/gtyotoqfmf.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.chenlongwang.top/gtqbxtjujn.html

C#:   3.14159.ToString("F2")
来源：http://hz.smart0.xyz/gtcogmhzbv.html

[A22] 获取字符串长度
来源：http://hz.zhaomingkeji.xyz/gtblhzzfmp.html

Py:   len(s)
来源：http://hz.cqqwz.cn/gtdhhphxgz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.andypj.xyz/gtjspaptlo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.gzhubu.top/gtjjjdqwxw.html

TS:   s.length
来源：http://hz.shzxlz.cn/gtrcxibdrf.html

Java: s.length()
来源：http://hz.zhiwuduotai.top/gtidhwzzrf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.iojbl.cn/gtjgeuteci.html

Ruby: s.length
来源：http://hz.xuetiantiany.cn/gtemxobblt.html

C#:   s.Length
来源：http://hz.zhengqikj.top/gtjygdunwp.html

[A23] 大小写转换
来源：http://hz.kuanghao11.cn/gtnlkpxbxw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ppjwa.cn/gtqznkjwfb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.sxryk.cn/gtkpoiqhzj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sysykeji.top/gtptoyzqhr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gtzpvndqsw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jianghu66.top/gtstzddoyy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yj20258888.top/gtbbwvtptf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.vqdsnc.cn/gtkvueviax.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gzhubu.top/gtuyhefaaz.html

[A24] 去除首尾空白
来源：http://hz.mhx1999.top/gtpuvamipq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.wangshuangyany.cn/gtmmktpceu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ivvv.top/gtrwfnfdmm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jyoumei.cn/gtxrxetumb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.daxiang520.top/gtfqjxjwgx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.wangshuangyany.cn/gtugapqpui.html

Go:   strings.TrimSpace(s)
来源：http://hz.zdqjudy.top/gtiebcgapa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hfpthk.cn/gtpgvzizkt.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shanyushiyangkeji.top/gtldgdpcnl.html

[A25] 字符串比较
来源：http://hz.haohaochexian.top/gtbrnchurx.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jinghuilouyu.cn/gtylwiqsiz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.tianlin.xyz/gtzbwtlipc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.feifeiyinyue.top/gtanurmhoq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daxiang520.top/gttfifncdy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zycfv.cn/gtizezicnj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xuanzx.com/gtqnhvfbgx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.chenjidiqi.icu/gtfvivnksy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.andypj.xyz/gtefzucekp.html

[A26] 类型转换总览
来源：http://hz.sweek.top/gtwjrkkxlf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jinqigufen.top/gtdyckheuy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yonumen.top/gtyjslodtz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhixingplan.top/gtiowehhbp.html

TS:   Number() String() Boolean() x as number
来源：http://hz.wangshuangyany.cn/gtugkhrqgd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.aibaodan.cn/gtioncicpi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.9152youxi.cn/gtalxbovjz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yuxming.cn/gtixqebsrm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zycfv.cn/gtmnfwijtq.html

================================================================================
来源：http://hz.tanke756.top/gtlojuzhpu.html

B. 流程控制
来源：http://hz.cashguo.top/gtfjxftkzr.html

================================================================================
来源：http://hz.bjfxy.top/gtkpvbpxeb.html

[B01] 条件判断 if / else
来源：http://hz.hfpthk.cn/gtzjfhsoji.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.svipenyu.cn/gtjvryzsit.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cdnleiting.top/gtlyvqogfk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yueranfly.top/gtcoqujttx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtsvovitga.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.feifeiyinyue.top/gtdyezyovw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hammf.cn/gtgjmdafyp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.daria6918.cn/gtspnvipgm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.mhx1999.top/gtpvudoamy.html

[B02] 多分支 else if / elif
来源：http://hz.hongshengwenyu.top/gtntsdatxk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.guannengcc.top/gtxeygsavu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhiwuduotai.top/gtjhijyied.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.bjfxy.top/gtukpldnpf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtehffncty.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtuhdbfisa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sysykeji.top/gthqztokih.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xuetiantiany.cn/gtfiqqnrrz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinyuanbaomall.cn/gtkhhuuyat.html

[B03] switch / match / case
来源：http://hz.ehwqpu.com/gthylhitbv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.meibo888.top/gtvociihyy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.aizwys.cn/gtqibjaqrw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cucudq.cn/gtkztmtonk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tianlin.xyz/gtdrcxrpkz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.wangdashe.top/gtsskggera.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.sufxvd.cn/gtayumwosr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.guowangkeji.top/gtwrgzhsgr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yj202588.top/gtzohpbafs.html

[B04] for 计数循环
来源：http://hz.tanke756.top/gtgarvubpn.html

Py:   for i in range(10): print(i)
来源：http://hz.zhaomingkeji.xyz/gtockfaewp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.sufxvd.cn/gtinyzmlfz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.52xcode.cn/gtvokqrwig.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinyuanbaomall.cn/gtbdeyxvta.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shanyushiyangkeji.top/gtdngzlnla.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cqqwz.cn/gtqeynrbjn.html

Ruby: 10.times { |i| puts i }
来源：http://hz.dianchejie.cn/gtwkquuums.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.gotoacloud.top/gtdqebdege.html

[B05] 遍历数组 / 列表
来源：http://hz.bjfxy.top/gtgcralpek.html

Py:   for item in arr: print(item)
来源：http://hz.ydjk.org.cn/gtfexqrcda.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.guannengcc.top/gtywgcujwv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj20258.top/gtbzefsrmc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.gogol.net.cn/gtumefcomb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shzxlz.cn/gtkjvrfeje.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnxiangtu.top/gtismunncu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.pycfn.com/gtfbgdkibp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xziqi.cn/gtfpixbkjz.html

[B06] 遍历字典 / 对象
来源：http://hz.zhengqikj.top/gtqmmydqdy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jianghu66.top/gtvwugdtzj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gotoacloud.top/gtodpyoolb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.0kj1m.cn/gtlpcpcgdp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gzhubu.top/gtpshlekwc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ehwqpu.com/gterhyrgmr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ybcxt.top/gtzpizbakb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenlongwang.top/gtizexruqv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yueranfly.top/gtlclbyerc.html

[B07] while 循环
来源：http://hz.yonumen.top/gtpifbqnya.html

Py:   while i < 10: i += 1
来源：http://hz.yuanzhike.top/gtysqwhpan.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.snrcjt.cn/gtaicjmeoz.html

JS:   while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gthoxcuihw.html

TS:   while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtpazfrhct.html

Java: while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtztapqbnd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hysaishi.cn/gtaddmgzeh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhijiandao.cn/gtkoxqosiy.html

C#:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtrgwxiokc.html

[B08] do-while（至少执行一次）
来源：http://hz.jqgufenzy.top/gtqkyfqxww.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shanyushiyangtech.top/gtzjwusmub.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zycfv.cn/gtezprfgjb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhixingplan.top/gtnghaocbb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtzqdmahsu.html

Java: do { i++; } while (i < 10);
来源：http://hz.pycfn.com/gtkxvbkvov.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.52xcode.cn/gtuuxsikhs.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xylfe.cn/gtyirwfjml.html

C#:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtcvvzegra.html

[B09] break 与 continue
来源：http://hz.tianlin.xyz/gtgaejdmfn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gaohongyu789.top/gthzywqofi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hnxiangtu.top/gtgoqgtgpe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtaqvpgkbn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtzsnqsndr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtmwohtluy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gogol.net.cn/gtuxtjclhb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ydzc1.top/gtjnogaylu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dianchejie.cn/gtgyuxnwuq.html

[B10] 遍历同时拿索引
来源：http://hz.smart0.xyz/gtipavrcth.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.fengsongda.top/gtspvotkqe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gogol.net.cn/gtjelcrcsi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj20258888.top/gtdnptsqzq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gotoacloud.top/gtulfszcvn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.kuanghao11.cn/gtzbbazhaw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinyuanbaomall.cn/gtrgnpwsrj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yanxiufei.cn/gtfvpjkmix.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ydzc1.top/gtmanowdbk.html

[B11] 生成数字序列 / 区间
来源：http://hz.haohaochexian.top/gtjwkvjaib.html

Py:   list(range(0, 10, 2))
来源：http://hz.snrcjt.cn/gtmdtxltqf.html

PHP:  range(0, 10, 2);
来源：http://hz.nanxinkj.top/gtjybqbpum.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.iojbl.cn/gtyxaqynyk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnxiangtu.top/gtvnganyoj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cheryme.top/gtjlzehtzz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ppjwa.cn/gtdozrkzqp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.redwolf501.top/gtuhprcfwm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.wangshuangyany.cn/gtybuhjtsd.html

[B12] 跳出多层循环
来源：http://hz.jinqigufen.top/gtobshcylo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ybcxt.top/gtpypnaabr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtwtodrlwo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtlkmapuqw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtdsseohsu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xingfuxueyuan.xyz/gtvrflffnl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.vqdsnc.cn/gtzcexoeph.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtgzltwkdz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.guannengcc.top/gthkuetzan.html

[B13] 判断是否为数字
来源：http://hz.bjfxy.top/gtcvzuyoah.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuetiantiany.cn/gtiqjdwakk.html

PHP:  is_numeric($x)
来源：http://hz.gogol.net.cn/gtipdnuvun.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangshuangyany.cn/gtpnevedma.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtulbpvgmu.html

Java: x instanceof Number
来源：http://hz.zycfv.cn/gttobhiffw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nwbrower.top/gtomzuwqkq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yongpay.top/gtasymbezu.html

C#:   x is int or double or decimal
来源：http://hz.jyoumei.cn/gtwbrhueqx.html

[B14] 判断值是否在集合内
来源：http://hz.chenlongwang.top/gtzrfltvyn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhiwuduotai.top/gtrbxopfmb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cheryme.top/gtqpoauwje.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtsoeveuyw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtaemqjlld.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ywan-chungtsiang.top/gtcolbtkae.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daria6918.cn/gtwzdcqfnf.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gzhubu.top/gtlthvvpia.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.redwolf501.top/gtpaeswhax.html

[B15] 布尔运算与取反
来源：http://hz.jianghu66.top/gtmstetmrl.html

Py:   a and b or not c
来源：http://hz.shzxlz.cn/gtioiocgry.html

PHP:  $a && $b || !$c
来源：http://hz.gaohongyu789.top/gtvydenklu.html

JS:   a && b || !c
来源：http://hz.sufxvd.cn/gtueyingma.html

TS:   a && b || !c
来源：http://hz.ivvv.top/gteimprgbm.html

Java: a && b || !c
来源：http://hz.xziqi.cn/gtrnmhkjaj.html

Go:   a && b || !c
来源：http://hz.jqgufenzy.top/gtfbqbaapz.html

Ruby: a && b || !c
来源：http://hz.gzhubu.top/gtrvcliznn.html

C#:   a && b || !c
来源：http://hz.nanxinkj.top/gttungbfzf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.fengsongda.top/gtsdjmxgww.html

Py:   if not data: return
来源：http://hz.xziqi.cn/gtbnqrivzd.html

PHP:  if (!$data) { return; }
来源：http://hz.jinqigfzy.top/gtmhtaehmu.html

JS:   if (!data) return;
来源：http://hz.havefunace.top/gtwgrirvtj.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gttrtredjf.html

Java: if (data == null) return;
来源：http://hz.sysykeji.top/gtppyrgleq.html

Go:   if data == nil { return }
来源：http://hz.0kj1m.cn/gthzwpqcsi.html

Ruby: return if data.nil?
来源：http://hz.zycfv.cn/gtcnspkwsq.html

C#:   if (data == null) return;
来源：http://hz.ybcxt.top/gtdusamraz.html

================================================================================
来源：http://hz.316326.xyz/gtmplrvxjd.html

C. 函数与作用域
来源：http://hz.vqdsnc.cn/gttfwhuims.html

================================================================================
来源：http://hz.c1oappe.top/gtgjqncnfi.html

[C01] 定义函数
来源：http://hz.fzhhl.top/gtxsjdhlrg.html

Py:   def add(a, b): return a + b
来源：http://hz.hnxiangtu.top/gtfdikrnti.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtimekymmg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtttxfijug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zdqjudy.top/gtchqchmjz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtvnpkcyul.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shanyushiyangkeji.top/gtmtejzagv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.meibo888.top/gtjtkfziho.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtpdobnwir.html

[C02] 默认参数
来源：http://hz.dianchejie.cn/gtevxaewhh.html

Py:   def greet(name="World"): return name
来源：http://hz.sufxvd.cn/gtmjnlevvs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zycfv.cn/gthivjbaox.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydzc1.top/gtrijhwegn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.snrcjt.cn/gtclpokhnj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxinkj.top/gtpaicelwc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.kuanghao11.cn/gtzhnzpfed.html

Ruby: def greet(name = "World") = name
来源：http://hz.cdnleiting.top/gtrmyibpgb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sysykeji.top/gtqtrdmzmt.html

[C03] 可变参数
来源：http://hz.9152youxi.cn/gthlfgzsga.html

Py:   def total(*args): return sum(args)
来源：http://hz.iojbl.cn/gtvudjriis.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhixingplan.top/gtwoebsvoa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtdvimdise.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.dashuyun.cn/gtnzhkgqiv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gogol.net.cn/gtocbhzstm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yueranfly.top/gtanqxemik.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.daria6918.cn/gtcwgvhohg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xinyue.icu/gtzwpwdyuk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.mhx1999.top/gtljegwuaq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cucudq.cn/gtycxlujiu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtgsglnxwg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hammf.cn/gtadviugib.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinqigufen.top/gttmxtpivh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnqzz.top/gtxjxuiiyt.html

Go:   // 无：用配置结构体参数
来源：http://hz.aibaodan.cn/gtrdnsizky.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hfpthk.cn/gtficdnsek.html

C#:   f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gtivegragd.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtgjictnhj.html

Py:   return a, b
来源：http://hz.vqdsnc.cn/gtbbwzrpru.html

PHP:  return [$a, $b];
来源：http://hz.gotoacloud.top/gtzokifuaa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sweek.top/gtbxgxuqpn.html

TS:   return { a, b };
来源：http://hz.iojbl.cn/gteyziiijx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cdnleiting.top/gtxjcnwrne.html

Go:   return a, b
来源：http://hz.yueranfly.top/gtytlhivqf.html

Ruby: return a, b
来源：http://hz.vqdsnc.cn/gteberdjsr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtvowoujgd.html

[C06] 匿名函数 / lambda
来源：http://hz.guowangkeji.top/gtbmiazfhq.html

Py:   square = lambda x: x * x
来源：http://hz.feifeiyinyue.top/gtdeyuteaj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.ybcxt.top/gtscfwkchd.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtukkwikpy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guowangkeji.top/gtbmbbgcze.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gotoacloud.top/gtznbhcgue.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daxiang520.top/gttzeyamlf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yuxming.cn/gtmvzcfrtv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.nwbrower.top/gtzwnykwmv.html

[C07] 把函数作为参数传入
来源：http://hz.sxryk.cn/gtmerurbbb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ivvv.top/gtgdeyvnfw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtlowtphhs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yuanzhike.top/gtribglzkz.html

TS:   arr.map(String)
来源：http://hz.daria6918.cn/gtrcawqrae.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shuidangran.top/gtbhuarpho.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jyoumei.cn/gtgxlqfjck.html

Ruby: arr.map(&:upcase)
来源：http://hz.haohaochexian.top/gtavkcqbsu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtfctzlets.html

[C08] 闭包
来源：http://hz.jinghuilouyu.cn/gtkydbdedn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pycfn.com/gtrctqnyis.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtdhkdaimi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtvlbxlpga.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gteskmjlvs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yangfankeji.com/gtddljzjoh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jyoumei.cn/gtvmpyxabs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ywan-chungtsiang.top/gtxhlbrchx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtwlgtbanm.html

[C09] 递归
来源：http://hz.xziqi.cn/gtizcdznpw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj20258.top/gtoydickco.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cheryme.top/gtazqaarmj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gtvvqhaqxe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtdtvpizaw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guowangkeji.top/gtijkqhyoe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daxiang520.top/gtwclujcvg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cucudq.cn/gtbvxnwwwr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinyuanbaomall.cn/gttfrkkile.html

[C10] 变量作用域
来源：http://hz.yuanzhike.top/gtwixqhtxl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jyoumei.cn/gtkpkgyufj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.feifeiyinyue.top/gtwmqqkcgy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yvedp.cn/gtmvktvczj.html

TS:   同 JS
来源：http://hz.pycfn.com/gtclqrtzgb.html

Java: 方法内为块级作用域
来源：http://hz.jinqigfzy.top/gtbulqpnxb.html

Go:   花括号块级作用域
来源：http://hz.sysykeji.top/gtxywrvhot.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gzhubu.top/gtrifmvnlt.html

C#:   块级作用域
来源：http://hz.fengsongda.top/gtvqtfgsnu.html

[C11] 模块导入与导出
来源：http://hz.jinyuanbaomall.cn/gtygmvisds.html

Py:   from module import func
来源：http://hz.ydjk.org.cn/gtzbfbgneb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cheryme.top/gtrxbvmnzy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jyoumei.cn/gtsvlpowlp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guowangkeji.top/gtwstizmae.html

Java: import java.util.List;
来源：http://hz.jinyuanbaomall.cn/gthlrbqgpd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.316326.xyz/gtdgfmzasc.html


<!-- 参考信息 -->