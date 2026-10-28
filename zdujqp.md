代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.chenjidiqi.icu/gtgreqpclk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.redwolf501.top/gtitisqrqw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.daxiang520.top/gttrrzuajm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhixingplan.top/gtcukwgyjc.html

[A26] 类型转换总览
来源：http://hz.ywan-chungtsiang.top/gtiaveqhcz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yuxming.cn/gtmmovfrzx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.vqdsnc.cn/gtrqtlqoqm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yueranfly.top/gtgzpfzfoc.html

TS:   Number() String() Boolean() x as number
来源：http://hz.0kj1m.cn/gtuvfaffch.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.wangshuangyany.cn/gtumhmghtg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yangfankeji.com/gtuhvnhrea.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.feifeiyinyue.top/gtfjumvods.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xingfuxueyuan.xyz/gtcfcimimu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtnbovqnep.html

B. 流程控制
来源：http://hz.wangdashe.top/gtzzqgkkil.html

================================================================================
来源：http://hz.wangdashe.top/gtvsnybyph.html

[B01] 条件判断 if / else
来源：http://hz.vqdsnc.cn/gthkrlrqpf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shangyingyoupin.top/gtubuqzczq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ppjwa.cn/gtexynnbdu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sysykeji.top/gtqdxqwkkh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gttpupufxy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtkfxfvimy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ydjk.org.cn/gtebrivifn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yangfankeji.com/gtnketsjpm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.mhx1999.top/gtsorvfdjs.html

[B02] 多分支 else if / elif
来源：http://hz.birdmap.top/gtnrlxgxcd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hammf.cn/gtdtruslhd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhixingplan.top/gteqvcxwvk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aibaodan.cn/gthsgfgvod.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtadohzalv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtprhrlglk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.cqqwz.cn/gtcygmpnar.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.shangyingyoupin.top/gtcdjeknlg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgufenzy.top/gtrfarzrqi.html

[B03] switch / match / case
来源：http://hz.zhixingplan.top/gtamcfinlh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258.top/gtgnohtsuu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jqgufenzy.top/gtgejoconp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhiwuduotai.top/gtulvkslne.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhijiandao.cn/gtpxkxaslv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.316326.xyz/gtligapapx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cucudq.cn/gtxgophymb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.smart0.xyz/gtazhesnsn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hysaishi.cn/gtsastfsmr.html

[B04] for 计数循环
来源：http://hz.shanyushiyangkeji.top/gtzxuzwzdp.html

Py:   for i in range(10): print(i)
来源：http://hz.iojbl.cn/gttmhkktuc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.c1oappe.top/gtbsqihcnb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zdqjudy.top/gtlcvnqpua.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.dashuyun.cn/gtpdneibls.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hnxiangtu.top/gtkacbuaay.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jyoumei.cn/gtljjxfbol.html

Ruby: 10.times { |i| puts i }
来源：http://hz.c1oappe.top/gtvevhxgah.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.dianchejie.cn/gtlhlgwpie.html

[B05] 遍历数组 / 列表
来源：http://hz.daxiang520.top/gtereqhzsg.html

Py:   for item in arr: print(item)
来源：http://hz.yj20258888.top/gtlxomsxjk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.dashuyun.cn/gtesnpjdbz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.gogol.net.cn/gtrqdcucyd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.daxiang520.top/gtbhqvzudm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cashguo.top/gtnikaneuw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guowangkeji.top/gtnswbwfit.html

Ruby: arr.each { |item| puts item }
来源：http://hz.chenzaomai.com/gtmkigvglw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.fengsongda.top/gtqvkidhmy.html

[B06] 遍历字典 / 对象
来源：http://hz.xuetiantiany.cn/gtguciawtw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.316326.xyz/gtlhiofvdo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cashguo.top/gtmbxperkn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yonumen.top/gtysxopkyo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.quarkkingdee.top/gtbgmxdmlm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.nanxinkj.top/gtpdpfgfde.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.cdnleiting.top/gtnuqynmbo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yj202588.top/gtqhcgsdgx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.dashuyun.cn/gtmdwvkgoq.html

[B07] while 循环
来源：http://hz.jyoumei.cn/gtkiznmtai.html

Py:   while i < 10: i += 1
来源：http://hz.hfpthk.cn/gtshfppyxv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.redwolf501.top/gthewjmtaw.html

JS:   while (i < 10) { i++; }
来源：http://hz.316326.xyz/gtdyqrlhth.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtnxsmroyn.html

Java: while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtrwknonzg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.birdmap.top/gtjbsirwti.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yueranfly.top/gtkmvvaecc.html

C#:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtrqrvhois.html

[B08] do-while（至少执行一次）
来源：http://hz.shangyingyoupin.top/gtktrlzrae.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jqgfzy.top/gtxcaxyamx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.dashuyun.cn/gteowbmovo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gtjszihknp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtpnvlyopz.html

Java: do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtpdoztgyu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.meibo888.top/gtgafjzkrg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.shuidangran.top/gtcixhjzpq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtvqflddqr.html

[B09] break 与 continue
来源：http://hz.gzhubu.top/gthtmecewk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hammf.cn/gtxlapablr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gogol.net.cn/gtfvheknzl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtvtrctyuv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtdqidwefz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtdwgzqajp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigufen.top/gtsryoxcac.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gzhubu.top/gtumjuxxyj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtyxzymvws.html

[B10] 遍历同时拿索引
来源：http://hz.havefunace.top/gtnkophgzg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ybcxt.top/gtehmtpnsj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jyoumei.cn/gttbhkijcw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.guowangkeji.top/gtmedoxzfr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.iojbl.cn/gtjkttqeha.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.52xcode.cn/gtxxivisqb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hammf.cn/gtixkzqiwb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.birdmap.top/gtdqffvpss.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigufen.top/gtfzlnqzmt.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhaomingkeji.xyz/gtponefwnc.html

Py:   list(range(0, 10, 2))
来源：http://hz.gogol.net.cn/gtqseivtlp.html

PHP:  range(0, 10, 2);
来源：http://hz.sxryk.cn/gtllkqdgnl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtdwkclfme.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gtbsxhieyl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jiagoushi.top/gtykvqxheo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.iojbl.cn/gtuostgbyc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hnxiangtu.top/gteqygnunm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenlongwang.top/gtysipxekv.html

[B12] 跳出多层循环
来源：http://hz.cdnleiting.top/gtetsswyas.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zycfv.cn/gtfwyfzyln.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gogol.net.cn/gtxxzxaotu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.kuanghao11.cn/gtscjiuejf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.havefunace.top/gtakxnfldr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtwtentjci.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nanxinkj.top/gtwjyoybex.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnqzz.top/gtvrnppycf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shuidangran.top/gtjmnylgmo.html

[B13] 判断是否为数字
来源：http://hz.316326.xyz/gtragmijtd.html

Py:   isinstance(x, (int, float))
来源：http://hz.redwolf501.top/gtytsiokjc.html

PHP:  is_numeric($x)
来源：http://hz.ybcxt.top/gtwcjushqq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.quarkkingdee.top/gtdppeyazo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtmwtqtrdf.html

Java: x instanceof Number
来源：http://hz.ppjwa.cn/gtzktqoqte.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.andypj.xyz/gtonnzdrkh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhijiandao.cn/gtmoyglaft.html

C#:   x is int or double or decimal
来源：http://hz.hfpthk.cn/gtaujnftvu.html

[B14] 判断值是否在集合内
来源：http://hz.nwbrower.top/gtqzzuchkn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenlongwang.top/gtmqxjdsss.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgufenzy.top/gttbhakbzv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtwylyflsq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtuvmazlau.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuxming.cn/gtthhkdoxn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yj20258.top/gtwmzyyitl.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ppjwa.cn/gtksqnkmfe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ppjwa.cn/gtygyfkedc.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangkeji.top/gtzvuprnhg.html

Py:   a and b or not c
来源：http://hz.zhiwuduotai.top/gtrxnhnqzw.html

PHP:  $a && $b || !$c
来源：http://hz.sufxvd.cn/gtkixlbckz.html

JS:   a && b || !c
来源：http://hz.zhongyouzk.top/gttjsfocfh.html

TS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtlobgaexz.html

Java: a && b || !c
来源：http://hz.gotoacloud.top/gtybvppjtq.html

Go:   a && b || !c
来源：http://hz.sweek.top/gtazcscnup.html

Ruby: a && b || !c
来源：http://hz.nwbrower.top/gtjkxgohet.html

C#:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtoecxxlfc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hnxiangtu.top/gtlojiuriv.html

Py:   if not data: return
来源：http://hz.zdqjudy.top/gtgpxhtnyv.html

PHP:  if (!$data) { return; }
来源：http://hz.sufxvd.cn/gtdvvvjaun.html

JS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtjlyoluke.html

TS:   if (!data) return;
来源：http://hz.yongpay.top/gtcdrmmixs.html

Java: if (data == null) return;
来源：http://hz.yongpay.top/gtpavpspuk.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gtfnlisbuf.html

Ruby: return if data.nil?
来源：http://hz.gaohongyu789.top/gtpmnulgen.html

C#:   if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtdxehjdmv.html

================================================================================
来源：http://hz.sxryk.cn/gtmmhuzxfr.html

C. 函数与作用域
来源：http://hz.dashuyun.cn/gtepgowlqa.html

================================================================================
来源：http://hz.nwbrower.top/gteotwcjdn.html

[C01] 定义函数
来源：http://hz.gzhubu.top/gtijvokovr.html

Py:   def add(a, b): return a + b
来源：http://hz.gzhubu.top/gtbbbfabfl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hysaishi.cn/gtfugmhmtc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xuanzx.com/gtuzxzxbzn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtjyemmlrc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtnvagmely.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenjidiqi.icu/gtrzvhkhnc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.fzhhl.top/gteylyiazo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtffhchhkr.html

[C02] 默认参数
来源：http://hz.ivvv.top/gtzzldiptt.html

Py:   def greet(name="World"): return name
来源：http://hz.chenzaomai.com/gthkokbqnb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhixingplan.top/gtfsvljovw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinqigufen.top/gtobptaitj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tanke756.top/gtxcqcnxtf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigfzy.top/gtsmcdzusv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxuanxn.top/gtnvrwkjpr.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gtubzungaw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258888.top/gtgxyaskte.html

[C03] 可变参数
来源：http://hz.quarkkingdee.top/gtnaskpeoo.html

Py:   def total(*args): return sum(args)
来源：http://hz.yonumen.top/gtgmzwcdsp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jyoumei.cn/gtcnuwfxed.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gttrquhtnm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtyxvxfoqe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tianlin.xyz/gtvuhfxjym.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cheryme.top/gtepllkxpq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tanke756.top/gtrentwors.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenzaomai.com/gtgrerbuzg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gaohongyu789.top/gtetyddjap.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tianlin.xyz/gtybatjwnf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yangfankeji.com/gtsigjuwgq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtvzmssdfr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.birdmap.top/gtrjixykjj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.redwolf501.top/gtpgbhlttf.html

Go:   // 无：用配置结构体参数
来源：http://hz.xingfuxueyuan.xyz/gtzwpjxmzg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtxrknpopb.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtogwzytww.html

[C05] 返回多个值
来源：http://hz.yvedp.cn/gtshdhdtey.html

Py:   return a, b
来源：http://hz.yj202588.top/gtrrchmwem.html

PHP:  return [$a, $b];
来源：http://hz.ybcxt.top/gttjsxkfno.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shzxlz.cn/gtbcakftmj.html

TS:   return { a, b };
来源：http://hz.kuanghao11.cn/gtlirmlcao.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.tian-w.cn/gtzyskvwqm.html

Go:   return a, b
来源：http://hz.tanke756.top/gtbsuqzlqu.html

Ruby: return a, b
来源：http://hz.iojbl.cn/gtefgermdr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ybcxt.top/gtxvfifhyy.html

[C06] 匿名函数 / lambda
来源：http://hz.zdqjudy.top/gtcoxigxmm.html

Py:   square = lambda x: x * x
来源：http://hz.daria6918.cn/gtuwduymnk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.feifeiyinyue.top/gtqrhbhpok.html

JS:   const square = x => x * x;
来源：http://hz.ywan-chungtsiang.top/gtxzpfakau.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.316326.xyz/gtpdhkltmk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.vqdsnc.cn/gtkrjzfzhh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aizwys.cn/gtxabobzme.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj202588.top/gtffjzzsrx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenlongwang.top/gtcxrvrzfu.html

[C07] 把函数作为参数传入
来源：http://hz.jinghuilouyu.cn/gtvgislqek.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydjk.org.cn/gtuqedfhmj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yanxiufei.cn/gtfnyvvakj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cdnleiting.top/gtoxhyqkmq.html

TS:   arr.map(String)
来源：http://hz.316326.xyz/gtjdizaphj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtcqymrene.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cashguo.top/gtegufiwdk.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangkeji.top/gtrqhytgak.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnxiangtu.top/gtzpoqodwk.html

[C08] 闭包
来源：http://hz.jqgfzy.top/gtmebcdkvz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yongpay.top/gtmbhkgnlb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hongshengwenyu.top/gtxldhdfgy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtgbgxdsxe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtghqrljyt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigufen.top/gtyfywmviq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.52xcode.cn/gtburyiiqf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.kuanghao11.cn/gtuamlqqoy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtxamfblyg.html

[C09] 递归
来源：http://hz.andypj.xyz/gtxtkulzsv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtphxtvfuo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yonumen.top/gtwowonydv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtdayomrrf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtglptkuzx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gotoacloud.top/gtmfkpwqyp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hongshengwenyu.top/gtehoawkyn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtufdhfnnp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuetiantiany.cn/gtrbosfrqf.html

[C10] 变量作用域
来源：http://hz.dashuyun.cn/gteavybsvy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hongshengwenyu.top/gtspirszqc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hammf.cn/gteyixliio.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.fengsongda.top/gtrgjdnfil.html

TS:   同 JS
来源：http://hz.52xcode.cn/gtuhanyzds.html

Java: 方法内为块级作用域
来源：http://hz.zhixingplan.top/gtupluhujp.html

Go:   花括号块级作用域
来源：http://hz.gzhubu.top/gtumwwrshq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sweek.top/gtwgsysyev.html

C#:   块级作用域
来源：http://hz.chenlongwang.top/gtrltxqchl.html

[C11] 模块导入与导出
来源：http://hz.smart0.xyz/gtmaypysra.html

Py:   from module import func
来源：http://hz.snrcjt.cn/gtgipvxlay.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gtudqjskct.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dianchejie.cn/gtrzfhhorr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenlongwang.top/gtdftocbbs.html

Java: import java.util.List;
来源：http://hz.ydzc1.top/gtzkaxnbre.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinyuanbaomall.cn/gttsydsmtj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fzhhl.top/gtwmbhmtkb.html

C#:   using System.Text;
来源：http://hz.shanyushiyangkeji.top/gtcwtwcoxi.html

[C12] 立即执行函数 IIFE
来源：http://hz.tianlin.xyz/gtyojiwmry.html

Py:   (lambda: print("run"))()
来源：http://hz.yongpay.top/gtyvdmcicg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jiagoushi.top/gtixzkagte.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtdqzurvrq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.9152youxi.cn/gtdurcnyuc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tianlin.xyz/gtuouznsve.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.birdmap.top/gthmwlzben.html

Ruby: -> { puts "run" }.call
来源：http://hz.tianlin.xyz/gtdsufsmav.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nanxuanxn.top/gtwlvnemew.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtsxzzfjrv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zdqjudy.top/gtsgtfinsw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtcygdanzo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenzaomai.com/gtpibdapgm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtlyvmsmbo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtnxwkjjhs.html

Go:   func add(a, b int) int
来源：http://hz.nanxuanxn.top/gtivielktm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guowangkeji.top/gtzkmakfmk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ivvv.top/gtiveoejtn.html

[C14] 泛型函数
来源：http://hz.hnqzz.top/gtbgujblut.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.vqdsnc.cn/gtjcmfcfkk.html

PHP:  // 无泛型
来源：http://hz.xinyue.icu/gtixsyrggi.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtztohjfjd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.kuanghao11.cn/gtpcinqgif.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cqqwz.cn/gtfgdqvkqd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hfpthk.cn/gtgqnjmmwy.html

Ruby: # 无泛型
来源：http://hz.vqdsnc.cn/gtzozukkmq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jlsjyb.cn/gtahvknlhs.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gtpwoxksse.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jyoumei.cn/gtafdkqepr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gaohongyu789.top/gtbmmboemg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dashuyun.cn/gtgvaarkut.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jyoumei.cn/gtsjwslexr.html

Java: // 无解构
来源：http://hz.zdqjudy.top/gtssrhosfl.html

Go:   // 无解构
来源：http://hz.svipenyu.cn/gtmgovtriw.html

Ruby: a, b = pair
来源：http://hz.jianghu66.top/gtwcqlqpbs.html

C#:   var (a, b) = pair;
来源：http://hz.fzhhl.top/gtlqkvpnyc.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtzfrndvev.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pengpengdd.cyou/gtxauzshhp.html


<!-- 参考信息 -->