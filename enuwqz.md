代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.jinghuilouyu.cn/gtbvcgeril.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.gogol.net.cn/gtbuekgxfo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.mhx1999.top/gtdlyjabhj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yj20258888.top/gtbjkrezzi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.cqqwz.cn/gtjvwyfuwb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.redwolf501.top/gtlfmbuxuf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.daxiang520.top/gtvlruzytu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.daxiang520.top/gtparkeidt.html

[A26] 类型转换总览
来源：http://hz.yuanzhike.top/gtexxtwdqy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.9152youxi.cn/gteyykjdgn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xingfuxueyuan.xyz/gtttdcgrik.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gotoacloud.top/gtygsajurs.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xuetiantiany.cn/gtuolthnse.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.c1oappe.top/gtzheprvbb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ivvv.top/gtytgzjoxx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.gaohongyu789.top/gtqyvgejwb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yanxiufei.cn/gtdxdkcfre.html

================================================================================
来源：http://hz.hfpthk.cn/gtlduhddql.html

B. 流程控制
来源：http://hz.havefunace.top/gtudsahfwj.html

================================================================================
来源：http://hz.meibo888.top/gthyemwcvg.html

[B01] 条件判断 if / else
来源：http://hz.shanyushiyangkeji.top/gtljsjyolf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cashguo.top/gtscujsnfl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yj20258.top/gttsfjribd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.316326.xyz/gttxbnuoxo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gtisetuadf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtbpyugsfe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yuxming.cn/gtmaejyztm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gotoacloud.top/gtftojcxyr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gttylvikui.html

[B02] 多分支 else if / elif
来源：http://hz.fengsongda.top/gtuxgwaxle.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.tanke756.top/gtivnvjyuw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.pengpengdd.cyou/gtzknvrpvp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gtrincxsrg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtxvvdduwr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhaomingkeji.xyz/gteldxewoh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.andypj.xyz/gtwmltkqsh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jlsjyb.cn/gtydylxipk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangshuangyany.cn/gthtttnssy.html

[B03] switch / match / case
来源：http://hz.yuanzhike.top/gtroihrvsk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.c1oappe.top/gtngmiygwg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shanyushiyangtech.top/gtxjqipvay.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258.top/gtprvklvxj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.guannengcc.top/gthpslzfbq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sxryk.cn/gttnwsqywf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ehwqpu.com/gtovyegweo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.guowangkeji.top/gtnlehvenr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.haohaochexian.top/gtsvzvkcsj.html

[B04] for 计数循环
来源：http://hz.shzxlz.cn/gtcdjgeqzt.html

Py:   for i in range(10): print(i)
来源：http://hz.nanxuanxn.top/gtrxgmpltl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.chenlongwang.top/gtiydxekae.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ywan-chungtsiang.top/gtvfexuzxl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuanzx.com/gtuafbawlu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ybcxt.top/gtcogogpwc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhijiandao.cn/gtefzsxzkt.html

Ruby: 10.times { |i| puts i }
来源：http://hz.pengpengdd.cyou/gtgppdkpcv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yangfankeji.com/gteupcevyg.html

[B05] 遍历数组 / 列表
来源：http://hz.gotoacloud.top/gtzkksyngg.html

Py:   for item in arr: print(item)
来源：http://hz.zhaomingkeji.xyz/gtxjdokuaa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hongshengwenyu.top/gtzphavgqs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.daxiang520.top/gtvavpajvv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.iojbl.cn/gtbftzdwaq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ybcxt.top/gtctkjsgjv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shangyingyoupin.top/gtxvrddwsn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.iojbl.cn/gtajdxmnht.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.chenjidiqi.icu/gtreisrhlx.html

[B06] 遍历字典 / 对象
来源：http://hz.yueranfly.top/gtvstsoecg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.quarkkingdee.top/gtmoxmqrdb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gzhubu.top/gtzwqwzwya.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.quarkkingdee.top/gtoeukyfxw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhongyouzk.top/gtelodtkxv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtmxotfjkp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.snrcjt.cn/gthxkqkgrb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.quarkkingdee.top/gtpaircers.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ivvv.top/gtqwlkssti.html

[B07] while 循环
来源：http://hz.hnqzz.top/gtubpzfiah.html

Py:   while i < 10: i += 1
来源：http://hz.quarkkingdee.top/gtqmcopfwe.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cdnleiting.top/gtvbwoxmkl.html

JS:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gtxfzzsvfg.html

TS:   while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtbcucdyxb.html

Java: while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtalfugfka.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.svipenyu.cn/gtdujlhaoe.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtzvvuqmfr.html

C#:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtgiaotsmk.html

[B08] do-while（至少执行一次）
来源：http://hz.aibaodan.cn/gtietqlpei.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shzxlz.cn/gtfpvrdbhs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.snrcjt.cn/gtjnegehqa.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtbjolaffo.html

TS:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtwjpfxdja.html

Java: do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gttynwxcwt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.dashuyun.cn/gtfhfgjuso.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.guowangkeji.top/gtdcczjzod.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gteyqqoxyn.html

[B09] break 与 continue
来源：http://hz.smart0.xyz/gtwxwkyugn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yvedp.cn/gtacowkwox.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.daria6918.cn/gtkljagweg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtxcyyyvvb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtotvbyqkq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtdvxhhktw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ivvv.top/gtpvgdeopd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yuanzhike.top/gtnrsavmln.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtckcsuyqy.html

[B10] 遍历同时拿索引
来源：http://hz.9152youxi.cn/gtxvkqilen.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ydzc1.top/gtfedsjmup.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sufxvd.cn/gtbbgxcgsr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.meibo888.top/gtdjqfvbhz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yuanzhike.top/gtbyculvmq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.feifeiyinyue.top/gtbjvqwygy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pengpengdd.cyou/gtnxvmvqqk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.dashuyun.cn/gtdbmndzsv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.vqdsnc.cn/gtnaangosc.html

[B11] 生成数字序列 / 区间
来源：http://hz.gzhubu.top/gtvmdsffwm.html

Py:   list(range(0, 10, 2))
来源：http://hz.haohaochexian.top/gtbnrqmxae.html

PHP:  range(0, 10, 2);
来源：http://hz.xylfe.cn/gtzolhauvj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shzxlz.cn/gtvpkdaaad.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtojysymqg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yj202588.top/gtlttkadab.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ppjwa.cn/gtcrughoeq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tianlin.xyz/gtuovtdpuf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhiwuduotai.top/gtzshgozdh.html

[B12] 跳出多层循环
来源：http://hz.zhijiandao.cn/gtizjjgwri.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hongshengwenyu.top/gttmfsszfr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sxryk.cn/gtrhybnmga.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangkeji.top/gtkagjnnmw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtofpveofc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtjipxbmak.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yangfankeji.com/gtcftnyvyc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.52xcode.cn/gteesatevk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cdnleiting.top/gtvqtlnwic.html

[B13] 判断是否为数字
来源：http://hz.daria6918.cn/gtjksjtyxz.html

Py:   isinstance(x, (int, float))
来源：http://hz.svipenyu.cn/gtzjvqhdin.html

PHP:  is_numeric($x)
来源：http://hz.wangshuangyany.cn/gtqpydoepq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtkswwipcr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gtzwdzzjuc.html

Java: x instanceof Number
来源：http://hz.zhijiandao.cn/gtsrpyfjsu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.pengpengdd.cyou/gtbyjnabnq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nanxinkj.top/gtshfyhjlr.html

C#:   x is int or double or decimal
来源：http://hz.zhongyouzk.top/gtywuzakkw.html

[B14] 判断值是否在集合内
来源：http://hz.zhoulong.xyz/gtlmbcakyj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yj20258.top/gtipyftzsi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhijiandao.cn/gtgaxcacey.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.aibaodan.cn/gtnfopswtv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yuanzhike.top/gtqhtztpac.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.haohaochexian.top/gtmrowglct.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yvedp.cn/gtszpilxew.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.birdmap.top/gtxfgnlpqs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtybtyvhvb.html

[B15] 布尔运算与取反
来源：http://hz.havefunace.top/gtlxpstdnx.html

Py:   a and b or not c
来源：http://hz.jqgfzy.top/gteqeebznf.html

PHP:  $a && $b || !$c
来源：http://hz.redwolf501.top/gtnxghteyi.html

JS:   a && b || !c
来源：http://hz.316326.xyz/gtuwusylns.html

TS:   a && b || !c
来源：http://hz.zdqjudy.top/gtmedayquo.html

Java: a && b || !c
来源：http://hz.tian-w.cn/gtrkirxmkb.html

Go:   a && b || !c
来源：http://hz.gogol.net.cn/gtrtqxtyln.html

Ruby: a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtwwobldme.html

C#:   a && b || !c
来源：http://hz.tanke756.top/gtxckvnfnw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yueranfly.top/gttyhtydsq.html

Py:   if not data: return
来源：http://hz.zhijiandao.cn/gtgcfbqatu.html

PHP:  if (!$data) { return; }
来源：http://hz.9152youxi.cn/gtabteyfvx.html

JS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gtshieyjoy.html

TS:   if (!data) return;
来源：http://hz.yonumen.top/gtqgghhgor.html

Java: if (data == null) return;
来源：http://hz.52xcode.cn/gtnkpcyimh.html

Go:   if data == nil { return }
来源：http://hz.zhiwuduotai.top/gtgadnfcen.html

Ruby: return if data.nil?
来源：http://hz.dashuyun.cn/gtrplwhbdf.html

C#:   if (data == null) return;
来源：http://hz.0kj1m.cn/gtcvryzvqt.html

================================================================================
来源：http://hz.yj20258.top/gtqgawvbaa.html

C. 函数与作用域
来源：http://hz.hfpthk.cn/gtvxvucfrz.html

================================================================================
来源：http://hz.yonumen.top/gtcnubcopm.html

[C01] 定义函数
来源：http://hz.sweek.top/gtregfnweb.html

Py:   def add(a, b): return a + b
来源：http://hz.zycfv.cn/gtxkcxuqfu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtlhwqcqrv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yangfankeji.com/gtugzgasco.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtplybwrkm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtinnvpabv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgfzy.top/gtetbcxepp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhongyouzk.top/gtgxpyiyen.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtuasbervr.html

[C02] 默认参数
来源：http://hz.cdnleiting.top/gtltxzmfhv.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtecyyyoeb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258888.top/gtmtdkcrrc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.daria6918.cn/gtgzqlabco.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.316326.xyz/gtdtusvtfc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangshuangyany.cn/gtczozhcdp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhaomingkeji.xyz/gtpvlbphql.html

Ruby: def greet(name = "World") = name
来源：http://hz.zdqjudy.top/gtveviiqbo.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guowangkeji.top/gtztnbcdan.html

[C03] 可变参数
来源：http://hz.yj20258.top/gtpyjvleya.html

Py:   def total(*args): return sum(args)
来源：http://hz.bjfxy.top/gthgnvlygw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jlsjyb.cn/gtdadrtijj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtualtdbtx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtjjazrurv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.316326.xyz/gtmvuexhot.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.haohaochexian.top/gtuaonlrct.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigfzy.top/gtpobisuih.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gtivdtdncg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hysaishi.cn/gtfkycroot.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gaohongyu789.top/gtoocjfbip.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinqigufen.top/gtrpbwlyyk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gzhubu.top/gtqcfxazed.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yanxiufei.cn/gtkbezmovb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ybcxt.top/gtkaixxbmn.html

Go:   // 无：用配置结构体参数
来源：http://hz.andypj.xyz/gtwmpqtwvl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.smart0.xyz/gteqriiqpk.html

C#:   f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtvtjwudne.html

[C05] 返回多个值
来源：http://hz.cdnleiting.top/gttdmdwqrb.html

Py:   return a, b
来源：http://hz.zhongyouzk.top/gtenlcaxay.html

PHP:  return [$a, $b];
来源：http://hz.ybcxt.top/gtzbwzikkd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.bjfxy.top/gtmupgqxem.html

TS:   return { a, b };
来源：http://hz.nanxuanxn.top/gtobaqcwnf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.9152youxi.cn/gtpruaetjb.html

Go:   return a, b
来源：http://hz.hnqzz.top/gtntdugkai.html

Ruby: return a, b
来源：http://hz.chenlongwang.top/gtzmtdtymh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.52xcode.cn/gtdyzwahds.html

[C06] 匿名函数 / lambda
来源：http://hz.0kj1m.cn/gtpexuhnhs.html

Py:   square = lambda x: x * x
来源：http://hz.sufxvd.cn/gtpkmtynrk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhoulong.xyz/gtyasnbrqf.html

JS:   const square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtyoueropd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.guowangkeji.top/gtawgxekqy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.52xcode.cn/gtqpvwapgb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenjidiqi.icu/gthifzjtil.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xinyue.icu/gtbzflimyq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ydjk.org.cn/gtlxfhcotk.html

[C07] 把函数作为参数传入
来源：http://hz.dashuyun.cn/gtgzeyhxaj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.wangdashe.top/gtuqxznhgw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj202588.top/gthmbncbnv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.iojbl.cn/gtrtjoqoty.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtlxrfiaai.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhijiandao.cn/gtwdoqccyx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.nanxinkj.top/gtbkxbnnrc.html

Ruby: arr.map(&:upcase)
来源：http://hz.jqgufenzy.top/gtcjqeotvb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gotoacloud.top/gthognuwdm.html

[C08] 闭包
来源：http://hz.xziqi.cn/gtcqcdiznm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhongyouzk.top/gtgkrtmxdu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.feifeiyinyue.top/gtqyggoqla.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtzqsrrrmx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.fengsongda.top/gtkdwmajxc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aibaodan.cn/gtsqbexpbp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gotoacloud.top/gtbnonhlcp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aibaodan.cn/gtoricgsyc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.feifeiyinyue.top/gtmwmmpyig.html

[C09] 递归
来源：http://hz.jiagoushi.top/gtbqfxcfmh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gtagondfgp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ydzc1.top/gtuwhwmnhg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gttulhilzr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtsoanhmfp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.aizwys.cn/gtfokqlfps.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuanzx.com/gtwaqgdvon.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtlmoukblx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenjidiqi.icu/gtvxjyqpsk.html

[C10] 变量作用域
来源：http://hz.dashuyun.cn/gtahvvimbp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.birdmap.top/gtgxykkvif.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hfpthk.cn/gtmjhlmetg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtwoqdfegv.html

TS:   同 JS
来源：http://hz.xuetiantiany.cn/gtkxirwcdg.html

Java: 方法内为块级作用域
来源：http://hz.ydjk.org.cn/gtztsufgxj.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtajmivpdv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.birdmap.top/gtdlwymtie.html

C#:   块级作用域
来源：http://hz.ehwqpu.com/gtlfrxrcwq.html

[C11] 模块导入与导出
来源：http://hz.ywan-chungtsiang.top/gtiburonci.html

Py:   from module import func
来源：http://hz.mhx1999.top/gtdgzvtrww.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ywan-chungtsiang.top/gtycjejrob.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yj202588.top/gtqublncnv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydjk.org.cn/gtiiacgull.html

Java: import java.util.List;
来源：http://hz.xuetiantiany.cn/gtmnodgnvx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jiagoushi.top/gtlamxqrii.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yonumen.top/gttofeaast.html

C#:   using System.Text;
来源：http://hz.hnxiangtu.top/gtxutwyale.html

[C12] 立即执行函数 IIFE
来源：http://hz.316326.xyz/gtfwabuenu.html

Py:   (lambda: print("run"))()
来源：http://hz.sxryk.cn/gtlrowowpw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangkeji.top/gtyvvohhqx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtpkrtqrud.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtiwpcpznv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yonumen.top/gtspsbqwko.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hammf.cn/gtogiknfcz.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhijiandao.cn/gtanblljvf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.svipenyu.cn/gtkutkybco.html

[C13] 类型声明 / 类型注解
来源：http://hz.shzxlz.cn/gtmeucgutv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yj20258888.top/gtcytcbhpc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtyikdwhnx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tanke756.top/gtwwvuvexf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.vqdsnc.cn/gtronkyhyl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtabdlcmod.html

Go:   func add(a, b int) int
来源：http://hz.9152youxi.cn/gtrdmutgxg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.aibaodan.cn/gtoohssxoz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dashuyun.cn/gtbletqsyw.html

[C14] 泛型函数
来源：http://hz.tianlin.xyz/gtdfcaasdg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xziqi.cn/gtfyrwwzeo.html

PHP:  // 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtsajsnpod.html

JS:   // 无泛型
来源：http://hz.shuidangran.top/gtylqtpgnx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.andypj.xyz/gtnzfphdis.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ehwqpu.com/gtfnsqcsqp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shanyushiyangkeji.top/gtplvjmmgo.html

Ruby: # 无泛型
来源：http://hz.quarkkingdee.top/gtfxnvlvro.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuxming.cn/gtdqzxsjbf.html

[C15] 解构 / 展开参数
来源：http://hz.nwbrower.top/gtzwawjijx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jinqigfzy.top/gtqjcukfnp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj20258888.top/gtfljzsmgv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jianghu66.top/gtvcxbykwf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.kuanghao11.cn/gtxojzpqln.html

Java: // 无解构
来源：http://hz.jlsjyb.cn/gtzngcseiv.html

Go:   // 无解构
来源：http://hz.hysaishi.cn/gtywqjwqgp.html


<!-- 参考信息 -->