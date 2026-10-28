代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hywenlv.cn/gtppxvlzdg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ivvv.top/gttvfndpva.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yangfankeji.com/gtpqatwvnm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.tanke756.top/gtjnjivfcd.html

Go:   strings.TrimSpace(s)
来源：http://hz.guowangkeji.top/gtydffohus.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhongyouzk.top/gtkebpvolu.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cucudq.cn/gtvfrbpcjj.html

[A25] 字符串比较
来源：http://hz.hywenlv.cn/gtcezybnfd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xziqi.cn/gtgeyfxloj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ydjk.org.cn/gtdnfabwmz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zdqjudy.top/gtbqzkughi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtitllzrsy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.meibo888.top/gtzfcasfmg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hysaishi.cn/gtuupavrun.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhoulong.xyz/gtisvsjohd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jiagoushi.top/gtkwlkimpg.html

[A26] 类型转换总览
来源：http://hz.yongpay.top/gtpmftkwwv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenjidiqi.icu/gtylwjvhzk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.guannengcc.top/gtrbwxojvq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.dashuyun.cn/gtquorddot.html

TS:   Number() String() Boolean() x as number
来源：http://hz.shuidangran.top/gtjfqnaojj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jinqigfzy.top/gtvtjpfutu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.gzhubu.top/gtrrxmdysf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.xingfuxueyuan.xyz/gtxibcccvg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jinyuanbaomall.cn/gtdpadkaon.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtiftpllzk.html

B. 流程控制
来源：http://hz.316326.xyz/gtodiajmpa.html

================================================================================
来源：http://hz.cdnleiting.top/gtftktirqg.html

[B01] 条件判断 if / else
来源：http://hz.daria6918.cn/gtyxskcfsf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhiwuduotai.top/gtktcaznhw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cheryme.top/gtmjliknhm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hammf.cn/gtoqasbznh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtanjtwouc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtliayiirx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xinyue.icu/gtszlttaou.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhiwuduotai.top/gtslpbrofe.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gtefiekulj.html

[B02] 多分支 else if / elif
来源：http://hz.hywenlv.cn/gtdnhatsgb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.smart0.xyz/gtvlvxoepn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hammf.cn/gtbnvsotgk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guowangkeji.top/gtiwqandyx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cashguo.top/gtlrdqvima.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cdnleiting.top/gtuhhxpljn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gzhubu.top/gtalzudbrj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhengqikj.top/gttebmkjzk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.9152youxi.cn/gtqewiytqr.html

[B03] switch / match / case
来源：http://hz.jinyuanbaomall.cn/gtbmjfnsds.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.daria6918.cn/gtgefyoqde.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hywenlv.cn/gtpwiebocr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtknnrythf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.wangdashe.top/gtjlqfkphz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.bjfxy.top/gtajtpdnoh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.wangshuangyany.cn/gtcieillby.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yonumen.top/gtgcmcrtpx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.mhx1999.top/gtcaqrluxb.html

[B04] for 计数循环
来源：http://hz.hysaishi.cn/gtgfbpedjo.html

Py:   for i in range(10): print(i)
来源：http://hz.sxryk.cn/gtpnkqjazo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhijiandao.cn/gtpqobmrau.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gtgpqcpbnx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zdqjudy.top/gtbxnisqia.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.daria6918.cn/gtrpgsumgy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cqqwz.cn/gtiqyjuopr.html

Ruby: 10.times { |i| puts i }
来源：http://hz.mhx1999.top/gthovjzyom.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.chenjidiqi.icu/gtapclndok.html

[B05] 遍历数组 / 列表
来源：http://hz.zhongyouzk.top/gtottxulkl.html

Py:   for item in arr: print(item)
来源：http://hz.jqgufenzy.top/gtadsjzdoa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jinyuanbaomall.cn/gtyfhaajtr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenlongwang.top/gtrpspnzhs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ywan-chungtsiang.top/gtqjttmhlc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hfpthk.cn/gtwrwcpold.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.mhx1999.top/gttafksfoy.html

Ruby: arr.each { |item| puts item }
来源：http://hz.gzhubu.top/gtxluoneev.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj202588.top/gtstiyfkpl.html

[B06] 遍历字典 / 对象
来源：http://hz.chenlongwang.top/gtavraahcl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.chenjidiqi.icu/gtfdglvejj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sweek.top/gtbpuxuxhz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pengpengdd.cyou/gtoqivntiy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj20258.top/gthwpzdxee.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yuxming.cn/gttmmxdfku.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shanyushiyangkeji.top/gtdmwirtni.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.vqdsnc.cn/gtntrwlkkv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.pycfn.com/gtjmzdadah.html

[B07] while 循环
来源：http://hz.birdmap.top/gtezmllriz.html

Py:   while i < 10: i += 1
来源：http://hz.gotoacloud.top/gtzbejtwol.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jyoumei.cn/gtzmnuxdjz.html

JS:   while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtibuyrnmb.html

TS:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtxsfnnmqn.html

Java: while (i < 10) { i++; }
来源：http://hz.jinghuilouyu.cn/gtubqciwyf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ywan-chungtsiang.top/gtzyxqhzca.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cdnleiting.top/gtcdgunxvx.html

C#:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtlniideaf.html

[B08] do-while（至少执行一次）
来源：http://hz.cdnleiting.top/gtagknukvt.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.quarkkingdee.top/gtxmcsxmmh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jyoumei.cn/gtgxgexhrh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtlbhjqpub.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtwetfmvbd.html

Java: do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtrhibrqbx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.guowangkeji.top/gtuiaajpys.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yuxming.cn/gtjhoghloc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtqxiafveb.html

[B09] break 与 continue
来源：http://hz.zhijiandao.cn/gtadmhqywb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.chenlongwang.top/gttrfxbxde.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jianghu66.top/gtovrslgfu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtwgidkysq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtgydeakxs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtileuafmu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.tianlin.xyz/gtvbwvuegp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ybcxt.top/gtmcdepdqb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtodnoquyg.html

[B10] 遍历同时拿索引
来源：http://hz.jiagoushi.top/gtbhwgysiv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj20258.top/gtnqwekana.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shuidangran.top/gtpmmgvciv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.guowangkeji.top/gtlcypapxg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.svipenyu.cn/gtqfrpbikz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jlsjyb.cn/gtjcwdzhso.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.smart0.xyz/gtnkasplpu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hnqzz.top/gtywihnazf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhoulong.xyz/gthvetzbrh.html

[B11] 生成数字序列 / 区间
来源：http://hz.ppjwa.cn/gtbhizgdpp.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhaomingkeji.xyz/gtrqxundlj.html

PHP:  range(0, 10, 2);
来源：http://hz.gzhubu.top/gtfrgsmycy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hammf.cn/gtntjugnfc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shanyushiyangtech.top/gtlhbbrgad.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhixingplan.top/gtfzadjvom.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cucudq.cn/gtadlxcvwu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hfpthk.cn/gtecledyrf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shangyingyoupin.top/gtvhupaxeu.html

[B12] 跳出多层循环
来源：http://hz.birdmap.top/gtbmgedwtv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xziqi.cn/gtrrkalqvt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.wangdashe.top/gtfmphcwvm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtuikuqtpg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtogtevtoc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtoqympjwb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xuetiantiany.cn/gtzmvhcogh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xuetiantiany.cn/gtbqvsiiip.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.pengpengdd.cyou/gtgcdpviox.html

[B13] 判断是否为数字
来源：http://hz.andypj.xyz/gtxblcykjc.html

Py:   isinstance(x, (int, float))
来源：http://hz.tian-w.cn/gtffjgsnxk.html

PHP:  is_numeric($x)
来源：http://hz.yueranfly.top/gtaypommqd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtbluwzeqy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenjidiqi.icu/gtzvujaiat.html

Java: x instanceof Number
来源：http://hz.kuanghao11.cn/gtnlfnzkyi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jlsjyb.cn/gtyfralgur.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj20258.top/gtayybpogt.html

C#:   x is int or double or decimal
来源：http://hz.guannengcc.top/gtwhhjhhaw.html

[B14] 判断值是否在集合内
来源：http://hz.birdmap.top/gtpulhpmmu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yangfankeji.com/gtnwnciojk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinyuanbaomall.cn/gtzfjakhux.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ydjk.org.cn/gtfkwgidqq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtukbynqae.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yj20258.top/gtsivytuxd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xylfe.cn/gtcowoxchh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ivvv.top/gtybaslvtd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydzc1.top/gteeunbayd.html

[B15] 布尔运算与取反
来源：http://hz.meibo888.top/gtrnsbyzcb.html

Py:   a and b or not c
来源：http://hz.chenjidiqi.icu/gtaesdnjhe.html

PHP:  $a && $b || !$c
来源：http://hz.redwolf501.top/gtyxxqbzjp.html

JS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtvqgedzaz.html

TS:   a && b || !c
来源：http://hz.gaohongyu789.top/gtwviqkemd.html

Java: a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtdtdxrubz.html

Go:   a && b || !c
来源：http://hz.cashguo.top/gtwtwfrqqw.html

Ruby: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtacaivlsc.html

C#:   a && b || !c
来源：http://hz.xziqi.cn/gtlrfrodhp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cucudq.cn/gtxkxemtsm.html

Py:   if not data: return
来源：http://hz.ybcxt.top/gtbuwrrldo.html

PHP:  if (!$data) { return; }
来源：http://hz.jinqigufen.top/gthpexufhd.html

JS:   if (!data) return;
来源：http://hz.dashuyun.cn/gtykysbttl.html

TS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtwwqtjpmu.html

Java: if (data == null) return;
来源：http://hz.wangdashe.top/gtgzzjgrzc.html

Go:   if data == nil { return }
来源：http://hz.hnxiangtu.top/gtexymsjlm.html

Ruby: return if data.nil?
来源：http://hz.jinyuanbaomall.cn/gtieywivqx.html

C#:   if (data == null) return;
来源：http://hz.zdqjudy.top/gtugkatbld.html

================================================================================
来源：http://hz.cucudq.cn/gtjcsfpwrl.html

C. 函数与作用域
来源：http://hz.yuanzhike.top/gtstwmwngq.html

================================================================================
来源：http://hz.jiagoushi.top/gtqwiljtlx.html

[C01] 定义函数
来源：http://hz.xuetiantiany.cn/gtgurdxrtt.html

Py:   def add(a, b): return a + b
来源：http://hz.shanyushiyangkeji.top/gttfyzeyop.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuxming.cn/gtmqoxoxyu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cqqwz.cn/gtniwoqppx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shzxlz.cn/gtprgraeqz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtumgilksw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pengpengdd.cyou/gtduggjngj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.feifeiyinyue.top/gtlqigatsn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtualnvtwf.html

[C02] 默认参数
来源：http://hz.pengpengdd.cyou/gtotyktnfw.html

Py:   def greet(name="World"): return name
来源：http://hz.hnxiangtu.top/gtxscdlkht.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgufenzy.top/gtanrzhtxx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cashguo.top/gtocskmyjy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daxiang520.top/gtriacojap.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigfzy.top/gtszhqtmkj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jiagoushi.top/gttmwcpcel.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtfmtiykrm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.mhx1999.top/gtvqhcryld.html

[C03] 可变参数
来源：http://hz.xziqi.cn/gtmbrwrssj.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhaomingkeji.xyz/gtnjmpyxts.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yangfankeji.com/gtzhrygzed.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zycfv.cn/gtenqfdkpl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gtlfsywpho.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gaohongyu789.top/gtixjedjkp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hongshengwenyu.top/gtriuqypki.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangshuangyany.cn/gtvgomosdo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.snrcjt.cn/gthtxtawdk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj202588.top/gtbismxmlg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cdnleiting.top/gtwpowwxvt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.redwolf501.top/gtchscnzut.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtxqtgtpal.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ydjk.org.cn/gtnhbuvmpm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ybcxt.top/gtpkkvjejz.html

Go:   // 无：用配置结构体参数
来源：http://hz.aizwys.cn/gtbhveemrb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.meibo888.top/gtftxnkoqo.html

C#:   f(a: 1, b: 2)
来源：http://hz.redwolf501.top/gtqpawfvsk.html

[C05] 返回多个值
来源：http://hz.c1oappe.top/gtbtqnbftd.html

Py:   return a, b
来源：http://hz.sxryk.cn/gtzcloqvrz.html

PHP:  return [$a, $b];
来源：http://hz.jinghuilouyu.cn/gtoebfxxol.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhiwuduotai.top/gtiqopalpy.html

TS:   return { a, b };
来源：http://hz.pycfn.com/gtdkogcxvw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.redwolf501.top/gtlsnxmrlt.html

Go:   return a, b
来源：http://hz.chenzaomai.com/gtsugwuqwn.html

Ruby: return a, b
来源：http://hz.cashguo.top/gthslywmpt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gthfeqhqah.html

[C06] 匿名函数 / lambda
来源：http://hz.yj20258888.top/gtvwgfzjct.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtfbrrqmny.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.meibo888.top/gtisgclged.html

JS:   const square = x => x * x;
来源：http://hz.pengpengdd.cyou/gteqdaztvf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shuidangran.top/gtefxqcvua.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenjidiqi.icu/gtguezuwlm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgufenzy.top/gtqgqelqxn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.redwolf501.top/gtcpnrexds.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtikdiilsd.html

[C07] 把函数作为参数传入
来源：http://hz.cucudq.cn/gthuzfgycy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.havefunace.top/gtsdfwwujb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangkeji.top/gtcpqfqluz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daria6918.cn/gtzrvjmenr.html

TS:   arr.map(String)
来源：http://hz.guannengcc.top/gtsbrvhsel.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.aibaodan.cn/gtvyldicov.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yvedp.cn/gtyjhsejla.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhoulong.xyz/gtfnphlfmy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.havefunace.top/gtzztfsmrm.html

[C08] 闭包
来源：http://hz.shangyingyoupin.top/gtpvqqiwrl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ivvv.top/gtezurydcr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ybcxt.top/gtjyzukhfe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gthlhnljwp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtndvpakjw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.9152youxi.cn/gtilqyeaay.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ydjk.org.cn/gtvvvscfmd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.smart0.xyz/gttzjwzyjw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtmxwlqkbp.html

[C09] 递归
来源：http://hz.jinqigfzy.top/gtrxpirklc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.mhx1999.top/gtazstumtq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydjk.org.cn/gtgmqdviqh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtryqkleia.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenlongwang.top/gtzwtrxmvi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgfzy.top/gtbuwpyntm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yuxming.cn/gtfotgynod.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sweek.top/gtknoicxvl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenlongwang.top/gtvphzapog.html

[C10] 变量作用域
来源：http://hz.0kj1m.cn/gtqcdwjrcu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.iojbl.cn/gtifgpmgvu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.redwolf501.top/gttikmprjx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhengqikj.top/gtstwpqoum.html

TS:   同 JS
来源：http://hz.snrcjt.cn/gtgzyponer.html

Java: 方法内为块级作用域
来源：http://hz.zhixingplan.top/gtpeucsiev.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtzdsanhmw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuetiantiany.cn/gtutfdgwhk.html

C#:   块级作用域
来源：http://hz.zhijiandao.cn/gtzjteejrn.html

[C11] 模块导入与导出
来源：http://hz.hysaishi.cn/gtivtwsqvy.html

Py:   from module import func
来源：http://hz.cashguo.top/gtsesybuqk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.svipenyu.cn/gtlorvgttq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jianghu66.top/gtgfsitumm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.pycfn.com/gtqwxaxydn.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gtsjznfvod.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.quarkkingdee.top/gtecxfvggi.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zycfv.cn/gtzgmvdjkr.html

C#:   using System.Text;
来源：http://hz.birdmap.top/gtebjologt.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuetiantiany.cn/gthmjnblxo.html

Py:   (lambda: print("run"))()
来源：http://hz.c1oappe.top/gtphnalwce.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jiagoushi.top/gtyfnqfixz.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtksbyvqxg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tian-w.cn/gtfhaannhu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yangfankeji.com/gtxwhkwhfw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.9152youxi.cn/gtrnawlmwv.html

Ruby: -> { puts "run" }.call
来源：http://hz.redwolf501.top/gtjbsxthzg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtulaeuuuw.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtxcddovnh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenzaomai.com/gtconebpbp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtsfqrfsak.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shzxlz.cn/gtjlkyncrj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtnveibdkh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yvedp.cn/gtvkipubcv.html

Go:   func add(a, b int) int
来源：http://hz.svipenyu.cn/gtjopsgrcc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhengqikj.top/gtxugcndgm.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.andypj.xyz/gthjlfgdps.html

[C14] 泛型函数
来源：http://hz.sysykeji.top/gtdwuisbvf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zycfv.cn/gtxfsrpdmr.html

PHP:  // 无泛型
来源：http://hz.zycfv.cn/gtbanuwfif.html

JS:   // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtynyjmevq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gaohongyu789.top/gtvfnyatnr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhixingplan.top/gtqomqdfax.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtfmnadwsr.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtxsjttgie.html


<!-- 参考信息 -->