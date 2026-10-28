代发 wailian999

[A26] 类型转换总览
来源：http://hz.quarkkingdee.top/gtgueumgdz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yuanzhike.top/gtqfrypgot.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.mhx1999.top/gtcwdihwex.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.guannengcc.top/gtaydpzfux.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xingfuxueyuan.xyz/gtoevloqls.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cashguo.top/gtleczgdkl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jqgfzy.top/gtnbwecrhg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.smart0.xyz/gtsmqlywrv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhiwuduotai.top/gtjlhfifds.html

================================================================================
来源：http://hz.dashuyun.cn/gtelljyjfz.html

B. 流程控制
来源：http://hz.meibo888.top/gtxohukxnj.html

================================================================================
来源：http://hz.fzhhl.top/gtqxbrpofd.html

[B01] 条件判断 if / else
来源：http://hz.52xcode.cn/gtmueirwvh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.pycfn.com/gtxatwymbo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ehwqpu.com/gtfbttpxwa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.havefunace.top/gtmyizbcov.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jqgfzy.top/gtybyouffd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtefrrdhlw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhijiandao.cn/gtyyyvlvcr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.shanyushiyangtech.top/gtsrbrwvgl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hongshengwenyu.top/gttpsunclb.html

[B02] 多分支 else if / elif
来源：http://hz.yonumen.top/gtadmktdtc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.dashuyun.cn/gtggarntwh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.cashguo.top/gtkszbulma.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtjrrwphuo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gtmdxchzah.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aizwys.cn/gtgjqdiyny.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.aizwys.cn/gterqlilcb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.tian-w.cn/gtqenbtfpa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinyuanbaomall.cn/gtnstbzmer.html

[B03] switch / match / case
来源：http://hz.yj20258.top/gtgithlppg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.chenjidiqi.icu/gtrlcfoknt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.chenlongwang.top/gtibshiijj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xuetiantiany.cn/gtqxnkyvpq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.smart0.xyz/gthlthxlpa.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jqgfzy.top/gtsipdicrb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.quarkkingdee.top/gtbcjhxgrw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cucudq.cn/gtupclrtar.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhongyouzk.top/gtejhwlvby.html

[B04] for 计数循环
来源：http://hz.guowangkeji.top/gtulprzgfi.html

Py:   for i in range(10): print(i)
来源：http://hz.yvedp.cn/gtzfyuwdee.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.haohaochexian.top/gtjcokczoi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shuidangran.top/gtmvqztbrn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhixingplan.top/gtzmnetohf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yongpay.top/gtvfmbueof.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.svipenyu.cn/gtocxhnrvf.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cucudq.cn/gtidevoamu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jinghuilouyu.cn/gtfgcvmran.html

[B05] 遍历数组 / 列表
来源：http://hz.hfpthk.cn/gthwonsaex.html

Py:   for item in arr: print(item)
来源：http://hz.snrcjt.cn/gtivwnzewa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.andypj.xyz/gtvemxzvlm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zdqjudy.top/gtjoobpyqt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zycfv.cn/gtdphcdxlc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jlsjyb.cn/gtbrqaxyqx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.wangdashe.top/gtzajfpwpv.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shangyingyoupin.top/gtlhuqwduf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj20258.top/gtlwaadxpt.html

[B06] 遍历字典 / 对象
来源：http://hz.cucudq.cn/gtlbgoemvg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhiwuduotai.top/gtvjhebagb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ehwqpu.com/gtsdzeweoe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuanzhike.top/gthpbwzwuy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jlsjyb.cn/gtofvpblwt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.bjfxy.top/gtztfwrlwr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ppjwa.cn/gtnohhjhgz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shangyingyoupin.top/gtvparvcuj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.bjfxy.top/gtyisrzeou.html

[B07] while 循环
来源：http://hz.redwolf501.top/gtyujrptql.html

Py:   while i < 10: i += 1
来源：http://hz.fengsongda.top/gtauoirici.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jianghu66.top/gtaktwtjuq.html

JS:   while (i < 10) { i++; }
来源：http://hz.hnxiangtu.top/gtkdkszbxb.html

TS:   while (i < 10) { i++; }
来源：http://hz.yvedp.cn/gtghmgcwgv.html

Java: while (i < 10) { i++; }
来源：http://hz.pycfn.com/gtktzxdcrk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xinyue.icu/gtmdlrhutm.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhengqikj.top/gtfhjnehle.html

C#:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangkeji.top/gtlntshodg.html

[B08] do-while（至少执行一次）
来源：http://hz.ydjk.org.cn/gttzihcedy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinyuanbaomall.cn/gtuvomwuxz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ybcxt.top/gtmdxzvlqw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtkosgxnaj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtqgrmljnz.html

Java: do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtvlmjwsgw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.9152youxi.cn/gtmphtkdfy.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.wangdashe.top/gtpvujauoy.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jinghuilouyu.cn/gtnqfhdftt.html

[B09] break 与 continue
来源：http://hz.kuanghao11.cn/gtxxyearkx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sweek.top/gteyxlfchm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.fengsongda.top/gtuxmiwtcc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gtncwnfljt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtmwwxoxvo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtvwnpsgbd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.daria6918.cn/gthvewcgvi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jlsjyb.cn/gteumvuzym.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtumexyxjq.html

[B10] 遍历同时拿索引
来源：http://hz.daria6918.cn/gtgnftkion.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hysaishi.cn/gteejzjekq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenlongwang.top/gtpnwnwshr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.svipenyu.cn/gtdyugcrup.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jyoumei.cn/gthzyewzet.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.haohaochexian.top/gtxybxapao.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yanxiufei.cn/gteelupeld.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ppjwa.cn/gtxclyjiji.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yuanzhike.top/gttrovcran.html

[B11] 生成数字序列 / 区间
来源：http://hz.ybcxt.top/gtjivlpjdc.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtypfwxfzw.html

PHP:  range(0, 10, 2);
来源：http://hz.ehwqpu.com/gtgbykgydp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigufen.top/gtluzgzyop.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jlsjyb.cn/gtxgxyqijl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.snrcjt.cn/gtzpruajat.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shangyingyoupin.top/gtbyyrjsjq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinghuilouyu.cn/gtwimlgoaa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yuanzhike.top/gthcwpfydb.html

[B12] 跳出多层循环
来源：http://hz.wangshuangyany.cn/gtxunwlyhz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shuidangran.top/gtrddukniz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.mhx1999.top/gtedbdhims.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtskzijwew.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gaohongyu789.top/gtqxkqwita.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.quarkkingdee.top/gtmcfpnvkt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hfpthk.cn/gtnrqlqjjy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ehwqpu.com/gtrwufpbcb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shzxlz.cn/gtupybchcy.html

[B13] 判断是否为数字
来源：http://hz.xingfuxueyuan.xyz/gtpjnxofaf.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnxiangtu.top/gtbciysyla.html

PHP:  is_numeric($x)
来源：http://hz.yuanzhike.top/gtzeksghpl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.havefunace.top/gtctipjzvi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinyuanbaomall.cn/gtupgjysqr.html

Java: x instanceof Number
来源：http://hz.quarkkingdee.top/gtmugcgdhx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.316326.xyz/gtklamhimu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xinyue.icu/gtnwrgzhng.html

C#:   x is int or double or decimal
来源：http://hz.yj202588.top/gtljefgnli.html

[B14] 判断值是否在集合内
来源：http://hz.jianghu66.top/gtifruuwce.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xziqi.cn/gtpatkhtje.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yueranfly.top/gtrajuthki.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhengqikj.top/gtzoixnckk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cqqwz.cn/gtjiylatbq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yueranfly.top/gtwtfeyyne.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ehwqpu.com/gtmnecyhud.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.quarkkingdee.top/gtqesyazvg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxuanxn.top/gtyqdawjtt.html

[B15] 布尔运算与取反
来源：http://hz.zhixingplan.top/gtwmifitqm.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtpemwobmz.html

PHP:  $a && $b || !$c
来源：http://hz.sxryk.cn/gtuyrbaaks.html

JS:   a && b || !c
来源：http://hz.gzhubu.top/gtattpmqkc.html

TS:   a && b || !c
来源：http://hz.cucudq.cn/gtcpkogjpl.html

Java: a && b || !c
来源：http://hz.svipenyu.cn/gtelaqeyfo.html

Go:   a && b || !c
来源：http://hz.hnqzz.top/gtgokziduh.html

Ruby: a && b || !c
来源：http://hz.jianghu66.top/gtulcbjprq.html

C#:   a && b || !c
来源：http://hz.feifeiyinyue.top/gttqqksndc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhijiandao.cn/gtbylvwafk.html

Py:   if not data: return
来源：http://hz.jinqigfzy.top/gtbyhyjude.html

PHP:  if (!$data) { return; }
来源：http://hz.hammf.cn/gtbsmtmbdw.html

JS:   if (!data) return;
来源：http://hz.xinyue.icu/gtdvghxiei.html

TS:   if (!data) return;
来源：http://hz.chenzaomai.com/gtaewbakyo.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gteadcjjih.html

Go:   if data == nil { return }
来源：http://hz.ehwqpu.com/gtqgmsfjij.html

Ruby: return if data.nil?
来源：http://hz.gotoacloud.top/gttpukwbew.html

C#:   if (data == null) return;
来源：http://hz.quarkkingdee.top/gtmwuyszfz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmhhljyat.html

C. 函数与作用域
来源：http://hz.ppjwa.cn/gtfjqsgozj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtblloxejv.html

[C01] 定义函数
来源：http://hz.fzhhl.top/gtzdgkbgul.html

Py:   def add(a, b): return a + b
来源：http://hz.ybcxt.top/gtypthctzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tian-w.cn/gtpntcxqwq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yvedp.cn/gtpeiqqpdh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtmzjwjjcl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hammf.cn/gtpitqetdb.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ywan-chungtsiang.top/gttavcgfyf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgfzy.top/gtppisdpav.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtdfsuugjt.html

[C02] 默认参数
来源：http://hz.zdqjudy.top/gtmtxuxbnh.html

Py:   def greet(name="World"): return name
来源：http://hz.aibaodan.cn/gtxngoxpvf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ppjwa.cn/gtsrpydrye.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtxjegnzbh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cheryme.top/gtkycwmxxc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.quarkkingdee.top/gtvkaypqjh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxuanxn.top/gtpvoqsxlf.html

Ruby: def greet(name = "World") = name
来源：http://hz.hfpthk.cn/gthmhlaofg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jianghu66.top/gtexomxsfo.html

[C03] 可变参数
来源：http://hz.sxryk.cn/gtimrbsmxk.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj202588.top/gtjbjtpjfq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jianghu66.top/gtbtwjealf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yangfankeji.com/gtwpwpcflv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtpteputpx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gtzomrjnha.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnxiangtu.top/gtsgwvjyei.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shuidangran.top/gtoaxouexc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.9152youxi.cn/gtzvmmoccf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shanyushiyangkeji.top/gtqumnmtvh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hywenlv.cn/gtavbkddfs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.52xcode.cn/gtsvquyduq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtjadtjydl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.0kj1m.cn/gtkfgusezx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daxiang520.top/gtcjtyvubj.html

Go:   // 无：用配置结构体参数
来源：http://hz.tian-w.cn/gtnfdsmrdd.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtcidknqvx.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtplkkqcsc.html

[C05] 返回多个值
来源：http://hz.chenlongwang.top/gtkhszzojo.html

Py:   return a, b
来源：http://hz.zhixingplan.top/gttdwaultp.html

PHP:  return [$a, $b];
来源：http://hz.zdqjudy.top/gtcdlofugj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.gogol.net.cn/gtayciuvtw.html

TS:   return { a, b };
来源：http://hz.shanyushiyangtech.top/gtfqfmtgrh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtzsphhcfc.html

Go:   return a, b
来源：http://hz.shuidangran.top/gtnnwrkvcs.html

Ruby: return a, b
来源：http://hz.ppjwa.cn/gtkdcjvoqk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hongshengwenyu.top/gtqfewpovt.html

[C06] 匿名函数 / lambda
来源：http://hz.yanxiufei.cn/gtohbnmgyq.html

Py:   square = lambda x: x * x
来源：http://hz.jqgufenzy.top/gthmlwhqsy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cheryme.top/gttdwmrvcs.html

JS:   const square = x => x * x;
来源：http://hz.hywenlv.cn/gtkvocrjhu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sweek.top/gticqsxcjw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangdashe.top/gtfnvozryb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guowangkeji.top/gtrmrdtgen.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxinkj.top/gtoesegxer.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258.top/gtopqgkslx.html

[C07] 把函数作为参数传入
来源：http://hz.ehwqpu.com/gttfziatqb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinqigufen.top/gtpttlmalo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hongshengwenyu.top/gtjndmisdl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.guowangkeji.top/gtnrwpvakd.html

TS:   arr.map(String)
来源：http://hz.zhaomingkeji.xyz/gtbpvfwwcn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gzhubu.top/gtngqkoudd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gtlkkgwoar.html

Ruby: arr.map(&:upcase)
来源：http://hz.aibaodan.cn/gtnhqbxwvz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydjk.org.cn/gtexnjlnsf.html

[C08] 闭包
来源：http://hz.shangyingyoupin.top/gtzrfpjihk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxuanxn.top/gtnnxqttow.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ywan-chungtsiang.top/gtvjfqiizu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtbqjcsnok.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtkuszvtil.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinghuilouyu.cn/gtphvyinya.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zdqjudy.top/gtmuczfcib.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258.top/gtzlfdlodu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtuvqmvtux.html

[C09] 递归
来源：http://hz.cdnleiting.top/gtjxezgnwg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenlongwang.top/gtkdzhxfgj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.pycfn.com/gtwqajobxf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtdpgikojl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daxiang520.top/gtzupdvfth.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jiagoushi.top/gtfzcrfcke.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhengqikj.top/gtdwpikjat.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtqgobhtjk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtsbqcqbgg.html

[C10] 变量作用域
来源：http://hz.ydzc1.top/gtodnbuplk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.havefunace.top/gtcqaoftih.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yonumen.top/gtdotibcjf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hysaishi.cn/gtzwyrjguc.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtwdsxnhwl.html

Java: 方法内为块级作用域
来源：http://hz.daxiang520.top/gtglwpsdoa.html

Go:   花括号块级作用域
来源：http://hz.gotoacloud.top/gtfrowabzn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.svipenyu.cn/gtoeyuyael.html

C#:   块级作用域
来源：http://hz.daxiang520.top/gtqlnspqbl.html

[C11] 模块导入与导出
来源：http://hz.xingfuxueyuan.xyz/gtbdgnajyn.html

Py:   from module import func
来源：http://hz.zdqjudy.top/gtuvikofhu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtlggjneir.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cqqwz.cn/gtxsjbqbra.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhengqikj.top/gtugjyarcv.html

Java: import java.util.List;
来源：http://hz.ivvv.top/gtuaiillyy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.haohaochexian.top/gtvetltopp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pycfn.com/gthivbzbsq.html

C#:   using System.Text;
来源：http://hz.haohaochexian.top/gtegwebndx.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhoulong.xyz/gthzmhzita.html

Py:   (lambda: print("run"))()
来源：http://hz.cucudq.cn/gtlsvogoaa.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nwbrower.top/gtsmkamzko.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangtech.top/gtpnqdnwcx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtrvgjwfbr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangkeji.top/gtunkqgdbq.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cdnleiting.top/gthljbyzas.html

Ruby: -> { puts "run" }.call
来源：http://hz.jqgfzy.top/gtfugoofgr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jqgfzy.top/gtasbnqdbt.html

[C13] 类型声明 / 类型注解
来源：http://hz.sweek.top/gtpslkkhpn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cashguo.top/gtnxbgztxt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtjvxtrzye.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daxiang520.top/gtpscqaqby.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtylsjuggd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtlnfdtfcy.html

Go:   func add(a, b int) int
来源：http://hz.hnqzz.top/gtehbbiipt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydjk.org.cn/gtvyzocsgi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ywan-chungtsiang.top/gtnatytxul.html

[C14] 泛型函数
来源：http://hz.yanxiufei.cn/gtfxjblphs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhongyouzk.top/gtgxrhxaun.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtfkyzqhoc.html

JS:   // 无泛型
来源：http://hz.haohaochexian.top/gtvhsrarip.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hysaishi.cn/gtryvtpdhy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hongshengwenyu.top/gtqrhjavmp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhongyouzk.top/gtqlmrfmcs.html

Ruby: # 无泛型
来源：http://hz.hammf.cn/gtpfjxbkaz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.gaohongyu789.top/gtjcyaggyr.html

[C15] 解构 / 展开参数
来源：http://hz.dashuyun.cn/gtnkhuocnq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258.top/gtkqykcdev.html

PHP:  [$a, $b] = $pair;
来源：http://hz.vqdsnc.cn/gtdlefrxbs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sweek.top/gtjxflbhos.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cucudq.cn/gtjestfqoz.html

Java: // 无解构
来源：http://hz.jyoumei.cn/gtafkadaae.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtbmtzwdvk.html

Ruby: a, b = pair
来源：http://hz.shuidangran.top/gtvlllursb.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gtezlfvhfj.html

[C16] 函数 / 方法重载
来源：http://hz.sweek.top/gtsaivrans.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhongyouzk.top/gtygqzdypv.html

PHP:  // 无重载
来源：http://hz.yj20258888.top/gtcpvmcjrm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtluezmpnm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hammf.cn/gtdkfzinra.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhiwuduotai.top/gtjzurslub.html


<!-- 参考信息 -->