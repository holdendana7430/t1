代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.pycfn.com/gtortxvyto.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.tianlin.xyz/gtqcowdrhl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.gogol.net.cn/gtbvqksgoy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ehwqpu.com/gtruhzuwsv.html

[A26] 类型转换总览
来源：http://hz.ywan-chungtsiang.top/gtrtusxusn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yvedp.cn/gtfdkswuat.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhixingplan.top/gtanctjxtt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.dianchejie.cn/gtejkafmwf.html

TS:   Number() String() Boolean() x as number
来源：http://hz.redwolf501.top/gtggdatvyt.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhengqikj.top/gtezdfkiya.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.guowangkeji.top/gtmqwvhnbn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhiwuduotai.top/gtkdkqkqzb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.cdnleiting.top/gteohcjdtv.html

================================================================================
来源：http://hz.sweek.top/gtguzkeydk.html

B. 流程控制
来源：http://hz.jinyuanbaomall.cn/gtrgniqxcq.html

================================================================================
来源：http://hz.ybcxt.top/gtdiajbdoo.html

[B01] 条件判断 if / else
来源：http://hz.cheryme.top/gtozqoszsh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.xuetiantiany.cn/gthhqiczgb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jqgfzy.top/gtbqvgyhik.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.iojbl.cn/gtmvshuvil.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yangfankeji.com/gthblrxuya.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.daria6918.cn/gtzwxmovms.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jinqigufen.top/gtfllvphsk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.vqdsnc.cn/gtslsxgcrt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gtsoiygtlx.html

[B02] 多分支 else if / elif
来源：http://hz.0kj1m.cn/gtvhovqcnt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.ydzc1.top/gtkrfhrwsm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.fengsongda.top/gtyiulmstk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtuktvspwn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtwjcbfgkk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gteuqfzbzw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhaomingkeji.xyz/gtgcbsrlvi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.tanke756.top/gtowveagfh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gttbqfradz.html

[B03] switch / match / case
来源：http://hz.shanyushiyangkeji.top/gthcgoflww.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sweek.top/gtmrmxmhnu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daria6918.cn/gtkpaciuxt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sweek.top/gtuerqqkpx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yanxiufei.cn/gtrcwnkxzs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.vqdsnc.cn/gtjgxysesb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.tianlin.xyz/gtcqpvhddp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ivvv.top/gtxprgutwv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.nanxinkj.top/gtoefslpih.html

[B04] for 计数循环
来源：http://hz.sufxvd.cn/gtaylfmdsw.html

Py:   for i in range(10): print(i)
来源：http://hz.yvedp.cn/gtoycyllxv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cashguo.top/gtyyzozmpn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.iojbl.cn/gtoimzegol.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tian-w.cn/gtwlxisqua.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xinyue.icu/gtqlfqfcac.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.mhx1999.top/gteqridrpt.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cashguo.top/gtbechwkug.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.aibaodan.cn/gtjnnwsmal.html

[B05] 遍历数组 / 列表
来源：http://hz.meibo888.top/gtfhacvebe.html

Py:   for item in arr: print(item)
来源：http://hz.tianlin.xyz/gtkxcovgjw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.c1oappe.top/gtyneczuxq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhixingplan.top/gtmipbxyln.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.smart0.xyz/gtkzchwgyl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xinyue.icu/gtyavdjcfv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhongyouzk.top/gtualwtnqt.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj20258888.top/gtejivubxd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gotoacloud.top/gtndicfudh.html

[B06] 遍历字典 / 对象
来源：http://hz.xziqi.cn/gtmymvapmz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cdnleiting.top/gtjsnesebe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hammf.cn/gtqrrlzjab.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gtwfmpqnjv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shzxlz.cn/gtzhkoejup.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yanxiufei.cn/gtoiatdvbl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shanyushiyangtech.top/gtqinhbhlw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shanyushiyangtech.top/gtziyrytjv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.dashuyun.cn/gtdyhfyaxc.html

[B07] while 循环
来源：http://hz.cqqwz.cn/gtckywmcgl.html

Py:   while i < 10: i += 1
来源：http://hz.kuanghao11.cn/gtfvvvvwtj.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xinyue.icu/gtaqjsqxjm.html

JS:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtfwwswncg.html

TS:   while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gtpyzxfqpp.html

Java: while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtbspbidwf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yanxiufei.cn/gtclghfltc.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinqigufen.top/gtesgckenp.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtxpzwraem.html

[B08] do-while（至少执行一次）
来源：http://hz.xinyue.icu/gtfpjqayci.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hongshengwenyu.top/gtmhhzsukg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hfpthk.cn/gtuyjvtnxe.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtqenxrdxa.html

TS:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gthqigsxpw.html

Java: do { i++; } while (i < 10);
来源：http://hz.jinqigfzy.top/gtkguuqcmi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cdnleiting.top/gtbkxahqco.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.redwolf501.top/gtmlwojdzm.html

C#:   do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtaprubbay.html

[B09] break 与 continue
来源：http://hz.jqgufenzy.top/gtkxresjjr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.snrcjt.cn/gtjxpemaev.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xziqi.cn/gtiwvxymmd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gteiqhfzws.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtyxqkoxvl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtajzghjlf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhongyouzk.top/gtrtksfule.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ydjk.org.cn/gtshopximh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gthxjyprzo.html

[B10] 遍历同时拿索引
来源：http://hz.xuanzx.com/gtwnpaldxi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhongyouzk.top/gtkdblyijy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.dianchejie.cn/gtfybsiiei.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gtjcqtmbce.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ivvv.top/gtebpsedkp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hnxiangtu.top/gtqfjsjxjs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yueranfly.top/gtuogxapvd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinghuilouyu.cn/gtplrtrazp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhongyouzk.top/gtvfqptawd.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgufenzy.top/gtljdiuifa.html

Py:   list(range(0, 10, 2))
来源：http://hz.birdmap.top/gtlzowptqa.html

PHP:  range(0, 10, 2);
来源：http://hz.aibaodan.cn/gtokjzyvqs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.haohaochexian.top/gtfwnjljpq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj20258888.top/gtgmjddjoe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhixingplan.top/gtmwtcafao.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gtfgosllyw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xziqi.cn/gtvfwawvon.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigfzy.top/gtfwkdzuwo.html

[B12] 跳出多层循环
来源：http://hz.aibaodan.cn/gtosukcodx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhongyouzk.top/gtgdrtxuwj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hnqzz.top/gtsgooiizq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtayulspoe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtrinotybe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.havefunace.top/gtenopskdw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yanxiufei.cn/gtbpbcxlzw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cashguo.top/gtrmanlqyt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.guannengcc.top/gtgmpradek.html

[B13] 判断是否为数字
来源：http://hz.aibaodan.cn/gtdowsqyxj.html

Py:   isinstance(x, (int, float))
来源：http://hz.quarkkingdee.top/gtnuiwvfnn.html

PHP:  is_numeric($x)
来源：http://hz.zycfv.cn/gtzlckwtyh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daxiang520.top/gthzfkxsnw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenzaomai.com/gtdvtvblld.html

Java: x instanceof Number
来源：http://hz.pengpengdd.cyou/gthccbymjr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.daria6918.cn/gtyreaxoew.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xingfuxueyuan.xyz/gtsxqwecvf.html

C#:   x is int or double or decimal
来源：http://hz.guannengcc.top/gtadvsxako.html

[B14] 判断值是否在集合内
来源：http://hz.cheryme.top/gtjoiptiwj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenlongwang.top/gtfnwxtndh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hywenlv.cn/gtcjulricc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhixingplan.top/gtbrpohrdz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtdxozusue.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.kuanghao11.cn/gtkedcacrt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xziqi.cn/gtyecniyim.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shanyushiyangkeji.top/gtqxdnnlke.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shangyingyoupin.top/gtnluqvguy.html

[B15] 布尔运算与取反
来源：http://hz.xuanzx.com/gtbgjefnlh.html

Py:   a and b or not c
来源：http://hz.feifeiyinyue.top/gtcmkiyxbw.html

PHP:  $a && $b || !$c
来源：http://hz.nwbrower.top/gtihgxoofu.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtosmiyteo.html

TS:   a && b || !c
来源：http://hz.jianghu66.top/gtjeuvkgbe.html

Java: a && b || !c
来源：http://hz.meibo888.top/gtjlfrkjqu.html

Go:   a && b || !c
来源：http://hz.wangdashe.top/gtqfgkhjxg.html

Ruby: a && b || !c
来源：http://hz.52xcode.cn/gtgjfnpojj.html

C#:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtdfskbnpy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shzxlz.cn/gtexphxzof.html

Py:   if not data: return
来源：http://hz.redwolf501.top/gtzznsyoew.html

PHP:  if (!$data) { return; }
来源：http://hz.chenlongwang.top/gtnwtedgqu.html

JS:   if (!data) return;
来源：http://hz.wangdashe.top/gtrefsghqu.html

TS:   if (!data) return;
来源：http://hz.andypj.xyz/gtifahopfx.html

Java: if (data == null) return;
来源：http://hz.shuidangran.top/gturuiaknm.html

Go:   if data == nil { return }
来源：http://hz.chenzaomai.com/gtvpwyorpf.html

Ruby: return if data.nil?
来源：http://hz.yongpay.top/gtemjemboy.html

C#:   if (data == null) return;
来源：http://hz.sxryk.cn/gtvupylzck.html

================================================================================
来源：http://hz.xuanzx.com/gtxdiriktt.html

C. 函数与作用域
来源：http://hz.mhx1999.top/gthzqktmzf.html

================================================================================
来源：http://hz.ydjk.org.cn/gtgbvyrgmy.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtosyzpxek.html

Py:   def add(a, b): return a + b
来源：http://hz.zhaomingkeji.xyz/gtqnkexgrz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtqfhhpcjl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhengqikj.top/gtqmduhztn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cashguo.top/gtbxcotxnr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ybcxt.top/gtoqepfoyi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtszayrmec.html

Ruby: def add(a, b); a + b; end
来源：http://hz.svipenyu.cn/gthtegvfwv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtbcrccoym.html

[C02] 默认参数
来源：http://hz.shuidangran.top/gtjhxzhmat.html

Py:   def greet(name="World"): return name
来源：http://hz.ppjwa.cn/gtqagnwoyw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.daxiang520.top/gtujrxddxc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tianlin.xyz/gthbghlebp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.9152youxi.cn/gtrorxgrev.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xziqi.cn/gttpnpahsm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhijiandao.cn/gttkdbykmk.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtkdctglvz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dashuyun.cn/gtmhoaxbqd.html

[C03] 可变参数
来源：http://hz.shanyushiyangtech.top/gthvavofcg.html

Py:   def total(*args): return sum(args)
来源：http://hz.gotoacloud.top/gtfivagqdi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinqigfzy.top/gtrotjpfcd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtulotzopo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtfdjsubqj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gaohongyu789.top/gtwfxrksfo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.quarkkingdee.top/gtxtzatngt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ybcxt.top/gtiqrclspe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.daria6918.cn/gtwjbkrqdu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.chenjidiqi.icu/gtobkigwrv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuanzhike.top/gtngozxhkj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gotoacloud.top/gtdfmguqiy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtvoyznbzz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gogol.net.cn/gtkgxszgfr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gaohongyu789.top/gtzaskehcr.html

Go:   // 无：用配置结构体参数
来源：http://hz.daria6918.cn/gtdzncwxcv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtugwhxqeg.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtvtnrvzel.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gtnxbwlant.html

Py:   return a, b
来源：http://hz.jinghuilouyu.cn/gtkvddcvpa.html

PHP:  return [$a, $b];
来源：http://hz.guowangkeji.top/gtvosumlyp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guannengcc.top/gtpxzdapem.html

TS:   return { a, b };
来源：http://hz.bjfxy.top/gtecwezweb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guowangkeji.top/gtojmlhify.html

Go:   return a, b
来源：http://hz.aibaodan.cn/gtpjoacemm.html

Ruby: return a, b
来源：http://hz.c1oappe.top/gtggtswgeo.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.chenjidiqi.icu/gtwvdxmxdn.html

[C06] 匿名函数 / lambda
来源：http://hz.c1oappe.top/gtkceurbxo.html

Py:   square = lambda x: x * x
来源：http://hz.jqgfzy.top/gtctdnrbkh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hnqzz.top/gthptlteco.html

JS:   const square = x => x * x;
来源：http://hz.xziqi.cn/gtvuylpnot.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuanzx.com/gttolypquv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhengqikj.top/gttwqhkjii.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.daxiang520.top/gtlnbnjhtn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhaomingkeji.xyz/gtpzjyaikj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xuetiantiany.cn/gthblaaqfp.html

[C07] 把函数作为参数传入
来源：http://hz.xuanzx.com/gtpfgdbnyl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhongyouzk.top/gtsytucdfe.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jlsjyb.cn/gtbwpwqcsc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yangfankeji.com/gtttiyoznj.html

TS:   arr.map(String)
来源：http://hz.aizwys.cn/gtvdogtqhh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.snrcjt.cn/gtdxaulgkc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgufenzy.top/gtoahypely.html

Ruby: arr.map(&:upcase)
来源：http://hz.tianlin.xyz/gtpkurzfjl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hfpthk.cn/gttikymciw.html

[C08] 闭包
来源：http://hz.pengpengdd.cyou/gtaadkmjmv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zdqjudy.top/gtikqchcms.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yuanzhike.top/gtyxwbwsyd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtkxzxcrml.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtyrqsqytb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuanzx.com/gtesjhwpnr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.svipenyu.cn/gttvmtmysb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xingfuxueyuan.xyz/gtufrtyfce.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtlpukyjki.html

[C09] 递归
来源：http://hz.jinqigfzy.top/gtdjgvnzvk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daxiang520.top/gtcgcmicgw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tianlin.xyz/gtfeqcegtg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aibaodan.cn/gtuzhsqkea.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jqgfzy.top/gtswctpkqb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtomtqbyiu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jiagoushi.top/gtdvkjdfxx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.mhx1999.top/gtnesftjpp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hongshengwenyu.top/gtphapskyc.html

[C10] 变量作用域
来源：http://hz.316326.xyz/gtrpnpxuyg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258888.top/gtimtvryaf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.chenzaomai.com/gtxwgsdwzs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yanxiufei.cn/gtisqqlduh.html

TS:   同 JS
来源：http://hz.c1oappe.top/gtqkjzhzlz.html

Java: 方法内为块级作用域
来源：http://hz.jqgufenzy.top/gtnkdftpcw.html

Go:   花括号块级作用域
来源：http://hz.daria6918.cn/gtythtkior.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jianghu66.top/gtmphomdtd.html

C#:   块级作用域
来源：http://hz.svipenyu.cn/gthjwjjrng.html

[C11] 模块导入与导出
来源：http://hz.yuanzhike.top/gttmpcovfa.html

Py:   from module import func
来源：http://hz.nanxinkj.top/gtbygrrptz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.quarkkingdee.top/gtxwihxket.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydjk.org.cn/gtbszjdxsk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.wangdashe.top/gtbjtnwjcg.html

Java: import java.util.List;
来源：http://hz.gogol.net.cn/gtfswddgfc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.birdmap.top/gtfkvtyfpi.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xziqi.cn/gtuamabqxo.html

C#:   using System.Text;
来源：http://hz.ybcxt.top/gtduqqduwy.html

[C12] 立即执行函数 IIFE
来源：http://hz.daxiang520.top/gtunxrvijm.html

Py:   (lambda: print("run"))()
来源：http://hz.mhx1999.top/gtdkcupwkz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yvedp.cn/gtocuciepf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sufxvd.cn/gtgcwctvut.html

TS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtqwbdgypc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zycfv.cn/gtojygcqyr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj20258888.top/gtkgwckvtg.html

Ruby: -> { puts "run" }.call
来源：http://hz.yueranfly.top/gtpvgbxria.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nwbrower.top/gtxzfwgerx.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhengqikj.top/gtofwioobg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.andypj.xyz/gtfmnelosi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtjbkazdbz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xingfuxueyuan.xyz/gtofqtacdq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtdsqqzktb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtqjwhxjio.html

Go:   func add(a, b int) int
来源：http://hz.jinqigfzy.top/gtampuojmg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guannengcc.top/gtarrdwiod.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cucudq.cn/gtjkpibhhe.html

[C14] 泛型函数
来源：http://hz.9152youxi.cn/gtnvujrzyl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.snrcjt.cn/gtjogkhnra.html

PHP:  // 无泛型
来源：http://hz.wangshuangyany.cn/gtizusumnp.html

JS:   // 无泛型
来源：http://hz.chenzaomai.com/gtphtnqhvn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daria6918.cn/gtadajocfh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhaomingkeji.xyz/gtjlthayma.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangdashe.top/gtbbyrcqdy.html

Ruby: # 无泛型
来源：http://hz.cdnleiting.top/gtbrpeuvnw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gaohongyu789.top/gtzyfdycvr.html

[C15] 解构 / 展开参数
来源：http://hz.daria6918.cn/gtahpromsy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.guannengcc.top/gtgsxplusi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtksomwowz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtkpgayuat.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.0kj1m.cn/gtocbopbxz.html

Java: // 无解构
来源：http://hz.hywenlv.cn/gtpwvyiazz.html

Go:   // 无解构
来源：http://hz.zycfv.cn/gtbknbotlr.html

Ruby: a, b = pair
来源：http://hz.jinqigufen.top/gtkpqdgysg.html

C#:   var (a, b) = pair;
来源：http://hz.jiagoushi.top/gtnaxhpfkw.html

[C16] 函数 / 方法重载
来源：http://hz.vqdsnc.cn/gtxglnwzzv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhijiandao.cn/gtuyzhfizi.html


<!-- 参考信息 -->