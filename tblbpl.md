代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jinqigufen.top/gtxszbjrka.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gtxbkebjti.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinqigfzy.top/gtjfqwxfps.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ybcxt.top/gtzuwuvjct.html

[A26] 类型转换总览
来源：http://hz.yvedp.cn/gttpijuhsp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shanyushiyangtech.top/gtszrxqlcs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ydzc1.top/gtfwiwcwib.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.smart0.xyz/gtxtyxwvgl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cashguo.top/gtxdgjkinz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yj202588.top/gtjygukxsh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.vqdsnc.cn/gthqzddvec.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ywan-chungtsiang.top/gtyjkuezqy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.aibaodan.cn/gttfkbmbty.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqkeybopy.html

B. 流程控制
来源：http://hz.hysaishi.cn/gtinvczwjm.html

================================================================================
来源：http://hz.gaohongyu789.top/gthbdepicc.html

[B01] 条件判断 if / else
来源：http://hz.shanyushiyangkeji.top/gtldnpnfxv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinghuilouyu.cn/gtidinixyj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tian-w.cn/gthzycmltf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xingfuxueyuan.xyz/gtldaijsli.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.dashuyun.cn/gtwuasywvn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ydjk.org.cn/gtvqbbvpbp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.316326.xyz/gtfieslksd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jinghuilouyu.cn/gtbxezgqnv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.iojbl.cn/gthmznbqrc.html

[B02] 多分支 else if / elif
来源：http://hz.cucudq.cn/gtsuhnvxjg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shanyushiyangtech.top/gtgdcnmocy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yvedp.cn/gtqdgxtakd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtpgapjwng.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangtech.top/gtbgvyhqhy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gtounnpsdr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sweek.top/gtqsuwzkea.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.nanxuanxn.top/gtwhnwdjxz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtphdkfddf.html

[B03] switch / match / case
来源：http://hz.cdnleiting.top/gtrsljfevs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hywenlv.cn/gtadkykniu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ydjk.org.cn/gtesrpdgsg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jyoumei.cn/gtijubweoe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258888.top/gtviqrzqbr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.xziqi.cn/gtrbwkevek.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.xuetiantiany.cn/gttqhjcwwo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.fengsongda.top/gtbwawlaek.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yongpay.top/gtvsoeaphx.html

[B04] for 计数循环
来源：http://hz.andypj.xyz/gthbkznjin.html

Py:   for i in range(10): print(i)
来源：http://hz.meibo888.top/gtmbrkltmd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cqqwz.cn/gtbjzddynv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xziqi.cn/gtjzidsdhk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cheryme.top/gtqqpxgyid.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jqgufenzy.top/gtvputyasy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.svipenyu.cn/gtolqopgsb.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jinghuilouyu.cn/gtckyyeslj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jqgufenzy.top/gtkmhzpwrp.html

[B05] 遍历数组 / 列表
来源：http://hz.xylfe.cn/gtpwgxuklg.html

Py:   for item in arr: print(item)
来源：http://hz.feifeiyinyue.top/gtagttgpqy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hammf.cn/gtjzucuosn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ywan-chungtsiang.top/gtphxsamzh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj20258.top/gtqqhxwsnu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.feifeiyinyue.top/gtgargqxmy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnxiangtu.top/gtzdpkpeix.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yuanzhike.top/gtgnciqxvt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hysaishi.cn/gtdsglfvaq.html

[B06] 遍历字典 / 对象
来源：http://hz.jiagoushi.top/gtuynwsvjt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.chenzaomai.com/gtywgebzji.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yongpay.top/gtiubgbbqr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.iojbl.cn/gttxusfrfk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nanxinkj.top/gtgxtrtvrm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.chenlongwang.top/gtkkjyiwse.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nanxinkj.top/gtzemrboxj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zdqjudy.top/gtcoqenmfj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hnxiangtu.top/gtsmlzndlz.html

[B07] while 循环
来源：http://hz.jinghuilouyu.cn/gttrabiaeg.html

Py:   while i < 10: i += 1
来源：http://hz.ppjwa.cn/gtrdmvbuxo.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.redwolf501.top/gtpxerlljh.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhoulong.xyz/gticfzuwji.html

TS:   while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtmbtmjzcd.html

Java: while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtndikqdry.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhiwuduotai.top/gtmwkgnmxp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ehwqpu.com/gtcbyarobf.html

C#:   while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtohkckgsm.html

[B08] do-while（至少执行一次）
来源：http://hz.shanyushiyangkeji.top/gtxgbqiyjg.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.pycfn.com/gtiblcrmii.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258888.top/gtlvowtfbh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtemrhjqkk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtfbcdsfzz.html

Java: do { i++; } while (i < 10);
来源：http://hz.shangyingyoupin.top/gtheqxrvtt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.0kj1m.cn/gtlvhntbqg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.dashuyun.cn/gtwbdqwdwb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtgislixzh.html

[B09] break 与 continue
来源：http://hz.cucudq.cn/gtwfmujkpd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pycfn.com/gteiqakoqn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtowbuveoq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtqqwmiusz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtxcdwmbkj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtbrmcajga.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.andypj.xyz/gtzpwuwxjh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hnqzz.top/gtsmtjezzs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtkpguemlq.html

[B10] 遍历同时拿索引
来源：http://hz.sufxvd.cn/gtrwetiahy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jlsjyb.cn/gtetbosuqr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.andypj.xyz/gttbzfidli.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yvedp.cn/gtufeuhhnz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.c1oappe.top/gtjljgafoy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.pycfn.com/gttjyujmka.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yangfankeji.com/gtnbkjollx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yuxming.cn/gtyznemywo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.gogol.net.cn/gtkghriqtn.html

[B11] 生成数字序列 / 区间
来源：http://hz.ehwqpu.com/gtdamemkit.html

Py:   list(range(0, 10, 2))
来源：http://hz.tianlin.xyz/gtbyluiaqe.html

PHP:  range(0, 10, 2);
来源：http://hz.jinghuilouyu.cn/gtgecrniqp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gtkezwelyl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.nwbrower.top/gtfndyhqwk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenzaomai.com/gtdfudinok.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cdnleiting.top/gtvtvncvqd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhengqikj.top/gtvclclzug.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ivvv.top/gtotvwarfk.html

[B12] 跳出多层循环
来源：http://hz.jqgufenzy.top/gtnputlrnp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hnqzz.top/gtxqdqnumd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.0kj1m.cn/gtiigajilq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtjbzenuhi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sysykeji.top/gtzsmnupli.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtyemxmloi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258.top/gtebjkvkyt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.quarkkingdee.top/gtrxvlsmow.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.iojbl.cn/gtcdrdajuy.html

[B13] 判断是否为数字
来源：http://hz.jqgufenzy.top/gtqcphtvwm.html

Py:   isinstance(x, (int, float))
来源：http://hz.yueranfly.top/gtoidfimvp.html

PHP:  is_numeric($x)
来源：http://hz.quarkkingdee.top/gtbuqzpihm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yanxiufei.cn/gtfeuirikf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtgfndpkcg.html

Java: x instanceof Number
来源：http://hz.jlsjyb.cn/gtfitehmxs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gzhubu.top/gtwhjmsece.html

Ruby: x.is_a?(Numeric)
来源：http://hz.iojbl.cn/gtftqpalce.html

C#:   x is int or double or decimal
来源：http://hz.52xcode.cn/gtjneckgzd.html

[B14] 判断值是否在集合内
来源：http://hz.yangfankeji.com/gtyzauicgz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.bjfxy.top/gttyfkoflh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.feifeiyinyue.top/gtosvmcska.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gtodbisfxn.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtqchckgsv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tianlin.xyz/gtzplwlrbn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.bjfxy.top/gtghxsyrnu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nwbrower.top/gtlbevbipn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aizwys.cn/gthwwjsjgu.html

[B15] 布尔运算与取反
来源：http://hz.meibo888.top/gtpklginvo.html

Py:   a and b or not c
来源：http://hz.sysykeji.top/gtfgonqltc.html

PHP:  $a && $b || !$c
来源：http://hz.ybcxt.top/gtcmyiyyib.html

JS:   a && b || !c
来源：http://hz.sysykeji.top/gtqgbwmcko.html

TS:   a && b || !c
来源：http://hz.bjfxy.top/gtczremogt.html

Java: a && b || !c
来源：http://hz.dianchejie.cn/gtlzemlbzv.html

Go:   a && b || !c
来源：http://hz.hnxiangtu.top/gtpjwgapta.html

Ruby: a && b || !c
来源：http://hz.yj20258.top/gtfeuszcjr.html

C#:   a && b || !c
来源：http://hz.nanxinkj.top/gtvdjnlthk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gteuxqrptv.html

Py:   if not data: return
来源：http://hz.sweek.top/gtaoyzoqav.html

PHP:  if (!$data) { return; }
来源：http://hz.andypj.xyz/gtmudvtoaw.html

JS:   if (!data) return;
来源：http://hz.jlsjyb.cn/gtvummizuj.html

TS:   if (!data) return;
来源：http://hz.hnqzz.top/gtbncddyzv.html

Java: if (data == null) return;
来源：http://hz.dashuyun.cn/gtgijlafld.html

Go:   if data == nil { return }
来源：http://hz.yangfankeji.com/gtttyplvpz.html

Ruby: return if data.nil?
来源：http://hz.ppjwa.cn/gtoqblciyk.html

C#:   if (data == null) return;
来源：http://hz.9152youxi.cn/gterbyjfud.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthkqcpzcn.html

C. 函数与作用域
来源：http://hz.snrcjt.cn/gtmkjqjjaf.html

================================================================================
来源：http://hz.fzhhl.top/gtjjzebpes.html

[C01] 定义函数
来源：http://hz.yj20258.top/gtvzlsmvpw.html

Py:   def add(a, b): return a + b
来源：http://hz.yuanzhike.top/gtqefkmvlh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtpbsarkwl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cdnleiting.top/gtjbeqzeye.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtbjtlycdy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtvqsoxnpq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ivvv.top/gtuzsudtsj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yuxming.cn/gtryjzjrsk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtnajzalgk.html

[C02] 默认参数
来源：http://hz.zhiwuduotai.top/gtdoiituyy.html

Py:   def greet(name="World"): return name
来源：http://hz.ehwqpu.com/gtqbszfskz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zdqjudy.top/gtafibytki.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtztewicxk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenlongwang.top/gtpavdssna.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sweek.top/gthsuozbtn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gzhubu.top/gtrwdyiqlw.html

Ruby: def greet(name = "World") = name
来源：http://hz.jlsjyb.cn/gtjffayjtf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangkeji.top/gtmsmxoguu.html

[C03] 可变参数
来源：http://hz.ppjwa.cn/gttzxtvyri.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydzc1.top/gtrlasjkcl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhixingplan.top/gteqfnlagd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhoulong.xyz/gtmgrcmygn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtgzdtmrhs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.vqdsnc.cn/gtojynoidi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cashguo.top/gtfpadqsjg.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pycfn.com/gtqsvhsgyv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yj20258888.top/gtnxdxacfx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dashuyun.cn/gtewqqdaaw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenjidiqi.icu/gtiesbribv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tanke756.top/gtnizudnsb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtjntdjeae.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hysaishi.cn/gtarvwtrva.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhengqikj.top/gtyhrxmgtk.html

Go:   // 无：用配置结构体参数
来源：http://hz.ywan-chungtsiang.top/gtiwzpdsjo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ywan-chungtsiang.top/gtrpdutrtt.html

C#:   f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtxaczqgtq.html

[C05] 返回多个值
来源：http://hz.zhixingplan.top/gthhokmeqy.html

Py:   return a, b
来源：http://hz.jlsjyb.cn/gtnwfibqzw.html

PHP:  return [$a, $b];
来源：http://hz.zhiwuduotai.top/gtzzeqqstj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.bjfxy.top/gtdqayqbwo.html

TS:   return { a, b };
来源：http://hz.dianchejie.cn/gtajqasquz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxinkj.top/gtjqqzcupo.html

Go:   return a, b
来源：http://hz.9152youxi.cn/gtwehxztgf.html

Ruby: return a, b
来源：http://hz.chenzaomai.com/gtouwdytmw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hongshengwenyu.top/gteylblmrh.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gtetsuffvv.html

Py:   square = lambda x: x * x
来源：http://hz.ydjk.org.cn/gtchinpgyc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhiwuduotai.top/gtwxjceleh.html

JS:   const square = x => x * x;
来源：http://hz.xziqi.cn/gtyfnubskf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ydzc1.top/gtpnnfyqgf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cheryme.top/gteukpoaat.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ppjwa.cn/gtvkhfydev.html

Ruby: square = ->(x) { x * x }
来源：http://hz.dianchejie.cn/gtqqesmjfz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xinyue.icu/gtwjteroih.html

[C07] 把函数作为参数传入
来源：http://hz.gotoacloud.top/gtirmocqww.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daria6918.cn/gtylevspny.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj20258888.top/gtppgdovxu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.316326.xyz/gtvaakamnh.html

TS:   arr.map(String)
来源：http://hz.316326.xyz/gtjozxhswh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.c1oappe.top/gtjfggiawz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hfpthk.cn/gtsgqseuzn.html

Ruby: arr.map(&:upcase)
来源：http://hz.birdmap.top/gtgrbqxvdr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sufxvd.cn/gtqjkultbm.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtxavxqsdv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.c1oappe.top/gtjyrlcpew.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shzxlz.cn/gtqzrnswud.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtcsgtdlse.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.daxiang520.top/gtcldfthem.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cdnleiting.top/gtwjujfqet.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gotoacloud.top/gtunhudnfa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daxiang520.top/gtnyiciqsq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhijiandao.cn/gtwoyfnfnv.html

[C09] 递归
来源：http://hz.gotoacloud.top/gtlyfxficz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hywenlv.cn/gtaeojgwxt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ywan-chungtsiang.top/gtirmccyus.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jiagoushi.top/gthabeiesa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtgtllvnud.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yonumen.top/gthnccijst.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.9152youxi.cn/gtmhvvfiez.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tanke756.top/gtswutlsoi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yanxiufei.cn/gtxuaplrfl.html

[C10] 变量作用域
来源：http://hz.vqdsnc.cn/gtbwckjmjo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yueranfly.top/gtupmqicxh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xingfuxueyuan.xyz/gtnnyuovlk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jinqigufen.top/gthccvpgns.html

TS:   同 JS
来源：http://hz.316326.xyz/gtiyzpijcm.html

Java: 方法内为块级作用域
来源：http://hz.ydjk.org.cn/gtjkqeakoy.html

Go:   花括号块级作用域
来源：http://hz.jyoumei.cn/gtljkqfpar.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xingfuxueyuan.xyz/gtjepspwae.html

C#:   块级作用域
来源：http://hz.xinyue.icu/gtjpqmjhll.html

[C11] 模块导入与导出
来源：http://hz.haohaochexian.top/gtdmytgdhi.html

Py:   from module import func
来源：http://hz.xuetiantiany.cn/gtwwztugsz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhiwuduotai.top/gtwosmbbjh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jiagoushi.top/gtkcivfvrd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.0kj1m.cn/gtudrgrzop.html

Java: import java.util.List;
来源：http://hz.cashguo.top/gtxziwbzjs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydjk.org.cn/gtmcilmzkm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuxming.cn/gtsteflmvu.html

C#:   using System.Text;
来源：http://hz.bjfxy.top/gtjgqlsbpp.html

[C12] 立即执行函数 IIFE
来源：http://hz.wangdashe.top/gtwntuhycy.html

Py:   (lambda: print("run"))()
来源：http://hz.ydzc1.top/gtbzqebsku.html

PHP:  (function () { echo "run"; })();
来源：http://hz.wangshuangyany.cn/gtzbhecqhn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shuidangran.top/gtgyubhlne.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtnrysiszf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xingfuxueyuan.xyz/gtluqblbie.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cucudq.cn/gtvjykmusf.html

Ruby: -> { puts "run" }.call
来源：http://hz.ehwqpu.com/gtzaporlxn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tanke756.top/gtfdkwpdhm.html

[C13] 类型声明 / 类型注解
来源：http://hz.tian-w.cn/gtlxtxsbmw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hammf.cn/gtclxrqqgv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtpevmfjzt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.andypj.xyz/gtfxcxpssh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenzaomai.com/gtbzguoqqw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gttbesqfdc.html

Go:   func add(a, b int) int
来源：http://hz.jinyuanbaomall.cn/gtbwfvwmqu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cqqwz.cn/gtalcjzymc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guowangkeji.top/gtdkjtvmxv.html

[C14] 泛型函数
来源：http://hz.jinghuilouyu.cn/gtwcmtoljq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.daria6918.cn/gtesncbyug.html

PHP:  // 无泛型
来源：http://hz.yuxming.cn/gtjivkmhpk.html

JS:   // 无泛型
来源：http://hz.ppjwa.cn/gtsoqkwtcc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhongyouzk.top/gtxdrlxsyo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shzxlz.cn/gtoioeaaii.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jlsjyb.cn/gtwiecpmqe.html

Ruby: # 无泛型
来源：http://hz.shanyushiyangkeji.top/gtpzddptub.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jlsjyb.cn/gtjbqgqkex.html

[C15] 解构 / 展开参数
来源：http://hz.daxiang520.top/gtyvpzfhgp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.jianghu66.top/gtqrgekjob.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yueranfly.top/gthpreymft.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtuagrnhru.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cdnleiting.top/gtvsqjajfc.html

Java: // 无解构
来源：http://hz.haohaochexian.top/gtrqmcnrai.html

Go:   // 无解构
来源：http://hz.feifeiyinyue.top/gtbbakpsbi.html

Ruby: a, b = pair
来源：http://hz.bjfxy.top/gtpsxnkhxw.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gthceqbwrz.html

[C16] 函数 / 方法重载
来源：http://hz.9152youxi.cn/gtjkcukmqw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.andypj.xyz/gtqcqlnfju.html


<!-- 参考信息 -->