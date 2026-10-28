代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.9152youxi.cn/gtmarturlz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.guowangkeji.top/gtomeevomk.html

[A24] 去除首尾空白
来源：http://hz.ywan-chungtsiang.top/gtfcatqnqh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shanyushiyangtech.top/gtjulcwsiq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yangfankeji.com/gtknbnirdi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.andypj.xyz/gtmwrqtvdz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.mhx1999.top/gtpzjhhmxc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.vqdsnc.cn/gttejrbdzn.html

Go:   strings.TrimSpace(s)
来源：http://hz.meibo888.top/gtyevhxpkz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhiwuduotai.top/gtthyqeuqr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.xinyue.icu/gtvmahyhid.html

[A25] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gtrhkwhidv.html

Py:   s1 == s2; s1 != s2
来源：http://hz.0kj1m.cn/gtfuuvboce.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ybcxt.top/gtwdabfjhu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nwbrower.top/gtpqpdcsqs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sufxvd.cn/gtuweyxpvr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xuetiantiany.cn/gtgcgiubgw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xylfe.cn/gtovltjzzx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.xuetiantiany.cn/gtqninyonl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.pycfn.com/gtwmitqwgj.html

[A26] 类型转换总览
来源：http://hz.havefunace.top/gteachbzdh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sufxvd.cn/gtpjhaxxcq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cheryme.top/gthhbpxylj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ydjk.org.cn/gtowyadatv.html

TS:   Number() String() Boolean() x as number
来源：http://hz.nanxinkj.top/gthirdbaoe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenlongwang.top/gteqhmkuyf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.guannengcc.top/gtbpsqtijw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.birdmap.top/gtfinqicux.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hnqzz.top/gtbyormyyq.html

================================================================================
来源：http://hz.fengsongda.top/gtxuveupte.html

B. 流程控制
来源：http://hz.jinqigufen.top/gtponbgzxp.html

================================================================================
来源：http://hz.yangfankeji.com/gtphlpjbrh.html

[B01] 条件判断 if / else
来源：http://hz.jinghuilouyu.cn/gtuqmkuqkh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.hnxiangtu.top/gtfocefhcb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zdqjudy.top/gtvrcpijyl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gtzhjjcmuc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtmdytxkmd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gtrxejlfiy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.daxiang520.top/gtdjuzwjzv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cheryme.top/gtikaqlopb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jianghu66.top/gteoiujqiy.html

[B02] 多分支 else if / elif
来源：http://hz.jlsjyb.cn/gtafxwehnq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.bjfxy.top/gtkqtlmbzq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.kuanghao11.cn/gtuervasic.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.c1oappe.top/gtukhauqac.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.haohaochexian.top/gtjhbjvswu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nwbrower.top/gtycsykgqp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.dianchejie.cn/gtilnjsgou.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.chenzaomai.com/gtdaeububc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tanke756.top/gtvkowovzz.html

[B03] switch / match / case
来源：http://hz.zhengqikj.top/gthraeimur.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.shanyushiyangkeji.top/gtgbouauwm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hammf.cn/gtopsgfzdo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenlongwang.top/gtmupytaaf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sufxvd.cn/gtsajvqmad.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtydrfyitz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.daxiang520.top/gtiewqlqky.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhengqikj.top/gtgavpviuu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yuxming.cn/gtimimqzjh.html

[B04] for 计数循环
来源：http://hz.ehwqpu.com/gtzzfwcuct.html

Py:   for i in range(10): print(i)
来源：http://hz.zhixingplan.top/gtydkvibtk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.guannengcc.top/gtedoxbect.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtesnpccka.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.havefunace.top/gtmrsaplpd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.guannengcc.top/gtrfwpqgnw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hnqzz.top/gtrziihrrp.html

Ruby: 10.times { |i| puts i }
来源：http://hz.dashuyun.cn/gtutfxsphf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xinyue.icu/gtcyfamycb.html

[B05] 遍历数组 / 列表
来源：http://hz.svipenyu.cn/gtzlhqikxb.html

Py:   for item in arr: print(item)
来源：http://hz.ydzc1.top/gttjzjqwzp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.redwolf501.top/gtxtalnthp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenzaomai.com/gtztboqfro.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhijiandao.cn/gttiuzoakx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj20258.top/gtxnmvvumz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.52xcode.cn/gtgfsyievq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.chenjidiqi.icu/gtxayuzqcr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ywan-chungtsiang.top/gttijyiuwc.html

[B06] 遍历字典 / 对象
来源：http://hz.zhixingplan.top/gtqdjftnnx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yonumen.top/gtxsoendta.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.chenjidiqi.icu/gtscruamur.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinqigufen.top/gtnbcujmuq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.birdmap.top/gtebwduzhk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.chenjidiqi.icu/gtafejjjlg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhijiandao.cn/gtykdmrmkk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ydzc1.top/gtqczzkcml.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jianghu66.top/gtntpqynlw.html

[B07] while 循环
来源：http://hz.dianchejie.cn/gtabsrfclf.html

Py:   while i < 10: i += 1
来源：http://hz.daxiang520.top/gttlidqkjf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yueranfly.top/gtcngvmbno.html

JS:   while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gtdsmpbyjc.html

TS:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtbzbtzzza.html

Java: while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtqydecryu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.pengpengdd.cyou/gtfsnqeoqh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jiagoushi.top/gtcnzulblv.html

C#:   while (i < 10) { i++; }
来源：http://hz.xuanzx.com/gtvhcjqosc.html

[B08] do-while（至少执行一次）
来源：http://hz.aizwys.cn/gtjtxupkpk.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yvedp.cn/gtgkrnfydw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hysaishi.cn/gtcjsasjdy.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhengqikj.top/gtijhkubdd.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtdqqllcef.html

Java: do { i++; } while (i < 10);
来源：http://hz.shzxlz.cn/gthxldjlht.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nanxinkj.top/gtewzvdvol.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yuxming.cn/gtxsmlxgaw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gthmftrvqy.html

[B09] break 与 continue
来源：http://hz.yj202588.top/gtijszlmqo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sxryk.cn/gtlllzaxbd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.vqdsnc.cn/gtqwfexgaj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtdfyfffbu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtpcgzyqtm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gthyxuvrrx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nanxinkj.top/gttgfvwpcs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gtpjfznbkj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gthzzcxlpk.html

[B10] 遍历同时拿索引
来源：http://hz.quarkkingdee.top/gtezobukne.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.kuanghao11.cn/gtagulxrdc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xuanzx.com/gthrsaoyug.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gtbnrcpfdb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ybcxt.top/gtykkzfcfn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yuanzhike.top/gtmqgjpjrc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shzxlz.cn/gtixjbizcs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aibaodan.cn/gtxrstbrnp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigufen.top/gtvnmsefsv.html

[B11] 生成数字序列 / 区间
来源：http://hz.tanke756.top/gtpgybyuoe.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtqissmlqe.html

PHP:  range(0, 10, 2);
来源：http://hz.jyoumei.cn/gtmlhvegib.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gtyhylonyx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhiwuduotai.top/gtivuhkblr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhoulong.xyz/gtomwkrbnh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yj20258888.top/gtouxzlbgj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.bjfxy.top/gtabvbfgbr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yuanzhike.top/gtdtpzywbq.html

[B12] 跳出多层循环
来源：http://hz.sweek.top/gtwqufepdr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yanxiufei.cn/gtnjxmlaln.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jiagoushi.top/gtvdlknjwe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtezuyyxqu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtsokadnti.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtcblsrfyh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.aibaodan.cn/gtlcopkhso.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gaohongyu789.top/gtwaowjqno.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xinyue.icu/gtpufywxzy.html

[B13] 判断是否为数字
来源：http://hz.xingfuxueyuan.xyz/gtfnzznedk.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhengqikj.top/gtgccvzwms.html

PHP:  is_numeric($x)
来源：http://hz.c1oappe.top/gtjnsoheuy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tian-w.cn/gtjphclzsm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gtuomnugtw.html

Java: x instanceof Number
来源：http://hz.jqgufenzy.top/gtaiezmaga.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.smart0.xyz/gtjgdwbamq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhongyouzk.top/gtfyslfliq.html

C#:   x is int or double or decimal
来源：http://hz.kuanghao11.cn/gtpmcozmxn.html

[B14] 判断值是否在集合内
来源：http://hz.fengsongda.top/gtxnwrfkah.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nwbrower.top/gtvavqnhfx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hnxiangtu.top/gtkvzlzuyi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gtqtjecphd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tanke756.top/gtolypjzte.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.0kj1m.cn/gtetyuhdzb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhijiandao.cn/gtezkcobne.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj20258.top/gticfmkrst.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxinkj.top/gtswgcrhah.html

[B15] 布尔运算与取反
来源：http://hz.pengpengdd.cyou/gtfvjuzcmf.html

Py:   a and b or not c
来源：http://hz.iojbl.cn/gtxxlqwlcw.html

PHP:  $a && $b || !$c
来源：http://hz.svipenyu.cn/gtquoyjnkv.html

JS:   a && b || !c
来源：http://hz.jianghu66.top/gtsxkevsuq.html

TS:   a && b || !c
来源：http://hz.cucudq.cn/gtqebbxwfr.html

Java: a && b || !c
来源：http://hz.cdnleiting.top/gtycsopjax.html

Go:   a && b || !c
来源：http://hz.pycfn.com/gtomgbqglh.html

Ruby: a && b || !c
来源：http://hz.yueranfly.top/gtyabiktey.html

C#:   a && b || !c
来源：http://hz.cashguo.top/gtpkoqeqfg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gtrxoovptb.html

Py:   if not data: return
来源：http://hz.shzxlz.cn/gtxdqesrss.html

PHP:  if (!$data) { return; }
来源：http://hz.nanxinkj.top/gtmoioynax.html

JS:   if (!data) return;
来源：http://hz.sysykeji.top/gtmfkxzknv.html

TS:   if (!data) return;
来源：http://hz.hammf.cn/gtpelrfmls.html

Java: if (data == null) return;
来源：http://hz.cucudq.cn/gtnfoomnze.html

Go:   if data == nil { return }
来源：http://hz.shuidangran.top/gtdtuojoln.html

Ruby: return if data.nil?
来源：http://hz.jinyuanbaomall.cn/gtqzqswtni.html

C#:   if (data == null) return;
来源：http://hz.ydzc1.top/gtdnpaurrn.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqyumzycm.html

C. 函数与作用域
来源：http://hz.cqqwz.cn/gtbteghloi.html

================================================================================
来源：http://hz.zhiwuduotai.top/gteawwvkdf.html

[C01] 定义函数
来源：http://hz.tian-w.cn/gtrmdefham.html

Py:   def add(a, b): return a + b
来源：http://hz.jiagoushi.top/gtqcdubphm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dashuyun.cn/gtvuigwdua.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.daria6918.cn/gtdsvdfenm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtimapichn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gteewpwqtq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.52xcode.cn/gtyonexvai.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtnlxhpjtx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtbfvyabow.html

[C02] 默认参数
来源：http://hz.vqdsnc.cn/gtlhcynmmb.html

Py:   def greet(name="World"): return name
来源：http://hz.ybcxt.top/gtukjmzuiw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.quarkkingdee.top/gtegxxqtbn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.haohaochexian.top/gtivtiziuc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.vqdsnc.cn/gtfreweojf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnxiangtu.top/gtflmowcfe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtvhhvzpde.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhoulong.xyz/gthemkaksb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258888.top/gtbwtfbnhm.html

[C03] 可变参数
来源：http://hz.zhiwuduotai.top/gtbhtibqbe.html

Py:   def total(*args): return sum(args)
来源：http://hz.nwbrower.top/gtowgusccs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangshuangyany.cn/gtfqxvtoco.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gttwczefnx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gttmjcnxql.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ehwqpu.com/gtqjkmxrzc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yonumen.top/gtgupyrmum.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuetiantiany.cn/gtwxioghps.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhijiandao.cn/gtwakvamdq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhengqikj.top/gtnwfsldem.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ivvv.top/gtxmpoinfe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtottwhqna.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuanzx.com/gtnisbvlsz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cdnleiting.top/gtarccxvmc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinghuilouyu.cn/gtbgckanyl.html

Go:   // 无：用配置结构体参数
来源：http://hz.ywan-chungtsiang.top/gttywzosaw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtqrktwkbb.html

C#:   f(a: 1, b: 2)
来源：http://hz.cashguo.top/gtmkxunbov.html

[C05] 返回多个值
来源：http://hz.jqgfzy.top/gtqrxayrno.html

Py:   return a, b
来源：http://hz.hongshengwenyu.top/gtvlbdnxaj.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gtxumseerp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinqigufen.top/gtsxijbnpx.html

TS:   return { a, b };
来源：http://hz.yj20258888.top/gtejkwrjuq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dashuyun.cn/gtwcqdxdqx.html

Go:   return a, b
来源：http://hz.hysaishi.cn/gtrosukyqr.html

Ruby: return a, b
来源：http://hz.yj202588.top/gteasbruoc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gtvqtvbvow.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtxxeipzuc.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangkeji.top/gtouotltwu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinqigufen.top/gtmzbxxppb.html

JS:   const square = x => x * x;
来源：http://hz.iojbl.cn/gtzdymvjzh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.vqdsnc.cn/gtmgjsktsm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yangfankeji.com/gtuhbhlrju.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cdnleiting.top/gtnnfkxkns.html

Ruby: square = ->(x) { x * x }
来源：http://hz.feifeiyinyue.top/gttynbogpd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.smart0.xyz/gtfxgpfkgb.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtwyvbvolk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.meibo888.top/gtqerscckd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tian-w.cn/gtxkizpqvm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xziqi.cn/gttltsjxxq.html

TS:   arr.map(String)
来源：http://hz.yongpay.top/gtawpuhgxw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cqqwz.cn/gtviioyylf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xuetiantiany.cn/gtgngoiymo.html

Ruby: arr.map(&:upcase)
来源：http://hz.havefunace.top/gtsorovjxg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yanxiufei.cn/gtjzjfuuze.html

[C08] 闭包
来源：http://hz.yongpay.top/gtmzwjerpq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hnxiangtu.top/gtvypwywty.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hysaishi.cn/gtzdewdezz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtsofqjydf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shanyushiyangtech.top/gtyajocmhb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cdnleiting.top/gtcslfjkvx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yangfankeji.com/gtnmgvsnxp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtamgktbbj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hongshengwenyu.top/gtwadihkal.html

[C09] 递归
来源：http://hz.hywenlv.cn/gtbyrmzwwx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhongyouzk.top/gtcprlzwvh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gtdvarisga.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sysykeji.top/gtqxrxwfnk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtzueazxkn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydzc1.top/gttfmegrjy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.smart0.xyz/gtjypgstib.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.guannengcc.top/gtqzikmgcv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydjk.org.cn/gtloecijlr.html

[C10] 变量作用域
来源：http://hz.zhaomingkeji.xyz/gtmpxkuigi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydzc1.top/gtjripylji.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydjk.org.cn/gtguvizntt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenjidiqi.icu/gtlbmnfevo.html

TS:   同 JS
来源：http://hz.hnxiangtu.top/gtlhbmvcvi.html

Java: 方法内为块级作用域
来源：http://hz.jyoumei.cn/gtbzhustdz.html

Go:   花括号块级作用域
来源：http://hz.yangfankeji.com/gtsgmlqiln.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhijiandao.cn/gttrqpedio.html

C#:   块级作用域
来源：http://hz.jqgfzy.top/gtobtzgzhq.html

[C11] 模块导入与导出
来源：http://hz.gogol.net.cn/gtqhtquilm.html

Py:   from module import func
来源：http://hz.ivvv.top/gtuerfvnac.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gzhubu.top/gtbmodvbir.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hysaishi.cn/gtpgvphamw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zdqjudy.top/gtxohaabqz.html

Java: import java.util.List;
来源：http://hz.shanyushiyangkeji.top/gtvpgshwdt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jqgufenzy.top/gtonjtgtsz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.svipenyu.cn/gtxpcstudk.html

C#:   using System.Text;
来源：http://hz.chenlongwang.top/gtyzrtstxv.html

[C12] 立即执行函数 IIFE
来源：http://hz.haohaochexian.top/gtndhnlgva.html

Py:   (lambda: print("run"))()
来源：http://hz.yj202588.top/gtlxkjiuff.html

PHP:  (function () { echo "run"; })();
来源：http://hz.wangdashe.top/gturtjhwvp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cashguo.top/gtvugbgjqr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj20258.top/gtoazmclmy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgufenzy.top/gtksnplafl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yangfankeji.com/gtfupqetpx.html

Ruby: -> { puts "run" }.call
来源：http://hz.xuanzx.com/gtqzrplucc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.chenlongwang.top/gtaxkwcsfz.html

[C13] 类型声明 / 类型注解
来源：http://hz.dianchejie.cn/gtkpdsircf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gtcpwzbprr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuetiantiany.cn/gtvmdcbhge.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sysykeji.top/gtdbovqowy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtngbuykqk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtfguyfqqx.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangkeji.top/gtjfwtbwjb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgufenzy.top/gtvjqkegmm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jlsjyb.cn/gtjpvxwqzr.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtfouvxjxv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuanzx.com/gthaviyplb.html

PHP:  // 无泛型
来源：http://hz.gotoacloud.top/gtcchwrjoi.html

JS:   // 无泛型
来源：http://hz.cqqwz.cn/gtktgdduni.html


<!-- 参考信息 -->