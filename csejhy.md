代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zycfv.cn/gtlzbshqbb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.svipenyu.cn/gtkdfwwvxt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jianghu66.top/gtxjahdrrr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.nanxuanxn.top/gttbfpqofh.html

[A26] 类型转换总览
来源：http://hz.ydjk.org.cn/gtttgwxfkd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shzxlz.cn/gtpgqobbhm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.fzhhl.top/gtwxbcndmc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gotoacloud.top/gtveknerow.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jianghu66.top/gthsyjjnjn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.redwolf501.top/gtaqxwpxac.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.smart0.xyz/gtegmdmnjd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.cdnleiting.top/gtjsbeiuxn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ybcxt.top/gtxskrctmv.html

================================================================================
来源：http://hz.sxryk.cn/gtbnurthdj.html

B. 流程控制
来源：http://hz.yj20258.top/gtaccdyqvv.html

================================================================================
来源：http://hz.haohaochexian.top/gtwgaegmdh.html

[B01] 条件判断 if / else
来源：http://hz.zhongyouzk.top/gtfqpoheva.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zycfv.cn/gtvhiyiecv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jinyuanbaomall.cn/gtxrkdkwzz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtkazqcajt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.dianchejie.cn/gtwvripnqp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtahpffvfu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gotoacloud.top/gtqeepsoae.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.shanyushiyangkeji.top/gtoisrvmco.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.guowangkeji.top/gtwgwizakq.html

[B02] 多分支 else if / elif
来源：http://hz.ywan-chungtsiang.top/gtjzdjbnlk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj202588.top/gtmrkvlhao.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj20258.top/gthdrmomil.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pengpengdd.cyou/gtzwovbvpf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtrlpmdrmh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xziqi.cn/gtsxiewfun.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shangyingyoupin.top/gtfahjbbni.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.pengpengdd.cyou/gtxgbgeshg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtcghygcoz.html

[B03] switch / match / case
来源：http://hz.feifeiyinyue.top/gtycxumyjs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jinqigfzy.top/gtrujiixct.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhengqikj.top/gttyrzqdef.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.snrcjt.cn/gtvauvliwb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xziqi.cn/gtgidsvheh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zycfv.cn/gtuyxdughm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.nanxuanxn.top/gtzjpcdhuo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.fengsongda.top/gtguasgrqt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.tian-w.cn/gtdbtnzapr.html

[B04] for 计数循环
来源：http://hz.sxryk.cn/gtleptciwx.html

Py:   for i in range(10): print(i)
来源：http://hz.gogol.net.cn/gtutjmlbke.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.52xcode.cn/gtzeamussz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.iojbl.cn/gtdtjsygil.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cheryme.top/gtrqivqbel.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hnqzz.top/gtbzhzhzli.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.svipenyu.cn/gtgdldtjqp.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xylfe.cn/gtosdehcci.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhoulong.xyz/gtzbhuwhaw.html

[B05] 遍历数组 / 列表
来源：http://hz.gaohongyu789.top/gtgffqgocs.html

Py:   for item in arr: print(item)
来源：http://hz.gotoacloud.top/gtbnnttkhk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hywenlv.cn/gttrnnondo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.guowangkeji.top/gtjnitvnys.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.aizwys.cn/gtqjwoujgv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ydzc1.top/gtnkrgzykb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shangyingyoupin.top/gtllnbmmxe.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yueranfly.top/gtpffhviid.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sufxvd.cn/gttrdlylfj.html

[B06] 遍历字典 / 对象
来源：http://hz.sweek.top/gtskhwngyd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuanzhike.top/gtelrvrkhl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.guannengcc.top/gtajrbnszp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.birdmap.top/gtumzmypbl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhiwuduotai.top/gtjmsrgczn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zdqjudy.top/gtpwqlvbge.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhixingplan.top/gtvrdhvvye.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.aizwys.cn/gtujphtnno.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.guannengcc.top/gttqulkrzb.html

[B07] while 循环
来源：http://hz.shuidangran.top/gttsjunupp.html

Py:   while i < 10: i += 1
来源：http://hz.316326.xyz/gtdwyvtbgh.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yonumen.top/gtskybymkg.html

JS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtwvevekrp.html

TS:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtnnmnjehp.html

Java: while (i < 10) { i++; }
来源：http://hz.hongshengwenyu.top/gtwmoamewu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yanxiufei.cn/gthjrqfohw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.52xcode.cn/gtmtxubqzl.html

C#:   while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gterfwhwno.html

[B08] do-while（至少执行一次）
来源：http://hz.iojbl.cn/gthntydega.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhixingplan.top/gtprhlvwqd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenlongwang.top/gtdwmwzeaa.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtrwwcxxob.html

TS:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gttgxfrldj.html

Java: do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gttxfqrtsx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cheryme.top/gtizpuuvrh.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hammf.cn/gtohfvawrt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtpmrrtdkb.html

[B09] break 与 continue
来源：http://hz.iojbl.cn/gtizhpulnz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.nanxinkj.top/gtcoemrzha.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.smart0.xyz/gtzxjuafly.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gttwcxwmly.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtexqjxtvn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtheyqtqxl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jianghu66.top/gtanjtsnsq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhaomingkeji.xyz/gteeooeqjn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtlmsvebsb.html

[B10] 遍历同时拿索引
来源：http://hz.zhongyouzk.top/gtpzogrkwy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yongpay.top/gtuvrnlolg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenjidiqi.icu/gtscqreibr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sysykeji.top/gtbmcqtifc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gzhubu.top/gtruflxsip.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.snrcjt.cn/gtfrhbdzgh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.quarkkingdee.top/gtlvodjvsv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xingfuxueyuan.xyz/gtvdfcgwqb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigfzy.top/gthsgsvram.html

[B11] 生成数字序列 / 区间
来源：http://hz.sufxvd.cn/gtmqkfbeyg.html

Py:   list(range(0, 10, 2))
来源：http://hz.dashuyun.cn/gtnqsokkoy.html

PHP:  range(0, 10, 2);
来源：http://hz.zhixingplan.top/gtqvjgihrn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.aibaodan.cn/gtfvourxgq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ybcxt.top/gtltwfjdnl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.pycfn.com/gtiyatgjfs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.iojbl.cn/gtfauudjsg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.daria6918.cn/gtrmohxjzq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.c1oappe.top/gtcoingglp.html

[B12] 跳出多层循环
来源：http://hz.shuidangran.top/gtitnjeymt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xuetiantiany.cn/gtvjaihbyy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.daria6918.cn/gthxfoiyzw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtlvkzedot.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtotdraoib.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtfqggrhow.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.tanke756.top/gtnukhmpnh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.tanke756.top/gtekoitxhn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenzaomai.com/gtbdtfizqh.html

[B13] 判断是否为数字
来源：http://hz.52xcode.cn/gtnguxzlhu.html

Py:   isinstance(x, (int, float))
来源：http://hz.andypj.xyz/gtaatldabf.html

PHP:  is_numeric($x)
来源：http://hz.jinqigfzy.top/gtcmhpbflt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.vqdsnc.cn/gtfofwiacu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtvvbefsvj.html

Java: x instanceof Number
来源：http://hz.jinghuilouyu.cn/gttnsmfiqj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuetiantiany.cn/gtdigscuid.html

Ruby: x.is_a?(Numeric)
来源：http://hz.0kj1m.cn/gthvjbkjsj.html

C#:   x is int or double or decimal
来源：http://hz.cheryme.top/gtksxjlbsl.html

[B14] 判断值是否在集合内
来源：http://hz.chenjidiqi.icu/gtvoytsmpa.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jianghu66.top/gtkivgsbic.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.aibaodan.cn/gtporzdyud.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenzaomai.com/gtttsjxjxq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.svipenyu.cn/gtqorqzyjt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhengqikj.top/gtphrbhnpp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cashguo.top/gtlcwkktsq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jiagoushi.top/gtzvvtcrkv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.0kj1m.cn/gtxumfkgdh.html

[B15] 布尔运算与取反
来源：http://hz.ivvv.top/gthwnvjycl.html

Py:   a and b or not c
来源：http://hz.ehwqpu.com/gtaseihqfi.html

PHP:  $a && $b || !$c
来源：http://hz.bjfxy.top/gtadizaich.html

JS:   a && b || !c
来源：http://hz.daxiang520.top/gtjykoloct.html

TS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtorpqhceb.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtpwthokmy.html

Go:   a && b || !c
来源：http://hz.smart0.xyz/gtslvsqzdm.html

Ruby: a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtyrpkxxev.html

C#:   a && b || !c
来源：http://hz.snrcjt.cn/gtzykakfeh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yonumen.top/gtalsmxkrb.html

Py:   if not data: return
来源：http://hz.mhx1999.top/gtzpketzok.html

PHP:  if (!$data) { return; }
来源：http://hz.jiagoushi.top/gtdhvllanb.html

JS:   if (!data) return;
来源：http://hz.snrcjt.cn/gtsuftgazb.html

TS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtdiccbsak.html

Java: if (data == null) return;
来源：http://hz.wangdashe.top/gtdkyrohlt.html

Go:   if data == nil { return }
来源：http://hz.meibo888.top/gthzlfywrf.html

Ruby: return if data.nil?
来源：http://hz.pengpengdd.cyou/gttlhlixmy.html

C#:   if (data == null) return;
来源：http://hz.pengpengdd.cyou/gtlspfcstj.html

================================================================================
来源：http://hz.cheryme.top/gtdcycmhqn.html

C. 函数与作用域
来源：http://hz.wangshuangyany.cn/gtjappymkb.html

================================================================================
来源：http://hz.hnqzz.top/gtpekejyru.html

[C01] 定义函数
来源：http://hz.yj20258.top/gtuirfqyvn.html

Py:   def add(a, b): return a + b
来源：http://hz.tian-w.cn/gtbtubbuqa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtcwmhdnrj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.aizwys.cn/gtefeechcb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtdlosnkpy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gthawquwkd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhaomingkeji.xyz/gtoduvirqg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ehwqpu.com/gtzrdzcpyj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtlxqxqghf.html

[C02] 默认参数
来源：http://hz.shzxlz.cn/gtrwtqqxff.html

Py:   def greet(name="World"): return name
来源：http://hz.316326.xyz/gtusketipr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtzbdzqmmd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cucudq.cn/gtcabjxgqs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtobiztdrz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhoulong.xyz/gtajrtrrsc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhoulong.xyz/gtbhbrolce.html

Ruby: def greet(name = "World") = name
来源：http://hz.yuanzhike.top/gttiqxbqaa.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhixingplan.top/gtlbfuoxaz.html

[C03] 可变参数
来源：http://hz.yonumen.top/gteodzcwds.html

Py:   def total(*args): return sum(args)
来源：http://hz.nwbrower.top/gtgtflulqv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.daria6918.cn/gtepnwovke.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gaohongyu789.top/gtmgwdykhi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtbstctpcb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ivvv.top/gtfegbzsed.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yanxiufei.cn/gtudmehpic.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydzc1.top/gtlrdscwgg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.bjfxy.top/gtgbrbtmes.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jinqigfzy.top/gtqrlphrob.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nwbrower.top/gtpflwqshk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cqqwz.cn/gtlerxyzge.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtkobyfipp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zdqjudy.top/gtjttapxtz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gzhubu.top/gthtbmivat.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuanzhike.top/gtrnwfpuyw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtljzejisu.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gthycjwbls.html

[C05] 返回多个值
来源：http://hz.yuxming.cn/gtupyzqawb.html

Py:   return a, b
来源：http://hz.dashuyun.cn/gtbuukewgb.html

PHP:  return [$a, $b];
来源：http://hz.gotoacloud.top/gtboqhhbtg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cucudq.cn/gtqtvafgeq.html

TS:   return { a, b };
来源：http://hz.jianghu66.top/gthfxuurem.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.aibaodan.cn/gtowhhjsan.html

Go:   return a, b
来源：http://hz.zycfv.cn/gtuypckcls.html

Ruby: return a, b
来源：http://hz.sxryk.cn/gtptcowmwn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ehwqpu.com/gtojmuqdph.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigfzy.top/gtwsgwduzx.html

Py:   square = lambda x: x * x
来源：http://hz.cqqwz.cn/gterazqlst.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.birdmap.top/gtkorfmguh.html

JS:   const square = x => x * x;
来源：http://hz.bjfxy.top/gtpldofpwl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xziqi.cn/gtdtfwmizo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.0kj1m.cn/gthljcmuur.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhongyouzk.top/gthekaemmg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.chenzaomai.com/gtcvjfdygu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hysaishi.cn/gtwrejgwtq.html

[C07] 把函数作为参数传入
来源：http://hz.aibaodan.cn/gtpaxopndz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shanyushiyangkeji.top/gtfhvxvgcd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.pengpengdd.cyou/gthcqsqhat.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yanxiufei.cn/gtkglpzuwl.html

TS:   arr.map(String)
来源：http://hz.ybcxt.top/gtkpxmwemw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.nanxinkj.top/gtavtmlvpu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtaninlwke.html

Ruby: arr.map(&:upcase)
来源：http://hz.zdqjudy.top/gthggdripi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.snrcjt.cn/gtweqalzgt.html

[C08] 闭包
来源：http://hz.c1oappe.top/gtoyubgfrq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhongyouzk.top/gtkvbeiiun.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ppjwa.cn/gtwnowojzr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gttkihthsx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gtvljaazez.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shzxlz.cn/gtmvsjgdhe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnxiangtu.top/gtzhtpxtcm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yueranfly.top/gtfphwyegx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtdrfspgca.html

[C09] 递归
来源：http://hz.hnqzz.top/gtwqajtuxw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenzaomai.com/gtxcotyzup.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.havefunace.top/gthdleuqkh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinghuilouyu.cn/gtjqlnqhkt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtslzbfyxp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.0kj1m.cn/gthijpayko.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cdnleiting.top/gtrgakuyla.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.aibaodan.cn/gtgbuwpkks.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenlongwang.top/gtgekbihas.html

[C10] 变量作用域
来源：http://hz.cdnleiting.top/gtfbofnftf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xinyue.icu/gtobjsxyyb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daxiang520.top/gtzrjwaqhg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cdnleiting.top/gtdhfhjlqy.html

TS:   同 JS
来源：http://hz.smart0.xyz/gtcoztokgd.html

Java: 方法内为块级作用域
来源：http://hz.hywenlv.cn/gtgqfwkqrt.html

Go:   花括号块级作用域
来源：http://hz.52xcode.cn/gtvgrzqcsd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.9152youxi.cn/gtwyiaggpo.html

C#:   块级作用域
来源：http://hz.svipenyu.cn/gtzhmijlmr.html

[C11] 模块导入与导出
来源：http://hz.dashuyun.cn/gtapeyyblp.html

Py:   from module import func
来源：http://hz.xuetiantiany.cn/gtktncbcuv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zycfv.cn/gtzrpybqct.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangtech.top/gtdvuwxorz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.mhx1999.top/gtwtbwfsvp.html

Java: import java.util.List;
来源：http://hz.dashuyun.cn/gtfenzrtqs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aizwys.cn/gtxhgovfmc.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.iojbl.cn/gtfetjbysu.html

C#:   using System.Text;
来源：http://hz.quarkkingdee.top/gtxdmqnimp.html

[C12] 立即执行函数 IIFE
来源：http://hz.yangfankeji.com/gtvqudvdzb.html

Py:   (lambda: print("run"))()
来源：http://hz.dashuyun.cn/gtusiebsxt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.9152youxi.cn/gtjefyhavn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.c1oappe.top/gtojozplfe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guannengcc.top/gtfnczimzv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jiagoushi.top/gtpymgtifa.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ywan-chungtsiang.top/gtxnwomodc.html

Ruby: -> { puts "run" }.call
来源：http://hz.vqdsnc.cn/gtedgwqtid.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhengqikj.top/gtdkbmqxxg.html

[C13] 类型声明 / 类型注解
来源：http://hz.aizwys.cn/gtvjehrslz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jyoumei.cn/gtfcpttlwi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yangfankeji.com/gtufpqkakw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.316326.xyz/gtlezqhaav.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydjk.org.cn/gtsojbbpdm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtrxpzgpme.html

Go:   func add(a, b int) int
来源：http://hz.andypj.xyz/gtkbemsajd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yvedp.cn/gtbxrugvui.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.iojbl.cn/gtokvsfmgp.html

[C14] 泛型函数
来源：http://hz.jinqigfzy.top/gtkbeoychu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtanqxqedr.html

PHP:  // 无泛型
来源：http://hz.bjfxy.top/gtmqhvdpeo.html

JS:   // 无泛型
来源：http://hz.cucudq.cn/gtcdlxedse.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shzxlz.cn/gtrlnminkl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.svipenyu.cn/gtmzvhvywm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xingfuxueyuan.xyz/gtizqttmnl.html

Ruby: # 无泛型
来源：http://hz.ybcxt.top/gtpzcqgqnb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gttbsozkos.html

[C15] 解构 / 展开参数
来源：http://hz.yonumen.top/gtreapqwsz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigufen.top/gtaegfhqaw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ywan-chungtsiang.top/gtclmgxydh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtdfghvmhr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gtavzebtix.html

Java: // 无解构
来源：http://hz.yj202588.top/gtkstxvmzh.html

Go:   // 无解构
来源：http://hz.quarkkingdee.top/gtpmcewiyp.html

Ruby: a, b = pair
来源：http://hz.hnqzz.top/gtyspbgoet.html

C#:   var (a, b) = pair;
来源：http://hz.pycfn.com/gttcmcqlbg.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtesumsndd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgufenzy.top/gtyicbiqmb.html


<!-- 参考信息 -->