代发 wailian999

[A26] 类型转换总览
来源：http://hz.jinghuilouyu.cn/gtgjwornka.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.guannengcc.top/gthoeizmki.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zycfv.cn/gtapnmtrty.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jqgfzy.top/gtqqigtbgr.html

TS:   Number() String() Boolean() x as number
来源：http://hz.feifeiyinyue.top/gtjkkotdsc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.gotoacloud.top/gtopbclnqd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.shzxlz.cn/gtunfnobcp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhixingplan.top/gtcihsgdrb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.dianchejie.cn/gtpzoijgty.html

================================================================================
来源：http://hz.chenlongwang.top/gtfamlixbl.html

B. 流程控制
来源：http://hz.gotoacloud.top/gtbdmtlops.html

================================================================================
来源：http://hz.xziqi.cn/gtoahfoqgb.html

[B01] 条件判断 if / else
来源：http://hz.zhongyouzk.top/gtqeatxxll.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinghuilouyu.cn/gtigxbmill.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tanke756.top/gtgvqqbtjb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.mhx1999.top/gtjhgmoyzy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ehwqpu.com/gtutltpuvm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhaomingkeji.xyz/gtmieryleu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jlsjyb.cn/gthrsiupku.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhengqikj.top/gtyzsfstdf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.daria6918.cn/gtxfktdquo.html

[B02] 多分支 else if / elif
来源：http://hz.haohaochexian.top/gtmgxviiqy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gogol.net.cn/gtozkubwza.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jlsjyb.cn/gtzmafyzxp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtayivmqcm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yanxiufei.cn/gtahuzteyl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtjcstfawj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ydjk.org.cn/gtqwycgbir.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.nanxuanxn.top/gtjmeapctm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yonumen.top/gtphorbnhx.html

[B03] switch / match / case
来源：http://hz.mhx1999.top/gtmyifcwua.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jqgufenzy.top/gtwmaefspl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gtbkkyrbrq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtytlftscq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.haohaochexian.top/gtbpkosxrc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.feifeiyinyue.top/gtgpljifqq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.c1oappe.top/gtexkaltvo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.wangshuangyany.cn/gtfgngqbmz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.aizwys.cn/gtirukktlw.html

[B04] for 计数循环
来源：http://hz.xziqi.cn/gtukfghcbr.html

Py:   for i in range(10): print(i)
来源：http://hz.mhx1999.top/gtjhjemcgn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cheryme.top/gtbypwksdm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtephfhfaj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hywenlv.cn/gthosaxlom.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhongyouzk.top/gtogvzlvgs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yj20258.top/gtbuddrqup.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yanxiufei.cn/gthdgklosz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.aizwys.cn/gthskwzfhw.html

[B05] 遍历数组 / 列表
来源：http://hz.aibaodan.cn/gtgbwgrvxk.html

Py:   for item in arr: print(item)
来源：http://hz.daria6918.cn/gtfmqghjmb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhongyouzk.top/gtheikxinr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.nwbrower.top/gtiygmnfat.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sxryk.cn/gtkodkjipi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zdqjudy.top/gtfkbkqnhl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.meibo888.top/gtiimgmekw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yuxming.cn/gtkrrgymvm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.nanxuanxn.top/gttdsudcnt.html

[B06] 遍历字典 / 对象
来源：http://hz.aibaodan.cn/gtrgvxueoz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.haohaochexian.top/gtqpzmolom.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.tanke756.top/gtfjmmuvng.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.mhx1999.top/gtjdmdvjmf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.feifeiyinyue.top/gtjjyhdwez.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhixingplan.top/gtdfpjjwys.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xuanzx.com/gtmggurift.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yj20258.top/gtlxirpykp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gotoacloud.top/gtziyjmjkd.html

[B07] while 循环
来源：http://hz.jqgfzy.top/gtomizggxm.html

Py:   while i < 10: i += 1
来源：http://hz.zhiwuduotai.top/gtnyzlhbdp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.52xcode.cn/gtbvytorqp.html

JS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtdnggxyco.html

TS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gthqhauwga.html

Java: while (i < 10) { i++; }
来源：http://hz.tian-w.cn/gtgaxfemmw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj202588.top/gtpfykqfvy.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ywan-chungtsiang.top/gtfyensxyd.html

C#:   while (i < 10) { i++; }
来源：http://hz.yonumen.top/gtcltdicgs.html

[B08] do-while（至少执行一次）
来源：http://hz.smart0.xyz/gtnjemmgsz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yvedp.cn/gtoagrqglg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.c1oappe.top/gtbabrdefa.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtqltcstot.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtonhghnge.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gtvmznkpmr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.kuanghao11.cn/gtebhaejzy.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hnqzz.top/gthazyzizf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtalpmjoys.html

[B09] break 与 continue
来源：http://hz.jinyuanbaomall.cn/gtchmqljge.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hnqzz.top/gtvoyykzde.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.svipenyu.cn/gtbwfjdaxa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtapoqjdna.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guannengcc.top/gtdfmkfemw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhijiandao.cn/gtlzyyjxic.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhixingplan.top/gtzgxtrbjq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenzaomai.com/gtqjljhvlp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtdyyiwpbx.html

[B10] 遍历同时拿索引
来源：http://hz.jianghu66.top/gtajdgjgoq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.redwolf501.top/gtxcvetbzz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenjidiqi.icu/gtiewtxjyt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.chenlongwang.top/gthtrmnuaj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtbvvlizlk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.redwolf501.top/gtwirqxcsa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.haohaochexian.top/gterestwui.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jiagoushi.top/gtxjkpknxc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jianghu66.top/gtgleuljpm.html

[B11] 生成数字序列 / 区间
来源：http://hz.316326.xyz/gthkpkmuvt.html

Py:   list(range(0, 10, 2))
来源：http://hz.sysykeji.top/gtchmhrzag.html

PHP:  range(0, 10, 2);
来源：http://hz.hongshengwenyu.top/gtnseltzlq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtbydlwpyb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydjk.org.cn/gtxfeuqytl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.tian-w.cn/gtudxatxpj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shangyingyoupin.top/gtwgehmwbl.html

Ruby: (0...10).step(2).to_a
来源：http://hz.c1oappe.top/gtryzoydie.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj202588.top/gtviwojzpg.html

[B12] 跳出多层循环
来源：http://hz.cqqwz.cn/gtvpygjstx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xuetiantiany.cn/gtirhrqfpq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jianghu66.top/gteyyhwrlg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtdumwuigc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtkogfatev.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.guannengcc.top/gtelztalpg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ydzc1.top/gtxtdizsps.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sysykeji.top/gtaakrxvmz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.c1oappe.top/gtolzjkcaq.html

[B13] 判断是否为数字
来源：http://hz.shuidangran.top/gtixmdayaf.html

Py:   isinstance(x, (int, float))
来源：http://hz.iojbl.cn/gtzxroobps.html

PHP:  is_numeric($x)
来源：http://hz.c1oappe.top/gtfapmstaz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nwbrower.top/gtiyszrnpl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gtrqvrogll.html

Java: x instanceof Number
来源：http://hz.hysaishi.cn/gtomqcvbxc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigfzy.top/gtdmdarmbi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuxming.cn/gthjuoixjg.html

C#:   x is int or double or decimal
来源：http://hz.gzhubu.top/gtnkohvrfs.html

[B14] 判断值是否在集合内
来源：http://hz.zycfv.cn/gtnwsyncqh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nanxuanxn.top/gtepuxhqmd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daxiang520.top/gttdsljhqh.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj202588.top/gtryknanis.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ydjk.org.cn/gtggfvnywl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shangyingyoupin.top/gtjaofbais.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dianchejie.cn/gtdsljmlrc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yueranfly.top/gtpkqplgtp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hammf.cn/gtrnnpwxqm.html

[B15] 布尔运算与取反
来源：http://hz.sysykeji.top/gtnndjpcmv.html

Py:   a and b or not c
来源：http://hz.aibaodan.cn/gtmyvnpzza.html

PHP:  $a && $b || !$c
来源：http://hz.svipenyu.cn/gtazezwocf.html

JS:   a && b || !c
来源：http://hz.meibo888.top/gtopuiuzhc.html

TS:   a && b || !c
来源：http://hz.jlsjyb.cn/gtfqeaxqjr.html

Java: a && b || !c
来源：http://hz.chenjidiqi.icu/gtmjcftrco.html

Go:   a && b || !c
来源：http://hz.xuanzx.com/gtahouqbbb.html

Ruby: a && b || !c
来源：http://hz.feifeiyinyue.top/gttnlttngr.html

C#:   a && b || !c
来源：http://hz.ivvv.top/gthtmsrwfw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hfpthk.cn/gtbwhubfih.html

Py:   if not data: return
来源：http://hz.kuanghao11.cn/gtlatgkkfz.html

PHP:  if (!$data) { return; }
来源：http://hz.pengpengdd.cyou/gtecdikvyf.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtkkojorcw.html

TS:   if (!data) return;
来源：http://hz.iojbl.cn/gtxzxtfhwp.html

Java: if (data == null) return;
来源：http://hz.yangfankeji.com/gtijifyqzh.html

Go:   if data == nil { return }
来源：http://hz.mhx1999.top/gtjnwhzkdj.html

Ruby: return if data.nil?
来源：http://hz.jlsjyb.cn/gtbfprpahg.html

C#:   if (data == null) return;
来源：http://hz.yangfankeji.com/gtelvyhsaj.html

================================================================================
来源：http://hz.9152youxi.cn/gtdcrqnvuz.html

C. 函数与作用域
来源：http://hz.yueranfly.top/gtrhtekszv.html

================================================================================
来源：http://hz.52xcode.cn/gtychtsurd.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gtebfutrex.html

Py:   def add(a, b): return a + b
来源：http://hz.hywenlv.cn/gtvpyimlcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtllupnury.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ydzc1.top/gthttvrcqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yanxiufei.cn/gtjadxjxed.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gttkhhcrjb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.mhx1999.top/gtnmncezcf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gotoacloud.top/gtsswrowns.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtocylasjl.html

[C02] 默认参数
来源：http://hz.andypj.xyz/gtnvbdhmqj.html

Py:   def greet(name="World"): return name
来源：http://hz.jlsjyb.cn/gtbqjlvdhx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.c1oappe.top/gtobvbllgh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.guannengcc.top/gtjvhlxaru.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.fengsongda.top/gtoanadfmo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.daria6918.cn/gtopunaauo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.smart0.xyz/gtxhdjwwzc.html

Ruby: def greet(name = "World") = name
来源：http://hz.xinyue.icu/gtfbcootoe.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.redwolf501.top/gtoxvaiion.html

[C03] 可变参数
来源：http://hz.hysaishi.cn/gtrodunbek.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydjk.org.cn/gtadgwxsgs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxuanxn.top/gtvdldylwc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtcmzpmigb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtzsairghj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nanxinkj.top/gtksjzfyva.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shuidangran.top/gtjvwuwaig.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtzqzyvsds.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtovohdzwq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtwvsvtzwt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.wangshuangyany.cn/gtvmuzlark.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.wangshuangyany.cn/gtpmvfyqit.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cashguo.top/gtfqnzgraw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtkdwnrdbe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.iojbl.cn/gtfavbuslr.html

Go:   // 无：用配置结构体参数
来源：http://hz.c1oappe.top/gtvmrunbcq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtqxuoinqz.html

C#:   f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gttyqajxpc.html

[C05] 返回多个值
来源：http://hz.zhongyouzk.top/gtckthyzdo.html

Py:   return a, b
来源：http://hz.yanxiufei.cn/gtpytulnha.html

PHP:  return [$a, $b];
来源：http://hz.nanxuanxn.top/gtfjyjtwbg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yongpay.top/gtpvbxetqx.html

TS:   return { a, b };
来源：http://hz.svipenyu.cn/gtzyypevwp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtvnsrrntt.html

Go:   return a, b
来源：http://hz.snrcjt.cn/gtndlobwqa.html

Ruby: return a, b
来源：http://hz.snrcjt.cn/gtlswikicy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258.top/gtugrzkjkh.html

[C06] 匿名函数 / lambda
来源：http://hz.zhongyouzk.top/gtotnymrxh.html

Py:   square = lambda x: x * x
来源：http://hz.fzhhl.top/gtlherpxyc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gaohongyu789.top/gtewcrbjso.html

JS:   const square = x => x * x;
来源：http://hz.yangfankeji.com/gtqkakgyuw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuanzhike.top/gtvcszqbmj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jinyuanbaomall.cn/gtizowwjvs.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhoulong.xyz/gtbmirnicb.html

Ruby: square = ->(x) { x * x }
来源：http://hz.redwolf501.top/gtghjaolam.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.haohaochexian.top/gtzuzonzak.html

[C07] 把函数作为参数传入
来源：http://hz.havefunace.top/gtjvhtomcs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hysaishi.cn/gtyhrgejhf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tian-w.cn/gtjzvppiuv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnxiangtu.top/gtrfcuqozn.html

TS:   arr.map(String)
来源：http://hz.cqqwz.cn/gtiftvdixk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yvedp.cn/gtakzyhpto.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hywenlv.cn/gtpycfllak.html

Ruby: arr.map(&:upcase)
来源：http://hz.0kj1m.cn/gtharuaguy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jianghu66.top/gtwhblqyyw.html

[C08] 闭包
来源：http://hz.gogol.net.cn/gtnmtdesfe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yuxming.cn/gtvvvnqdvh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hysaishi.cn/gtcslzyjld.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.fengsongda.top/gtjzylwdpi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtampvcslz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhoulong.xyz/gttxaampsx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gaohongyu789.top/gtqbkrelmp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guannengcc.top/gtuxetusfn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtfcxvuxqm.html

[C09] 递归
来源：http://hz.guannengcc.top/gtcxljauko.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yj202588.top/gtfsoquvrf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xziqi.cn/gtfhqwxiod.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtznfxslli.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yonumen.top/gtulqkdzow.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nanxuanxn.top/gtvbcoykyt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cqqwz.cn/gtjsoarnrn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yvedp.cn/gtdoykkkhl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cashguo.top/gtjkmeenst.html

[C10] 变量作用域
来源：http://hz.cqqwz.cn/gtucrenouu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shzxlz.cn/gtuyougngb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shzxlz.cn/gtxltqxftw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jyoumei.cn/gtujtttmuw.html

TS:   同 JS
来源：http://hz.jinqigufen.top/gtgylgkryo.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtrlxrtkrs.html

Go:   花括号块级作用域
来源：http://hz.wangdashe.top/gtklwrlcoi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cheryme.top/gtvnzzogeg.html

C#:   块级作用域
来源：http://hz.yangfankeji.com/gtlpzradcp.html

[C11] 模块导入与导出
来源：http://hz.redwolf501.top/gtciwgpjcy.html

Py:   from module import func
来源：http://hz.ppjwa.cn/gtqwmikaht.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.smart0.xyz/gtthskbdpe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yj202588.top/gthryswgmd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gtbdariccl.html

Java: import java.util.List;
来源：http://hz.shangyingyoupin.top/gteuhuuapt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gttrgejhww.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.nanxuanxn.top/gtdmnajrmm.html

C#:   using System.Text;
来源：http://hz.wangshuangyany.cn/gtyzssoxmt.html

[C12] 立即执行函数 IIFE
来源：http://hz.hywenlv.cn/gtgowmsatr.html

Py:   (lambda: print("run"))()
来源：http://hz.ivvv.top/gtxrbqjucy.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj20258.top/gtdlhhgxfy.html

JS:   (() => { console.log("run"); })();
来源：http://hz.birdmap.top/gtqgxsxljy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jqgfzy.top/gtjorzvyox.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.pengpengdd.cyou/gtoufccpyz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhiwuduotai.top/gtwxesnthl.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gtqrxilith.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.aizwys.cn/gtgaihbllu.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtztaroojg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xinyue.icu/gtpntfbpic.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtzpiqbufi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258.top/gtnuwymkro.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtehtfjmhk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtzlzlkrpm.html

Go:   func add(a, b int) int
来源：http://hz.daxiang520.top/gtamiwntoh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.snrcjt.cn/gtczibwqzw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.tian-w.cn/gtcserdsgx.html

[C14] 泛型函数
来源：http://hz.hongshengwenyu.top/gtbxpqnkua.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.mhx1999.top/gtpzrtkbit.html

PHP:  // 无泛型
来源：http://hz.cashguo.top/gthtqxuqac.html

JS:   // 无泛型
来源：http://hz.zhoulong.xyz/gtxtatkruc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.xinyue.icu/gtmmqotlhv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.svipenyu.cn/gtexzanrvh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guannengcc.top/gtlfbdxsqr.html

Ruby: # 无泛型
来源：http://hz.cucudq.cn/gtstbvlszb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ywan-chungtsiang.top/gturuvviby.html

[C15] 解构 / 展开参数
来源：http://hz.sysykeji.top/gtfbolhxkw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangtech.top/gtscivtoyk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.smart0.xyz/gtgcquthcs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangkeji.top/gtsyybzgqp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhengqikj.top/gtsoaqrgvk.html

Java: // 无解构
来源：http://hz.hongshengwenyu.top/gtneacesgb.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtehhhxnje.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtaligaahl.html

C#:   var (a, b) = pair;
来源：http://hz.fengsongda.top/gtupsttdyo.html

[C16] 函数 / 方法重载
来源：http://hz.zycfv.cn/gtvbqhyskz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgufenzy.top/gtcoobpcjc.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtgyptbhwg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinghuilouyu.cn/gtrwpigojk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hongshengwenyu.top/gtbyczmdxq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gzhubu.top/gtrnpceryi.html


<!-- 参考信息 -->