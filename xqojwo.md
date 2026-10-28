代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hnxiangtu.top/gtifvuhtvu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.daxiang520.top/gtenqbharm.html

[A24] 去除首尾空白
来源：http://hz.cucudq.cn/gtuvldxlpq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.andypj.xyz/gttnzdvibn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yuanzhike.top/gttktrmwjg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jqgufenzy.top/gteazhxlho.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jiagoushi.top/gtfzgcsgyn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ydjk.org.cn/gtlpcylmvn.html

Go:   strings.TrimSpace(s)
来源：http://hz.kuanghao11.cn/gtbmcvsdrk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinqigufen.top/gtzqsguhic.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yongpay.top/gtdhsftbcv.html

[A25] 字符串比较
来源：http://hz.jyoumei.cn/gtmimpdnzh.html

Py:   s1 == s2; s1 != s2
来源：http://hz.0kj1m.cn/gtqzsrpwrj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhongyouzk.top/gtxkmvmgpm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tianlin.xyz/gtgngrzgkg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenjidiqi.icu/gtzzokuxlc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.aibaodan.cn/gtiofmahzl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhengqikj.top/gtvoixpqez.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.fzhhl.top/gtpbxqalbl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jlsjyb.cn/gtfwrnvfve.html

[A26] 类型转换总览
来源：http://hz.dianchejie.cn/gtsqbnzefa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.haohaochexian.top/gtjyzlqszm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhixingplan.top/gtowbmwocx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ydzc1.top/gttkrlcwuk.html

TS:   Number() String() Boolean() x as number
来源：http://hz.hnqzz.top/gtscbpedhs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.quarkkingdee.top/gtfqngwmkt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhiwuduotai.top/gtjginqyln.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.tian-w.cn/gtclqfsilz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.vqdsnc.cn/gtqdhpxqep.html

================================================================================
来源：http://hz.hammf.cn/gthfnlxsxz.html

B. 流程控制
来源：http://hz.kuanghao11.cn/gtajzmbqjg.html

================================================================================
来源：http://hz.316326.xyz/gtphxrpnaw.html

[B01] 条件判断 if / else
来源：http://hz.havefunace.top/gtlohremzf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yongpay.top/gtmwagipik.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ehwqpu.com/gtditkcfnd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtbwvxslni.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtvzxbevjl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhengqikj.top/gtcyrrmhkh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.meibo888.top/gtdclftutl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gzhubu.top/gtclmvepzm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.mhx1999.top/gtucnmucgp.html

[B02] 多分支 else if / elif
来源：http://hz.jlsjyb.cn/gtpmgxadxh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhiwuduotai.top/gtwnqlxztg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj20258.top/gtvblkjvkq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtsdmaqjyl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtssvewxiy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shuidangran.top/gtyxraespq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gotoacloud.top/gtlybnplrh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sufxvd.cn/gtkzxbscoc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cqqwz.cn/gtdkoicoyg.html

[B03] switch / match / case
来源：http://hz.shangyingyoupin.top/gtpszlrwnf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xziqi.cn/gtdojfzszf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.aizwys.cn/gtlvrgwxsa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sysykeji.top/gtgqdkjokm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hywenlv.cn/gtbmbbrrsk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.gaohongyu789.top/gtwvnrsfzz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.quarkkingdee.top/gtkmplkjzl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jiagoushi.top/gtlfxrjctv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yuxming.cn/gtqndvlrjm.html

[B04] for 计数循环
来源：http://hz.mhx1999.top/gtunsdiswb.html

Py:   for i in range(10): print(i)
来源：http://hz.yueranfly.top/gtwvmpbbdo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.vqdsnc.cn/gtqhbkxynx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhongyouzk.top/gtlzottjnr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.guannengcc.top/gtjlquuylk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cdnleiting.top/gtrtmbgwmg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.wangshuangyany.cn/gtzmfdaajm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jinyuanbaomall.cn/gtxhuakvzj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zdqjudy.top/gtbszvycgc.html

[B05] 遍历数组 / 列表
来源：http://hz.xuetiantiany.cn/gtfpvfmulw.html

Py:   for item in arr: print(item)
来源：http://hz.jiagoushi.top/gtnvyqbirl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.meibo888.top/gtcvadrxio.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gttxqrynfr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuanzhike.top/gtuermdufr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sweek.top/gtzkfwfkjk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guowangkeji.top/gttrbjvdac.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shzxlz.cn/gtklljuwit.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj20258.top/gtrldkyzkc.html

[B06] 遍历字典 / 对象
来源：http://hz.jiagoushi.top/gtgxhporyi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhoulong.xyz/gtbdsgsvhn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jianghu66.top/gtcyfisknj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sufxvd.cn/gtgllejeub.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.birdmap.top/gtdumpfrql.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gzhubu.top/gtcmepevzb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.chenlongwang.top/gtgtzrczrw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jqgfzy.top/gtgovnyukt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.pycfn.com/gtwzzcvbdy.html

[B07] while 循环
来源：http://hz.jiagoushi.top/gtvynjpais.html

Py:   while i < 10: i += 1
来源：http://hz.smart0.xyz/gtxvhkqifl.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ydjk.org.cn/gtsgrwljzw.html

JS:   while (i < 10) { i++; }
来源：http://hz.andypj.xyz/gtcvsexdzc.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtsrchkjjc.html

Java: while (i < 10) { i++; }
来源：http://hz.hysaishi.cn/gthhpsgzem.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jqgufenzy.top/gtdweqdrzp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.daxiang520.top/gtsxcrknef.html

C#:   while (i < 10) { i++; }
来源：http://hz.zycfv.cn/gtozuwlwwa.html

[B08] do-while（至少执行一次）
来源：http://hz.c1oappe.top/gtaxiuimtv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhixingplan.top/gtveaemxgt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.quarkkingdee.top/gtetdzgzdm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtmvnlyehe.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtqpbpfbfi.html

Java: do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtierhpxwj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.gaohongyu789.top/gthqsimlxo.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ybcxt.top/gtsxmhphmk.html

C#:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtpzdbcyac.html

[B09] break 与 continue
来源：http://hz.smart0.xyz/gtbnabqjgz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.kuanghao11.cn/gtnggqugsf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.nwbrower.top/gtzqpcqzru.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtacrnyqnv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtcqeyaxiq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtbpgitzzf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgfzy.top/gtvyqoxhhh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.gogol.net.cn/gtccurshll.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtbgjudnog.html

[B10] 遍历同时拿索引
来源：http://hz.dashuyun.cn/gtmcrbjcft.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cdnleiting.top/gtthgjmyxt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ybcxt.top/gtvqoiexzj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yonumen.top/gtzlfxuxzu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yonumen.top/gtllymkxlu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jiagoushi.top/gtxqtxyjoh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pengpengdd.cyou/gtkshwbgog.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tianlin.xyz/gtzzkkdggq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.redwolf501.top/gtbexqewrm.html

[B11] 生成数字序列 / 区间
来源：http://hz.0kj1m.cn/gtuzlyblqm.html

Py:   list(range(0, 10, 2))
来源：http://hz.shangyingyoupin.top/gtdfnyrdan.html

PHP:  range(0, 10, 2);
来源：http://hz.bjfxy.top/gtiwbplmbv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tianlin.xyz/gtpcwhwmbd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuxming.cn/gtozclhdzo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jqgfzy.top/gtkoidsxtr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhijiandao.cn/gtdmrzkyhu.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jlsjyb.cn/gtzdpkywzf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yanxiufei.cn/gttrmkcuhg.html

[B12] 跳出多层循环
来源：http://hz.gaohongyu789.top/gteqzbjsdx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gogol.net.cn/gtnehqhvrb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jlsjyb.cn/gtyrwuevhu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtvbrcokrg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gthasiotwu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.smart0.xyz/gtpsjhyvpa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ydzc1.top/gtwtevkvng.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yvedp.cn/gtyaqtnjgf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.andypj.xyz/gtfzgmhxio.html

[B13] 判断是否为数字
来源：http://hz.yj20258.top/gtiauvmbza.html

Py:   isinstance(x, (int, float))
来源：http://hz.redwolf501.top/gtbrreecfn.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gtgnaevfrp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtwgbjnria.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtrvcejgmn.html

Java: x instanceof Number
来源：http://hz.ydzc1.top/gtfhijqlqp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.snrcjt.cn/gtjjbhdkus.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jiagoushi.top/gtmuawkpaw.html

C#:   x is int or double or decimal
来源：http://hz.fengsongda.top/gtdjhihucf.html

[B14] 判断值是否在集合内
来源：http://hz.jqgufenzy.top/gtdfxvoifd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhaomingkeji.xyz/gtmcskrcku.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhixingplan.top/gttpmsynot.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yuanzhike.top/gtlviwdhrr.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gthplojcew.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.dashuyun.cn/gtkmljnqlu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhijiandao.cn/gtpnbltanq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhiwuduotai.top/gtohscqhip.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.svipenyu.cn/gtxpgbbsdl.html

[B15] 布尔运算与取反
来源：http://hz.yanxiufei.cn/gtygixxqod.html

Py:   a and b or not c
来源：http://hz.andypj.xyz/gtsltnzmup.html

PHP:  $a && $b || !$c
来源：http://hz.dianchejie.cn/gtamyesubo.html

JS:   a && b || !c
来源：http://hz.nanxinkj.top/gtruikfksp.html

TS:   a && b || !c
来源：http://hz.xziqi.cn/gteeindqln.html

Java: a && b || !c
来源：http://hz.hnxiangtu.top/gtiiwrgijg.html

Go:   a && b || !c
来源：http://hz.nanxuanxn.top/gtykzgtdke.html

Ruby: a && b || !c
来源：http://hz.gogol.net.cn/gttjwalmkh.html

C#:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtuvyccmbd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sufxvd.cn/gtjcbljjxm.html

Py:   if not data: return
来源：http://hz.jyoumei.cn/gthvxulnfn.html

PHP:  if (!$data) { return; }
来源：http://hz.yueranfly.top/gtsruobufl.html

JS:   if (!data) return;
来源：http://hz.yj20258.top/gtuppizvgs.html

TS:   if (!data) return;
来源：http://hz.smart0.xyz/gtvjmdvuwx.html

Java: if (data == null) return;
来源：http://hz.gotoacloud.top/gtylgpidum.html

Go:   if data == nil { return }
来源：http://hz.guannengcc.top/gtejktdvrh.html

Ruby: return if data.nil?
来源：http://hz.sxryk.cn/gteqcwhyhc.html

C#:   if (data == null) return;
来源：http://hz.yuxming.cn/gthooetffj.html

================================================================================
来源：http://hz.9152youxi.cn/gtablzrgdp.html

C. 函数与作用域
来源：http://hz.nanxuanxn.top/gteouvjgot.html

================================================================================
来源：http://hz.shzxlz.cn/gtgkmksfcy.html

[C01] 定义函数
来源：http://hz.xinyue.icu/gtdyuhtzcz.html

Py:   def add(a, b): return a + b
来源：http://hz.sweek.top/gtwytdmzcr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gthjjcytsu.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gzhubu.top/gtpvxnoaid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtlubxtreb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gthnkcteno.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgfzy.top/gtlosekuav.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj20258.top/gtvuvycnwy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtuuszynik.html

[C02] 默认参数
来源：http://hz.jiagoushi.top/gtevbgmokv.html

Py:   def greet(name="World"): return name
来源：http://hz.9152youxi.cn/gtfpamlqrt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.0kj1m.cn/gtnakfrajk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jiagoushi.top/gtkvopzsej.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cashguo.top/gtpccwpnjs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxinkj.top/gtcroggudv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.iojbl.cn/gtbprbewtb.html

Ruby: def greet(name = "World") = name
来源：http://hz.aizwys.cn/gtpjoheppt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.havefunace.top/gtvqwsizrc.html

[C03] 可变参数
来源：http://hz.yj20258888.top/gtxkgsgdew.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj202588.top/gtvrakwnmm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dianchejie.cn/gtdzyepuds.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtgaxkxrjf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.redwolf501.top/gthqzbwthq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtgvvxjfhv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.cashguo.top/gtxxpryrhh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.mhx1999.top/gtfbifqriz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gtunkgyzff.html

[C04] 命名参数 / 关键字参数
来源：http://hz.meibo888.top/gttwnselfy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guannengcc.top/gtcsksbzfj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenlongwang.top/gtemymdcwe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtsuameqje.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sweek.top/gtzvvhismt.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinqigufen.top/gtvjybdrla.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhaomingkeji.xyz/gtttkfvvnx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtxsdswyai.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtxmqpskoy.html

[C05] 返回多个值
来源：http://hz.meibo888.top/gtxykkssuu.html

Py:   return a, b
来源：http://hz.gaohongyu789.top/gtqbhifagr.html

PHP:  return [$a, $b];
来源：http://hz.gaohongyu789.top/gtotubgxrn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtezwdddbn.html

TS:   return { a, b };
来源：http://hz.pycfn.com/gtsdhsayqx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinqigufen.top/gtttwumyic.html

Go:   return a, b
来源：http://hz.pengpengdd.cyou/gtkubiswin.html

Ruby: return a, b
来源：http://hz.hfpthk.cn/gtymcnjuhw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shuidangran.top/gtekxkmmmx.html

[C06] 匿名函数 / lambda
来源：http://hz.jlsjyb.cn/gtcieukmkn.html

Py:   square = lambda x: x * x
来源：http://hz.yueranfly.top/gtzptpsmtq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.bjfxy.top/gtxhguutxk.html

JS:   const square = x => x * x;
来源：http://hz.yanxiufei.cn/gtmdxywdid.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gaohongyu789.top/gttysgwzxl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jqgfzy.top/gtukhukceg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigufen.top/gtfxsenork.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cqqwz.cn/gtyhfuzjyl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ivvv.top/gtctvfgyme.html

[C07] 把函数作为参数传入
来源：http://hz.smart0.xyz/gtvgqxnvfc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xziqi.cn/gtpalawlop.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.smart0.xyz/gtajaqdkrh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.havefunace.top/gtdrinqhoj.html

TS:   arr.map(String)
来源：http://hz.daxiang520.top/gtoxjdwwtl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.tianlin.xyz/gtnttotmng.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenlongwang.top/gtqktnihvx.html

Ruby: arr.map(&:upcase)
来源：http://hz.316326.xyz/gtqdkxufeb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.iojbl.cn/gtbczyyxxr.html

[C08] 闭包
来源：http://hz.jyoumei.cn/gtqwpubrhp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hongshengwenyu.top/gtyjstptyt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hysaishi.cn/gtnvgwmwqw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtuxsholdz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gzhubu.top/gtmybwjlgh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cqqwz.cn/gtqjuhsguy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cdnleiting.top/gtcexhlxvk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xinyue.icu/gtunhvvwae.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yvedp.cn/gtysdwsoqd.html

[C09] 递归
来源：http://hz.zhiwuduotai.top/gthpoeaano.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cucudq.cn/gtezrpbyeq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.mhx1999.top/gtchapfsvu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenjidiqi.icu/gtdzrqszgt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ybcxt.top/gtbzcivhgx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgufenzy.top/gterplgopc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yj20258.top/gtbsefqwst.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhaomingkeji.xyz/gtslywrfte.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hywenlv.cn/gtmgarxtai.html

[C10] 变量作用域
来源：http://hz.shanyushiyangtech.top/gtjdjkodjc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hnxiangtu.top/gtklyiayfa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shangyingyoupin.top/gtbbejggmx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jyoumei.cn/gtkiahaymb.html

TS:   同 JS
来源：http://hz.snrcjt.cn/gthudzrtyd.html

Java: 方法内为块级作用域
来源：http://hz.wangdashe.top/gtnwymxida.html

Go:   花括号块级作用域
来源：http://hz.chenjidiqi.icu/gtoyyzoqyq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cashguo.top/gtjewjhoap.html

C#:   块级作用域
来源：http://hz.hnqzz.top/gtvepwdyme.html

[C11] 模块导入与导出
来源：http://hz.yueranfly.top/gtyxcvdxee.html

Py:   from module import func
来源：http://hz.birdmap.top/gtmhmarkrk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhoulong.xyz/gtnqqglgko.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gotoacloud.top/gtonhtflzd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yj20258.top/gtijldyhle.html

Java: import java.util.List;
来源：http://hz.mhx1999.top/gtndbidbcf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhoulong.xyz/gtbpaivobh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.9152youxi.cn/gtaujgwrdq.html

C#:   using System.Text;
来源：http://hz.vqdsnc.cn/gtchzabllt.html

[C12] 立即执行函数 IIFE
来源：http://hz.pengpengdd.cyou/gtalfgynia.html

Py:   (lambda: print("run"))()
来源：http://hz.zhoulong.xyz/gtuziufaah.html

PHP:  (function () { echo "run"; })();
来源：http://hz.cashguo.top/gtwltrocci.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hysaishi.cn/gtoveikyie.html

TS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtcnekbsqm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.aizwys.cn/gtlyrlmpho.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cheryme.top/gtocwqxfse.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtfgjdzugi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yanxiufei.cn/gtxoijkfbl.html

[C13] 类型声明 / 类型注解
来源：http://hz.andypj.xyz/gtsywosrtj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenzaomai.com/gtkbsgbiqd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtmxdeserz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.pengpengdd.cyou/gtemhdbbmo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtvjptgtjn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtzxuamujw.html

Go:   func add(a, b int) int
来源：http://hz.kuanghao11.cn/gtknqkwtbn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sxryk.cn/gtzfkfrvyp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cdnleiting.top/gtaqswxlhb.html

[C14] 泛型函数
来源：http://hz.xuetiantiany.cn/gtknpufdbh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jqgfzy.top/gtmkhwnmdu.html

PHP:  // 无泛型
来源：http://hz.yanxiufei.cn/gtfgcmiyda.html

JS:   // 无泛型
来源：http://hz.zhengqikj.top/gtxmsnbbpt.html


<!-- 参考信息 -->