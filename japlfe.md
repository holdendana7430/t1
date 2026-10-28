代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.haohaochexian.top/gttvabfstj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shangyingyoupin.top/gtuforlxzi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jqgufenzy.top/gtzwdazzzt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.cheryme.top/gtpnuazyig.html

[A26] 类型转换总览
来源：http://hz.cqqwz.cn/gtssxikhnp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shangyingyoupin.top/gteshnjdab.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.sufxvd.cn/gtonjgohhm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.haohaochexian.top/gtkqocgwou.html

TS:   Number() String() Boolean() x as number
来源：http://hz.mhx1999.top/gtbnptzghl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenzaomai.com/gtcbudwyze.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yueranfly.top/gtylclrgft.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.birdmap.top/gtesigadwz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.dashuyun.cn/gtkhteqwee.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtuihsmdbh.html

B. 流程控制
来源：http://hz.xuanzx.com/gtwcahohcg.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtlcjuhowy.html

[B01] 条件判断 if / else
来源：http://hz.316326.xyz/gtdwhomgts.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhengqikj.top/gtrouagwwp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.aizwys.cn/gtsbdvkiis.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtmfuaffmz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtvyrfqzgc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shuidangran.top/gtkrxjwzrd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cdnleiting.top/gtmsumvguq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.nanxinkj.top/gtvoaxogmo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.aizwys.cn/gthjuhjiqd.html

[B02] 多分支 else if / elif
来源：http://hz.xuanzx.com/gtnksplwvl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj202588.top/gtngapeohg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tanke756.top/gtxtarcriq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigfzy.top/gtwahdyial.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgufenzy.top/gtzkeuofsi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cdnleiting.top/gtjbegicrs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gotoacloud.top/gtbpzjcbiv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinqigufen.top/gtwqjkwqpw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.havefunace.top/gtxitrtdue.html

[B03] switch / match / case
来源：http://hz.pengpengdd.cyou/gtbxonsrqw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yongpay.top/gtmwdwyuqp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gogol.net.cn/gttedowria.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gogol.net.cn/gtfexyhxre.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yueranfly.top/gtchkexfli.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.havefunace.top/gtpvojtpym.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhengqikj.top/gteusgoisu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.redwolf501.top/gtwoueexir.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.kuanghao11.cn/gtjfdfurgq.html

[B04] for 计数循环
来源：http://hz.c1oappe.top/gtzsvtwgkz.html

Py:   for i in range(10): print(i)
来源：http://hz.shanyushiyangtech.top/gtbdmsuawv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cqqwz.cn/gtbrmxdsth.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.c1oappe.top/gtaduubeht.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.havefunace.top/gtnopmhitg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.feifeiyinyue.top/gtljlajhwm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.havefunace.top/gtcafflwzw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhiwuduotai.top/gtblvyaqtr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhixingplan.top/gtjhshacql.html

[B05] 遍历数组 / 列表
来源：http://hz.tanke756.top/gtuvxpebcf.html

Py:   for item in arr: print(item)
来源：http://hz.dashuyun.cn/gtgilonfps.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhiwuduotai.top/gtlogdxxyu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zdqjudy.top/gtcjanlaoq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtsifflqnx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.svipenyu.cn/gtuhavirij.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.chenzaomai.com/gtojwgqzdn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.nanxuanxn.top/gtwedzgsen.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xylfe.cn/gtspuhbvsd.html

[B06] 遍历字典 / 对象
来源：http://hz.iojbl.cn/gtvytyuhhs.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jiagoushi.top/gtpqgyjhry.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.bjfxy.top/gtjqnmokxj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cdnleiting.top/gtkumlwasw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuanzx.com/gthtgtimjm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.svipenyu.cn/gtfxhqzqsl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.pycfn.com/gtloeiwemx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jqgfzy.top/gtmfulpcnw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhaomingkeji.xyz/gtodquhfys.html

[B07] while 循环
来源：http://hz.nanxuanxn.top/gtguxjmagl.html

Py:   while i < 10: i += 1
来源：http://hz.jinqigfzy.top/gtswyfeyai.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.wangdashe.top/gtrctepevy.html

JS:   while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtrufqenlz.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtanoetgqr.html

Java: while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtwftwuhhc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ybcxt.top/gtahqhckmd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cashguo.top/gttusgwwvh.html

C#:   while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gtjhswzamb.html

[B08] do-while（至少执行一次）
来源：http://hz.zycfv.cn/gtrizocmif.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yueranfly.top/gtthmhdhlc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.pycfn.com/gteqaqmtip.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gtinxhbdid.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtncfiikqg.html

Java: do { i++; } while (i < 10);
来源：http://hz.pengpengdd.cyou/gthlypkzkc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ppjwa.cn/gtpsargudi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.kuanghao11.cn/gtqrvihejs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtgxolqjlb.html

[B09] break 与 continue
来源：http://hz.cqqwz.cn/gtcxamplqx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.chenzaomai.com/gtznggylpo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.haohaochexian.top/gtkbaecfxb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtzklqjjpg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtktcxrzzd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtohtibveu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xingfuxueyuan.xyz/gtivlpuwse.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.svipenyu.cn/gtdmbhctky.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtyqkxsmte.html

[B10] 遍历同时拿索引
来源：http://hz.shangyingyoupin.top/gtyxqzjxze.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.smart0.xyz/gtposdivod.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.dianchejie.cn/gtuxfnplhw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtaqtrbszq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtngipvfzc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jqgufenzy.top/gtipptjqhx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jyoumei.cn/gtxmsjhrdy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hongshengwenyu.top/gtonjqbmyk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xinyue.icu/gtyhbgmire.html

[B11] 生成数字序列 / 区间
来源：http://hz.cheryme.top/gtbuemkufw.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhongyouzk.top/gtdiopadfu.html

PHP:  range(0, 10, 2);
来源：http://hz.aibaodan.cn/gtdzphlmkl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xylfe.cn/gttiqhxcjn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yonumen.top/gtewtsldfg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.daria6918.cn/gtpbqayhrn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.316326.xyz/gtahhunxda.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cdnleiting.top/gteffwdezo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ybcxt.top/gtwsvwggtu.html

[B12] 跳出多层循环
来源：http://hz.yvedp.cn/gtuwvnabyu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sweek.top/gtlhmssdpu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.dashuyun.cn/gtnduhitcr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cqqwz.cn/gtwgaclpmf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtcrhldhkz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtvyqrfyhg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenlongwang.top/gtrxtbnsdq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.aibaodan.cn/gtfirzxyyr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sysykeji.top/gtubgzmbeo.html

[B13] 判断是否为数字
来源：http://hz.gogol.net.cn/gtbtqkydrb.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtsjvsndsc.html

PHP:  is_numeric($x)
来源：http://hz.jqgufenzy.top/gtgxhujdhb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.bjfxy.top/gtrcjwozjf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtdgjninvg.html

Java: x instanceof Number
来源：http://hz.aibaodan.cn/gtevwnilxm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xinyue.icu/gtczboscbw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.9152youxi.cn/gteboehpxi.html

C#:   x is int or double or decimal
来源：http://hz.ivvv.top/gtdhqhyhhb.html

[B14] 判断值是否在集合内
来源：http://hz.zhengqikj.top/gthmqurljt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xylfe.cn/gtqcqzebsq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhaomingkeji.xyz/gtqlqaxxwl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gtrbwhzxkr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtzurzrlmi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tanke756.top/gtvwlszfvf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ppjwa.cn/gtdycrvdvq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.svipenyu.cn/gtfmhliqmb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydjk.org.cn/gtyiwxmgpm.html

[B15] 布尔运算与取反
来源：http://hz.feifeiyinyue.top/gtvktelfjx.html

Py:   a and b or not c
来源：http://hz.chenlongwang.top/gtnvlolowa.html

PHP:  $a && $b || !$c
来源：http://hz.yj202588.top/gtwmkuisbg.html

JS:   a && b || !c
来源：http://hz.gaohongyu789.top/gtorexggec.html

TS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtnisxojpq.html

Java: a && b || !c
来源：http://hz.daria6918.cn/gthslsthlo.html

Go:   a && b || !c
来源：http://hz.guowangkeji.top/gtpzdtwdby.html

Ruby: a && b || !c
来源：http://hz.hnxiangtu.top/gtpegnaqef.html

C#:   a && b || !c
来源：http://hz.yuxming.cn/gtvqckrhtl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gzhubu.top/gtqxmrajvw.html

Py:   if not data: return
来源：http://hz.fzhhl.top/gtkswloxim.html

PHP:  if (!$data) { return; }
来源：http://hz.aizwys.cn/gtpqdutaah.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gtretqjekg.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gtgprfzysj.html

Java: if (data == null) return;
来源：http://hz.ywan-chungtsiang.top/gttaqgrrma.html

Go:   if data == nil { return }
来源：http://hz.xziqi.cn/gtbpsitqjt.html

Ruby: return if data.nil?
来源：http://hz.chenlongwang.top/gtaiybneog.html

C#:   if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtkyqerwgz.html

================================================================================
来源：http://hz.tian-w.cn/gtjzsojiba.html

C. 函数与作用域
来源：http://hz.shanyushiyangkeji.top/gtndpwvomn.html

================================================================================
来源：http://hz.ehwqpu.com/gtecoduwvm.html

[C01] 定义函数
来源：http://hz.redwolf501.top/gtterdczsd.html

Py:   def add(a, b): return a + b
来源：http://hz.hfpthk.cn/gthluvkdnh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gthyrmasmz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtapomnzsz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.snrcjt.cn/gtzgnwuxyc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtzoubtmkq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jyoumei.cn/gthrjguwyo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtrtgmvjsi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtkwicviwy.html

[C02] 默认参数
来源：http://hz.andypj.xyz/gtlzwvoynv.html

Py:   def greet(name="World"): return name
来源：http://hz.daxiang520.top/gtmblisulc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgufenzy.top/gtxvqgfsdz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.aizwys.cn/gtivwihcun.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuanzhike.top/gttfggwhri.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtygajojcg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhaomingkeji.xyz/gttvieifoe.html

Ruby: def greet(name = "World") = name
来源：http://hz.jlsjyb.cn/gtxwfzltph.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhoulong.xyz/gtchdsfwom.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtzullahdv.html

Py:   def total(*args): return sum(args)
来源：http://hz.cdnleiting.top/gtvehyqgbx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ydzc1.top/gtgyynbbtj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtbojwcvac.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gotoacloud.top/gtwleqqvkq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zdqjudy.top/gtxznqipzl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangkeji.top/gtkieakivh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jyoumei.cn/gtlkloqdwe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.birdmap.top/gtcnscogsv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gotoacloud.top/gttwiarduh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinghuilouyu.cn/gtskseojxg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.316326.xyz/gtcgjsikqd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.smart0.xyz/gtctbbfzou.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sxryk.cn/gtappiwkkm.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.meibo888.top/gtnmidmhyg.html

Go:   // 无：用配置结构体参数
来源：http://hz.shangyingyoupin.top/gtoudvnvmu.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtnbdwhdsu.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtnygkoejk.html

[C05] 返回多个值
来源：http://hz.gaohongyu789.top/gtdfipjqpz.html

Py:   return a, b
来源：http://hz.jiagoushi.top/gtedatmokm.html

PHP:  return [$a, $b];
来源：http://hz.daria6918.cn/gtpdjwchnm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhoulong.xyz/gtostlsdmh.html

TS:   return { a, b };
来源：http://hz.316326.xyz/gtssrarsfo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sysykeji.top/gtpjhetwbg.html

Go:   return a, b
来源：http://hz.xingfuxueyuan.xyz/gtegdpkqde.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtajapmpax.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jqgfzy.top/gtprycflri.html

[C06] 匿名函数 / lambda
来源：http://hz.xinyue.icu/gtoddcpiqs.html

Py:   square = lambda x: x * x
来源：http://hz.ivvv.top/gtlhjsretp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sweek.top/gtkdlesude.html

JS:   const square = x => x * x;
来源：http://hz.dianchejie.cn/gtkxrapqts.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinqigufen.top/gtyfkixtsi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.52xcode.cn/gtcmmpuoee.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuanzhike.top/gtuuzksqai.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tianlin.xyz/gtslqlczoi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gttmvlbewy.html

[C07] 把函数作为参数传入
来源：http://hz.ydjk.org.cn/gthprgbtdq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shzxlz.cn/gtrkpdlfmi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.pengpengdd.cyou/gtqjnfghqn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dianchejie.cn/gtzjgufugc.html

TS:   arr.map(String)
来源：http://hz.chenjidiqi.icu/gtvnfxljhe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinqigufen.top/gtfcltdqvl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yueranfly.top/gtijrumzfj.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenzaomai.com/gtnjrpmigp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.xylfe.cn/gtkexxawxs.html

[C08] 闭包
来源：http://hz.shzxlz.cn/gtoobnayan.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aizwys.cn/gtnulqdxbe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangkeji.top/gtrqmxxxuz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtsbhahqry.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtetnxudlm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhoulong.xyz/gtlovpgqkt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jyoumei.cn/gteyqdhzpm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yonumen.top/gtqbddfglb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gttooyphtg.html

[C09] 递归
来源：http://hz.dashuyun.cn/gtazedgaud.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daxiang520.top/gtregcaggn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jlsjyb.cn/gtegohfdys.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gtzugbhwni.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zycfv.cn/gtqhjfhvke.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tian-w.cn/gtogcelwaj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.gzhubu.top/gtagdhjebf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ehwqpu.com/gtrxnngref.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.quarkkingdee.top/gtdwvrhhkz.html

[C10] 变量作用域
来源：http://hz.xingfuxueyuan.xyz/gtsxhjvkej.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ivvv.top/gtxpprznsy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhaomingkeji.xyz/gtydsnylaf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.snrcjt.cn/gtwgveuefg.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtzemlmuqk.html

Java: 方法内为块级作用域
来源：http://hz.feifeiyinyue.top/gtqbwevomd.html

Go:   花括号块级作用域
来源：http://hz.zhaomingkeji.xyz/gtxlpuydjo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhijiandao.cn/gteghwnuya.html

C#:   块级作用域
来源：http://hz.xinyue.icu/gtfdgfgapr.html

[C11] 模块导入与导出
来源：http://hz.havefunace.top/gtecsmzkie.html

Py:   from module import func
来源：http://hz.fzhhl.top/gtiocsawsl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gaohongyu789.top/gttitfiawc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shuidangran.top/gtdghzahmh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.svipenyu.cn/gtlmtrjoes.html

Java: import java.util.List;
来源：http://hz.ehwqpu.com/gtpjzwtpdv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.iojbl.cn/gtaicnbkjb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gtqbrhyhdt.html

C#:   using System.Text;
来源：http://hz.nanxuanxn.top/gthenyfixk.html

[C12] 立即执行函数 IIFE
来源：http://hz.daxiang520.top/gtfkdcwucs.html

Py:   (lambda: print("run"))()
来源：http://hz.shangyingyoupin.top/gtopocrnlb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aizwys.cn/gtrhcdsudf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhoulong.xyz/gtlxrxwvfm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tian-w.cn/gtjtnnxiir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hongshengwenyu.top/gtgkyyszkw.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.iojbl.cn/gtsihdejzx.html

Ruby: -> { puts "run" }.call
来源：http://hz.tanke756.top/gtyhiweamm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hammf.cn/gthkcmujok.html

[C13] 类型声明 / 类型注解
来源：http://hz.yonumen.top/gtvraahzxn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.daxiang520.top/gtyrwlrzbh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtlevivalm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258.top/gtnxneurpm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhiwuduotai.top/gtpgdmyluh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtjqmybhms.html

Go:   func add(a, b int) int
来源：http://hz.iojbl.cn/gtyfbzoqku.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj202588.top/gtjmmvzudy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.smart0.xyz/gttwewpktp.html

[C14] 泛型函数
来源：http://hz.yvedp.cn/gtrsxnpteb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shangyingyoupin.top/gtsblmdhoi.html

PHP:  // 无泛型
来源：http://hz.jiagoushi.top/gtnlhwxepl.html

JS:   // 无泛型
来源：http://hz.jianghu66.top/gtvpwebjzf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj20258888.top/gtkhrjfsmm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangdashe.top/gtsdottuln.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shanyushiyangkeji.top/gtwzsfdaks.html

Ruby: # 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtlgslkaam.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.nwbrower.top/gtnqfbisbz.html

[C15] 解构 / 展开参数
来源：http://hz.cucudq.cn/gtlbxesoqw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.sysykeji.top/gtltltlufb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenjidiqi.icu/gtngwndnvz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.pengpengdd.cyou/gtsmhaerxi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jianghu66.top/gtokaxqhzv.html

Java: // 无解构
来源：http://hz.smart0.xyz/gtqtjjavyz.html

Go:   // 无解构
来源：http://hz.dashuyun.cn/gtytnnytjm.html

Ruby: a, b = pair
来源：http://hz.jyoumei.cn/gtbnzarvxu.html

C#:   var (a, b) = pair;
来源：http://hz.0kj1m.cn/gtkaqgwric.html

[C16] 函数 / 方法重载
来源：http://hz.sufxvd.cn/gttjqrnhkn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sufxvd.cn/gttsavjofz.html


<!-- 参考信息 -->