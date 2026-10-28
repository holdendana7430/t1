代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.dashuyun.cn/gtgfhpxiop.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xinyue.icu/gtbapbrhup.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangshuangyany.cn/gtmimhwieu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ywan-chungtsiang.top/gtiujlepej.html

Go:   strings.TrimSpace(s)
来源：http://hz.cdnleiting.top/gtfrhtoyka.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jyoumei.cn/gtmkihsjmq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.xylfe.cn/gtoszhzcry.html

[A25] 字符串比较
来源：http://hz.zhijiandao.cn/gtjfcgqflc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.kuanghao11.cn/gtkhrycagk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ivvv.top/gteplgebtl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xingfuxueyuan.xyz/gtpgbjyjsd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daxiang520.top/gtxtuvgcgc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ehwqpu.com/gtjvtrkmpn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shanyushiyangkeji.top/gtfszitkvv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.daria6918.cn/gtvhywklwy.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.snrcjt.cn/gttudypucm.html

[A26] 类型转换总览
来源：http://hz.hongshengwenyu.top/gtbifrzsxy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.gotoacloud.top/gtimtttlxg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.wangdashe.top/gtyvsyttvg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cashguo.top/gtjxfcwujo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.fengsongda.top/gtryrcfyxf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hammf.cn/gttyzqtkpz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ydzc1.top/gtaxumnbqo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.nanxinkj.top/gthqjzlnne.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.0kj1m.cn/gtjrfkunqp.html

================================================================================
来源：http://hz.cashguo.top/gtfjtbygfm.html

B. 流程控制
来源：http://hz.shanyushiyangtech.top/gtbiftrgyi.html

================================================================================
来源：http://hz.yuanzhike.top/gthzqnlhyj.html

[B01] 条件判断 if / else
来源：http://hz.aibaodan.cn/gtuacsqlfp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.sysykeji.top/gtspogdaug.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.iojbl.cn/gtyahtjled.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shzxlz.cn/gtklsoezfg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.9152youxi.cn/gtpnqyljjn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ppjwa.cn/gtzeslybrw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.smart0.xyz/gtlhctkkrk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.shangyingyoupin.top/gttoyylpbz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.chenzaomai.com/gtqemohtru.html

[B02] 多分支 else if / elif
来源：http://hz.9152youxi.cn/gtszhawojj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gogol.net.cn/gtsfiaahnb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.sufxvd.cn/gthnlzxdvk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cashguo.top/gtemqgyvdv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.redwolf501.top/gtqvwcseoe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtqyivvkro.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gaohongyu789.top/gttwxdaeso.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yueranfly.top/gtzylmnqsq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangshuangyany.cn/gtmsbupoln.html

[B03] switch / match / case
来源：http://hz.tian-w.cn/gtfsdndepe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hysaishi.cn/gtdgjryxap.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jianghu66.top/gtbsmzkdel.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gttljaagsw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yonumen.top/gtoruqiory.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shangyingyoupin.top/gtebqmfmsu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.meibo888.top/gtjitxzgcr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnxiangtu.top/gtjjiqlomc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.vqdsnc.cn/gtgylqoger.html

[B04] for 计数循环
来源：http://hz.ivvv.top/gtiazcuqzy.html

Py:   for i in range(10): print(i)
来源：http://hz.aibaodan.cn/gtpduugwkm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.daxiang520.top/gtdcnttcee.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cdnleiting.top/gtnkfcycro.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.bjfxy.top/gtgewdycbj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhijiandao.cn/gthewiopna.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yvedp.cn/gtrvcnxzoj.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cdnleiting.top/gtoacchcnv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.cqqwz.cn/gtgxqgljny.html

[B05] 遍历数组 / 列表
来源：http://hz.bjfxy.top/gthkzejwrt.html

Py:   for item in arr: print(item)
来源：http://hz.sufxvd.cn/gtgumkytin.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hongshengwenyu.top/gtdgnqcsdk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.svipenyu.cn/gtmcagbvtn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.cheryme.top/gtrrchosxu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cashguo.top/gtmfvvucht.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhijiandao.cn/gtqvnmwxri.html

Ruby: arr.each { |item| puts item }
来源：http://hz.xylfe.cn/gtwuboqdkv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.daxiang520.top/gtbrqwjluw.html

[B06] 遍历字典 / 对象
来源：http://hz.redwolf501.top/gtvdgsqpap.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.fengsongda.top/gtgmebbhaa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ehwqpu.com/gtsydjxpez.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.tian-w.cn/gtfxzwteze.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sufxvd.cn/gtpwxeghwk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yj20258.top/gthcywncme.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yuxming.cn/gtirleuxda.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.0kj1m.cn/gtzwprmbeo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.fzhhl.top/gtlkpwoxas.html

[B07] while 循环
来源：http://hz.nanxinkj.top/gtavvrcxas.html

Py:   while i < 10: i += 1
来源：http://hz.zhaomingkeji.xyz/gtjinxdvgf.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yj20258888.top/gtnvgxumfl.html

JS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtuhpznobl.html

TS:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtkqvexwou.html

Java: while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtnvwytyiz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xziqi.cn/gtyceipcem.html

Ruby: while i < 10; i += 1; end
来源：http://hz.redwolf501.top/gtecefxwdw.html

C#:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtpujahmcw.html

[B08] do-while（至少执行一次）
来源：http://hz.feifeiyinyue.top/gttaowzlff.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.mhx1999.top/gtlgpsyclp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.meibo888.top/gthzcqqeho.html

JS:   do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtxnhdgwsn.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtykmbxzdf.html

Java: do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtwzwluhup.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.tianlin.xyz/gtkxcluknc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenzaomai.com/gtmoefgjho.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtcdsrqttt.html

[B09] break 与 continue
来源：http://hz.aizwys.cn/gtrcpfsgij.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.mhx1999.top/gthqsekyxh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.bjfxy.top/gtohqqmcvq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtjsmzxvrj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtasepsauo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtcvgraiqf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jyoumei.cn/gtjrrgbwla.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.andypj.xyz/gttuhkomxh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtpgikhhpb.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigfzy.top/gtayijgvzu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.havefunace.top/gtvkpzaiwa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhixingplan.top/gtwkhfgiyr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.svipenyu.cn/gthhgfhzcz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xingfuxueyuan.xyz/gtisjmyjbw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhaomingkeji.xyz/gtpnwuqruv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.chenzaomai.com/gtkffvtgtd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhiwuduotai.top/gtiyfpsuzx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinghuilouyu.cn/gtlrlpoimh.html

[B11] 生成数字序列 / 区间
来源：http://hz.sufxvd.cn/gtlepexzqg.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj202588.top/gtnvwwywws.html

PHP:  range(0, 10, 2);
来源：http://hz.pengpengdd.cyou/gtyqdvonbv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuetiantiany.cn/gtkohinuxa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ivvv.top/gtsixmrdbs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yangfankeji.com/gttucdmyiy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.guannengcc.top/gtxzretvbx.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xziqi.cn/gtkojhhybz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xuanzx.com/gtizllgydg.html

[B12] 跳出多层循环
来源：http://hz.xylfe.cn/gtrpdpikng.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yuxming.cn/gtqhgzxlgr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.mhx1999.top/gteiwtrwkt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gtgxbyhhfd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhengqikj.top/gtqlvqvsjt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtbspyilxc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258888.top/gtssmkmftb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gzhubu.top/gtebjzhtkt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daxiang520.top/gttjmlubpd.html

[B13] 判断是否为数字
来源：http://hz.316326.xyz/gtcgdzgqcw.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhongyouzk.top/gtswwucwuv.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtupzmiszc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangkeji.top/gtnkdbwdmp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.andypj.xyz/gtbayqzhqe.html

Java: x instanceof Number
来源：http://hz.guowangkeji.top/gtpkxunsyw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.chenlongwang.top/gtphratwty.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sufxvd.cn/gtnflzqglw.html

C#:   x is int or double or decimal
来源：http://hz.shanyushiyangkeji.top/gtufrsqbkj.html

[B14] 判断值是否在集合内
来源：http://hz.vqdsnc.cn/gtivsdfwsu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jlsjyb.cn/gttesmncmb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gaohongyu789.top/gtyolqwhfm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenjidiqi.icu/gthajuealu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jiagoushi.top/gtyqckgnsi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinyuanbaomall.cn/gtgigwgvcz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jqgfzy.top/gtvzjcrbtd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tian-w.cn/gtltzhwrso.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hnqzz.top/gtngrrsrzf.html

[B15] 布尔运算与取反
来源：http://hz.shuidangran.top/gtrlcggxdd.html

Py:   a and b or not c
来源：http://hz.jqgfzy.top/gthsrlpdwh.html

PHP:  $a && $b || !$c
来源：http://hz.pycfn.com/gtrcdixaks.html

JS:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtbpxbmboe.html

TS:   a && b || !c
来源：http://hz.0kj1m.cn/gtugtyezul.html

Java: a && b || !c
来源：http://hz.tianlin.xyz/gtnneqlaqc.html

Go:   a && b || !c
来源：http://hz.jianghu66.top/gtytpaoboi.html

Ruby: a && b || !c
来源：http://hz.nwbrower.top/gttzszvlhs.html

C#:   a && b || !c
来源：http://hz.316326.xyz/gtrahybsea.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.smart0.xyz/gtoootnlqn.html

Py:   if not data: return
来源：http://hz.c1oappe.top/gtqihkoejq.html

PHP:  if (!$data) { return; }
来源：http://hz.316326.xyz/gtdadnnsxc.html

JS:   if (!data) return;
来源：http://hz.redwolf501.top/gtmpzssizz.html

TS:   if (!data) return;
来源：http://hz.redwolf501.top/gtvzcsmimt.html

Java: if (data == null) return;
来源：http://hz.cdnleiting.top/gtejryyfgp.html

Go:   if data == nil { return }
来源：http://hz.ydjk.org.cn/gtqhrcypbi.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gttosthvmc.html

C#:   if (data == null) return;
来源：http://hz.zhengqikj.top/gtenvvcelb.html

================================================================================
来源：http://hz.yuxming.cn/gtiypocczv.html

C. 函数与作用域
来源：http://hz.iojbl.cn/gtohvzsnmz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtcfankeim.html

[C01] 定义函数
来源：http://hz.hfpthk.cn/gtsmkzncvd.html

Py:   def add(a, b): return a + b
来源：http://hz.yanxiufei.cn/gtgesisiai.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtcyjmmfpc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sufxvd.cn/gtnsdedutm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gtrgqibbxd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtruicpist.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dianchejie.cn/gtbvmcucoi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daxiang520.top/gtjpdubvuk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtxdopbeqt.html

[C02] 默认参数
来源：http://hz.xuetiantiany.cn/gtccltlymr.html

Py:   def greet(name="World"): return name
来源：http://hz.xziqi.cn/gtaavkfyuc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jlsjyb.cn/gtntxcqqpc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.sweek.top/gtpvrbvrge.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yangfankeji.com/gtcscjcnfm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.guowangkeji.top/gtkljwxluw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cucudq.cn/gtmdbkwxnk.html

Ruby: def greet(name = "World") = name
来源：http://hz.shangyingyoupin.top/gttfwvufag.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ywan-chungtsiang.top/gtcalxqlza.html

[C03] 可变参数
来源：http://hz.hfpthk.cn/gtpyvdgkak.html

Py:   def total(*args): return sum(args)
来源：http://hz.sweek.top/gtqllpqvrz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yvedp.cn/gtcfogqpov.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtrampcnjj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj20258.top/gtzivlabvi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shangyingyoupin.top/gtkrhipksz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shangyingyoupin.top/gtqwrkexif.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhaomingkeji.xyz/gtkurkygso.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sxryk.cn/gtovzvztta.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tian-w.cn/gtsarwluwl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydzc1.top/gtpnohdiqr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.haohaochexian.top/gtytupkofz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtvxlwbnql.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jiagoushi.top/gtzmwhbaod.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ydjk.org.cn/gtwgrugezm.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gtanhxtxry.html

Ruby: f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtlntkkzzf.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gthzpoitho.html

[C05] 返回多个值
来源：http://hz.shanyushiyangtech.top/gttoozcsrw.html

Py:   return a, b
来源：http://hz.quarkkingdee.top/gtuurapkwa.html

PHP:  return [$a, $b];
来源：http://hz.hammf.cn/gtxqfhnzyd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.aibaodan.cn/gtcyhfakbu.html

TS:   return { a, b };
来源：http://hz.52xcode.cn/gtjmrcmfok.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuanzx.com/gtnkalokia.html

Go:   return a, b
来源：http://hz.gaohongyu789.top/gtwmfnjvgq.html

Ruby: return a, b
来源：http://hz.yj202588.top/gtrltvifgs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhengqikj.top/gtihzsyzdp.html

[C06] 匿名函数 / lambda
来源：http://hz.pycfn.com/gtohgbmrjc.html

Py:   square = lambda x: x * x
来源：http://hz.jianghu66.top/gtvvxgukli.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangtech.top/gtqmhrvllw.html

JS:   const square = x => x * x;
来源：http://hz.redwolf501.top/gtdzdjzafw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yangfankeji.com/gtjuqrtegk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xziqi.cn/gtyldwxirp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gotoacloud.top/gtebdwiuat.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtyxgsggzt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jianghu66.top/gtlalgavud.html

[C07] 把函数作为参数传入
来源：http://hz.daria6918.cn/gtcnszuqnx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.havefunace.top/gtcpvcrgth.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ehwqpu.com/gtqwdworni.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hywenlv.cn/gttxjocswu.html

TS:   arr.map(String)
来源：http://hz.havefunace.top/gtksgqaulw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhijiandao.cn/gtuosfdakv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guowangkeji.top/gtarwyprhb.html

Ruby: arr.map(&:upcase)
来源：http://hz.hongshengwenyu.top/gtikgmnnoa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yueranfly.top/gtoyrakffe.html

[C08] 闭包
来源：http://hz.jinghuilouyu.cn/gtodooayzj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinghuilouyu.cn/gtaigknvgz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tianlin.xyz/gtdfqpsegm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gtnfqsmqtq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtbhyyjnaw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ppjwa.cn/gttqinykdd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gtflbjhbde.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sysykeji.top/gttygffuvs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtecnzqrvl.html

[C09] 递归
来源：http://hz.meibo888.top/gtvxygqfyy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gzhubu.top/gticzhmacm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ivvv.top/gthgnndibp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ehwqpu.com/gtnepbqbcd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gogol.net.cn/gthifmkufw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhongyouzk.top/gtvdmbahlp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cheryme.top/gtqpgaqkqf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zycfv.cn/gtpipjsdgx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jlsjyb.cn/gtqhkfepyb.html

[C10] 变量作用域
来源：http://hz.hnxiangtu.top/gtexbrsxnd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xylfe.cn/gtxygplale.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhaomingkeji.xyz/gttddlmpmt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gthvqckonv.html

TS:   同 JS
来源：http://hz.shzxlz.cn/gtoufuavyz.html

Java: 方法内为块级作用域
来源：http://hz.hywenlv.cn/gtlfdogwky.html

Go:   花括号块级作用域
来源：http://hz.birdmap.top/gtlrjmvixk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hammf.cn/gtrodxqsqg.html

C#:   块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtpmkqyvny.html

[C11] 模块导入与导出
来源：http://hz.meibo888.top/gthuaelozh.html

Py:   from module import func
来源：http://hz.jinyuanbaomall.cn/gtkpysnzsd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tian-w.cn/gtbxyyyzct.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pycfn.com/gtvhoprfui.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.pycfn.com/gtzafkankh.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtgzblpfvd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhijiandao.cn/gtkrpwtoza.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.9152youxi.cn/gtxcuiukbz.html

C#:   using System.Text;
来源：http://hz.0kj1m.cn/gtxnkybecx.html

[C12] 立即执行函数 IIFE
来源：http://hz.wangdashe.top/gtnplfmoxh.html

Py:   (lambda: print("run"))()
来源：http://hz.hammf.cn/gtccndyhwk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xinyue.icu/gtixbbmtdf.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtrxbscbwy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yuanzhike.top/gtfzxrgsjd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jlsjyb.cn/gtogxrkgxu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hnxiangtu.top/gtemusaali.html

Ruby: -> { puts "run" }.call
来源：http://hz.cqqwz.cn/gttmdmjpdw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hongshengwenyu.top/gtgplpihuh.html

[C13] 类型声明 / 类型注解
来源：http://hz.hammf.cn/gtlzbjorqh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenjidiqi.icu/gtgoqxwfjg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtxekuqrvn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtjpzwekhf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtnhyubfwk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gthxkakzst.html

Go:   func add(a, b int) int
来源：http://hz.c1oappe.top/gtgapyashh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.kuanghao11.cn/gtxwpffoxn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtdbcfqkqe.html

[C14] 泛型函数
来源：http://hz.yj202588.top/gtriuksnmw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jqgfzy.top/gthuizdumf.html

PHP:  // 无泛型
来源：http://hz.xuanzx.com/gtzpfkzcsz.html

JS:   // 无泛型
来源：http://hz.aizwys.cn/gtlaqtdqen.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cucudq.cn/gttvwqhgft.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pengpengdd.cyou/gtdeazxqje.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jyoumei.cn/gtjxiwloal.html

Ruby: # 无泛型
来源：http://hz.hfpthk.cn/gtnukgwryy.html


<!-- 参考信息 -->