代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://hz.wangshuangyany.cn/gtdhfsarne.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hammf.cn/gtoozuafos.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhiwuduotai.top/gttgwtyzfv.html

[A25] 字符串比较
来源：http://hz.yonumen.top/gtrfoephjs.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ybcxt.top/gtieghrhri.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.316326.xyz/gtyungxxvi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.dashuyun.cn/gtivkisslp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tian-w.cn/gtlmlccqhr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.iojbl.cn/gtptkbphfk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hnqzz.top/gtzcsntntu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.nanxinkj.top/gtnmgzyrvd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ywan-chungtsiang.top/gtejqtsjxm.html

[A26] 类型转换总览
来源：http://hz.xuanzx.com/gtyqkqlxku.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hammf.cn/gtkqdbebmt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.chenlongwang.top/gtdnfrsdbu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ivvv.top/gtwzcifpfa.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jyoumei.cn/gtdelarmoz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jinqigufen.top/gtnparxsaz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yongpay.top/gtjzclqmox.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.c1oappe.top/gtddplmqka.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jiagoushi.top/gtllhkkwcy.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthxsebgpy.html

B. 流程控制
来源：http://hz.havefunace.top/gtaawqryeb.html

================================================================================
来源：http://hz.yuxming.cn/gtwcshsoqj.html

[B01] 条件判断 if / else
来源：http://hz.yuanzhike.top/gtfotvtlem.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yj20258888.top/gtrrwigqco.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.smart0.xyz/gtjblfomef.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtdxzqujsu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtetbedcrg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtpmoadufs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.fengsongda.top/gtzecgoxmq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.chenzaomai.com/gtzflguxtr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ydjk.org.cn/gttnhzrpwk.html

[B02] 多分支 else if / elif
来源：http://hz.svipenyu.cn/gtjblcepeb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shanyushiyangkeji.top/gtmgmvlsjb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hnqzz.top/gtyftdfbte.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtnsiiukcj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.c1oappe.top/gtbeffsunm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtynrjbpjl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jqgfzy.top/gtbfbjydik.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.cheryme.top/gtpsvlhvgc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.haohaochexian.top/gtngffgrlj.html

[B03] switch / match / case
来源：http://hz.zycfv.cn/gtjilthjje.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.52xcode.cn/gtnxxzrvtk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.birdmap.top/gtzsfmqxhx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.birdmap.top/gtueupnrji.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cucudq.cn/gtslsbtpeo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yuanzhike.top/gtbquwbhix.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.tianlin.xyz/gtsgobaiha.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhoulong.xyz/gtkqqqljgi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.shanyushiyangtech.top/gtrxquipzi.html

[B04] for 计数循环
来源：http://hz.zycfv.cn/gtklrqqfxn.html

Py:   for i in range(10): print(i)
来源：http://hz.nanxuanxn.top/gtxyixaszh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xuanzx.com/gtwgesbptp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangshuangyany.cn/gtzlnxqyem.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ywan-chungtsiang.top/gtmtzvmmxq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhixingplan.top/gtoluiqhdu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.kuanghao11.cn/gtsjwjjzxx.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ydjk.org.cn/gtmljeulhx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hywenlv.cn/gtmpcobkpb.html

[B05] 遍历数组 / 列表
来源：http://hz.bjfxy.top/gtfmayjldn.html

Py:   for item in arr: print(item)
来源：http://hz.snrcjt.cn/gtyxqpsqcd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.meibo888.top/gtfbermviv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cqqwz.cn/gtxudcgtiv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.guowangkeji.top/gtzexzgcdt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.nanxinkj.top/gtjdwedioy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.bjfxy.top/gtaltqpoyu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cheryme.top/gtsbkveygt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.dianchejie.cn/gtihwrxhti.html

[B06] 遍历字典 / 对象
来源：http://hz.jyoumei.cn/gtmwfxxzex.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cdnleiting.top/gtugsxwqaa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.tian-w.cn/gteecphqqx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yvedp.cn/gtahafbifh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.chenjidiqi.icu/gtmbcekamg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.andypj.xyz/gtwjdevcpq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangshuangyany.cn/gtiweoocwl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhoulong.xyz/gtfrzvxzbs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hnqzz.top/gtimgknoye.html

[B07] while 循环
来源：http://hz.zycfv.cn/gtzrshhfzi.html

Py:   while i < 10: i += 1
来源：http://hz.jinqigufen.top/gtpicqjpbk.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.pycfn.com/gtckacdndr.html

JS:   while (i < 10) { i++; }
来源：http://hz.bjfxy.top/gtqsbjjsau.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhoulong.xyz/gtxhktfpuk.html

Java: while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gttvegxekp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zdqjudy.top/gtmotmzlxr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.smart0.xyz/gtblntlyyw.html

C#:   while (i < 10) { i++; }
来源：http://hz.aibaodan.cn/gtsizyaiqv.html

[B08] do-while（至少执行一次）
来源：http://hz.xuetiantiany.cn/gtjaluohsz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhongyouzk.top/gtjqwefvbr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.tianlin.xyz/gtyccteguo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtahyxihni.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gttvvornvb.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhoulong.xyz/gtpkgzkkwy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ywan-chungtsiang.top/gtfrytzmmb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hywenlv.cn/gtufnyftrz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aizwys.cn/gthkyxtmfe.html

[B09] break 与 continue
来源：http://hz.ybcxt.top/gtvsmzecoc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.redwolf501.top/gtpqwjsxdo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hfpthk.cn/gtdnjmmhji.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtqasqcvhq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtgpicnzgb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtxpjkaibp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigfzy.top/gtkzahqjgh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.kuanghao11.cn/gtlwmuzebd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtfmmgkouj.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtihytlecs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.wangshuangyany.cn/gttqcujurb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.iojbl.cn/gtqgvtwztf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.wangdashe.top/gtwvjjjttu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hammf.cn/gtvdnjsvpx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.haohaochexian.top/gthdhbffdi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.meibo888.top/gtrcksodmq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hnqzz.top/gtkcilvyws.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigufen.top/gtnmyaaopy.html

[B11] 生成数字序列 / 区间
来源：http://hz.nanxinkj.top/gtutksbhhv.html

Py:   list(range(0, 10, 2))
来源：http://hz.vqdsnc.cn/gtilktbjxj.html

PHP:  range(0, 10, 2);
来源：http://hz.wangdashe.top/gtuvkcrqgn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shanyushiyangkeji.top/gtvsxnsuaj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuanzhike.top/gtqxrlsmzu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.havefunace.top/gtjyrequuq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.feifeiyinyue.top/gtjshxzbom.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ehwqpu.com/gtiwqggquv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.52xcode.cn/gthkhkjeve.html

[B12] 跳出多层循环
来源：http://hz.c1oappe.top/gtpotlrzhn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yvedp.cn/gtyanimexl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cashguo.top/gtjwvmhppu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtijtusnju.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gticbuftdl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtnqmzpyno.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ivvv.top/gtalpadxko.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.c1oappe.top/gtirzazase.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sxryk.cn/gteyvwyknh.html

[B13] 判断是否为数字
来源：http://hz.cdnleiting.top/gtriuftbvq.html

Py:   isinstance(x, (int, float))
来源：http://hz.hysaishi.cn/gthmwiemvd.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtbjryardz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xinyue.icu/gtpngbeyjz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cucudq.cn/gtgzmbqxfa.html

Java: x instanceof Number
来源：http://hz.shangyingyoupin.top/gtjrcvpgmd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.fzhhl.top/gtnridwmjp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.52xcode.cn/gtdweonssf.html

C#:   x is int or double or decimal
来源：http://hz.shanyushiyangkeji.top/gtrdytqxbu.html

[B14] 判断值是否在集合内
来源：http://hz.jinqigfzy.top/gtuxrfywen.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ppjwa.cn/gtgecgfylz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.kuanghao11.cn/gtqqaobcgu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258.top/gtysooiswn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.haohaochexian.top/gtytwdzrtp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxuanxn.top/gtifleimkh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinyuanbaomall.cn/gtmstzcjlv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.chenlongwang.top/gtgtwtljvy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sufxvd.cn/gtabiiirjx.html

[B15] 布尔运算与取反
来源：http://hz.wangshuangyany.cn/gtduinnbhn.html

Py:   a and b or not c
来源：http://hz.jlsjyb.cn/gtofqqoyqx.html

PHP:  $a && $b || !$c
来源：http://hz.andypj.xyz/gtpxhiivlh.html

JS:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtugxdlamk.html

TS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtfdwxkxra.html

Java: a && b || !c
来源：http://hz.nwbrower.top/gtmkmukyie.html

Go:   a && b || !c
来源：http://hz.gogol.net.cn/gtgedqhdks.html

Ruby: a && b || !c
来源：http://hz.pycfn.com/gtvaihbqgy.html

C#:   a && b || !c
来源：http://hz.nwbrower.top/gtnnzaamqk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gzhubu.top/gtgxafsffe.html

Py:   if not data: return
来源：http://hz.redwolf501.top/gtixuohsqt.html

PHP:  if (!$data) { return; }
来源：http://hz.smart0.xyz/gttalbpaxe.html

JS:   if (!data) return;
来源：http://hz.andypj.xyz/gtqqikduhu.html

TS:   if (!data) return;
来源：http://hz.bjfxy.top/gtcaocywqu.html

Java: if (data == null) return;
来源：http://hz.andypj.xyz/gtltvzybyg.html

Go:   if data == nil { return }
来源：http://hz.guowangkeji.top/gtjslfzfab.html

Ruby: return if data.nil?
来源：http://hz.wangdashe.top/gtoucmoyhy.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtrkcfssmo.html

================================================================================
来源：http://hz.nanxinkj.top/gtbrheftxh.html

C. 函数与作用域
来源：http://hz.tian-w.cn/gtfujgufss.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtewroeoez.html

[C01] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtcvpcvdhd.html

Py:   def add(a, b): return a + b
来源：http://hz.jinyuanbaomall.cn/gtqekcmiqw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtlbuojhpa.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.c1oappe.top/gtxzfmzjzw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtbkpnhuiz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtogiwyrsg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cqqwz.cn/gtstbkdmsu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.birdmap.top/gtlzejebqk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtkrioskuw.html

[C02] 默认参数
来源：http://hz.havefunace.top/gtqooprbbt.html

Py:   def greet(name="World"): return name
来源：http://hz.fengsongda.top/gtkvuwnnkb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xuetiantiany.cn/gtmhdaaxgp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenlongwang.top/gtxgrrucgf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhoulong.xyz/gtkyypicoi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuxming.cn/gtkvrdmulc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yongpay.top/gtaikdbyfs.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgufenzy.top/gtsbnvrbsz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtkdkqtmkb.html

[C03] 可变参数
来源：http://hz.zhijiandao.cn/gtqlqvxmgf.html

Py:   def total(*args): return sum(args)
来源：http://hz.zycfv.cn/gtltyczfnr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gtnxptaapz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtsyspgsqe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.bjfxy.top/gtgotlwvkq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.haohaochexian.top/gtuevfzgzl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.316326.xyz/gtwxuyfevm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuanzhike.top/gtskeyrkxz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cdnleiting.top/gtodthxooo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ivvv.top/gtvontqeif.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yvedp.cn/gtpiycejng.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangdashe.top/gtdhnnsjfv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtlcrbjrur.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.havefunace.top/gtabqoarbl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shangyingyoupin.top/gtkkoxhdds.html

Go:   // 无：用配置结构体参数
来源：http://hz.c1oappe.top/gtjyzilwbx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gtlgmmrbge.html

C#:   f(a: 1, b: 2)
来源：http://hz.aibaodan.cn/gtqxrpgioh.html

[C05] 返回多个值
来源：http://hz.jinghuilouyu.cn/gtjpovcjkw.html

Py:   return a, b
来源：http://hz.daxiang520.top/gtmqxwybsp.html

PHP:  return [$a, $b];
来源：http://hz.xuetiantiany.cn/gtjtsyhfkb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cashguo.top/gtvyolwdsq.html

TS:   return { a, b };
来源：http://hz.sysykeji.top/gtdxeuqrlv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.mhx1999.top/gtptinrdzg.html

Go:   return a, b
来源：http://hz.guowangkeji.top/gtbgklpdwc.html

Ruby: return a, b
来源：http://hz.xingfuxueyuan.xyz/gtuznwzbds.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtiifnqsvg.html

[C06] 匿名函数 / lambda
来源：http://hz.nwbrower.top/gtkvrbxwqi.html

Py:   square = lambda x: x * x
来源：http://hz.xziqi.cn/gtrpsycxxg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nanxinkj.top/gttjjfjagt.html

JS:   const square = x => x * x;
来源：http://hz.hnqzz.top/gtnxspupsm.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuxming.cn/gtsrmzhawc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.0kj1m.cn/gtxyukymee.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xinyue.icu/gtnqvcspbk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jianghu66.top/gtemmnpynt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.52xcode.cn/gtgztnpotb.html

[C07] 把函数作为参数传入
来源：http://hz.svipenyu.cn/gtjiaxycmf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jlsjyb.cn/gtxpwducbs.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aibaodan.cn/gtgwzktrbd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hongshengwenyu.top/gtcczadrkb.html

TS:   arr.map(String)
来源：http://hz.cashguo.top/gtnzchdxbw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhaomingkeji.xyz/gtsxxmiugd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj202588.top/gtivniurtj.html

Ruby: arr.map(&:upcase)
来源：http://hz.sweek.top/gtxbpjytli.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinqigufen.top/gtodarkebo.html

[C08] 闭包
来源：http://hz.fengsongda.top/gtglusaxpz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinghuilouyu.cn/gtibysklvf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zdqjudy.top/gttvsyshxk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtodufazzh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtclyttpym.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ywan-chungtsiang.top/gtjkefpzzu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shanyushiyangtech.top/gtfwtvwbaq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ehwqpu.com/gtozqkqqhc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gtriknkcvy.html

[C09] 递归
来源：http://hz.gogol.net.cn/gtcsomapss.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xinyue.icu/gtexocrqcy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dashuyun.cn/gtkfqrjupf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gtlqeswdnu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hywenlv.cn/gtakefbfnn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xuanzx.com/gtllmonawy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yangfankeji.com/gtncohvkrw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pycfn.com/gtvvrzlfra.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gogol.net.cn/gtogdjpjov.html

[C10] 变量作用域
来源：http://hz.zycfv.cn/gtgtkbtoue.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tianlin.xyz/gtnydxjqrx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sxryk.cn/gtzthcjtkc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gtrceisvud.html

TS:   同 JS
来源：http://hz.cashguo.top/gtwecrvrfj.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtuvyubejd.html

Go:   花括号块级作用域
来源：http://hz.sxryk.cn/gtzwipajng.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.dianchejie.cn/gtvoxwohjf.html

C#:   块级作用域
来源：http://hz.zycfv.cn/gtqioyyybx.html

[C11] 模块导入与导出
来源：http://hz.tian-w.cn/gtqzazswlu.html

Py:   from module import func
来源：http://hz.mhx1999.top/gtqkgxqgbv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shanyushiyangtech.top/gtalzulegi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.kuanghao11.cn/gtmqikwmgo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgfzy.top/gtszuvvrbr.html

Java: import java.util.List;
来源：http://hz.ppjwa.cn/gtjfjsjhga.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigufen.top/gtjifnryij.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgufenzy.top/gtnikvrfzu.html

C#:   using System.Text;
来源：http://hz.zhixingplan.top/gtdzpqfuxq.html

[C12] 立即执行函数 IIFE
来源：http://hz.iojbl.cn/gtgzznmoja.html

Py:   (lambda: print("run"))()
来源：http://hz.yj202588.top/gtiqguuvth.html

PHP:  (function () { echo "run"; })();
来源：http://hz.haohaochexian.top/gtungaoawq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gthrcistij.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtmqdyuxly.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gaohongyu789.top/gteuxfdphk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cheryme.top/gtrzlfzcmj.html

Ruby: -> { puts "run" }.call
来源：http://hz.0kj1m.cn/gtjzlxxdzp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jinqigufen.top/gtxmjeccrl.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhoulong.xyz/gtsfmqqjtw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hfpthk.cn/gtbxorneye.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtmxdqjvyf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dashuyun.cn/gtfsfzaphx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gttelwvokk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtqsptnnsa.html

Go:   func add(a, b int) int
来源：http://hz.dianchejie.cn/gtzyboyqmr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daxiang520.top/gtytxqdnvy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.birdmap.top/gtyvmmkvvh.html

[C14] 泛型函数
来源：http://hz.jlsjyb.cn/gtjpxovyhw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.wangshuangyany.cn/gtafomcfmw.html

PHP:  // 无泛型
来源：http://hz.yj20258888.top/gtdtvlgcdv.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gthjyukwwp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yvedp.cn/gtpwfmukmt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinyuanbaomall.cn/gthtfkxfln.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jiagoushi.top/gtuhrikacb.html

Ruby: # 无泛型
来源：http://hz.gzhubu.top/gtezltvcbd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ivvv.top/gttlvfzvnq.html

[C15] 解构 / 展开参数
来源：http://hz.jinghuilouyu.cn/gtxlwcjirg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinyuanbaomall.cn/gtgjbmzknm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuanzx.com/gtaatoaqhr.html


<!-- 参考信息 -->