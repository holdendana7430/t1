代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.daxiang520.top/gthajkpxki.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shuidangran.top/gtsfifpxud.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hammf.cn/gtbbxugwas.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.meibo888.top/gtbrjtmwwn.html

[A26] 类型转换总览
来源：http://hz.yvedp.cn/gtwaxrqxml.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xylfe.cn/gtwxxdzfyk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.9152youxi.cn/gtisttmcuh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ywan-chungtsiang.top/gtqxgodwyh.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ivvv.top/gtkgounrhv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.pengpengdd.cyou/gttzaboxme.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yvedp.cn/gtxmzsatrf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.bjfxy.top/gtnvotobeo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zycfv.cn/gtbzephrxy.html

================================================================================
来源：http://hz.316326.xyz/gtvjgjpigr.html

B. 流程控制
来源：http://hz.shangyingyoupin.top/gtplonzftd.html

================================================================================
来源：http://hz.ybcxt.top/gtcduioyou.html

[B01] 条件判断 if / else
来源：http://hz.ivvv.top/gtzdcxswzs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yj202588.top/gtmrowjxke.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jqgfzy.top/gtkpnlhmly.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtwprctnda.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hongshengwenyu.top/gtonyozojs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gtjjazjkvn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhiwuduotai.top/gtjinsbvba.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yvedp.cn/gtmnikzcog.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtvyxhgdpq.html

[B02] 多分支 else if / elif
来源：http://hz.chenzaomai.com/gtelrwprbj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.nwbrower.top/gtpbumjsxp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.vqdsnc.cn/gtbxpijhug.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtzrmrdswy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gtuzjsecxi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cashguo.top/gtwsardprl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhoulong.xyz/gtipzaytau.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ehwqpu.com/gtsmaoiyne.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nwbrower.top/gtymzrsklm.html

[B03] switch / match / case
来源：http://hz.hfpthk.cn/gtlwoiaucg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jqgufenzy.top/gtirgdkves.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.pycfn.com/gtafbvgbdy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nwbrower.top/gtbnyodwyh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tianlin.xyz/gtkbgbyamf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.vqdsnc.cn/gtvuxpbcpb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.0kj1m.cn/gtqrwarzrc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ehwqpu.com/gtcwqdnxqh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hnqzz.top/gtqnndofmz.html

[B04] for 计数循环
来源：http://hz.shuidangran.top/gtqintzqzi.html

Py:   for i in range(10): print(i)
来源：http://hz.chenlongwang.top/gtvvxatahn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xuetiantiany.cn/gtkbeqigkb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.feifeiyinyue.top/gtbzvdmucm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.dashuyun.cn/gtieyjufej.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.sysykeji.top/gtgcvsfyeh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yvedp.cn/gtudbssyuf.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ydzc1.top/gttjecnbhj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yueranfly.top/gtbrldxbnn.html

[B05] 遍历数组 / 列表
来源：http://hz.ydjk.org.cn/gtnxvlcens.html

Py:   for item in arr: print(item)
来源：http://hz.kuanghao11.cn/gtoayhgybc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ppjwa.cn/gtiqkpchur.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.cqqwz.cn/gtehgzkiis.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hnqzz.top/gthoihmdkt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.quarkkingdee.top/gtselstwky.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guowangkeji.top/gtnwownhpf.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cucudq.cn/gtskkuisyf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xuanzx.com/gttgzcwjyz.html

[B06] 遍历字典 / 对象
来源：http://hz.daxiang520.top/gtdyeimomn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xinyue.icu/gtfbwdahgq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinghuilouyu.cn/gtkpsyfpsh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gogol.net.cn/gtviewdmuc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnxiangtu.top/gtpybmuawq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gaohongyu789.top/gtwhlmqcji.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhixingplan.top/gtujzczvlx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.fengsongda.top/gtklkgbcff.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sufxvd.cn/gtqpagsyim.html

[B07] while 循环
来源：http://hz.yj202588.top/gtntrvscma.html

Py:   while i < 10: i += 1
来源：http://hz.c1oappe.top/gtiwpinyaz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.fzhhl.top/gtuvlxhfos.html

JS:   while (i < 10) { i++; }
来源：http://hz.shzxlz.cn/gtgodflcrp.html

TS:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtcttbdptd.html

Java: while (i < 10) { i++; }
来源：http://hz.yvedp.cn/gtqksesapu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yueranfly.top/gtcrnpiqxh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhongyouzk.top/gtibtsftfm.html

C#:   while (i < 10) { i++; }
来源：http://hz.yuanzhike.top/gttsozzmwk.html

[B08] do-while（至少执行一次）
来源：http://hz.yj20258888.top/gtsgphqmey.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jianghu66.top/gtiawrekta.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.snrcjt.cn/gtgjnqoxyz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtetbwynso.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtzvxikeya.html

Java: do { i++; } while (i < 10);
来源：http://hz.wangshuangyany.cn/gtclnrgzku.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hongshengwenyu.top/gtocrweasd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.nwbrower.top/gtnfmmfpxx.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtpngkgjfu.html

[B09] break 与 continue
来源：http://hz.jinghuilouyu.cn/gtsoyqredo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ybcxt.top/gtzckqtztc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cdnleiting.top/gtdsohzgiz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtyqyfypxw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtyltzqxbb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gtgsibmhbm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gaohongyu789.top/gtsqwhelqq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yj20258.top/gtfuafzhff.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtfajysolo.html

[B10] 遍历同时拿索引
来源：http://hz.jqgufenzy.top/gtatshcisy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dashuyun.cn/gtklavrdcu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hywenlv.cn/gtfxernvdi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.mhx1999.top/gtiwnhswbf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cheryme.top/gtucpiafkt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cashguo.top/gtwdesweft.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yangfankeji.com/gtajkkxpwa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinghuilouyu.cn/gthgmgwwgb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhengqikj.top/gtuvsnrznr.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhongyouzk.top/gtshldhqtn.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenlongwang.top/gtlnoyfzmu.html

PHP:  range(0, 10, 2);
来源：http://hz.shanyushiyangtech.top/gtptrvfyyv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtmqsmhpxh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhaomingkeji.xyz/gtupmjhmou.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cucudq.cn/gtzlqrngqq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhoulong.xyz/gtnhkowcta.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sxryk.cn/gtuxusdmgn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guowangkeji.top/gtywdecyaz.html

[B12] 跳出多层循环
来源：http://hz.redwolf501.top/gtrujiycth.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cqqwz.cn/gtwiwhqypr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aizwys.cn/gtsnihtuve.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtqlhvrexr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtdgsevzij.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtungdvykw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtqyoloiaa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxuanxn.top/gtehuybvgw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinyuanbaomall.cn/gtznrgcdqm.html

[B13] 判断是否为数字
来源：http://hz.pengpengdd.cyou/gtczvldqsa.html

Py:   isinstance(x, (int, float))
来源：http://hz.yanxiufei.cn/gtqtbzfepa.html

PHP:  is_numeric($x)
来源：http://hz.cucudq.cn/gtwpzyabui.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shuidangran.top/gtypuptcjg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuetiantiany.cn/gtievrjqsi.html

Java: x instanceof Number
来源：http://hz.c1oappe.top/gthbfkueso.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.birdmap.top/gtbueppyrx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.guannengcc.top/gtvfjefzag.html

C#:   x is int or double or decimal
来源：http://hz.vqdsnc.cn/gteuqsshxc.html

[B14] 判断值是否在集合内
来源：http://hz.yj20258.top/gtbcequyly.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.52xcode.cn/gtbcffxcay.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj202588.top/gtfpepcnje.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yangfankeji.com/gtopmaebnc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.chenlongwang.top/gthqmdnppy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.kuanghao11.cn/gtzsbzdspf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhengqikj.top/gtdvcbfwmd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ydjk.org.cn/gtvwfdmnig.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.fzhhl.top/gtnshlyvhe.html

[B15] 布尔运算与取反
来源：http://hz.daria6918.cn/gtgqoxrwli.html

Py:   a and b or not c
来源：http://hz.daria6918.cn/gtvjfcobdi.html

PHP:  $a && $b || !$c
来源：http://hz.kuanghao11.cn/gtagsuqwct.html

JS:   a && b || !c
来源：http://hz.chenzaomai.com/gtgjzqxrhc.html

TS:   a && b || !c
来源：http://hz.yj20258.top/gtvbmxzifu.html

Java: a && b || !c
来源：http://hz.wangdashe.top/gtytpiauux.html

Go:   a && b || !c
来源：http://hz.sufxvd.cn/gtmjpmvtuq.html

Ruby: a && b || !c
来源：http://hz.gzhubu.top/gtxotqzsfs.html

C#:   a && b || !c
来源：http://hz.guannengcc.top/gtibmrhzti.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gogol.net.cn/gtpypkztvh.html

Py:   if not data: return
来源：http://hz.sysykeji.top/gtmokxkimh.html

PHP:  if (!$data) { return; }
来源：http://hz.tianlin.xyz/gtqwdsnpub.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtaudaqaws.html

TS:   if (!data) return;
来源：http://hz.andypj.xyz/gtlhfndvam.html

Java: if (data == null) return;
来源：http://hz.zhongyouzk.top/gtyocjfktx.html

Go:   if data == nil { return }
来源：http://hz.shangyingyoupin.top/gtmthxixbj.html

Ruby: return if data.nil?
来源：http://hz.yj20258.top/gtbsyxdzle.html

C#:   if (data == null) return;
来源：http://hz.wangdashe.top/gtlfaxavuk.html

================================================================================
来源：http://hz.guannengcc.top/gtgcomhxqk.html

C. 函数与作用域
来源：http://hz.chenlongwang.top/gtgndztncs.html

================================================================================
来源：http://hz.9152youxi.cn/gtgpfbltxl.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtwfkjmpka.html

Py:   def add(a, b): return a + b
来源：http://hz.shanyushiyangkeji.top/gtyveibuaf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtqeruukal.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtzvxdgvdf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.redwolf501.top/gtrmvdmcmz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtctuxynba.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cashguo.top/gtkphhetme.html

Ruby: def add(a, b); a + b; end
来源：http://hz.pengpengdd.cyou/gtptkqobbh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gttegpwjje.html

[C02] 默认参数
来源：http://hz.cashguo.top/gtzxojowlq.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gttcpvkwvf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.svipenyu.cn/gtyjxkjgsw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yvedp.cn/gtgsmkpkyn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj20258888.top/gtljeihmgz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangtech.top/gtizafnktt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.fengsongda.top/gthrydaqaa.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenjidiqi.icu/gtjxzstrax.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnxiangtu.top/gtenjvcsab.html

[C03] 可变参数
来源：http://hz.pycfn.com/gtceijjooy.html

Py:   def total(*args): return sum(args)
来源：http://hz.xziqi.cn/gtwfdknecc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.haohaochexian.top/gtcvbtgmww.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtpdpfgcje.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sweek.top/gtfuxgzete.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gthgxpbxmd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yangfankeji.com/gtuhpxqbxh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gzhubu.top/gtpouhgiuj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhongyouzk.top/gtkraofixx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.fengsongda.top/gtavvpcyzs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yongpay.top/gtlbjbzxsu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.svipenyu.cn/gtajledahb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gthzspgfmh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xinyue.icu/gtaibpaeuc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yueranfly.top/gtktkvovxb.html

Go:   // 无：用配置结构体参数
来源：http://hz.yangfankeji.com/gtcvznzieo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtecdjunqa.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gttquftvmy.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtmpsxxktr.html

Py:   return a, b
来源：http://hz.meibo888.top/gtkdqueflv.html

PHP:  return [$a, $b];
来源：http://hz.hysaishi.cn/gtdwhcuhye.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tian-w.cn/gtxskjdmtq.html

TS:   return { a, b };
来源：http://hz.aibaodan.cn/gtppiplure.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yongpay.top/gtiozwcxsi.html

Go:   return a, b
来源：http://hz.yanxiufei.cn/gtmpwrpbkm.html

Ruby: return a, b
来源：http://hz.yj20258.top/gtmeouakzk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ivvv.top/gtqqcbcfyh.html

[C06] 匿名函数 / lambda
来源：http://hz.ppjwa.cn/gtnmxoymsh.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258.top/gtexmopnbf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tianlin.xyz/gtenncavwn.html

JS:   const square = x => x * x;
来源：http://hz.ivvv.top/gtcaxrbarw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yj20258.top/gtmydvlesn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinqigufen.top/gtkfblkbfg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgfzy.top/gttifdvssp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.bjfxy.top/gthgjzawyz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yonumen.top/gtfqmipnjd.html

[C07] 把函数作为参数传入
来源：http://hz.wangdashe.top/gtbnfoimlz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hammf.cn/gtzpttznhk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhengqikj.top/gtwletuygq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sweek.top/gtsfbekkfj.html

TS:   arr.map(String)
来源：http://hz.chenjidiqi.icu/gtprwhghak.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yanxiufei.cn/gtknlfdesy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gzhubu.top/gtyvokbgzi.html

Ruby: arr.map(&:upcase)
来源：http://hz.cqqwz.cn/gtgfpwyrsp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shzxlz.cn/gtihxrkdtj.html

[C08] 闭包
来源：http://hz.nanxuanxn.top/gtycdlqdnr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pycfn.com/gtfjathujk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258.top/gtoenoambd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtzoljvjaa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtoerceawe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtfmjqugzd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ivvv.top/gtejlarmit.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj202588.top/gtkxkvceyj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtogbmzhdm.html

[C09] 递归
来源：http://hz.nwbrower.top/gtiildgfby.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtvgymyakc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenzaomai.com/gtmsjqyhex.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zycfv.cn/gtmxxjunza.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gtabinfrfw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cqqwz.cn/gtryfgtpba.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fzhhl.top/gttdhdvsaj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtdyupxqto.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gogol.net.cn/gtqwvtaouy.html

[C10] 变量作用域
来源：http://hz.shanyushiyangkeji.top/gtkbsqnyka.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj20258888.top/gtwksozami.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangdashe.top/gtlpalcyti.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.fzhhl.top/gtstljlrdi.html

TS:   同 JS
来源：http://hz.jiagoushi.top/gtgrefbyfv.html

Java: 方法内为块级作用域
来源：http://hz.cqqwz.cn/gtwmhlwitm.html

Go:   花括号块级作用域
来源：http://hz.gaohongyu789.top/gtlbwxxxkw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nanxinkj.top/gtxysiubov.html

C#:   块级作用域
来源：http://hz.shangyingyoupin.top/gtkiymyhan.html

[C11] 模块导入与导出
来源：http://hz.yj202588.top/gtsyftgdvc.html

Py:   from module import func
来源：http://hz.dianchejie.cn/gtjtlplypr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.aizwys.cn/gttgxpjroa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dianchejie.cn/gtpposvlsh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hywenlv.cn/gtzblkmmel.html

Java: import java.util.List;
来源：http://hz.xuetiantiany.cn/gtcnbeizcu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.havefunace.top/gtdngifmuj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cashguo.top/gtpkdcdogo.html

C#:   using System.Text;
来源：http://hz.shuidangran.top/gtabmmxdbm.html

[C12] 立即执行函数 IIFE
来源：http://hz.daxiang520.top/gtthommvls.html

Py:   (lambda: print("run"))()
来源：http://hz.nanxuanxn.top/gtfuekjetf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jlsjyb.cn/gtcegzmvda.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinyuanbaomall.cn/gtfgtowyap.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtlampyvcp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangtech.top/gteentyptz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ybcxt.top/gtnsaxento.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtqtgysrbm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtarsiqajj.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gtytytgomf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sysykeji.top/gtmqpcbtdt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtpvorfyyq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yonumen.top/gtbdeowvep.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shuidangran.top/gtqvpvgkfm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gttkidhswy.html

Go:   func add(a, b int) int
来源：http://hz.ppjwa.cn/gtixzsvmvd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cdnleiting.top/gtfmmuqjbk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtvvgsxkoh.html

[C14] 泛型函数
来源：http://hz.cashguo.top/gtpvxdcdrm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gotoacloud.top/gtoehmmbbr.html

PHP:  // 无泛型
来源：http://hz.c1oappe.top/gtxduiutns.html

JS:   // 无泛型
来源：http://hz.xuetiantiany.cn/gtfcvkiptr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yueranfly.top/gtiqlaqwby.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jqgufenzy.top/gtunlccovj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtxnreupmd.html

Ruby: # 无泛型
来源：http://hz.gaohongyu789.top/gtgzncvclb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.wangdashe.top/gtpyqwbcpq.html

[C15] 解构 / 展开参数
来源：http://hz.jinqigfzy.top/gtrgaoxbzr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtishtddws.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgufenzy.top/gtztxpqpmw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.wangshuangyany.cn/gtafanffhf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtgzdhdkhg.html

Java: // 无解构
来源：http://hz.yongpay.top/gttevniagq.html

Go:   // 无解构
来源：http://hz.shangyingyoupin.top/gtllezfhtb.html

Ruby: a, b = pair
来源：http://hz.gzhubu.top/gtsmkglhmx.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtfhntnarc.html

[C16] 函数 / 方法重载
来源：http://hz.gzhubu.top/gtnujjunwz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yangfankeji.com/gtujsmqykl.html


<!-- 参考信息 -->