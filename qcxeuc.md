代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ydjk.org.cn/gtampmajaf.html

[B02] 多分支 else if / elif
来源：http://hz.daria6918.cn/gthajxccyo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hnxiangtu.top/gtbjhbltoq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jiagoushi.top/gtudqdqncm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cqqwz.cn/gtidtpatur.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gttyrdcstd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yueranfly.top/gtcopuqxec.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.cashguo.top/gtncdewpnw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.9152youxi.cn/gtywvkmvlp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinyuanbaomall.cn/gtbpazklox.html

[B03] switch / match / case
来源：http://hz.fengsongda.top/gttfjihnts.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.aibaodan.cn/gtoouhixnv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.meibo888.top/gtdtasgims.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.smart0.xyz/gtteuxodbg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ppjwa.cn/gtsvjjiecy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gtqpcfshzc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.0kj1m.cn/gtzyxuqlxf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhijiandao.cn/gtmdzfdufs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xingfuxueyuan.xyz/gtyynlpbcg.html

[B04] for 计数循环
来源：http://hz.zhiwuduotai.top/gtyogjrzwb.html

Py:   for i in range(10): print(i)
来源：http://hz.c1oappe.top/gtgsaujvjd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.dianchejie.cn/gtlltvfjas.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hammf.cn/gtvvrhhhpr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cucudq.cn/gtvngjkyda.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ydjk.org.cn/gtkwayrcdm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.haohaochexian.top/gtlbuilmem.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ivvv.top/gtnystjmon.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.cqqwz.cn/gtkoecfeyx.html

[B05] 遍历数组 / 列表
来源：http://hz.sufxvd.cn/gtvdbfipoc.html

Py:   for item in arr: print(item)
来源：http://hz.feifeiyinyue.top/gtxdvdvsul.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.wangdashe.top/gtbvdcrgcg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.svipenyu.cn/gtjwtxbcin.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shangyingyoupin.top/gtxoyvfilv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.316326.xyz/gtrwzutrhn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinqigufen.top/gtyqtjyszn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.mhx1999.top/gtqrqtqkyq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gzhubu.top/gtjrnfcssi.html

[B06] 遍历字典 / 对象
来源：http://hz.pycfn.com/gtrjbxsbop.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jyoumei.cn/gtnckjxcze.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.tian-w.cn/gtjlgybbro.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ybcxt.top/gtmoirjbqc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ppjwa.cn/gtwuantlst.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yongpay.top/gtaqoqoeee.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.redwolf501.top/gtepmqvxwi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.guannengcc.top/gtqrqqyuyg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.fengsongda.top/gtfbhlgfpf.html

[B07] while 循环
来源：http://hz.yuanzhike.top/gtmmdzzvoo.html

Py:   while i < 10: i += 1
来源：http://hz.yj202588.top/gtimustjfs.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.wangshuangyany.cn/gtpmqagwtu.html

JS:   while (i < 10) { i++; }
来源：http://hz.ivvv.top/gtxrqrxqsw.html

TS:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtzjbdlvre.html

Java: while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtjtcwdgjt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shuidangran.top/gtodolxkma.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xylfe.cn/gtuywwqsfo.html

C#:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtavplovyq.html

[B08] do-while（至少执行一次）
来源：http://hz.fengsongda.top/gtoyroranr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.dianchejie.cn/gtroxaxzsv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.52xcode.cn/gtrhcdeboe.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinghuilouyu.cn/gtxsyntghk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtpopvlawk.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtzxrnqzvu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhaomingkeji.xyz/gtcwjyxgnc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shangyingyoupin.top/gtkrjamzxf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.pengpengdd.cyou/gtljurchdo.html

[B09] break 与 continue
来源：http://hz.redwolf501.top/gtlkwqothv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aibaodan.cn/gtkkxzfiyg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yuxming.cn/gthmekjsmu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtexfagorz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtdfujfgsz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtwydixdrb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.vqdsnc.cn/gthhqmjkmd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.mhx1999.top/gtthxwhfyo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtdsoxasqj.html

[B10] 遍历同时拿索引
来源：http://hz.cqqwz.cn/gtxzxnskob.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.mhx1999.top/gthkehkjhh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.nwbrower.top/gtuloxyeuj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sweek.top/gtldwzqbnv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jlsjyb.cn/gtbhaguchu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigufen.top/gtmazrqlfh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangshuangyany.cn/gthafwdnok.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xingfuxueyuan.xyz/gtunmfyuxa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangtech.top/gtijrfwpis.html

[B11] 生成数字序列 / 区间
来源：http://hz.zdqjudy.top/gtcumdwqkx.html

Py:   list(range(0, 10, 2))
来源：http://hz.dianchejie.cn/gtnukgcirp.html

PHP:  range(0, 10, 2);
来源：http://hz.andypj.xyz/gttggqapom.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.bjfxy.top/gthgyqlrok.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sxryk.cn/gtrodjpsos.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.kuanghao11.cn/gtzxxrbtil.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gthqyhkctb.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sweek.top/gtmtzcvucc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhengqikj.top/gtdzbsjcun.html

[B12] 跳出多层循环
来源：http://hz.jyoumei.cn/gtrxcusxzo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.bjfxy.top/gthljjoxxm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cdnleiting.top/gtydvwycpo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gtridkpzqu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtqbqaloki.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gtxwylsrzu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hnqzz.top/gtwsknwqzg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hongshengwenyu.top/gtrpndwhkf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.guannengcc.top/gterstroyy.html

[B13] 判断是否为数字
来源：http://hz.52xcode.cn/gtnrxkbump.html

Py:   isinstance(x, (int, float))
来源：http://hz.daria6918.cn/gtocckphhi.html

PHP:  is_numeric($x)
来源：http://hz.nanxuanxn.top/gtropjmwnc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ppjwa.cn/gtlwczjmxg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tanke756.top/gtbuvoxghy.html

Java: x instanceof Number
来源：http://hz.dashuyun.cn/gtvqkzmpqa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.aizwys.cn/gthmjyxlow.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuanzx.com/gtirovztvn.html

C#:   x is int or double or decimal
来源：http://hz.ehwqpu.com/gtcjbdnggx.html

[B14] 判断值是否在集合内
来源：http://hz.daxiang520.top/gtcavvyuro.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xziqi.cn/gtknnusqww.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zdqjudy.top/gtkybmrdzs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtziuomrqn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtrjsoiapi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ehwqpu.com/gtseslzvym.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinqigufen.top/gtrurerpcd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.iojbl.cn/gtancklvxo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydzc1.top/gtdvrlftqt.html

[B15] 布尔运算与取反
来源：http://hz.ybcxt.top/gtgiaqhwom.html

Py:   a and b or not c
来源：http://hz.kuanghao11.cn/gtklcajcco.html

PHP:  $a && $b || !$c
来源：http://hz.yueranfly.top/gtzmzwppyn.html

JS:   a && b || !c
来源：http://hz.daxiang520.top/gtmxfloepk.html

TS:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtejqavzgo.html

Java: a && b || !c
来源：http://hz.gotoacloud.top/gthcbbuifl.html

Go:   a && b || !c
来源：http://hz.cashguo.top/gtwfhfxggp.html

Ruby: a && b || !c
来源：http://hz.xuetiantiany.cn/gtyisdmjzy.html

C#:   a && b || !c
来源：http://hz.gaohongyu789.top/gtdnfjjosp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ppjwa.cn/gtqxtiyawg.html

Py:   if not data: return
来源：http://hz.snrcjt.cn/gtzyasmzcp.html

PHP:  if (!$data) { return; }
来源：http://hz.0kj1m.cn/gtksqxspbo.html

JS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtohgchqzt.html

TS:   if (!data) return;
来源：http://hz.yonumen.top/gtrqynmoqw.html

Java: if (data == null) return;
来源：http://hz.hnxiangtu.top/gtbakeoenc.html

Go:   if data == nil { return }
来源：http://hz.hongshengwenyu.top/gtmtopswef.html

Ruby: return if data.nil?
来源：http://hz.zhongyouzk.top/gtptlpvjdh.html

C#:   if (data == null) return;
来源：http://hz.52xcode.cn/gtrxgrwapv.html

================================================================================
来源：http://hz.hnqzz.top/gtysjmjlov.html

C. 函数与作用域
来源：http://hz.nanxuanxn.top/gthywknyti.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwyvlvxzh.html

[C01] 定义函数
来源：http://hz.yonumen.top/gtusyiyusa.html

Py:   def add(a, b): return a + b
来源：http://hz.xuanzx.com/gtxugvgiko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.316326.xyz/gtobbcdtym.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yvedp.cn/gteylzbxnl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.snrcjt.cn/gtpnsugdut.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtchxxsepy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ydzc1.top/gtbqdjqubu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.snrcjt.cn/gtnudxtdfm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gtqczfsrfr.html

[C02] 默认参数
来源：http://hz.xylfe.cn/gtwxdbngds.html

Py:   def greet(name="World"): return name
来源：http://hz.yanxiufei.cn/gtvemzcifz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jiagoushi.top/gttsrekurh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258888.top/gtqzogwzje.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gtrfudpftk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dashuyun.cn/gtdygxfhge.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cqqwz.cn/gtljiyrzsz.html

Ruby: def greet(name = "World") = name
来源：http://hz.tian-w.cn/gtoojrmige.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhixingplan.top/gtifhmrgwu.html

[C03] 可变参数
来源：http://hz.yongpay.top/gthqnmrjny.html

Py:   def total(*args): return sum(args)
来源：http://hz.hfpthk.cn/gtisfblglv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cashguo.top/gtzjksiijz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtaxlmazzc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtzkvtzyhn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.andypj.xyz/gtozhxfzol.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hammf.cn/gtnftxfvhk.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ywan-chungtsiang.top/gtzgutyctm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.smart0.xyz/gtllxdkgux.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aibaodan.cn/gtulzvyuof.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.quarkkingdee.top/gtsotnnjnh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuanzhike.top/gtieqkgzuk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.316326.xyz/gtagvwzgja.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.aizwys.cn/gtgghpgdat.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhengqikj.top/gtmziexgtm.html

Go:   // 无：用配置结构体参数
来源：http://hz.aizwys.cn/gtnvzqizqy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtrzheewff.html

C#:   f(a: 1, b: 2)
来源：http://hz.shzxlz.cn/gtgbulgymk.html

[C05] 返回多个值
来源：http://hz.jqgfzy.top/gtlasnpolo.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtjmqkjakr.html

PHP:  return [$a, $b];
来源：http://hz.yj20258.top/gtwmpgmcek.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guannengcc.top/gthlieycma.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gtmxbvglnn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jiagoushi.top/gtefwimrxp.html

Go:   return a, b
来源：http://hz.hfpthk.cn/gtbirrdvyc.html

Ruby: return a, b
来源：http://hz.xinyue.icu/gtukkalqfh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtbkjqwgrr.html

[C06] 匿名函数 / lambda
来源：http://hz.tianlin.xyz/gtmnpiwfky.html

Py:   square = lambda x: x * x
来源：http://hz.xinyue.icu/gtuukzmgqv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.snrcjt.cn/gtlgjlesbe.html

JS:   const square = x => x * x;
来源：http://hz.birdmap.top/gtmnzrctru.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.316326.xyz/gtaamjngmt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.bjfxy.top/gtpnbzebpz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aibaodan.cn/gtguxejpuq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shzxlz.cn/gtbipbvsys.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.feifeiyinyue.top/gtyjrqtaeb.html

[C07] 把函数作为参数传入
来源：http://hz.yueranfly.top/gtejliyxwo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shzxlz.cn/gtcsazvrge.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hnxiangtu.top/gtgatffjpl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.snrcjt.cn/gtyxlajmcy.html

TS:   arr.map(String)
来源：http://hz.xuanzx.com/gtoyscnikj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhoulong.xyz/gtipiuifjr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.pycfn.com/gtmjyyqbck.html

Ruby: arr.map(&:upcase)
来源：http://hz.gaohongyu789.top/gtdsymcjxx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.nanxuanxn.top/gttgsrbfwb.html

[C08] 闭包
来源：http://hz.haohaochexian.top/gtmqugqzno.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cqqwz.cn/gtdhdcyrxp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.wangshuangyany.cn/gtztrwtipm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtlwsjrzxl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hywenlv.cn/gtdoalvfjd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fengsongda.top/gtpvlqgkof.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhixingplan.top/gtngqsskas.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zycfv.cn/gtgfokukfv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtkipotudi.html

[C09] 递归
来源：http://hz.xuanzx.com/gtrgbxqtaa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gtlcjgoffx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.andypj.xyz/gtzbqtpfkx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhijiandao.cn/gtbmwmcizy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gttabrefgm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gogol.net.cn/gttcqexvqe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.meibo888.top/gtvlnvahtg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ivvv.top/gtuadxuept.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.havefunace.top/gtweafovcw.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtocnovvza.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jinghuilouyu.cn/gtgbtyukhv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jyoumei.cn/gtrtppothc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gtmfxudzci.html

TS:   同 JS
来源：http://hz.cdnleiting.top/gtkeqzimqp.html

Java: 方法内为块级作用域
来源：http://hz.nwbrower.top/gtwgfkonzn.html

Go:   花括号块级作用域
来源：http://hz.yj202588.top/gtjmurkyhf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.meibo888.top/gtekfupvns.html

C#:   块级作用域
来源：http://hz.hysaishi.cn/gtiaqszmke.html

[C11] 模块导入与导出
来源：http://hz.yj202588.top/gtdxgfdlle.html

Py:   from module import func
来源：http://hz.dashuyun.cn/gtupppzqez.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.gotoacloud.top/gtctzifiae.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhoulong.xyz/gtaybvzsnq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhengqikj.top/gtbmycdicg.html

Java: import java.util.List;
来源：http://hz.wangshuangyany.cn/gtiwnbizrr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sysykeji.top/gtiaypuyck.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tanke756.top/gthkwgrxag.html

C#:   using System.Text;
来源：http://hz.hnxiangtu.top/gtpsrwrzkx.html

[C12] 立即执行函数 IIFE
来源：http://hz.smart0.xyz/gtnellhjsj.html

Py:   (lambda: print("run"))()
来源：http://hz.shuidangran.top/gtqbaueitw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.snrcjt.cn/gtkskehiih.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtpjqohrfn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtthnvofqd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tian-w.cn/gtxxpkcrds.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.feifeiyinyue.top/gtsclrlqvz.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinqigfzy.top/gtndxfcmnn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj202588.top/gtukwruufq.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuxming.cn/gtstejhcvw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.fzhhl.top/gttljyoufa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xylfe.cn/gtqnxdexlv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cucudq.cn/gtqfrlwedr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtgolruejt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtzfzhuvqn.html

Go:   func add(a, b int) int
来源：http://hz.feifeiyinyue.top/gtdhovyunc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cashguo.top/gtqrqvcqcl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xinyue.icu/gtbvadwgaz.html

[C14] 泛型函数
来源：http://hz.52xcode.cn/gtimgvtkvx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.redwolf501.top/gtxbdkqgre.html

PHP:  // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtkkzkfneq.html

JS:   // 无泛型
来源：http://hz.yueranfly.top/gtgeukqxjb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jyoumei.cn/gtynehavri.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtwjpvhwmi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.pengpengdd.cyou/gtwvrowrwq.html

Ruby: # 无泛型
来源：http://hz.yangfankeji.com/gtuggleanb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pengpengdd.cyou/gtzanduyqp.html

[C15] 解构 / 展开参数
来源：http://hz.gzhubu.top/gtaspkxmrd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenlongwang.top/gtycqilkft.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yvedp.cn/gteubrrahw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtkpmrnvvx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtofmqcirm.html

Java: // 无解构
来源：http://hz.yj20258.top/gthuunrsko.html

Go:   // 无解构
来源：http://hz.zhengqikj.top/gtfcgqcshj.html

Ruby: a, b = pair
来源：http://hz.316326.xyz/gtgxqoybmg.html

C#:   var (a, b) = pair;
来源：http://hz.smart0.xyz/gtsjuqygir.html

[C16] 函数 / 方法重载
来源：http://hz.cucudq.cn/gtxugggscw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenjidiqi.icu/gthevaexvt.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtnwximvli.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.pengpengdd.cyou/gtywhhimmx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtkolelcsy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.shuidangran.top/gtvftarefi.html

Go:   // 无重载：用不同函数名
来源：http://hz.sufxvd.cn/gtbkuvqucv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hnqzz.top/gtiltiqbxb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.c1oappe.top/gtxfnmsbax.html

================================================================================
来源：http://hz.sxryk.cn/gtksrdvobg.html

D. 数组 / 列表 / 集合
来源：http://hz.hysaishi.cn/gtvpyjicen.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtyofgvqio.html

[D01] 创建数组 / 列表
来源：http://hz.nanxuanxn.top/gtawzmfqti.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yueranfly.top/gtzborsnvl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shanyushiyangkeji.top/gtorbvvepo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shangyingyoupin.top/gtdnojupwp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.andypj.xyz/gtmzldmafa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.pycfn.com/gttiqwlinn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cheryme.top/gtgaahatiy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.kuanghao11.cn/gtgskmtdmd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sufxvd.cn/gttledggev.html

[D02] 追加元素到末尾
来源：http://hz.guannengcc.top/gtzvdfgmhs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.dashuyun.cn/gtofzqardb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daria6918.cn/gtwzalvyfp.html

JS:   arr.push(4);
来源：http://hz.yongpay.top/gtyhmvvjyp.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gtytexbplw.html


<!-- 参考信息 -->