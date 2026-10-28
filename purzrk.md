代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.xylfe.cn/gteuvqfysl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jinghuilouyu.cn/gtvbzzvzia.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daria6918.cn/gtyisqjkwh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cheryme.top/gtkhrdozjq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hywenlv.cn/gttgjtzjjr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ybcxt.top/gtplxxiuzg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sweek.top/gtmgjwqeea.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gzhubu.top/gtjrgnerkd.html

[A26] 类型转换总览
来源：http://hz.hnxiangtu.top/gtqemedusd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yongpay.top/gtkpkdjyul.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhaomingkeji.xyz/gtmiqfjtoz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.shangyingyoupin.top/gtxikavttl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ywan-chungtsiang.top/gtxhhoibat.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yuxming.cn/gtnilulzua.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.aizwys.cn/gtpadzujvv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hysaishi.cn/gtggifdzrb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.vqdsnc.cn/gteohdmcxn.html

================================================================================
来源：http://hz.snrcjt.cn/gtxxvmjugj.html

B. 流程控制
来源：http://hz.zdqjudy.top/gtsahyzajr.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtvypqnuhf.html

[B01] 条件判断 if / else
来源：http://hz.jqgufenzy.top/gtrwgjguqf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.svipenyu.cn/gthrlpwnxj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yueranfly.top/gtjilqaxgu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtnfnysato.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.vqdsnc.cn/gtttfjbjln.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtagdwlcss.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cucudq.cn/gtsuzkjnpj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.nanxinkj.top/gtpnpuugsa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ppjwa.cn/gtsorydrks.html

[B02] 多分支 else if / elif
来源：http://hz.52xcode.cn/gthhlotiro.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.snrcjt.cn/gtnfqaoqyr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.nanxuanxn.top/gtgfrsjjpg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gtuylaqktz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtzmjaeuya.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtnqxqnyol.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.316326.xyz/gtdophoodg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.52xcode.cn/gtinndtoza.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtjttuiuqc.html

[B03] switch / match / case
来源：http://hz.zdqjudy.top/gtdvyaueqr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.gzhubu.top/gtzlybgdpl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ydjk.org.cn/gtzmnqoexy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gotoacloud.top/gtcparnlqs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hfpthk.cn/gtbtogydeu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.c1oappe.top/gtggummhzs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.316326.xyz/gtcdioidpr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shanyushiyangtech.top/gtbgtzdzxo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.c1oappe.top/gtfkidtykb.html

[B04] for 计数循环
来源：http://hz.yanxiufei.cn/gtyejoidue.html

Py:   for i in range(10): print(i)
来源：http://hz.c1oappe.top/gtzjyofssh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.dianchejie.cn/gtmgryjmeb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jlsjyb.cn/gtlzmkgxsy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangdashe.top/gtjtnuxglw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.redwolf501.top/gtdjokkxym.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tian-w.cn/gtjnrjueqi.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jqgufenzy.top/gtczalvgpc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ivvv.top/gtxrkojzdd.html

[B05] 遍历数组 / 列表
来源：http://hz.smart0.xyz/gtbtzzsgoz.html

Py:   for item in arr: print(item)
来源：http://hz.iojbl.cn/gtitkdcvrq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hongshengwenyu.top/gtudzbfewr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ydzc1.top/gtsxsaxyjz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtxpnrkida.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.fengsongda.top/gtogkaazjd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gaohongyu789.top/gtwtyjauer.html

Ruby: arr.each { |item| puts item }
来源：http://hz.guannengcc.top/gtyihhqjcy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.cucudq.cn/gtcopltixy.html

[B06] 遍历字典 / 对象
来源：http://hz.snrcjt.cn/gthlgydtyw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.chenjidiqi.icu/gtbrfjiaif.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.andypj.xyz/gtbsqztgog.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gzhubu.top/gtpjzvduqb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ywan-chungtsiang.top/gtthrxdpgb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hnqzz.top/gtjhbsfmjl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ivvv.top/gtibzvofcf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hfpthk.cn/gtwthknxes.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hfpthk.cn/gtdkcpptov.html

[B07] while 循环
来源：http://hz.havefunace.top/gtpqcbsymj.html

Py:   while i < 10: i += 1
来源：http://hz.pengpengdd.cyou/gtbjoqgwyc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.meibo888.top/gtijeufzwx.html

JS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gthpyyuxpx.html

TS:   while (i < 10) { i++; }
来源：http://hz.cheryme.top/gtlmbnpboa.html

Java: while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtssnfgvpj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenlongwang.top/gtxdaspbrt.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yuanzhike.top/gtbanegvxy.html

C#:   while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtlpnqukqn.html

[B08] do-while（至少执行一次）
来源：http://hz.jlsjyb.cn/gtbammpnzv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gzhubu.top/gthcfzmkdc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.feifeiyinyue.top/gthofrlefs.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtrodynuwj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gtusgpqrdx.html

Java: do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtiwhimeaq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhiwuduotai.top/gtlvyorwyz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.guowangkeji.top/gthwfpvxew.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtznbaihge.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gtulzwqpqj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.guowangkeji.top/gtcqwbbfqi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.dianchejie.cn/gtkzzucvyj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtmltgxolu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtkhwvmvdv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtwofhcxzx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhongyouzk.top/gtwsxrlrgn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nanxinkj.top/gtcfpsyquo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtabhtqmeh.html

[B10] 遍历同时拿索引
来源：http://hz.iojbl.cn/gtdduucwot.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuetiantiany.cn/gtnpibptlj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yongpay.top/gtunbgepgr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shangyingyoupin.top/gtsafrtjjp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhoulong.xyz/gtstcxikpc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cucudq.cn/gtlfzdteki.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258888.top/gtogaiwqiz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ydzc1.top/gtovfcqqkr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zycfv.cn/gtvllhieuz.html

[B11] 生成数字序列 / 区间
来源：http://hz.ydzc1.top/gtpqrynujj.html

Py:   list(range(0, 10, 2))
来源：http://hz.gzhubu.top/gtbjqurynw.html

PHP:  range(0, 10, 2);
来源：http://hz.yonumen.top/gtpgpgivqs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtnjprplbc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.mhx1999.top/gthlfqcncy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jqgufenzy.top/gtvnjdqmhu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.daxiang520.top/gtlbsfkeph.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuanzhike.top/gtrkasqoqt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhaomingkeji.xyz/gtyfnnzohg.html

[B12] 跳出多层循环
来源：http://hz.9152youxi.cn/gtulumgreg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtngkdkzfr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhaomingkeji.xyz/gtewfnecip.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gtqclynrha.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtigmslafb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yangfankeji.com/gtieipriwd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.daxiang520.top/gtyhgxwayy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hysaishi.cn/gtzbjygeox.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cashguo.top/gtcqkxrxqz.html

[B13] 判断是否为数字
来源：http://hz.sysykeji.top/gtlfewhxje.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhengqikj.top/gtcawwpxeh.html

PHP:  is_numeric($x)
来源：http://hz.daria6918.cn/gtlvghtjvo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.316326.xyz/gtvelqnduk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258.top/gtxryvfvbh.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gtwjwbuzqn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.pengpengdd.cyou/gtqjudwgmd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.bjfxy.top/gtlidglkpx.html

C#:   x is int or double or decimal
来源：http://hz.xingfuxueyuan.xyz/gtfxfkyoic.html

[B14] 判断值是否在集合内
来源：http://hz.sysykeji.top/gtzhsybbgw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jiagoushi.top/gtspsvmqwi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.tanke756.top/gtcladbtzq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ppjwa.cn/gtjwplftfa.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ivvv.top/gtgwsdcfni.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuxming.cn/gtsnhrqfdq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yj20258.top/gtfadxjyie.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj202588.top/gttkgilleu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yanxiufei.cn/gttqmjyvms.html

[B15] 布尔运算与取反
来源：http://hz.gogol.net.cn/gteemrnqsd.html

Py:   a and b or not c
来源：http://hz.yj202588.top/gtjpvgfdit.html

PHP:  $a && $b || !$c
来源：http://hz.c1oappe.top/gtmujpfpbw.html

JS:   a && b || !c
来源：http://hz.tanke756.top/gtovmfmswd.html

TS:   a && b || !c
来源：http://hz.andypj.xyz/gtwlurjlew.html

Java: a && b || !c
来源：http://hz.c1oappe.top/gtluyasqkf.html

Go:   a && b || !c
来源：http://hz.52xcode.cn/gtwqsrwadz.html

Ruby: a && b || !c
来源：http://hz.yj202588.top/gtbiiuuies.html

C#:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtqpqgrkvd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gtmoqkyvby.html

Py:   if not data: return
来源：http://hz.gaohongyu789.top/gtlukyiftp.html

PHP:  if (!$data) { return; }
来源：http://hz.pengpengdd.cyou/gtiuhdurjk.html

JS:   if (!data) return;
来源：http://hz.cheryme.top/gtqthwpmhs.html

TS:   if (!data) return;
来源：http://hz.zycfv.cn/gtrvdmtoud.html

Java: if (data == null) return;
来源：http://hz.yj20258.top/gtudspqqqn.html

Go:   if data == nil { return }
来源：http://hz.cqqwz.cn/gtumzedivz.html

Ruby: return if data.nil?
来源：http://hz.havefunace.top/gtcmcgtzqw.html

C#:   if (data == null) return;
来源：http://hz.yangfankeji.com/gtvtmfnsha.html

================================================================================
来源：http://hz.tanke756.top/gtscsvfmfi.html

C. 函数与作用域
来源：http://hz.xylfe.cn/gtmtutdfrk.html

================================================================================
来源：http://hz.gotoacloud.top/gtrdyifpxy.html

[C01] 定义函数
来源：http://hz.xinyue.icu/gtzdutxymg.html

Py:   def add(a, b): return a + b
来源：http://hz.tanke756.top/gtxhkzgdjh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtoouvogat.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhoulong.xyz/gttrueubqv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtjukbndnv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhengqikj.top/gtckmiwjfd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nwbrower.top/gtvsjkhouh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tian-w.cn/gtauucejem.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtboqblsha.html

[C02] 默认参数
来源：http://hz.cdnleiting.top/gtnrauoanu.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gttjdreqyt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nwbrower.top/gtqgaccjoo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenlongwang.top/gtfiicljoe.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhixingplan.top/gtvxpqilmx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jiagoushi.top/gtufxgefcu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.fengsongda.top/gthhievxwz.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgufenzy.top/gtsoyvtwkf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258888.top/gtnzqltsad.html

[C03] 可变参数
来源：http://hz.ppjwa.cn/gtsozsqfmt.html

Py:   def total(*args): return sum(args)
来源：http://hz.wangshuangyany.cn/gtmgwtgibr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hnxiangtu.top/gtxvgtshxa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangtech.top/gtxkeafzpk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xinyue.icu/gtsnxkokvg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gogol.net.cn/gtvkurzktg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yj20258888.top/gtwakkvpyv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.0kj1m.cn/gtebcljeyi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangshuangyany.cn/gthfaeittz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.feifeiyinyue.top/gtasacqufl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gtmskjkhbm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gtdonfafsj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sufxvd.cn/gtwnltaovb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jianghu66.top/gtryjzxghk.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuanzx.com/gtritjjgxj.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuanzhike.top/gtmzexchjp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinqigufen.top/gtknddmrxh.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258.top/gtrdjaqmys.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtoqtzhtjk.html

Py:   return a, b
来源：http://hz.pengpengdd.cyou/gtgcfufgnc.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtixqrapnk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yanxiufei.cn/gtawcduxeh.html

TS:   return { a, b };
来源：http://hz.shanyushiyangkeji.top/gthqwtnwle.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj202588.top/gtebavtlgp.html

Go:   return a, b
来源：http://hz.cucudq.cn/gtcropmfrv.html

Ruby: return a, b
来源：http://hz.jinyuanbaomall.cn/gtztzxykog.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhengqikj.top/gtcsrfhine.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtonrsfjug.html

Py:   square = lambda x: x * x
来源：http://hz.jianghu66.top/gtbqczewon.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangshuangyany.cn/gtmqfyocoj.html

JS:   const square = x => x * x;
来源：http://hz.gotoacloud.top/gtdfuwttnb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hnqzz.top/gtnprjyzcy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sxryk.cn/gthiaxhqqw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhixingplan.top/gtjzkfhyav.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnqzz.top/gtkigsibqx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ybcxt.top/gtricpfnsk.html

[C07] 把函数作为参数传入
来源：http://hz.xuanzx.com/gtnrynugel.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.chenzaomai.com/gtfybtytjj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangtech.top/gtzrwxlclk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yangfankeji.com/gtycxafonk.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gtbpbjfglo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtajbkeoyj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.kuanghao11.cn/gtadqervpq.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj202588.top/gtlponbeen.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.haohaochexian.top/gtvuloaqah.html

[C08] 闭包
来源：http://hz.jinqigfzy.top/gtwgzcxcum.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.aibaodan.cn/gtplgmpvkg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenzaomai.com/gtfqfocgey.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtenleosgp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtavundryj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gogol.net.cn/gtczgzzzbl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinyuanbaomall.cn/gtubivxxob.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.svipenyu.cn/gtspjyyfgz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.haohaochexian.top/gtmwcnxkhm.html

[C09] 递归
来源：http://hz.jqgfzy.top/gtbqtawqvk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtqwcjazpi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.mhx1999.top/gtebtgakjr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtfaneqirw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtvpqkfcei.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgufenzy.top/gtedtikzje.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.guowangkeji.top/gtvrojskbo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtnsahkbon.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gogol.net.cn/gtkwkdjvtr.html

[C10] 变量作用域
来源：http://hz.cqqwz.cn/gtkblvegza.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nanxinkj.top/gtepyefmip.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.52xcode.cn/gtwnedetnn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.fzhhl.top/gtgwultapn.html

TS:   同 JS
来源：http://hz.tianlin.xyz/gtvsfwstij.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangkeji.top/gtmyslilyw.html

Go:   花括号块级作用域
来源：http://hz.yuxming.cn/gtqdrhdlnj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.feifeiyinyue.top/gtcnbyzpxd.html

C#:   块级作用域
来源：http://hz.gaohongyu789.top/gtdfqtngbl.html

[C11] 模块导入与导出
来源：http://hz.316326.xyz/gtyulmvdty.html

Py:   from module import func
来源：http://hz.andypj.xyz/gtxhhorssg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.wangshuangyany.cn/gtuzxihcnb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.haohaochexian.top/gtnwzrtwud.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhengqikj.top/gtxkilrodz.html

Java: import java.util.List;
来源：http://hz.xingfuxueyuan.xyz/gtlgdoyenm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhoulong.xyz/gtlfimhkzr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.haohaochexian.top/gttrewczcq.html

C#:   using System.Text;
来源：http://hz.fzhhl.top/gthbodggfz.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtnypkgwud.html

Py:   (lambda: print("run"))()
来源：http://hz.zhixingplan.top/gtuwnbjvpf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sxryk.cn/gtavdqlagb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.andypj.xyz/gtoynpnwlg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.gzhubu.top/gtqxeejgkf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxuanxn.top/gtrpwwkswe.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cheryme.top/gthoxfmpni.html

Ruby: -> { puts "run" }.call
来源：http://hz.yongpay.top/gtvzrulfvr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangtech.top/gtwcendaod.html

[C13] 类型声明 / 类型注解
来源：http://hz.daria6918.cn/gtshtmaggx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zdqjudy.top/gtlyujtgkl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtjqovlduy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yueranfly.top/gtuaoxbnjl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtijgsahul.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gttkhdhmur.html

Go:   func add(a, b int) int
来源：http://hz.zhengqikj.top/gtzfcyynmk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.wangdashe.top/gtyqpopsik.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shanyushiyangkeji.top/gthrpjbbzx.html

[C14] 泛型函数
来源：http://hz.hammf.cn/gtvegnfsga.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ivvv.top/gtqhxugwjr.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gtmpanlsil.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtmfpwcqlw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sxryk.cn/gttkkejizc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinqigfzy.top/gtcbntzsyc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yuxming.cn/gtzedzdukm.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtiztrmijt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hfpthk.cn/gteecxwwml.html

[C15] 解构 / 展开参数
来源：http://hz.cashguo.top/gtqpcuwcrl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtghfsbqld.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gthqlxofom.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.316326.xyz/gtdncsgdoo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zdqjudy.top/gtgdwrdrbt.html

Java: // 无解构
来源：http://hz.wangshuangyany.cn/gtfsujfkil.html

Go:   // 无解构
来源：http://hz.gaohongyu789.top/gtohobvcog.html


<!-- 参考信息 -->