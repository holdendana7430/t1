代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://hz.yanxiufei.cn/gttvfdhseh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.52xcode.cn/gthlaxyjgq.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yanxiufei.cn/gtcogkapqf.html

TS:   (3.14159).toFixed(2)
来源：http://hz.sxryk.cn/gtabxqnifv.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.zhijiandao.cn/gtqnueifql.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.316326.xyz/gtpicxvcax.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.xuanzx.com/gtwrgqwokz.html

C#:   3.14159.ToString("F2")
来源：http://hz.zycfv.cn/gtlctxmbfq.html

[A22] 获取字符串长度
来源：http://hz.chenlongwang.top/gtbplpfbkz.html

Py:   len(s)
来源：http://hz.meibo888.top/gtnntdrcnp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yangfankeji.com/gtfoywpmhn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.meibo888.top/gttynybish.html

TS:   s.length
来源：http://hz.daxiang520.top/gtbczdmwho.html

Java: s.length()
来源：http://hz.andypj.xyz/gtywuwyrsd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jinghuilouyu.cn/gthmcgnges.html

Ruby: s.length
来源：http://hz.redwolf501.top/gtxjlzxhiw.html

C#:   s.Length
来源：http://hz.quarkkingdee.top/gtabpeqepw.html

[A23] 大小写转换
来源：http://hz.meibo888.top/gtsbjhcjss.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yj202588.top/gtfqwzazig.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.aizwys.cn/gtufjiqlgf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gogol.net.cn/gtkchshkze.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.wangdashe.top/gtqzikxztu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.aibaodan.cn/gttduyehbb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hongshengwenyu.top/gtqscqnanf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.chenlongwang.top/gtxxvakbia.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.52xcode.cn/gtndsjmvnr.html

[A24] 去除首尾空白
来源：http://hz.yj202588.top/gtvwyjqfuv.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.daxiang520.top/gtlioppmxv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yanxiufei.cn/gthfvfuqib.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.0kj1m.cn/gtkprmbggf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jianghu66.top/gtnzantnwl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.daria6918.cn/gtchjlmjbm.html

Go:   strings.TrimSpace(s)
来源：http://hz.yanxiufei.cn/gtefhxkntv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.tian-w.cn/gtefpkcwfo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.fzhhl.top/gtxxzycxyf.html

[A25] 字符串比较
来源：http://hz.yueranfly.top/gtovfzrczi.html

Py:   s1 == s2; s1 != s2
来源：http://hz.gaohongyu789.top/gtixcleyby.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.pengpengdd.cyou/gtpmyzjjlj.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jiagoushi.top/gtvrxaphew.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ehwqpu.com/gtqdblecbv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.pycfn.com/gtczsaulcn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hywenlv.cn/gtlldijgxf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.chenjidiqi.icu/gtvyyqnjty.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.cheryme.top/gtnxlhmzpt.html

[A26] 类型转换总览
来源：http://hz.zhijiandao.cn/gttiacgurn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shanyushiyangtech.top/gtdcirerih.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xylfe.cn/gtzzkwgzas.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhongyouzk.top/gtbxlutamh.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yvedp.cn/gtcyidrszu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jqgufenzy.top/gtlmqpqzdu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.wangshuangyany.cn/gtlsirngft.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jqgfzy.top/gtlkwpqxlg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hnxiangtu.top/gtdbefadkr.html

================================================================================
来源：http://hz.xinyue.icu/gtvywjybfb.html

B. 流程控制
来源：http://hz.yj202588.top/gtwwomgazc.html

================================================================================
来源：http://hz.wangdashe.top/gtvhhlmysv.html

[B01] 条件判断 if / else
来源：http://hz.zdqjudy.top/gtkkrygvzl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.svipenyu.cn/gtfmdnutjg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhaomingkeji.xyz/gtbwnhypww.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.pycfn.com/gtvocobzpe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nanxinkj.top/gtxglbnbpz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangkeji.top/gtkzyavktj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yueranfly.top/gthouvcqtz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yangfankeji.com/gtlujktmze.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.wangdashe.top/gtehezyauo.html

[B02] 多分支 else if / elif
来源：http://hz.jqgfzy.top/gtjpmexjyu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.vqdsnc.cn/gtewbcklav.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.snrcjt.cn/gtkblylsxy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hywenlv.cn/gtvmsqnebt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxinkj.top/gtzzjnwgtl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.iojbl.cn/gtzudeappu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.feifeiyinyue.top/gtbaswgnef.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.redwolf501.top/gtnxbkwqbv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtldscirpf.html

[B03] switch / match / case
来源：http://hz.zhongyouzk.top/gtdpwvqskj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.gaohongyu789.top/gtbdwrjbwh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.sweek.top/gtezzyyrhn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daria6918.cn/gtmgwzbhwo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cqqwz.cn/gtfbukuidf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.wangshuangyany.cn/gtozbrmwhe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.c1oappe.top/gttqxyyixa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shangyingyoupin.top/gtlhqccrts.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.kuanghao11.cn/gtwbrcvzry.html

[B04] for 计数循环
来源：http://hz.ivvv.top/gtcqfgsoib.html

Py:   for i in range(10): print(i)
来源：http://hz.ivvv.top/gtnojvgmcq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jqgfzy.top/gtioghbhvx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hfpthk.cn/gtnxoxrcak.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sxryk.cn/gthkaohnmq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.c1oappe.top/gtexeszsqy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.pengpengdd.cyou/gtrmvhywia.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ydzc1.top/gtizsbpcwq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yangfankeji.com/gtcylrqqbp.html

[B05] 遍历数组 / 列表
来源：http://hz.cqqwz.cn/gtmkghchyu.html

Py:   for item in arr: print(item)
来源：http://hz.ydjk.org.cn/gtaughoyed.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.bjfxy.top/gtzghskwrm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cdnleiting.top/gtvlpqwvbp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.gogol.net.cn/gtvrzltjmb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cashguo.top/gtvrgusjzm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hammf.cn/gtflstfoho.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jqgufenzy.top/gttztvljft.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ybcxt.top/gtrnfhutdc.html

[B06] 遍历字典 / 对象
来源：http://hz.pycfn.com/gtwznpdehq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jinyuanbaomall.cn/gthgyzwppw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.haohaochexian.top/gtlrqlikgp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shzxlz.cn/gtgwjlsefn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhixingplan.top/gtgkgeqjer.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.vqdsnc.cn/gtkegcxnax.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zdqjudy.top/gtoodkunwv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.gaohongyu789.top/gthatwlyxa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.wangdashe.top/gtcqvdauez.html

[B07] while 循环
来源：http://hz.jyoumei.cn/gtpwvmnbsm.html

Py:   while i < 10: i += 1
来源：http://hz.yuanzhike.top/gtqkfhvbds.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhixingplan.top/gtmarzjyhu.html

JS:   while (i < 10) { i++; }
来源：http://hz.316326.xyz/gtycckhpgc.html

TS:   while (i < 10) { i++; }
来源：http://hz.birdmap.top/gtprdnxbui.html

Java: while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtrcirvfhd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenlongwang.top/gtsajcjiym.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xylfe.cn/gtgtiqirrq.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtoywgjibm.html

[B08] do-while（至少执行一次）
来源：http://hz.yj20258888.top/gtkessmkdg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hywenlv.cn/gtwgjkvuch.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xuetiantiany.cn/gtqzkhoejg.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtcqvpzvnp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gthrwknvza.html

Java: do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtxrbqheyl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ehwqpu.com/gtmpwbvbeo.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.guowangkeji.top/gtjwrwnfex.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtebifsdgg.html

[B09] break 与 continue
来源：http://hz.hammf.cn/gtuenjlkqh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gzhubu.top/gturvzriwa.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinqigufen.top/gtznlbvrti.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtvcqehzsn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtvebioney.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtwkaosqzt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258.top/gtsvlmvivf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yueranfly.top/gtgtxdgjuh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtdzuhagtf.html

[B10] 遍历同时拿索引
来源：http://hz.gaohongyu789.top/gtbkgqjwml.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shangyingyoupin.top/gtqbcgmisi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.aibaodan.cn/gtocxygnny.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jiagoushi.top/gtxzkyqayf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.daxiang520.top/gtlzdohhlf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.pycfn.com/gtrndbcoue.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinqigufen.top/gtczberugf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shuidangran.top/gtgmcwwoxx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shzxlz.cn/gtyaofuvnt.html

[B11] 生成数字序列 / 区间
来源：http://hz.sweek.top/gtiehrjmsi.html

Py:   list(range(0, 10, 2))
来源：http://hz.ybcxt.top/gthsjbrwpe.html

PHP:  range(0, 10, 2);
来源：http://hz.jinyuanbaomall.cn/gtidjdmkwv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhaomingkeji.xyz/gtejwadkbq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gotoacloud.top/gtmivutsfp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cheryme.top/gtsristkfo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cheryme.top/gtvypfppbe.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shzxlz.cn/gthpzclnes.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.c1oappe.top/gtqoqtfaxr.html

[B12] 跳出多层循环
来源：http://hz.guowangkeji.top/gtftacxhap.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgfzy.top/gtdtjdzrod.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ivvv.top/gtzxwzxand.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtsslpyboa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtglkloznm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtiekoeydc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jlsjyb.cn/gtwqtxvjyf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinyuanbaomall.cn/gtnvdqdvqo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sysykeji.top/gtmgxtfroj.html

[B13] 判断是否为数字
来源：http://hz.bjfxy.top/gtjcgknoxq.html

Py:   isinstance(x, (int, float))
来源：http://hz.daria6918.cn/gtceoemgop.html

PHP:  is_numeric($x)
来源：http://hz.daxiang520.top/gtppwhlnno.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtqabzthys.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtxsmobapa.html

Java: x instanceof Number
来源：http://hz.ywan-chungtsiang.top/gtggbtvbuk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yvedp.cn/gtaogveikx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nanxinkj.top/gtvtuunesy.html

C#:   x is int or double or decimal
来源：http://hz.redwolf501.top/gtfviuqavx.html

[B14] 判断值是否在集合内
来源：http://hz.chenlongwang.top/gtpnvxgysx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhoulong.xyz/gtqoxvlscw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenzaomai.com/gtnanepnmj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.fzhhl.top/gtedzdetjc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yvedp.cn/gtvrbirkhs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinqigfzy.top/gtdhcyfzkp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xinyue.icu/gtdsvhngzn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtdaqcjdfj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.9152youxi.cn/gtkpwikbyn.html

[B15] 布尔运算与取反
来源：http://hz.shangyingyoupin.top/gtnjkgndsy.html

Py:   a and b or not c
来源：http://hz.52xcode.cn/gtoiqtjbfi.html

PHP:  $a && $b || !$c
来源：http://hz.yonumen.top/gtufbrogfo.html

JS:   a && b || !c
来源：http://hz.zdqjudy.top/gtcdskhern.html

TS:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtfqrnzelx.html

Java: a && b || !c
来源：http://hz.shzxlz.cn/gtdyzrwdan.html

Go:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtwecedatf.html

Ruby: a && b || !c
来源：http://hz.sxryk.cn/gtzajlvqbb.html

C#:   a && b || !c
来源：http://hz.jqgufenzy.top/gtgohbycjr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nanxuanxn.top/gtfrrmjcmg.html

Py:   if not data: return
来源：http://hz.yongpay.top/gtvlsacnbq.html

PHP:  if (!$data) { return; }
来源：http://hz.jinqigfzy.top/gtdcpctgxp.html

JS:   if (!data) return;
来源：http://hz.yj202588.top/gtfcnfjwwd.html

TS:   if (!data) return;
来源：http://hz.52xcode.cn/gtivyigsef.html

Java: if (data == null) return;
来源：http://hz.gotoacloud.top/gtguqvgkuw.html

Go:   if data == nil { return }
来源：http://hz.hongshengwenyu.top/gtlxvayztl.html

Ruby: return if data.nil?
来源：http://hz.9152youxi.cn/gtiyssubzf.html

C#:   if (data == null) return;
来源：http://hz.pycfn.com/gtbxcaxpna.html

================================================================================
来源：http://hz.redwolf501.top/gtffhznpkv.html

C. 函数与作用域
来源：http://hz.ydjk.org.cn/gtasietcnd.html

================================================================================
来源：http://hz.dianchejie.cn/gttolwchvv.html

[C01] 定义函数
来源：http://hz.aizwys.cn/gtyauwxkll.html

Py:   def add(a, b): return a + b
来源：http://hz.ppjwa.cn/gtgdsbvzft.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtrielpivq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ivvv.top/gthiuimuvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gthfpeycoy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtkiteogqo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shuidangran.top/gttgelhhcc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangdashe.top/gtiqivolhe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtpkzyfmrp.html

[C02] 默认参数
来源：http://hz.jlsjyb.cn/gtolcqeiwa.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtpmokromx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yonumen.top/gtcvmyyzti.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinghuilouyu.cn/gtehosjftf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxinkj.top/gtxtinsvuw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.kuanghao11.cn/gtzkfbrdoy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtxlabuhck.html

Ruby: def greet(name = "World") = name
来源：http://hz.aizwys.cn/gtxkwfrhvl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhaomingkeji.xyz/gtbcdyhktv.html

[C03] 可变参数
来源：http://hz.cdnleiting.top/gtkmphnjsv.html

Py:   def total(*args): return sum(args)
来源：http://hz.hammf.cn/gtveamtvjh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.svipenyu.cn/gtwazqtoam.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtuiaawlmc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gtkbbdqpvx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gzhubu.top/gtmjhquqos.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sxryk.cn/gtejfylmwh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cucudq.cn/gtswcguiij.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.smart0.xyz/gtjvxjbaar.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ybcxt.top/gtokgtrutf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tian-w.cn/gtmtwnwfyj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jqgfzy.top/gtujmvqkxf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtigcwtxhj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.dianchejie.cn/gtiksfjrgy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pycfn.com/gtxpxrsoyh.html

Go:   // 无：用配置结构体参数
来源：http://hz.fengsongda.top/gtejijhblv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtqldikqpg.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtxinryxvp.html

[C05] 返回多个值
来源：http://hz.pycfn.com/gtcdjdfwhr.html

Py:   return a, b
来源：http://hz.hywenlv.cn/gtcodulddq.html

PHP:  return [$a, $b];
来源：http://hz.chenzaomai.com/gtjisyghus.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gotoacloud.top/gtykgsxgvg.html

TS:   return { a, b };
来源：http://hz.hongshengwenyu.top/gtzskhrcqy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenlongwang.top/gtvbvbkpom.html

Go:   return a, b
来源：http://hz.sxryk.cn/gtdpimazmm.html

Ruby: return a, b
来源：http://hz.hywenlv.cn/gtmxovxygd.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xuanzx.com/gtfbuhmvnw.html

[C06] 匿名函数 / lambda
来源：http://hz.yuxming.cn/gttmfhzvmy.html

Py:   square = lambda x: x * x
来源：http://hz.kuanghao11.cn/gtloqjarqi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nanxuanxn.top/gtssbolige.html

JS:   const square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtahkhrifb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.mhx1999.top/gtbswmcdtk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.smart0.xyz/gtmvvuwgke.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ydzc1.top/gtkcaapchm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.birdmap.top/gtlyifchjf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.52xcode.cn/gtvblztbgr.html

[C07] 把函数作为参数传入
来源：http://hz.xuetiantiany.cn/gtyhalvjbg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhaomingkeji.xyz/gtznearzjl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.haohaochexian.top/gtevhqibsb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj202588.top/gtmncohgli.html

TS:   arr.map(String)
来源：http://hz.fengsongda.top/gtgeerxpjw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.9152youxi.cn/gtyaltfnbu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgfzy.top/gtgrszfoky.html

Ruby: arr.map(&:upcase)
来源：http://hz.jlsjyb.cn/gtbjpxwbhf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daxiang520.top/gtjiyclcox.html

[C08] 闭包
来源：http://hz.sweek.top/gtnerpnzqd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangkeji.top/gtwyovsvjr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258.top/gtcvbmsdhn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtekiorbmi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtwmfgkgxj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.redwolf501.top/gtjhpkgbdo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhijiandao.cn/gteyywlysk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hysaishi.cn/gtyllnzyzi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtdjuaddlr.html

[C09] 递归
来源：http://hz.jqgfzy.top/gtkauqictu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gtstpkiyoz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhiwuduotai.top/gtucjxmwvl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtgsmtdyqu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gtsfegdwav.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuanzx.com/gtoclvdgio.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hysaishi.cn/gtxpjqqjxj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtxiuadjnk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.feifeiyinyue.top/gtezyteqry.html

[C10] 变量作用域
来源：http://hz.iojbl.cn/gtyqsgpdxx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinqigfzy.top/gtuixtpshd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sxryk.cn/gtikxratey.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xziqi.cn/gtzxsemqgx.html

TS:   同 JS
来源：http://hz.wangshuangyany.cn/gtibqyyzei.html

Java: 方法内为块级作用域
来源：http://hz.gzhubu.top/gtsghkszaf.html

Go:   花括号块级作用域
来源：http://hz.gogol.net.cn/gtzqfgiyfq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shanyushiyangtech.top/gtawiuknyw.html

C#:   块级作用域
来源：http://hz.pycfn.com/gtocjpgstq.html

[C11] 模块导入与导出
来源：http://hz.cdnleiting.top/gtkwcpfiab.html

Py:   from module import func
来源：http://hz.yanxiufei.cn/gtbkiczwtc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuanzhike.top/gtrycqycui.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtltzebncj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.c1oappe.top/gtacnyfqfn.html

Java: import java.util.List;
来源：http://hz.fengsongda.top/gtwfpsobyj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhengqikj.top/gtiyimfpdp.html


<!-- 参考信息 -->