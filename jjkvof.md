代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ybcxt.top/gtebpjolnn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.chenlongwang.top/gtbidbjtch.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sxryk.cn/gtjinmcoji.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.fzhhl.top/gtdutvmscy.html

[A26] 类型转换总览
来源：http://hz.shuidangran.top/gtsiimebkj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jqgfzy.top/gtnfaympjo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.fengsongda.top/gtbkwdyaei.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhengqikj.top/gtivpgpnyy.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yuanzhike.top/gtwwqeauzy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jlsjyb.cn/gtumfffzkf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.mhx1999.top/gtdhzceapv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jiagoushi.top/gtmnptgniz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jiagoushi.top/gttzsmrkcp.html

================================================================================
来源：http://hz.jlsjyb.cn/gtranfbocq.html

B. 流程控制
来源：http://hz.yuxming.cn/gtaggwjvut.html

================================================================================
来源：http://hz.chenlongwang.top/gtxwwjjsbv.html

[B01] 条件判断 if / else
来源：http://hz.dianchejie.cn/gtynicrjgt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.nwbrower.top/gtimjwgdgy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yongpay.top/gtxjwmrnbm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.dashuyun.cn/gtpmxdkvrm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.snrcjt.cn/gtvfwfhfaj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.dashuyun.cn/gtjsvzsult.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dashuyun.cn/gtlseyizjo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hysaishi.cn/gtrnzlgnek.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.cashguo.top/gtmfhjvlcu.html

[B02] 多分支 else if / elif
来源：http://hz.zhongyouzk.top/gtjpuketfs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jinghuilouyu.cn/gtrmvhitfh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhaomingkeji.xyz/gtxwdibnse.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hysaishi.cn/gtcbnwlgtl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenjidiqi.icu/gtpdyzpagu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtfxkermxu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hnxiangtu.top/gthszvdpjx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.smart0.xyz/gtqfalcmpn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gzhubu.top/gtwtbhstnp.html

[B03] switch / match / case
来源：http://hz.shanyushiyangtech.top/gtanfjjqqw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.shuidangran.top/gtdimqxtep.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gtidshlwbk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigufen.top/gtqgqqugiu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sweek.top/gtpjujbwsz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtcbdbfvsh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhengqikj.top/gtrerrgtfq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.tianlin.xyz/gtsjngpogd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.quarkkingdee.top/gtovxobkau.html

[B04] for 计数循环
来源：http://hz.cucudq.cn/gtljzrwjiu.html

Py:   for i in range(10): print(i)
来源：http://hz.quarkkingdee.top/gtmoxhnohh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.sufxvd.cn/gtdywebvaa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.guannengcc.top/gtprzmfyxm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tanke756.top/gtssboanoj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.iojbl.cn/gtcdilrrao.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhijiandao.cn/gtdorzjlyb.html

Ruby: 10.times { |i| puts i }
来源：http://hz.fzhhl.top/gtqkxyezsp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.vqdsnc.cn/gtnjxlfoka.html

[B05] 遍历数组 / 列表
来源：http://hz.zycfv.cn/gtrsdihozu.html

Py:   for item in arr: print(item)
来源：http://hz.redwolf501.top/gtnhuyizok.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.nwbrower.top/gtvnrssasp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhaomingkeji.xyz/gtwwjbmidh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgufenzy.top/gtezhktgwb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.gaohongyu789.top/gtkrozxavw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.0kj1m.cn/gtxpbhtqgu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ehwqpu.com/gtlmqxkieb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.tianlin.xyz/gtndludilp.html

[B06] 遍历字典 / 对象
来源：http://hz.smart0.xyz/gtexwaxrrh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sxryk.cn/gtlppvkicl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gzhubu.top/gtxncfzllj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gogol.net.cn/gtrqfflljc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.c1oappe.top/gtoyegwnuu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.snrcjt.cn/gtmkuxyetu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangdashe.top/gtqxknivpb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yj202588.top/gttxfzzoxb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xingfuxueyuan.xyz/gtvvufqynq.html

[B07] while 循环
来源：http://hz.fzhhl.top/gtfnvcerha.html

Py:   while i < 10: i += 1
来源：http://hz.yangfankeji.com/gtutkibphe.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.meibo888.top/gtuoidqngn.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhengqikj.top/gttgkdzzho.html

TS:   while (i < 10) { i++; }
来源：http://hz.aibaodan.cn/gtinbcowdf.html

Java: while (i < 10) { i++; }
来源：http://hz.yvedp.cn/gtroticpco.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.mhx1999.top/gtisxedxqy.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xuetiantiany.cn/gtimsgkydo.html

C#:   while (i < 10) { i++; }
来源：http://hz.sysykeji.top/gtumorozdi.html

[B08] do-while（至少执行一次）
来源：http://hz.yj20258.top/gtshtqocqd.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ybcxt.top/gtlfznjeej.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.tianlin.xyz/gtnueguomo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtmiyoxdlh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtvkubbdoo.html

Java: do { i++; } while (i < 10);
来源：http://hz.sweek.top/gthvucroov.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hywenlv.cn/gtavcbipcu.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.wangshuangyany.cn/gtdzrinkpd.html

C#:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtbdbdjuln.html

[B09] break 与 continue
来源：http://hz.316326.xyz/gtbfjuymtv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.guannengcc.top/gtkzpborwe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.wangdashe.top/gtprgctgzh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hfpthk.cn/gtdwempafp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtykwgfmid.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gteewuzctu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.andypj.xyz/gtnlbkzlhl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cdnleiting.top/gtxxbvefmk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtnhbuujxg.html

[B10] 遍历同时拿索引
来源：http://hz.guowangkeji.top/gtrurzthgr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.daxiang520.top/gtoobhkdug.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yvedp.cn/gtjcsqrkwt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gtzoaoytxb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zdqjudy.top/gtbnrbszri.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hammf.cn/gtsqpmwsjx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shangyingyoupin.top/gtxyevhjrh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhoulong.xyz/gtcnbqqvtl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dashuyun.cn/gtvdqaxrhq.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenjidiqi.icu/gtclukteom.html

Py:   list(range(0, 10, 2))
来源：http://hz.pycfn.com/gtpanpbazd.html

PHP:  range(0, 10, 2);
来源：http://hz.xziqi.cn/gtbzewkbfm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhongyouzk.top/gtpzgvfmrx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtepmczmqh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhijiandao.cn/gtvdkrsiye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhongyouzk.top/gteoovmfjp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.quarkkingdee.top/gttydigkii.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj20258888.top/gttywqwxpq.html

[B12] 跳出多层循环
来源：http://hz.52xcode.cn/gtfdxqbaai.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cheryme.top/gtjwrzxelg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinqigfzy.top/gtaiwbryll.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daxiang520.top/gthnqctsbu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tianlin.xyz/gtfuyffqod.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtwdbscdiv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenzaomai.com/gtsoxngdzf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hysaishi.cn/gtsyutsckl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnqzz.top/gtfrfhsaqd.html

[B13] 判断是否为数字
来源：http://hz.sweek.top/gtxouwtmcy.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtmnhajjil.html

PHP:  is_numeric($x)
来源：http://hz.zycfv.cn/gtbdipqqrj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gtnerkmuxk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yvedp.cn/gtdupwgqqz.html

Java: x instanceof Number
来源：http://hz.dianchejie.cn/gtnecogbou.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhijiandao.cn/gtctturpxo.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sysykeji.top/gtjtvdsieh.html

C#:   x is int or double or decimal
来源：http://hz.daria6918.cn/gtmxlzdydn.html

[B14] 判断值是否在集合内
来源：http://hz.hongshengwenyu.top/gthcwmlrlo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.pycfn.com/gtezkjnxxq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhengqikj.top/gtaanxqnec.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtptkxdsyk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xuetiantiany.cn/gtpvzpaucx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuxming.cn/gthxzummnw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cucudq.cn/gtawzmzykw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.fzhhl.top/gtgoawpbsl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj202588.top/gtudoypvtr.html

[B15] 布尔运算与取反
来源：http://hz.bjfxy.top/gtjlgrhvfz.html

Py:   a and b or not c
来源：http://hz.yonumen.top/gtgsmzbmoe.html

PHP:  $a && $b || !$c
来源：http://hz.hfpthk.cn/gtihrwqpsy.html

JS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtzwmcrycp.html

TS:   a && b || !c
来源：http://hz.yuxming.cn/gtvxjdnzli.html

Java: a && b || !c
来源：http://hz.cashguo.top/gtcbjyfzri.html

Go:   a && b || !c
来源：http://hz.daria6918.cn/gtbwcckwax.html

Ruby: a && b || !c
来源：http://hz.sxryk.cn/gtrrehchyb.html

C#:   a && b || !c
来源：http://hz.hnxiangtu.top/gtblbelkxl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.aizwys.cn/gtggpjvvfh.html

Py:   if not data: return
来源：http://hz.hfpthk.cn/gtspddryjq.html

PHP:  if (!$data) { return; }
来源：http://hz.chenzaomai.com/gtzmiztuoq.html

JS:   if (!data) return;
来源：http://hz.sxryk.cn/gtkhjkqgne.html

TS:   if (!data) return;
来源：http://hz.xuanzx.com/gtqsweurtd.html

Java: if (data == null) return;
来源：http://hz.xziqi.cn/gtkuafiglq.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gtkcntjgkx.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangtech.top/gtjytfkjhs.html

C#:   if (data == null) return;
来源：http://hz.yangfankeji.com/gtbxlbgptq.html

================================================================================
来源：http://hz.c1oappe.top/gtgddkfaaz.html

C. 函数与作用域
来源：http://hz.yonumen.top/gthjqkhfxb.html

================================================================================
来源：http://hz.cucudq.cn/gtkraqoxnw.html

[C01] 定义函数
来源：http://hz.9152youxi.cn/gtvdjblfzp.html

Py:   def add(a, b): return a + b
来源：http://hz.jqgfzy.top/gtxzkowzeu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtagifduxv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj20258.top/gtrzjjwuat.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtryavigpl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtclqvubvy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daxiang520.top/gtchsudcub.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj20258.top/gtrvimrfvn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtaqmyepih.html

[C02] 默认参数
来源：http://hz.316326.xyz/gthwxyspds.html

Py:   def greet(name="World"): return name
来源：http://hz.cheryme.top/gtpcirqgot.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.haohaochexian.top/gtoencvgpa.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.bjfxy.top/gtgjxiwgus.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.smart0.xyz/gttigsanbd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xingfuxueyuan.xyz/gtpokrugnw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhijiandao.cn/gtxzasrwyb.html

Ruby: def greet(name = "World") = name
来源：http://hz.dianchejie.cn/gtfvqbuder.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shuidangran.top/gtbyjglfts.html

[C03] 可变参数
来源：http://hz.zhoulong.xyz/gtahbbeppx.html

Py:   def total(*args): return sum(args)
来源：http://hz.birdmap.top/gtrgrlqyfc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.316326.xyz/gthcufhxar.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnqzz.top/gtdboydiij.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtbkppxuzu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuetiantiany.cn/gtzkcjyjce.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gaohongyu789.top/gtigsirjnn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pengpengdd.cyou/gtkijiywih.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.316326.xyz/gtlutungfu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dashuyun.cn/gtzqpcryda.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.bjfxy.top/gtsiqnamvc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gzhubu.top/gtywpwsdur.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtddpwigsr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.fzhhl.top/gtpbyylwiw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yueranfly.top/gtovcbskck.html

Go:   // 无：用配置结构体参数
来源：http://hz.nanxinkj.top/gtpdglprbh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gtbyfoskhd.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtsgnvzpuf.html

[C05] 返回多个值
来源：http://hz.jyoumei.cn/gtaivrustu.html

Py:   return a, b
来源：http://hz.yanxiufei.cn/gtterljzek.html

PHP:  return [$a, $b];
来源：http://hz.yj20258.top/gtsuthaecd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.dianchejie.cn/gtiwjwllsi.html

TS:   return { a, b };
来源：http://hz.zdqjudy.top/gtwhyvmzrj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tanke756.top/gtgbdehxin.html

Go:   return a, b
来源：http://hz.yuanzhike.top/gtxruohsww.html

Ruby: return a, b
来源：http://hz.ehwqpu.com/gtdlrxfeod.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtajeogwud.html

[C06] 匿名函数 / lambda
来源：http://hz.svipenyu.cn/gtxiudtxpz.html

Py:   square = lambda x: x * x
来源：http://hz.dashuyun.cn/gtgtcauoql.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhaomingkeji.xyz/gtvarkbqam.html

JS:   const square = x => x * x;
来源：http://hz.cqqwz.cn/gtiypmzfhh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgufenzy.top/gtytgmvzqi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guowangkeji.top/gtxgkwzfak.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pycfn.com/gtjtvwvqql.html

Ruby: square = ->(x) { x * x }
来源：http://hz.havefunace.top/gtnxawrome.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zycfv.cn/gtibeajpfv.html

[C07] 把函数作为参数传入
来源：http://hz.yongpay.top/gtmiemqniy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cheryme.top/gthefmjbjb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.haohaochexian.top/gtitmneadg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.haohaochexian.top/gtmzhcwyrg.html

TS:   arr.map(String)
来源：http://hz.yj20258.top/gtsbmlcbpw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daxiang520.top/gtjncysepu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jlsjyb.cn/gtytmhngmc.html

Ruby: arr.map(&:upcase)
来源：http://hz.xylfe.cn/gterkxeaqx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sxryk.cn/gtcdgqjbhj.html

[C08] 闭包
来源：http://hz.zhoulong.xyz/gtbozmlcco.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.0kj1m.cn/gtghzeqrzn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtirssinzh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtgpgutijn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gtejouwpte.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fengsongda.top/gtnlvnwcae.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sweek.top/gtpfupsisi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daxiang520.top/gtxrwcuezb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtozaqdkzz.html

[C09] 递归
来源：http://hz.gogol.net.cn/gtswisrits.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.kuanghao11.cn/gttjttrpaz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.bjfxy.top/gtqihordoj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtbtlftelb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guowangkeji.top/gtojyjvpdj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sufxvd.cn/gtnbzsrdfx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuetiantiany.cn/gtusglqhgn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jqgufenzy.top/gtaacmnyqb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj202588.top/gtmjjmdbze.html

[C10] 变量作用域
来源：http://hz.yongpay.top/gtgljxrjkf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zdqjudy.top/gtnuoeefrm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ivvv.top/gtrhpkjvaj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuanzx.com/gtswnjiptn.html

TS:   同 JS
来源：http://hz.zdqjudy.top/gtyylnivot.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtiipafzhk.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtjglvvwcr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigufen.top/gtiztwrous.html

C#:   块级作用域
来源：http://hz.mhx1999.top/gtkgponnvq.html

[C11] 模块导入与导出
来源：http://hz.sufxvd.cn/gtedljrnsc.html

Py:   from module import func
来源：http://hz.shzxlz.cn/gthoylkjec.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtsmxqvcqj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cucudq.cn/gtymyghksa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj202588.top/gtmhtwynpx.html

Java: import java.util.List;
来源：http://hz.quarkkingdee.top/gtayrbjept.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tian-w.cn/gtunfumzbw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zdqjudy.top/gtsfmdcans.html

C#:   using System.Text;
来源：http://hz.hysaishi.cn/gtyemeuahk.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhengqikj.top/gtojytfakw.html

Py:   (lambda: print("run"))()
来源：http://hz.yvedp.cn/gtfphlbvvi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.52xcode.cn/gtniqedbiq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtxgaxgedz.html

TS:   (() => { console.log("run"); })();
来源：http://hz.9152youxi.cn/gtvpzjflgr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.fzhhl.top/gtwnncpptj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gtzfimwznj.html

Ruby: -> { puts "run" }.call
来源：http://hz.pengpengdd.cyou/gtbwzmoeqp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hfpthk.cn/gtoxetuihh.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenlongwang.top/gtcirtvmfd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangshuangyany.cn/gtovefmpwh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gtgkxkbaig.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtzoocgpdl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxuanxn.top/gtzfuedtso.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtcmzhjuvd.html

Go:   func add(a, b int) int
来源：http://hz.cdnleiting.top/gtnuncvpjj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yongpay.top/gtxopbwlvd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gtretbwgqq.html

[C14] 泛型函数
来源：http://hz.kuanghao11.cn/gtrcatnnwn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gtnehyppco.html

PHP:  // 无泛型
来源：http://hz.gogol.net.cn/gtaoeijpxf.html

JS:   // 无泛型
来源：http://hz.haohaochexian.top/gtumgkdxae.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.vqdsnc.cn/gtrdpjllsl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shanyushiyangtech.top/gtykugzoaj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shzxlz.cn/gtvpadqqoq.html

Ruby: # 无泛型
来源：http://hz.bjfxy.top/gtmhmwfgyp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hysaishi.cn/gtiuivjftu.html

[C15] 解构 / 展开参数
来源：http://hz.yangfankeji.com/gtcqlsyaro.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jlsjyb.cn/gtqnkguvum.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhongyouzk.top/gtkdunigxw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sufxvd.cn/gtsobadhlk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.meibo888.top/gtngttsfva.html

Java: // 无解构
来源：http://hz.sysykeji.top/gtvzjhrikn.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtlmveudae.html

Ruby: a, b = pair
来源：http://hz.sufxvd.cn/gtuhjmcomn.html

C#:   var (a, b) = pair;
来源：http://hz.316326.xyz/gtftpiyykg.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtyzpehfcd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.c1oappe.top/gttmzvyfuk.html


<!-- 参考信息 -->