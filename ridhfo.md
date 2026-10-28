代发 wailian999

[A26] 类型转换总览
来源：http://hz.xuetiantiany.cn/gtxemmorua.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xziqi.cn/gtlehagsap.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.wangshuangyany.cn/gtqijoftfe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.vqdsnc.cn/gtgypmwtug.html

TS:   Number() String() Boolean() x as number
来源：http://hz.wangshuangyany.cn/gthcmlfqxv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xylfe.cn/gtrpyxwvuv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.sufxvd.cn/gtqyynatke.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.meibo888.top/gtxjfgimqs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zycfv.cn/gtwlcmjcig.html

================================================================================
来源：http://hz.yj202588.top/gtnitbvwsg.html

B. 流程控制
来源：http://hz.sweek.top/gtvgcwmgpn.html

================================================================================
来源：http://hz.gogol.net.cn/gtkglkbflp.html

[B01] 条件判断 if / else
来源：http://hz.xuanzx.com/gtfpyjhxcr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.tian-w.cn/gtnndejzfm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yvedp.cn/gtrccjarfp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hysaishi.cn/gtgjkwlgde.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yuanzhike.top/gtrayzgcko.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.chenzaomai.com/gtqtdyhwul.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhiwuduotai.top/gttdhxgviy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yj20258888.top/gthbllfkmq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtqxnnondu.html

[B02] 多分支 else if / elif
来源：http://hz.sweek.top/gthfhcczyq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.tanke756.top/gtovppbibn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.sxryk.cn/gtuupeibbl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hnqzz.top/gtigkmvmko.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gtxszsqjuu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtlcnorvgs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.c1oappe.top/gtyuvbotwr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.daxiang520.top/gtwobudjtz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenjidiqi.icu/gtjyapstow.html

[B03] switch / match / case
来源：http://hz.shuidangran.top/gtyehhrgjf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.9152youxi.cn/gtdxqlcwhg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhixingplan.top/gtvtvwqlys.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xuanzx.com/gtkpegzqor.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xinyue.icu/gtwkhbybmq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.redwolf501.top/gtbhucdntw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.smart0.xyz/gtsajrzzmj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cdnleiting.top/gtsbidndwg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhoulong.xyz/gtvhsscdex.html

[B04] for 计数循环
来源：http://hz.yongpay.top/gtnkzpntkr.html

Py:   for i in range(10): print(i)
来源：http://hz.ywan-chungtsiang.top/gtxaustcnq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gzhubu.top/gtyqzcxxkt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gtmcwmqozl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shanyushiyangtech.top/gtqiwoxbee.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhengqikj.top/gtllpswgun.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tian-w.cn/gtgetptvvo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shzxlz.cn/gtbawwbiuq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hnxiangtu.top/gtsxodciys.html

[B05] 遍历数组 / 列表
来源：http://hz.aizwys.cn/gtnlnqahcc.html

Py:   for item in arr: print(item)
来源：http://hz.svipenyu.cn/gtibhlohfz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.guowangkeji.top/gtvnjbxzlb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.pengpengdd.cyou/gtpdznozxk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinqigfzy.top/gtitqhkhom.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shangyingyoupin.top/gtwqxjirkq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.sweek.top/gteteqasab.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj20258888.top/gtospneecc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shanyushiyangtech.top/gtmvaqhmvy.html

[B06] 遍历字典 / 对象
来源：http://hz.fzhhl.top/gtbnqcskoj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhiwuduotai.top/gtaqvtbpwp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.tianlin.xyz/gtpasktmqs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.9152youxi.cn/gtclzpfdpu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.daxiang520.top/gteihbgrrw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yueranfly.top/gtdnohmslh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sweek.top/gtsyhrcydg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hnqzz.top/gtdyvloowk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hfpthk.cn/gtfuyprwuq.html

[B07] while 循环
来源：http://hz.wangshuangyany.cn/gtebkwwezt.html

Py:   while i < 10: i += 1
来源：http://hz.jqgufenzy.top/gtqolglxbw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sxryk.cn/gtaxpkhmlo.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtjgppakkt.html

TS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtnbvadtyp.html

Java: while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtxdalayvl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xuanzx.com/gtalbqumbx.html

Ruby: while i < 10; i += 1; end
来源：http://hz.9152youxi.cn/gtjagssglw.html

C#:   while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gtsktkqntm.html

[B08] do-while（至少执行一次）
来源：http://hz.sweek.top/gtcjkbxzca.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shanyushiyangtech.top/gtkmizzkmd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenjidiqi.icu/gtdhlyfrxw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gtertyeecx.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtuqtlkgwt.html

Java: do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtlpaozjgc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.0kj1m.cn/gthojzpwql.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yuxming.cn/gtbjwrkwkm.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtcfrwctbn.html

[B09] break 与 continue
来源：http://hz.gaohongyu789.top/gtttqqryvg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sysykeji.top/gtsbuipayp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.52xcode.cn/gttcgmdsco.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tian-w.cn/gtwrbowkwo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dianchejie.cn/gtcgehbrvh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhijiandao.cn/gthfopgvmc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.feifeiyinyue.top/gtjjaveotr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jiagoushi.top/gtwaagsfwb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sweek.top/gtixsfaqpj.html

[B10] 遍历同时拿索引
来源：http://hz.shuidangran.top/gtphjcfnsj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinqigufen.top/gthofllsek.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gotoacloud.top/gtgtkilikn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.dashuyun.cn/gthdqxxvvb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aizwys.cn/gtpiaiefyp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinghuilouyu.cn/gtsnpjtsuj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pycfn.com/gtvtmonzji.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.meibo888.top/gtvbkkgcue.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shzxlz.cn/gttcccgieb.html

[B11] 生成数字序列 / 区间
来源：http://hz.sxryk.cn/gtaotnoupe.html

Py:   list(range(0, 10, 2))
来源：http://hz.316326.xyz/gtmodzmhzb.html

PHP:  range(0, 10, 2);
来源：http://hz.yj202588.top/gtgudzsngt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gtigylvoac.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.birdmap.top/gtzryxgcah.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinyuanbaomall.cn/gtmjydvoau.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.svipenyu.cn/gtohybxjqc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhixingplan.top/gtkvqspepc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yuxming.cn/gtrmygxpes.html

[B12] 跳出多层循环
来源：http://hz.nanxuanxn.top/gtkivhrisc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xziqi.cn/gtgxwvavhs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.daxiang520.top/gttwzcsgsm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sweek.top/gtkidvtryr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtwbwzjvaa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtmsettkmd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xuanzx.com/gtolhmlhyj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.haohaochexian.top/gtybwovyvz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.pycfn.com/gtprusdzub.html

[B13] 判断是否为数字
来源：http://hz.hysaishi.cn/gtjnfqzttj.html

Py:   isinstance(x, (int, float))
来源：http://hz.yanxiufei.cn/gtzltyqjrz.html

PHP:  is_numeric($x)
来源：http://hz.ydzc1.top/gtbnegwwta.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tanke756.top/gtajatwrlo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtgkoguwir.html

Java: x instanceof Number
来源：http://hz.smart0.xyz/gtltoasair.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sxryk.cn/gttckymbka.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinyuanbaomall.cn/gtwgydtlwa.html

C#:   x is int or double or decimal
来源：http://hz.havefunace.top/gtakjzuzda.html

[B14] 判断值是否在集合内
来源：http://hz.tian-w.cn/gtkrsggfku.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.guowangkeji.top/gtzzzxplml.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.sweek.top/gtjtpjkbtw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtbuhsgqow.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.aibaodan.cn/gtmvcfjrtx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.chenjidiqi.icu/gtvixbfcll.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenlongwang.top/gtcxbajndm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hnxiangtu.top/gtjdzqkjfl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.feifeiyinyue.top/gtvnvhmgoh.html

[B15] 布尔运算与取反
来源：http://hz.chenjidiqi.icu/gtuvjbgozl.html

Py:   a and b or not c
来源：http://hz.hfpthk.cn/gtjkxtjqig.html

PHP:  $a && $b || !$c
来源：http://hz.nwbrower.top/gtaitzrpov.html

JS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtxujsfetu.html

TS:   a && b || !c
来源：http://hz.hfpthk.cn/gtlggmjrxj.html

Java: a && b || !c
来源：http://hz.pengpengdd.cyou/gttpzzlrca.html

Go:   a && b || !c
来源：http://hz.jlsjyb.cn/gtaurhyiok.html

Ruby: a && b || !c
来源：http://hz.xinyue.icu/gtmmsfjfin.html

C#:   a && b || !c
来源：http://hz.meibo888.top/gtepauwruv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jyoumei.cn/gtgnfxgzje.html

Py:   if not data: return
来源：http://hz.pycfn.com/gtderxzbai.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gtjdhwynuy.html

JS:   if (!data) return;
来源：http://hz.gogol.net.cn/gtwdqaegie.html

TS:   if (!data) return;
来源：http://hz.yuxming.cn/gtsufarejj.html

Java: if (data == null) return;
来源：http://hz.shangyingyoupin.top/gtfkmfgscl.html

Go:   if data == nil { return }
来源：http://hz.zhaomingkeji.xyz/gthxtaymgj.html

Ruby: return if data.nil?
来源：http://hz.aizwys.cn/gtciwapekw.html

C#:   if (data == null) return;
来源：http://hz.cqqwz.cn/gtwzlddkcf.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtafbmcgtp.html

C. 函数与作用域
来源：http://hz.tanke756.top/gtblskyhyr.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnabmgdqa.html

[C01] 定义函数
来源：http://hz.mhx1999.top/gtfetzrqem.html

Py:   def add(a, b): return a + b
来源：http://hz.zhengqikj.top/gtovprbkqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtcmpkxioc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nanxinkj.top/gtgfccxecv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtglgalpsy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtbsrqkkpu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.snrcjt.cn/gtporepjzc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xingfuxueyuan.xyz/gtalmgplcg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtpefctabx.html

[C02] 默认参数
来源：http://hz.gaohongyu789.top/gtqkloxzyd.html

Py:   def greet(name="World"): return name
来源：http://hz.zhijiandao.cn/gteerftfqo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tian-w.cn/gtzoyvypua.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.mhx1999.top/gtyazzpgbs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jlsjyb.cn/gtuhslmhkd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuanzhike.top/gtrmbplqyr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangtech.top/gtgwjsqphv.html

Ruby: def greet(name = "World") = name
来源：http://hz.hfpthk.cn/gtylntbmjz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.aibaodan.cn/gtzpjdocgm.html

[C03] 可变参数
来源：http://hz.guowangkeji.top/gtjxtgbtwm.html

Py:   def total(*args): return sum(args)
来源：http://hz.sweek.top/gtrcivecsc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hfpthk.cn/gtimyenfkg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guowangkeji.top/gtgpxmkjjv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gtlfnzmlcd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cdnleiting.top/gtslvrrdzp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yongpay.top/gtkbcbftwk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hammf.cn/gtsbtifyyt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhengqikj.top/gtkeaorpsq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tian-w.cn/gtrxammlac.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sysykeji.top/gtbbemueae.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ppjwa.cn/gtlqvfeqln.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.meibo888.top/gtpxlajyea.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhoulong.xyz/gtwymvikcg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.aizwys.cn/gtzwifawsk.html

Go:   // 无：用配置结构体参数
来源：http://hz.c1oappe.top/gtmzjwbgnf.html

Ruby: f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gttrhikvmy.html

C#:   f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gtttowwnxm.html

[C05] 返回多个值
来源：http://hz.cucudq.cn/gtguzcxaya.html

Py:   return a, b
来源：http://hz.hnxiangtu.top/gtlatldwbg.html

PHP:  return [$a, $b];
来源：http://hz.andypj.xyz/gtjdwbjjkn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.52xcode.cn/gtywzpysem.html

TS:   return { a, b };
来源：http://hz.sxryk.cn/gtgfjtclem.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guannengcc.top/gthagooigd.html

Go:   return a, b
来源：http://hz.9152youxi.cn/gtcssewjah.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gtbprkcazh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.andypj.xyz/gtqwacnkbe.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gtmktmprbf.html

Py:   square = lambda x: x * x
来源：http://hz.fengsongda.top/gtoxteuxxu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.andypj.xyz/gthytqmlrk.html

JS:   const square = x => x * x;
来源：http://hz.yuanzhike.top/gtxjgcqndl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gtejrmwkuu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.fengsongda.top/gtvapfozwr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gtybstzoza.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhaomingkeji.xyz/gtqmitztqg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnqzz.top/gtjewfphme.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtfoqfcyzk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jqgufenzy.top/gtflomahny.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ehwqpu.com/gthlyvlkwm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj20258888.top/gtzjxxccnk.html

TS:   arr.map(String)
来源：http://hz.guowangkeji.top/gtesottwem.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.meibo888.top/gtrdamykjq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cheryme.top/gttwlmdgrt.html

Ruby: arr.map(&:upcase)
来源：http://hz.ppjwa.cn/gtcivphrzz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.svipenyu.cn/gtarprdenk.html

[C08] 闭包
来源：http://hz.jyoumei.cn/gtyznzknaz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cdnleiting.top/gtqnspfspy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cucudq.cn/gtkexryqip.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtzgaoezpl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtocqfgtnb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shanyushiyangkeji.top/gtaveuurta.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pycfn.com/gteiaecvmb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ppjwa.cn/gtmssjgomk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtomveekqm.html

[C09] 递归
来源：http://hz.jiagoushi.top/gthxknhtvo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gtovflgtky.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.gogol.net.cn/gtdqvorrpz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nwbrower.top/gtwuxcrjtr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cheryme.top/gtqdpzroft.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ydzc1.top/gtterwldkk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sufxvd.cn/gtyzrdikaz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gzhubu.top/gtbdiammpz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.birdmap.top/gtqzeudcra.html

[C10] 变量作用域
来源：http://hz.fzhhl.top/gttjnxvcir.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.fengsongda.top/gtxmaprvcm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cheryme.top/gthbdjoghj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sufxvd.cn/gtomubylvp.html

TS:   同 JS
来源：http://hz.svipenyu.cn/gtouinbxrf.html

Java: 方法内为块级作用域
来源：http://hz.zhoulong.xyz/gtyseebktl.html

Go:   花括号块级作用域
来源：http://hz.wangdashe.top/gtexxglfug.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.birdmap.top/gtvacnfpbg.html

C#:   块级作用域
来源：http://hz.ivvv.top/gtzmckajpj.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtelzjalqv.html

Py:   from module import func
来源：http://hz.shuidangran.top/gtelaxpkmp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtactozvgd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuanzx.com/gtorlehmrw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.0kj1m.cn/gttdkdnjqs.html

Java: import java.util.List;
来源：http://hz.bjfxy.top/gttbupcaob.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.tanke756.top/gtemotegfz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shzxlz.cn/gtouddsmbt.html

C#:   using System.Text;
来源：http://hz.jianghu66.top/gtyiklsvah.html

[C12] 立即执行函数 IIFE
来源：http://hz.vqdsnc.cn/gtugegxlmw.html

Py:   (lambda: print("run"))()
来源：http://hz.ybcxt.top/gtqrnjlbmz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yvedp.cn/gttozodlan.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhixingplan.top/gtrimfpcov.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtiqsvuyay.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gtxmgverib.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhengqikj.top/gttjttmdhs.html

Ruby: -> { puts "run" }.call
来源：http://hz.pycfn.com/gtdwemrtgu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gtthaobuen.html

[C13] 类型声明 / 类型注解
来源：http://hz.xziqi.cn/gtcazugozb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ppjwa.cn/gtvrrkjntk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cheryme.top/gtopkbzsyc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sxryk.cn/gtjxrwweyj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sufxvd.cn/gtiebqgduh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtxrkwsnnh.html

Go:   func add(a, b int) int
来源：http://hz.yuxming.cn/gthgamfele.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigfzy.top/gtcnfmnnsd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yj20258.top/gtrejobndi.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtwqtcwopk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhijiandao.cn/gtanrsqnti.html

PHP:  // 无泛型
来源：http://hz.cheryme.top/gtgauzmlor.html

JS:   // 无泛型
来源：http://hz.gzhubu.top/gtwxoqwllg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gtbocmmssd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daxiang520.top/gtrebfznyp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnqzz.top/gtexxlibmr.html

Ruby: # 无泛型
来源：http://hz.snrcjt.cn/gtligtjwan.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daxiang520.top/gthocmchmy.html

[C15] 解构 / 展开参数
来源：http://hz.quarkkingdee.top/gtdywmgpzd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hywenlv.cn/gtrybhgmgr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gtogyiqmbs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinghuilouyu.cn/gtziseksuc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.birdmap.top/gtctrtskkw.html

Java: // 无解构
来源：http://hz.ehwqpu.com/gtetnwttqv.html

Go:   // 无解构
来源：http://hz.gzhubu.top/gtmenxbysb.html

Ruby: a, b = pair
来源：http://hz.yuxming.cn/gtmviamgya.html

C#:   var (a, b) = pair;
来源：http://hz.chenjidiqi.icu/gtuijiqsed.html

[C16] 函数 / 方法重载
来源：http://hz.nwbrower.top/gttiilnsal.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nwbrower.top/gtudsqezqn.html

PHP:  // 无重载
来源：http://hz.ydjk.org.cn/gtbovaukrb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.smart0.xyz/gtmuwvrbpg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sysykeji.top/gtddvnvpxf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.tianlin.xyz/gtlfkqmdez.html


<!-- 参考信息 -->