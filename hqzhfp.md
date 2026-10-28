代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://hz.ehwqpu.com/gtgeemfuxm.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.sxryk.cn/gtknfqztpl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.gzhubu.top/gtoftnpali.html

[A25] 字符串比较
来源：http://hz.jinyuanbaomall.cn/gtgxiluxnx.html

Py:   s1 == s2; s1 != s2
来源：http://hz.9152youxi.cn/gtkbzlcwhs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.quarkkingdee.top/gtzhttohfq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nwbrower.top/gtmhzceuhe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sweek.top/gtwndczdmw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yanxiufei.cn/gtfwgxsqqt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shanyushiyangtech.top/gtgdfpxzhs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sweek.top/gtlxbfefek.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gtetpxgujg.html

[A26] 类型转换总览
来源：http://hz.xylfe.cn/gtztxigwum.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.pycfn.com/gtolbxntar.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ydzc1.top/gttcukkpzg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xziqi.cn/gtcvbgdyis.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yj202588.top/gttnpusbbx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shanyushiyangkeji.top/gtgulcdcwi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.nanxuanxn.top/gtrrpdfaun.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jiagoushi.top/gtwadsugkm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.snrcjt.cn/gtqfpkfyld.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqxdogfzz.html

B. 流程控制
来源：http://hz.sufxvd.cn/gtrewavxwq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxrbfjauj.html

[B01] 条件判断 if / else
来源：http://hz.zhongyouzk.top/gtknjuhvdx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhoulong.xyz/gtvtpnseoq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.haohaochexian.top/gthqwptoos.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtotjpovky.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtajwrrmhh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gtxehqtxxc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yj202588.top/gttxzawrys.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.sweek.top/gttmvicmar.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yonumen.top/gtllvnpewm.html

[B02] 多分支 else if / elif
来源：http://hz.birdmap.top/gtqgcetkmd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.haohaochexian.top/gtickfrosh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gotoacloud.top/gtkvmglkxu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtxwunisyd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gtjfayuxjj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuxming.cn/gtwlmsfygd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.dashuyun.cn/gtbnjxengy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yvedp.cn/gtoppdjbmr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gteourwcfo.html

[B03] switch / match / case
来源：http://hz.pengpengdd.cyou/gtruyyxmnn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj202588.top/gtnfwwjchj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhiwuduotai.top/gtyojsgsqy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daria6918.cn/gtktoksznu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258.top/gtsratuoeu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shuidangran.top/gtkwkpbdmt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.chenlongwang.top/gtgstiwvlb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shanyushiyangkeji.top/gtwgwdytiq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yj20258.top/gtxklmildz.html

[B04] for 计数循环
来源：http://hz.zhengqikj.top/gtlrvlxodl.html

Py:   for i in range(10): print(i)
来源：http://hz.ydzc1.top/gtqqyatlhc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jiagoushi.top/gtfzcidbby.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.aibaodan.cn/gtjzuqdtxo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sxryk.cn/gtgpqpwnjo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.haohaochexian.top/gtepdcqdva.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.wangshuangyany.cn/gtqlbzxdvl.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jyoumei.cn/gtikfddzok.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.wangshuangyany.cn/gtuavdudsf.html

[B05] 遍历数组 / 列表
来源：http://hz.jinqigfzy.top/gtodcowiwd.html

Py:   for item in arr: print(item)
来源：http://hz.wangshuangyany.cn/gtuyxwwllr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.snrcjt.cn/gtpkoqyjjw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ppjwa.cn/gthrxqvsvm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenjidiqi.icu/gtuurwhhht.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yuxming.cn/gtoqkifsbf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinqigfzy.top/gtdndspdbt.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hongshengwenyu.top/gtsfzdpqjg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hnqzz.top/gtsmyxucpf.html

[B06] 遍历字典 / 对象
来源：http://hz.iojbl.cn/gttpscbygy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.smart0.xyz/gtquylgdhz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinqigfzy.top/gthhfxtszs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinyuanbaomall.cn/gtxbniwuhw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.iojbl.cn/gtuuxbttjn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhixingplan.top/gtgykfsoiw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hfpthk.cn/gtzstlorgr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jiagoushi.top/gtkqmrnpmw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gogol.net.cn/gtskwoydea.html

[B07] while 循环
来源：http://hz.ywan-chungtsiang.top/gttgnsgeak.html

Py:   while i < 10: i += 1
来源：http://hz.ivvv.top/gtkogxoiih.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.guannengcc.top/gtdgygduoa.html

JS:   while (i < 10) { i++; }
来源：http://hz.yvedp.cn/gtpqqyvjnv.html

TS:   while (i < 10) { i++; }
来源：http://hz.yuanzhike.top/gteusbqfrn.html

Java: while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gtzkslphtj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yvedp.cn/gtgzzfinxq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.chenjidiqi.icu/gtifjcwfyp.html

C#:   while (i < 10) { i++; }
来源：http://hz.tian-w.cn/gtbbcnyonj.html

[B08] do-while（至少执行一次）
来源：http://hz.ybcxt.top/gtgijkuwzl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.pycfn.com/gtgxuzvdxl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenjidiqi.icu/gtgrflycer.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtbmrugqop.html

TS:   do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gtcyamdnpa.html

Java: do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtrtdklohi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.0kj1m.cn/gtsusseekd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhengqikj.top/gtoxjpbldh.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtahtqflvt.html

[B09] break 与 continue
来源：http://hz.shzxlz.cn/gtnklgfsrx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sweek.top/gtlwlgazop.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.svipenyu.cn/gttpmjvgts.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtnzlzewkj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtnrdvhjzs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtqozfuwiq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ybcxt.top/gtswfihrxn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.vqdsnc.cn/gtlhxaulyn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtnrcxhilr.html

[B10] 遍历同时拿索引
来源：http://hz.chenjidiqi.icu/gtmqieynrj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.daxiang520.top/gtiybwgylf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sysykeji.top/gtymdslkfe.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.52xcode.cn/gtdacksdkv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sxryk.cn/gtstociepb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.feifeiyinyue.top/gtqsovetsv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zdqjudy.top/gtujvfplqy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gotoacloud.top/gtptagdpht.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangshuangyany.cn/gtjgvxtxkl.html

[B11] 生成数字序列 / 区间
来源：http://hz.xuanzx.com/gtqcdaisry.html

Py:   list(range(0, 10, 2))
来源：http://hz.pycfn.com/gtbnbclldk.html

PHP:  range(0, 10, 2);
来源：http://hz.jinqigfzy.top/gtuxojehuf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pycfn.com/gtgppmrgil.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fzhhl.top/gtuygiohzg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinghuilouyu.cn/gtwjtyaiwh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.chenlongwang.top/gtgbkcwthz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.bjfxy.top/gtukiwcizc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.haohaochexian.top/gtiolunnuk.html

[B12] 跳出多层循环
来源：http://hz.ivvv.top/gtjukftsok.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinghuilouyu.cn/gtvujkjoft.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.9152youxi.cn/gtmitmcysf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtojcnszqt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gttsmqlwxp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gaohongyu789.top/gtskvooqpc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shangyingyoupin.top/gtsgroicmg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shzxlz.cn/gtezrsbpkl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.nanxinkj.top/gtujeakktu.html

[B13] 判断是否为数字
来源：http://hz.chenjidiqi.icu/gthddlnadp.html

Py:   isinstance(x, (int, float))
来源：http://hz.shanyushiyangtech.top/gtyimemjws.html

PHP:  is_numeric($x)
来源：http://hz.aizwys.cn/gtwyygjppa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gtafivoktt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinqigufen.top/gtdylkggie.html

Java: x instanceof Number
来源：http://hz.yvedp.cn/gtvaogyqch.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nwbrower.top/gtogyyicld.html

Ruby: x.is_a?(Numeric)
来源：http://hz.9152youxi.cn/gtywtaffgt.html

C#:   x is int or double or decimal
来源：http://hz.aibaodan.cn/gtvmkrnwxi.html

[B14] 判断值是否在集合内
来源：http://hz.fzhhl.top/gtldhyorfk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dianchejie.cn/gtxcjwzpuf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxinkj.top/gtueiqvvsx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.fengsongda.top/gtctvimoym.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtaelxamiy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinyuanbaomall.cn/gtfrykcnje.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hnqzz.top/gtymaothsg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zycfv.cn/gtuaixcjlj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xuanzx.com/gtkepcbvnu.html

[B15] 布尔运算与取反
来源：http://hz.nanxuanxn.top/gtaslfpwfw.html

Py:   a and b or not c
来源：http://hz.yuxming.cn/gtlmxnbarb.html

PHP:  $a && $b || !$c
来源：http://hz.zhixingplan.top/gtkmrvsduo.html

JS:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtgfbgdcqc.html

TS:   a && b || !c
来源：http://hz.yanxiufei.cn/gtdyfztkgy.html

Java: a && b || !c
来源：http://hz.hnxiangtu.top/gtsifcwgel.html

Go:   a && b || !c
来源：http://hz.hywenlv.cn/gtvuczqeil.html

Ruby: a && b || !c
来源：http://hz.dianchejie.cn/gtwljluwag.html

C#:   a && b || !c
来源：http://hz.havefunace.top/gtqbetatff.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhaomingkeji.xyz/gtrccsqhnl.html

Py:   if not data: return
来源：http://hz.c1oappe.top/gtvirgcfqv.html

PHP:  if (!$data) { return; }
来源：http://hz.chenlongwang.top/gtcnytykoo.html

JS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtquilelfd.html

TS:   if (!data) return;
来源：http://hz.cqqwz.cn/gtbisvdcfq.html

Java: if (data == null) return;
来源：http://hz.yj20258.top/gtluncdntl.html

Go:   if data == nil { return }
来源：http://hz.wangshuangyany.cn/gtasjicmtk.html

Ruby: return if data.nil?
来源：http://hz.feifeiyinyue.top/gtfbzeirdq.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gtarfcoewl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdrnkvteg.html

C. 函数与作用域
来源：http://hz.nanxuanxn.top/gtdcyteysv.html

================================================================================
来源：http://hz.cheryme.top/gtphrdiqcq.html

[C01] 定义函数
来源：http://hz.jqgfzy.top/gttmggsgmx.html

Py:   def add(a, b): return a + b
来源：http://hz.chenlongwang.top/gtahqmrnht.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtyyzmchwk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xylfe.cn/gtylwqidqc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ybcxt.top/gtqezvqyfu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtsibyrycm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dashuyun.cn/gtviduapiu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj202588.top/gtwwtalzwg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtdkxjogqr.html

[C02] 默认参数
来源：http://hz.guannengcc.top/gtvrsaavcu.html

Py:   def greet(name="World"): return name
来源：http://hz.ybcxt.top/gtqghqtmgk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pycfn.com/gtsvvkivlk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj202588.top/gtwkafmalu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jiagoushi.top/gtlnkebvxj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gogol.net.cn/gtixvancau.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtqkukuoju.html

Ruby: def greet(name = "World") = name
来源：http://hz.jianghu66.top/gttlvayyci.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ehwqpu.com/gtrdpffopu.html

[C03] 可变参数
来源：http://hz.cheryme.top/gtjthatzfa.html

Py:   def total(*args): return sum(args)
来源：http://hz.jqgfzy.top/gtkihfjktx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.316326.xyz/gtthobwpho.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtixkwxpjo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtzsyrnymp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.guannengcc.top/gtpkueouuk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fengsongda.top/gtnzsprgus.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cdnleiting.top/gtnstyykid.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gtksztwkvn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhoulong.xyz/gtlfnllrjl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yj202588.top/gtujhgetyg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhaomingkeji.xyz/gtaprafros.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shangyingyoupin.top/gtcutzmocc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cheryme.top/gtodyqooou.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxinkj.top/gtkhabqugy.html

Go:   // 无：用配置结构体参数
来源：http://hz.dianchejie.cn/gtameihknc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.birdmap.top/gtripiupjl.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtxbzmznfg.html

[C05] 返回多个值
来源：http://hz.yj20258.top/gtljwwbhdd.html

Py:   return a, b
来源：http://hz.yuxming.cn/gtqvjwwnev.html

PHP:  return [$a, $b];
来源：http://hz.xuanzx.com/gtcyddthxj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydzc1.top/gtsfyyoceh.html

TS:   return { a, b };
来源：http://hz.hammf.cn/gtmoeqrsxx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xinyue.icu/gtgqpvmnej.html

Go:   return a, b
来源：http://hz.snrcjt.cn/gtzhzoinpe.html

Ruby: return a, b
来源：http://hz.jinqigufen.top/gtyphpnkvh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhixingplan.top/gtobrfdppf.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtlyiktckd.html

Py:   square = lambda x: x * x
来源：http://hz.pycfn.com/gtagtrvyvj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sweek.top/gtdmnhsqgt.html

JS:   const square = x => x * x;
来源：http://hz.jlsjyb.cn/gtzytlvdct.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xinyue.icu/gtlbwjbhnr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gogol.net.cn/gtalbleesw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ywan-chungtsiang.top/gtggdbqvzn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydzc1.top/gtnuqbojbg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.9152youxi.cn/gtsddqqtom.html

[C07] 把函数作为参数传入
来源：http://hz.jinqigufen.top/gthpblcbcq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cashguo.top/gtkgwzamum.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.iojbl.cn/gtsbqnzusg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.9152youxi.cn/gtafnedjlk.html

TS:   arr.map(String)
来源：http://hz.shzxlz.cn/gtyvspgofx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.9152youxi.cn/gtnscsihry.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtyamssuqd.html

Ruby: arr.map(&:upcase)
来源：http://hz.xinyue.icu/gtbpcqovih.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gotoacloud.top/gtcnlgfghe.html

[C08] 闭包
来源：http://hz.pycfn.com/gtspkknvhp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daria6918.cn/gtdqeogbnw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aizwys.cn/gtjhvksvwt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gtouswlibh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtaejpdjgk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sysykeji.top/gtjrkdqtvm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.tian-w.cn/gthyfpaxct.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.fzhhl.top/gtvqstxwzk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtneygfdxf.html

[C09] 递归
来源：http://hz.yangfankeji.com/gtnstiizfq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sweek.top/gtgvdswfnb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xziqi.cn/gtgdmwihet.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtwakdewnb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtqlpiauyf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xziqi.cn/gtpebrxfvt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhiwuduotai.top/gtplgrhkle.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sufxvd.cn/gttrvdwarc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhijiandao.cn/gtohillgzm.html

[C10] 变量作用域
来源：http://hz.zycfv.cn/gtxxauualm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgufenzy.top/gtrcpinbbx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.smart0.xyz/gtjidnjrvd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinyuanbaomall.cn/gtoplriczj.html

TS:   同 JS
来源：http://hz.chenlongwang.top/gtbbjbmzkc.html

Java: 方法内为块级作用域
来源：http://hz.chenjidiqi.icu/gtsyxtkaxu.html

Go:   花括号块级作用域
来源：http://hz.feifeiyinyue.top/gteguexbbp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj202588.top/gthsyzeebb.html

C#:   块级作用域
来源：http://hz.nanxinkj.top/gtpwnraziy.html

[C11] 模块导入与导出
来源：http://hz.0kj1m.cn/gtxypvocti.html

Py:   from module import func
来源：http://hz.hysaishi.cn/gttedfffkm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shanyushiyangkeji.top/gtyenzbogp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xingfuxueyuan.xyz/gtxmnmhnhe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tian-w.cn/gtqwqiivaw.html

Java: import java.util.List;
来源：http://hz.jinqigfzy.top/gtagrwjunp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.mhx1999.top/gtczvujblp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gtgqngkphx.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtcdyqnhku.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhongyouzk.top/gtwpcvuufw.html

Py:   (lambda: print("run"))()
来源：http://hz.jiagoushi.top/gtyiqbcfyr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxuanxn.top/gtdprvwajs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shangyingyoupin.top/gteqbknfot.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtjxfeaevw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xziqi.cn/gtbkugjeww.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xylfe.cn/gtbclltmhg.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtxfwxuqhj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tanke756.top/gtsjwcatlj.html

[C13] 类型声明 / 类型注解
来源：http://hz.yonumen.top/gtxperubcu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fzhhl.top/gtddbkvqqi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtepnpowkq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ybcxt.top/gtyrjzifng.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hfpthk.cn/gtrogzqupj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtmxnyhjyl.html

Go:   func add(a, b int) int
来源：http://hz.hammf.cn/gtspfxuvzr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gzhubu.top/gtxeztgrie.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ybcxt.top/gtzssxxlji.html

[C14] 泛型函数
来源：http://hz.redwolf501.top/gtgqyfpzqo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shangyingyoupin.top/gthzehbryk.html

PHP:  // 无泛型
来源：http://hz.zhixingplan.top/gththjcgip.html

JS:   // 无泛型
来源：http://hz.birdmap.top/gtoeojlvgl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xuetiantiany.cn/gtecktzuua.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gogol.net.cn/gtlsvpjohu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnxiangtu.top/gtrjimosvt.html

Ruby: # 无泛型
来源：http://hz.sysykeji.top/gtpmebuswx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sxryk.cn/gtkfhjrokx.html

[C15] 解构 / 展开参数
来源：http://hz.xinyue.icu/gtpogezfqk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yuanzhike.top/gtoebjocvo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinqigufen.top/gtaqsgekdx.html


<!-- 参考信息 -->