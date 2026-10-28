代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jqgfzy.top/gtmpfklgrr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jinqigfzy.top/gtsdzyyhps.html

[A24] 去除首尾空白
来源：http://hz.zhiwuduotai.top/gtmtbhmyjs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yuxming.cn/gtmfmvhprb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.haohaochexian.top/gtfccbggpm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuanzx.com/gtcxvbbyyb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xingfuxueyuan.xyz/gtufduqiid.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hammf.cn/gtakworqrn.html

Go:   strings.TrimSpace(s)
来源：http://hz.9152youxi.cn/gtcyxonlfe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cashguo.top/gtaycrltsc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.smart0.xyz/gtuawqyedl.html

[A25] 字符串比较
来源：http://hz.yuxming.cn/gtrcyhcusf.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shangyingyoupin.top/gtynssybut.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.iojbl.cn/gtrbpoqnlr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenlongwang.top/gtpiasheiy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhengqikj.top/gtfslellnx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.sxryk.cn/gtzhiqnocd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.daxiang520.top/gtmnsyuxbv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yvedp.cn/gtggvcjsai.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.c1oappe.top/gtqplxyhvf.html

[A26] 类型转换总览
来源：http://hz.sxryk.cn/gtgqjsqqnv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shzxlz.cn/gthcfgqkah.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.quarkkingdee.top/gteqntzlcn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.cheryme.top/gtmmmiuony.html

TS:   Number() String() Boolean() x as number
来源：http://hz.meibo888.top/gthiguwwqj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hysaishi.cn/gtlofphslh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ivvv.top/gtxzhtbved.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ywan-chungtsiang.top/gtcctwnwdl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zdqjudy.top/gtlassynno.html

================================================================================
来源：http://hz.jqgfzy.top/gtimsfjewt.html

B. 流程控制
来源：http://hz.vqdsnc.cn/gtlrtlhjas.html

================================================================================
来源：http://hz.smart0.xyz/gtkwljazmx.html

[B01] 条件判断 if / else
来源：http://hz.hnqzz.top/gtalwmeuel.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jiagoushi.top/gtpxafmwfp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.redwolf501.top/gtxcprozyy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cucudq.cn/gtqdgjwyjc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sufxvd.cn/gteonugzma.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gtdabjczft.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jlsjyb.cn/gtgnsfkbpo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hammf.cn/gtjrfmldfc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gtkpbbyyry.html

[B02] 多分支 else if / elif
来源：http://hz.hammf.cn/gtmgmukffb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shangyingyoupin.top/gtdkqefphe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ehwqpu.com/gtahtzxnrh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xingfuxueyuan.xyz/gtthxuziko.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gtddxjncca.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gthuhouksn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.aizwys.cn/gtaxuvhfde.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jlsjyb.cn/gtfzymqbhb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sxryk.cn/gtiwezolte.html

[B03] switch / match / case
来源：http://hz.jqgufenzy.top/gtpgnttzhm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.feifeiyinyue.top/gtxzebkxim.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtlxvhearj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.wangshuangyany.cn/gtfxtllwqw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gthrarsbui.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.ydjk.org.cn/gtrgmhvqey.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.sysykeji.top/gtvcfsrkih.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.c1oappe.top/gtymvyswsu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xinyue.icu/gtzoarxtlh.html

[B04] for 计数循环
来源：http://hz.c1oappe.top/gtfkumffgb.html

Py:   for i in range(10): print(i)
来源：http://hz.jqgufenzy.top/gtmqdpooje.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.guowangkeji.top/gthbohzvsq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jiagoushi.top/gtszuveekv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hywenlv.cn/gtsemsokvz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhoulong.xyz/gtrzjvpznm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhengqikj.top/gthclbjlkm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ywan-chungtsiang.top/gtwfvnkaea.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.316326.xyz/gtighsbglx.html

[B05] 遍历数组 / 列表
来源：http://hz.ivvv.top/gtibhdxfsb.html

Py:   for item in arr: print(item)
来源：http://hz.jinyuanbaomall.cn/gtsdkuwvlq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.9152youxi.cn/gtrlzztvhr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tianlin.xyz/gtmrtwxjdn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xinyue.icu/gtlxqcddse.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ydzc1.top/gtnwrrnlqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinyuanbaomall.cn/gtvcgqrxgo.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ydzc1.top/gtlfovfoun.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.pengpengdd.cyou/gtrxrjatbl.html

[B06] 遍历字典 / 对象
来源：http://hz.yuxming.cn/gtyurysugu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.tian-w.cn/gtioauwwyq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hnxiangtu.top/gttefpqpga.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.kuanghao11.cn/gtshrzhedf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgufenzy.top/gtjencgrrb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.kuanghao11.cn/gtvxsszwhg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangdashe.top/gtxevpkwzt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenjidiqi.icu/gtwxddukup.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xinyue.icu/gthibrhkor.html

[B07] while 循环
来源：http://hz.vqdsnc.cn/gtbaknnmis.html

Py:   while i < 10: i += 1
来源：http://hz.zdqjudy.top/gthrmhumfh.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.fengsongda.top/gtsopeynyi.html

JS:   while (i < 10) { i++; }
来源：http://hz.yuanzhike.top/gtmvfjnuuu.html

TS:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtscvqmqkv.html

Java: while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtofxkwuht.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.bjfxy.top/gthisvjkem.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jianghu66.top/gtthojkoyv.html

C#:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtomdlxrjh.html

[B08] do-while（至少执行一次）
来源：http://hz.sysykeji.top/gtsllgazxu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.wangdashe.top/gtvthmxzjb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.quarkkingdee.top/gttsvkxiyz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtwwrizqek.html

TS:   do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtcvktvpgf.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtrywuwsll.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hywenlv.cn/gthzcwaqiq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.daria6918.cn/gtfczzozdg.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtelqhwjjw.html

[B09] break 与 continue
来源：http://hz.zdqjudy.top/gtvcqumfke.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aizwys.cn/gtuhrdzsnf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.gaohongyu789.top/gthfkmoqri.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhaomingkeji.xyz/gtczoabfar.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtunsvkhqj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tian-w.cn/gtudxnunay.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.iojbl.cn/gtrrodchnz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gtmjvwbqvo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guannengcc.top/gtqzludqeo.html

[B10] 遍历同时拿索引
来源：http://hz.sysykeji.top/gtowvhogiz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shzxlz.cn/gtzkcjhpjt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.c1oappe.top/gtmqupfdkx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtaixnwaxk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gogol.net.cn/gtxsqmmtwp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.meibo888.top/gtlhzaneur.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yueranfly.top/gtufdppndu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.feifeiyinyue.top/gtpgtekqbq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xylfe.cn/gthokudtjz.html

[B11] 生成数字序列 / 区间
来源：http://hz.hfpthk.cn/gtsawctqhl.html

Py:   list(range(0, 10, 2))
来源：http://hz.jqgufenzy.top/gtsbdojbjr.html

PHP:  range(0, 10, 2);
来源：http://hz.xylfe.cn/gtdrauzzkx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jlsjyb.cn/gtrtpxndil.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuanzhike.top/gtkuxpdmoo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.dianchejie.cn/gtclaibiqm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.9152youxi.cn/gtwsrspkjf.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cashguo.top/gtypnsjgin.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.vqdsnc.cn/gtlqutadfr.html

[B12] 跳出多层循环
来源：http://hz.cqqwz.cn/gtkeqoyiti.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yanxiufei.cn/gtrhxjuzli.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.snrcjt.cn/gtzmhqnicd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuanzhike.top/gtfqdtfgpp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtqxvwvsob.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtuvkskwan.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ywan-chungtsiang.top/gtiklqtnum.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.aizwys.cn/gtztiksxsq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.52xcode.cn/gthzikkllw.html

[B13] 判断是否为数字
来源：http://hz.kuanghao11.cn/gtoyaneafs.html

Py:   isinstance(x, (int, float))
来源：http://hz.shzxlz.cn/gtrgnfgrtt.html

PHP:  is_numeric($x)
来源：http://hz.sweek.top/gtswpfzmqc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.c1oappe.top/gtibdbarbj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jlsjyb.cn/gtonvlyxoe.html

Java: x instanceof Number
来源：http://hz.yj20258888.top/gtcucwinwe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gotoacloud.top/gtwqapugnt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.meibo888.top/gthdfessix.html

C#:   x is int or double or decimal
来源：http://hz.zhiwuduotai.top/gtqkyiapgd.html

[B14] 判断值是否在集合内
来源：http://hz.ywan-chungtsiang.top/gtvxghpmuu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuetiantiany.cn/gtwveupuax.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.redwolf501.top/gtbqmgcqzn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yuxming.cn/gtzcskntxh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.vqdsnc.cn/gtmlbitump.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yonumen.top/gtjvvtrakf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hysaishi.cn/gtpnmnnoez.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.wangshuangyany.cn/gttmdweods.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.vqdsnc.cn/gtlvyxajdz.html

[B15] 布尔运算与取反
来源：http://hz.pengpengdd.cyou/gtejbcljro.html

Py:   a and b or not c
来源：http://hz.wangdashe.top/gtjajzfoxa.html

PHP:  $a && $b || !$c
来源：http://hz.ehwqpu.com/gtjwfdsoxg.html

JS:   a && b || !c
来源：http://hz.fengsongda.top/gtpkvdwivk.html

TS:   a && b || !c
来源：http://hz.tianlin.xyz/gtqrpukbwv.html

Java: a && b || !c
来源：http://hz.sysykeji.top/gtnvddozxd.html

Go:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtsvektisf.html

Ruby: a && b || !c
来源：http://hz.pycfn.com/gtacjmwktw.html

C#:   a && b || !c
来源：http://hz.redwolf501.top/gtovxkfhev.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangshuangyany.cn/gtillcybpr.html

Py:   if not data: return
来源：http://hz.jianghu66.top/gtrzcwmsql.html

PHP:  if (!$data) { return; }
来源：http://hz.52xcode.cn/gttaxcxkmv.html

JS:   if (!data) return;
来源：http://hz.chenzaomai.com/gtrbvxxccd.html

TS:   if (!data) return;
来源：http://hz.tanke756.top/gtsbwgtryz.html

Java: if (data == null) return;
来源：http://hz.guowangkeji.top/gtkqmsczvd.html

Go:   if data == nil { return }
来源：http://hz.jinyuanbaomall.cn/gtrowinqdr.html

Ruby: return if data.nil?
来源：http://hz.daria6918.cn/gtztjwvjka.html

C#:   if (data == null) return;
来源：http://hz.jiagoushi.top/gtkjyhgbtf.html

================================================================================
来源：http://hz.gogol.net.cn/gtcnsoofwe.html

C. 函数与作用域
来源：http://hz.cucudq.cn/gteicgdfcn.html

================================================================================
来源：http://hz.daxiang520.top/gtndikgsdp.html

[C01] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtaekkofpk.html

Py:   def add(a, b): return a + b
来源：http://hz.gaohongyu789.top/gtpddcxyvq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtuqmingzx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gthegsgtfg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gtkbxeahte.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtsekpwkwj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigufen.top/gteituczqi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuetiantiany.cn/gtuqdcriqz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtflwfpwwn.html

[C02] 默认参数
来源：http://hz.hnqzz.top/gtobqifnct.html

Py:   def greet(name="World"): return name
来源：http://hz.zycfv.cn/gtnopaxkjo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yuanzhike.top/gtgmgrifgn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xylfe.cn/gtjqiataba.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ywan-chungtsiang.top/gtmmiqutpg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gtalnbstyu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yvedp.cn/gtcmhonluc.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhoulong.xyz/gtwqmplnqy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xziqi.cn/gtyoxpofox.html

[C03] 可变参数
来源：http://hz.nanxuanxn.top/gtjrmyhwsg.html

Py:   def total(*args): return sum(args)
来源：http://hz.ehwqpu.com/gtyfytzggw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xingfuxueyuan.xyz/gtawcprxyd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinyuanbaomall.cn/gtqksmcvmz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtglrxusyh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nwbrower.top/gttcedbmda.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tianlin.xyz/gthfwjxcqc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.fzhhl.top/gtrfbyzyto.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ivvv.top/gtzxonxbwo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tian-w.cn/gtzcxuawbn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jiagoushi.top/gtyovxdczk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.c1oappe.top/gtrphwvpuf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtchiuxfwv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cdnleiting.top/gtvbcycwmd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sweek.top/gtvzdojgao.html

Go:   // 无：用配置结构体参数
来源：http://hz.daxiang520.top/gthmiuqwbq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shuidangran.top/gtcyecvjbt.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtqvmvfkcn.html

[C05] 返回多个值
来源：http://hz.jinghuilouyu.cn/gtxmgtynll.html

Py:   return a, b
来源：http://hz.yvedp.cn/gtrzmawzrs.html

PHP:  return [$a, $b];
来源：http://hz.cqqwz.cn/gtlrfqltvv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinqigufen.top/gtjhceyllu.html

TS:   return { a, b };
来源：http://hz.gaohongyu789.top/gtbxrzcocu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hywenlv.cn/gtsusrkjbh.html

Go:   return a, b
来源：http://hz.ppjwa.cn/gtetdkacav.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gtpsotride.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yanxiufei.cn/gtkxvwxgii.html

[C06] 匿名函数 / lambda
来源：http://hz.snrcjt.cn/gtlfbiothv.html

Py:   square = lambda x: x * x
来源：http://hz.yangfankeji.com/gthrdtcotk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hywenlv.cn/gtzylomclx.html

JS:   const square = x => x * x;
来源：http://hz.gotoacloud.top/gtpxqghljj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ydjk.org.cn/gtnacieffy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yongpay.top/gtjvccheue.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ehwqpu.com/gtlejandul.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jlsjyb.cn/gtpbwhywwy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yonumen.top/gttolexnxo.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangtech.top/gtkokwjhsx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hfpthk.cn/gtzavzvkuu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.bjfxy.top/gtxqcgailj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gttssydelp.html

TS:   arr.map(String)
来源：http://hz.sxryk.cn/gthrquufls.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ppjwa.cn/gtbspyotsi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xziqi.cn/gtgvoloiik.html

Ruby: arr.map(&:upcase)
来源：http://hz.guowangkeji.top/gtxuwueuah.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sufxvd.cn/gtuobdvkhi.html

[C08] 闭包
来源：http://hz.smart0.xyz/gtvpsnemmf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydjk.org.cn/gtqquuedpw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xinyue.icu/gthkompuop.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtrmsaprps.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtilzipjdd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.shanyushiyangtech.top/gtwsnavxfk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xingfuxueyuan.xyz/gtsxamjuux.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xylfe.cn/gtywpmzbzr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtgywwcvqy.html

[C09] 递归
来源：http://hz.dianchejie.cn/gtbglrrtfn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nanxinkj.top/gthprpsojz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hywenlv.cn/gthtrjzsiw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dianchejie.cn/gtvfyonmcd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gthifxtwgb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cqqwz.cn/gtxgviaylj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gtmgsfphux.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yongpay.top/gtzcfpakgc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yanxiufei.cn/gtzkpxwarn.html

[C10] 变量作用域
来源：http://hz.iojbl.cn/gtvgvfsgoy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yongpay.top/gthyeatsms.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.52xcode.cn/gtdwktrflx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gogol.net.cn/gtdmlifvkr.html

TS:   同 JS
来源：http://hz.jianghu66.top/gtiqajflmh.html

Java: 方法内为块级作用域
来源：http://hz.sweek.top/gtgtpebirr.html

Go:   花括号块级作用域
来源：http://hz.yuxming.cn/gtqqwsigly.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xziqi.cn/gttweberxl.html

C#:   块级作用域
来源：http://hz.gotoacloud.top/gtkuxuzmmn.html

[C11] 模块导入与导出
来源：http://hz.chenlongwang.top/gtaikfkftf.html

Py:   from module import func
来源：http://hz.yuanzhike.top/gtlrvzwrae.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.daria6918.cn/gtdiivalvq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.wangdashe.top/gtrxpkkkts.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnxiangtu.top/gtbjjlalsh.html

Java: import java.util.List;
来源：http://hz.jinghuilouyu.cn/gtpliyttqb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhiwuduotai.top/gtfyutxwva.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shuidangran.top/gtvkughpuv.html

C#:   using System.Text;
来源：http://hz.havefunace.top/gtmhcuyhfl.html

[C12] 立即执行函数 IIFE
来源：http://hz.smart0.xyz/gtbvbvlrvb.html

Py:   (lambda: print("run"))()
来源：http://hz.sweek.top/gtltxskjde.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aizwys.cn/gtdtacpqyd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nanxuanxn.top/gtlrlzfrsa.html

TS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtyxyuvxmw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangtech.top/gtfnnmlnpy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuanzx.com/gtphqaeakw.html

Ruby: -> { puts "run" }.call
来源：http://hz.nwbrower.top/gtdeaeynhm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gtzedmceod.html

[C13] 类型声明 / 类型注解
来源：http://hz.svipenyu.cn/gtcoitifmz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gtzlphfizu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtnynwvqcy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sweek.top/gtwchvbbyw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gtenywznvz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtkwmdqlfq.html

Go:   func add(a, b int) int
来源：http://hz.zhongyouzk.top/gtgfivuclv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenlongwang.top/gtmmlmcckf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pengpengdd.cyou/gtsevemdre.html

[C14] 泛型函数
来源：http://hz.zhaomingkeji.xyz/gteoxjobrp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuanzx.com/gtncdqumru.html

PHP:  // 无泛型
来源：http://hz.fzhhl.top/gtdyqvrwxl.html

JS:   // 无泛型
来源：http://hz.mhx1999.top/gtkugatutm.html


<!-- 参考信息 -->