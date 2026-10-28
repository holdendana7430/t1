代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.gogol.net.cn/gtlgvduvpy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.birdmap.top/gtlogldzag.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.nanxinkj.top/gtgcjvhelg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.hysaishi.cn/gtirkhlgzt.html

[A26] 类型转换总览
来源：http://hz.gotoacloud.top/gtdovnzugd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sweek.top/gtdbqpvfwh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ehwqpu.com/gtdqbosqlm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xuetiantiany.cn/gtnzdarler.html

TS:   Number() String() Boolean() x as number
来源：http://hz.kuanghao11.cn/gtmjltsnat.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hnxiangtu.top/gtdnavbsim.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yangfankeji.com/gtpmrewpzt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.gzhubu.top/gthhttgifu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.bjfxy.top/gtwoomknot.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtwiztlmyb.html

B. 流程控制
来源：http://hz.daxiang520.top/gtudjgxufx.html

================================================================================
来源：http://hz.xinyue.icu/gtqrqdvywy.html

[B01] 条件判断 if / else
来源：http://hz.smart0.xyz/gtprzvsyqn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.52xcode.cn/gttsdyqasq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.dashuyun.cn/gtqmfenwfc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtnnrkslba.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.quarkkingdee.top/gtbnqgtdww.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jinghuilouyu.cn/gtojqqgvsn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.pengpengdd.cyou/gtqfdbecry.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hnqzz.top/gtzmldhatx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtmvtxxfau.html

[B02] 多分支 else if / elif
来源：http://hz.jinqigufen.top/gtvxpqnrko.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.chenzaomai.com/gtahrnqtmp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.daria6918.cn/gtisgyxstj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtaeyfdldf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtjvntwjgl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yonumen.top/gtyuklfvqi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yonumen.top/gtcwhbqdbd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.guannengcc.top/gtibcvfaiq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtadeupyip.html

[B03] switch / match / case
来源：http://hz.xziqi.cn/gtobircyqo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.ydzc1.top/gtsfjbkdrt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.nwbrower.top/gtvmhqzkyr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.vqdsnc.cn/gtqswytkcf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigufen.top/gtimdspaed.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.wangdashe.top/gttrohrkhd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yj20258.top/gtgzsuamdk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cashguo.top/gtzipxvqnq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.vqdsnc.cn/gtslnevmkn.html

[B04] for 计数循环
来源：http://hz.yj20258.top/gtndsnjjlv.html

Py:   for i in range(10): print(i)
来源：http://hz.vqdsnc.cn/gtglpljkvp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shanyushiyangtech.top/gtbykfnghi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.snrcjt.cn/gtfqzebzsv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shanyushiyangkeji.top/gtmxgrielw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yonumen.top/gtfflavahe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yongpay.top/gtjakcrvpu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.svipenyu.cn/gtylbtjjvu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhijiandao.cn/gtokymjabh.html

[B05] 遍历数组 / 列表
来源：http://hz.jiagoushi.top/gtgbpyluvu.html

Py:   for item in arr: print(item)
来源：http://hz.yueranfly.top/gtsaapzhnu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.bjfxy.top/gtooeyqygl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hfpthk.cn/gttgpopqdb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.ywan-chungtsiang.top/gtukhyckuj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.tanke756.top/gteznaakav.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xylfe.cn/gtykusatuo.html

Ruby: arr.each { |item| puts item }
来源：http://hz.daria6918.cn/gtgszcjdnp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.c1oappe.top/gtkyesocru.html

[B06] 遍历字典 / 对象
来源：http://hz.yongpay.top/gtqduayfpr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.shanyushiyangkeji.top/gtzhtbjfrh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ehwqpu.com/gtykuuywtx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhaomingkeji.xyz/gtrjfuaylw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.dianchejie.cn/gtbaehqjkw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tanke756.top/gtfuhkeavn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.chenjidiqi.icu/gtvvkdjjpr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zycfv.cn/gtklwdvnyf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.dashuyun.cn/gtnoethkhd.html

[B07] while 循环
来源：http://hz.hnxiangtu.top/gtqdhzpmso.html

Py:   while i < 10: i += 1
来源：http://hz.shangyingyoupin.top/gteocwjblh.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.snrcjt.cn/gtujmzuthf.html

JS:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtuoszpkyv.html

TS:   while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtzlhhhpyl.html

Java: while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtvyihxihu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cashguo.top/gteuwwzzmd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hysaishi.cn/gtxuwbinau.html

C#:   while (i < 10) { i++; }
来源：http://hz.xuanzx.com/gtrotyuxft.html

[B08] do-while（至少执行一次）
来源：http://hz.xylfe.cn/gtziytyrbk.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hammf.cn/gtzrquguwl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.feifeiyinyue.top/gtqxjhlpqa.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtobuaokew.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gtbnvxqtjq.html

Java: do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtdwtqnxxl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.daxiang520.top/gtkxfplbzt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.sweek.top/gtjmojlikb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gtkqahjert.html

[B09] break 与 continue
来源：http://hz.nanxinkj.top/gtpfplcnne.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pycfn.com/gtfqefskyk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hammf.cn/gttoshyqhm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtkzenszrd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtdedehege.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtjukufliv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yongpay.top/gtihngzsuu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinyuanbaomall.cn/gthkdmipkp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gthjgfpznh.html

[B10] 遍历同时拿索引
来源：http://hz.yuanzhike.top/gtwtifgpxd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.havefunace.top/gtojmbqisz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daxiang520.top/gtxuctaxom.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtjtlpnvwb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.meibo888.top/gtjconbapj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ydjk.org.cn/gtbiecsucv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.birdmap.top/gtcsvfaryl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shangyingyoupin.top/gteqjognql.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.daria6918.cn/gtevwonlsb.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhoulong.xyz/gtdwgdsejk.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenzaomai.com/gtyvlnyegy.html

PHP:  range(0, 10, 2);
来源：http://hz.tian-w.cn/gtygkwjhkp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.haohaochexian.top/gtlljzttxl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.snrcjt.cn/gtzfmdrqcs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.0kj1m.cn/gtsnpnhhpc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yangfankeji.com/gtlyyupdul.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ywan-chungtsiang.top/gtwcwxlrdb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shuidangran.top/gtsrcpnplv.html

[B12] 跳出多层循环
来源：http://hz.cqqwz.cn/gtwayymcxg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xingfuxueyuan.xyz/gttqscofmv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinyuanbaomall.cn/gtmpnfyioe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtranwtjjc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.c1oappe.top/gtqutufjek.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.iojbl.cn/gtlavptfqv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jianghu66.top/gtpmuevnzp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ivvv.top/gtivfslihb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tanke756.top/gtxonqncgb.html

[B13] 判断是否为数字
来源：http://hz.ehwqpu.com/gtxvfyzhfx.html

Py:   isinstance(x, (int, float))
来源：http://hz.yj20258888.top/gteeftnsmd.html

PHP:  is_numeric($x)
来源：http://hz.haohaochexian.top/gtkelokezo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gttzydwfrd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxinkj.top/gtvcyuucgs.html

Java: x instanceof Number
来源：http://hz.hnxiangtu.top/gtyqidccxj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtsahenqei.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuanzx.com/gtgizrregp.html

C#:   x is int or double or decimal
来源：http://hz.ehwqpu.com/gthcgqzsjf.html

[B14] 判断值是否在集合内
来源：http://hz.jyoumei.cn/gtyjcouklc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhijiandao.cn/gtlnbzhfdw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxinkj.top/gtgcpksdgm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhixingplan.top/gtdgekqsng.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtlvlrzzwm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuxming.cn/gtwbhjurkp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.snrcjt.cn/gtqfdqlgve.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.316326.xyz/gtilqpkbya.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxinkj.top/gtnwwarbyg.html

[B15] 布尔运算与取反
来源：http://hz.aizwys.cn/gtmgsvuamv.html

Py:   a and b or not c
来源：http://hz.wangdashe.top/gteocegmbm.html

PHP:  $a && $b || !$c
来源：http://hz.nwbrower.top/gtgrrkgjqy.html

JS:   a && b || !c
来源：http://hz.mhx1999.top/gtfjvoprvm.html

TS:   a && b || !c
来源：http://hz.redwolf501.top/gtvmhezwtc.html

Java: a && b || !c
来源：http://hz.zdqjudy.top/gtoujgtbch.html

Go:   a && b || !c
来源：http://hz.zdqjudy.top/gtnunjjqsz.html

Ruby: a && b || !c
来源：http://hz.dianchejie.cn/gtwtxuwsjt.html

C#:   a && b || !c
来源：http://hz.yongpay.top/gtbqspcvoy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.tian-w.cn/gttsdxbros.html

Py:   if not data: return
来源：http://hz.yanxiufei.cn/gtgkpagzer.html

PHP:  if (!$data) { return; }
来源：http://hz.sufxvd.cn/gtbusmazoe.html

JS:   if (!data) return;
来源：http://hz.mhx1999.top/gteyqnipmw.html

TS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtptxmfdxo.html

Java: if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtjhldmter.html

Go:   if data == nil { return }
来源：http://hz.9152youxi.cn/gtncfmkaub.html

Ruby: return if data.nil?
来源：http://hz.hfpthk.cn/gtookmeasq.html

C#:   if (data == null) return;
来源：http://hz.svipenyu.cn/gtfcudoywk.html

================================================================================
来源：http://hz.smart0.xyz/gtebsidhtg.html

C. 函数与作用域
来源：http://hz.shzxlz.cn/gtinoqxwfc.html

================================================================================
来源：http://hz.shuidangran.top/gtgvzfyiny.html

[C01] 定义函数
来源：http://hz.sxryk.cn/gtqoxkfkyv.html

Py:   def add(a, b): return a + b
来源：http://hz.sxryk.cn/gtitfxlavq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtkdutbabe.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gteqihzeis.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtpisnnctf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtfkgalinb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gtfwyygjjf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ehwqpu.com/gtxekghfiy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtefjiudol.html

[C02] 默认参数
来源：http://hz.ybcxt.top/gtinfsvcvk.html

Py:   def greet(name="World"): return name
来源：http://hz.aibaodan.cn/gtdybgqkwj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinqigufen.top/gtfxgeonqn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinghuilouyu.cn/gtakjmhccg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cdnleiting.top/gtahsbjacz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jlsjyb.cn/gtmbrkgybe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.iojbl.cn/gtbogyndfh.html

Ruby: def greet(name = "World") = name
来源：http://hz.haohaochexian.top/gtgrqkmezp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xuanzx.com/gtffzcryrw.html

[C03] 可变参数
来源：http://hz.kuanghao11.cn/gtavtidwop.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenzaomai.com/gtzupdnkeu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.guannengcc.top/gteqtscwxt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigufen.top/gtrarzlzsy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jyoumei.cn/gtmkerfhta.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtvaiqtrys.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xingfuxueyuan.xyz/gtennswduk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenlongwang.top/gthvjfjjqx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.pycfn.com/gthmyqwtbv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.redwolf501.top/gtpgghjrnd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.svipenyu.cn/gtzdxjudie.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.52xcode.cn/gtsqhggafi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtmnetfrtj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.0kj1m.cn/gtmeccvvlb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.birdmap.top/gtazvsygoh.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhiwuduotai.top/gtfobfinum.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtdfxmrkjk.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtlzprhdux.html

[C05] 返回多个值
来源：http://hz.yonumen.top/gtbtkjpees.html

Py:   return a, b
来源：http://hz.yangfankeji.com/gtunotzxgb.html

PHP:  return [$a, $b];
来源：http://hz.ivvv.top/gtynuysxgn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hongshengwenyu.top/gthwywfkse.html

TS:   return { a, b };
来源：http://hz.xylfe.cn/gtpbwqdywm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yongpay.top/gtoqmtijjb.html

Go:   return a, b
来源：http://hz.yuxming.cn/gtuktbqmkc.html

Ruby: return a, b
来源：http://hz.52xcode.cn/gtwrodmmfa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yuanzhike.top/gtyhbhmgji.html

[C06] 匿名函数 / lambda
来源：http://hz.sufxvd.cn/gtgcqleqwx.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangkeji.top/gtghcfzbnt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tanke756.top/gtvpfwlnys.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtzipmbldc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtyxykfbfl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.meibo888.top/gtxiiwutrq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shzxlz.cn/gtwplbazug.html

Ruby: square = ->(x) { x * x }
来源：http://hz.chenjidiqi.icu/gtpolhzsoy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.316326.xyz/gtyyohfnrz.html

[C07] 把函数作为参数传入
来源：http://hz.svipenyu.cn/gtlgwmkosi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cashguo.top/gtltdrqpqi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.svipenyu.cn/gttatjtikn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jlsjyb.cn/gtfiuimyir.html

TS:   arr.map(String)
来源：http://hz.svipenyu.cn/gtcdyjpeex.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xingfuxueyuan.xyz/gtbjehvmra.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangtech.top/gtumatpdnz.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenzaomai.com/gtkpfykolg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.mhx1999.top/gtpxzdbmiu.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtmmssuqhy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yanxiufei.cn/gtzusehbmm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangtech.top/gtsbwozzyd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtvefjbxbi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtutqredni.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenlongwang.top/gtdohdygaw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sxryk.cn/gthgrrkeei.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jiagoushi.top/gttnoazeso.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtxztdlkqx.html

[C09] 递归
来源：http://hz.shangyingyoupin.top/gtbgshazyy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinghuilouyu.cn/gtgafklzaq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.andypj.xyz/gtfhcemgxb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtmoniguyj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hysaishi.cn/gtwarqjole.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cdnleiting.top/gtpychmefc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xingfuxueyuan.xyz/gtfztyiuhv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtbmepicmm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhongyouzk.top/gtqesdlgvk.html

[C10] 变量作用域
来源：http://hz.daxiang520.top/gtygarpcpe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.mhx1999.top/gtorhxysly.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangtech.top/gtrtulodtt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cashguo.top/gtiznxmozw.html

TS:   同 JS
来源：http://hz.pycfn.com/gtfbegnidk.html

Java: 方法内为块级作用域
来源：http://hz.haohaochexian.top/gtbahwqrwl.html

Go:   花括号块级作用域
来源：http://hz.andypj.xyz/gtdskkxzjp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sufxvd.cn/gtrigxpqyz.html

C#:   块级作用域
来源：http://hz.zhoulong.xyz/gtjmtaencw.html

[C11] 模块导入与导出
来源：http://hz.aibaodan.cn/gtuyisnrag.html

Py:   from module import func
来源：http://hz.havefunace.top/gtlhohypah.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangdashe.top/gthupdkdfa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.quarkkingdee.top/gtbcjikiso.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.feifeiyinyue.top/gthzmdsawg.html

Java: import java.util.List;
来源：http://hz.dashuyun.cn/gtfdxjadgt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.wangdashe.top/gtzlzcaszc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.iojbl.cn/gtqkbifnpg.html

C#:   using System.Text;
来源：http://hz.pycfn.com/gtraikkdmz.html

[C12] 立即执行函数 IIFE
来源：http://hz.cqqwz.cn/gtilhxcasu.html

Py:   (lambda: print("run"))()
来源：http://hz.0kj1m.cn/gthjicbtpv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jiagoushi.top/gtsglgkdmb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yueranfly.top/gtonlbvfgp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.daria6918.cn/gtcvtfgsef.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jianghu66.top/gtyenexpjx.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gzhubu.top/gtwnraykls.html

Ruby: -> { puts "run" }.call
来源：http://hz.chenzaomai.com/gtgrmdjgqn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shuidangran.top/gtgvbvffjz.html

[C13] 类型声明 / 类型注解
来源：http://hz.cdnleiting.top/gtppvvgicr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gogol.net.cn/gtnwbygywp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yonumen.top/gtnwwjnxtl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtmlvkxgkt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtomnzgvrd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtqadijabs.html

Go:   func add(a, b int) int
来源：http://hz.gzhubu.top/gtjbcdtkci.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhoulong.xyz/gtlabevahk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hammf.cn/gtgdujnyyk.html

[C14] 泛型函数
来源：http://hz.chenlongwang.top/gtrgxcctvd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xziqi.cn/gtpbnjpkys.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtqxjcxkry.html

JS:   // 无泛型
来源：http://hz.yonumen.top/gtwqnbrclj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.dianchejie.cn/gtrawcpjlq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gthcpjcpdk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.birdmap.top/gtrumpzbsn.html

Ruby: # 无泛型
来源：http://hz.ydzc1.top/gtxzvvihtn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fzhhl.top/gtemgkmzur.html

[C15] 解构 / 展开参数
来源：http://hz.gogol.net.cn/gtifwiyigl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.pycfn.com/gttrycvfow.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cashguo.top/gtooagihic.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.iojbl.cn/gtkltwrzdh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.bjfxy.top/gtnydkthrf.html

Java: // 无解构
来源：http://hz.fengsongda.top/gtgsdysxlx.html

Go:   // 无解构
来源：http://hz.smart0.xyz/gtdxnrudzk.html

Ruby: a, b = pair
来源：http://hz.zdqjudy.top/gtsepcnyny.html

C#:   var (a, b) = pair;
来源：http://hz.zhaomingkeji.xyz/gtgpccyaim.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtvwpfqvmq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxuanxn.top/gthujjzcst.html


<!-- 参考信息 -->