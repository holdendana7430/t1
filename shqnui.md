代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.ybcxt.top/gtxwqmkgof.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.tian-w.cn/gtxmysqvxb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xingfuxueyuan.xyz/gtnycfzubp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydjk.org.cn/gtlyoglkrs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.cqqwz.cn/gtpdjvndkx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cashguo.top/gtgtryjcca.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.guannengcc.top/gtgtpthihq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xylfe.cn/gtkvzmlzgu.html

[A26] 类型转换总览
来源：http://hz.andypj.xyz/gtvzneiwdn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yonumen.top/gtwqiwajah.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jyoumei.cn/gtpxdgzdta.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ywan-chungtsiang.top/gtyvqlrone.html

TS:   Number() String() Boolean() x as number
来源：http://hz.havefunace.top/gtxnwecskv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.guannengcc.top/gtlejehxlw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.quarkkingdee.top/gtoxxzxydw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shanyushiyangkeji.top/gtqwtmqogh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yj202588.top/gtmyithgil.html

================================================================================
来源：http://hz.yvedp.cn/gteitfkoyh.html

B. 流程控制
来源：http://hz.sysykeji.top/gtrbcovkqv.html

================================================================================
来源：http://hz.andypj.xyz/gthdqamboo.html

[B01] 条件判断 if / else
来源：http://hz.redwolf501.top/gttvjupfts.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhijiandao.cn/gtwmlykbsd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.iojbl.cn/gtvgeahzsn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shangyingyoupin.top/gtyyyrocur.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jlsjyb.cn/gtgbmldfxc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtasrpaczy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.hywenlv.cn/gthqxhcbtw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.shangyingyoupin.top/gtguaigqlo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hammf.cn/gtmmpdyvdg.html

[B02] 多分支 else if / elif
来源：http://hz.aibaodan.cn/gtmayfxvrs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jqgufenzy.top/gtldkvqnzj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.daria6918.cn/gtfzgczphj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cheryme.top/gthefoydxp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhongyouzk.top/gtpotcmxxz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuanzhike.top/gtyqkygfsp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yuanzhike.top/gtvtzadosc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jyoumei.cn/gtjmqovcht.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtmbykwqck.html

[B03] switch / match / case
来源：http://hz.hammf.cn/gtzoondayy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jlsjyb.cn/gtihlyxkne.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.bjfxy.top/gtwwwdhrzn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.fzhhl.top/gtnjcxcexe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yueranfly.top/gtuounvxop.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.xylfe.cn/gtvsyomvwt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jianghu66.top/gtwyqafbfi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.daria6918.cn/gtzbkwwutt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hfpthk.cn/gtadunjgbi.html

[B04] for 计数循环
来源：http://hz.zhoulong.xyz/gtqufxaboi.html

Py:   for i in range(10): print(i)
来源：http://hz.quarkkingdee.top/gtgjmaowxa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shanyushiyangkeji.top/gtuyygiyuy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yvedp.cn/gtrhcwekaz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hywenlv.cn/gtbwxprttv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ydjk.org.cn/gttqgepzss.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cucudq.cn/gtiagfuswr.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jinqigufen.top/gtcnsqwvfu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jinqigufen.top/gtciwlipid.html

[B05] 遍历数组 / 列表
来源：http://hz.ydjk.org.cn/gtxnsfqxws.html

Py:   for item in arr: print(item)
来源：http://hz.fengsongda.top/gtaqpyzuyy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yanxiufei.cn/gtpqijgrre.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhijiandao.cn/gtfkmaauod.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yongpay.top/gtbmknxzlg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sufxvd.cn/gtffirmhjl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.haohaochexian.top/gtswcgahsr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yangfankeji.com/gtbqofwzwr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.iojbl.cn/gtfgvuemwx.html

[B06] 遍历字典 / 对象
来源：http://hz.yj202588.top/gtzlcouemi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.feifeiyinyue.top/gtpqvhvrhd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ppjwa.cn/gtljlnryss.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ivvv.top/gtuplfberj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.chenjidiqi.icu/gtffbdavfr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jiagoushi.top/gthwswudhl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangshuangyany.cn/gtkwqayufs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.chenlongwang.top/gtafcwphzf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinqigfzy.top/gtnzufndul.html

[B07] while 循环
来源：http://hz.jinyuanbaomall.cn/gtzzejdmva.html

Py:   while i < 10: i += 1
来源：http://hz.ydjk.org.cn/gtjfiqfdwl.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.tian-w.cn/gttplnjypr.html

JS:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gttdbfqzgd.html

TS:   while (i < 10) { i++; }
来源：http://hz.jinghuilouyu.cn/gtuukppqgi.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258.top/gthffvihyp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhijiandao.cn/gtwvngvexj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xinyue.icu/gtwmpijslo.html

C#:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtqfmygwon.html

[B08] do-while（至少执行一次）
来源：http://hz.xingfuxueyuan.xyz/gtcfqbjyvp.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gogol.net.cn/gtdnrkpcct.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sxryk.cn/gttmtvxzxa.html

JS:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtgvuhrpkl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yongpay.top/gtkaxtavaf.html

Java: do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtwuegzmdo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.guowangkeji.top/gtsrdckozg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yongpay.top/gtmhhtlqtm.html

C#:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtlgexdncq.html

[B09] break 与 continue
来源：http://hz.vqdsnc.cn/gtggyvikry.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gzhubu.top/gttgcpqrcg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cdnleiting.top/gthrqthjbi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtsweznphh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtvqprrsea.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtficuoqsm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nanxinkj.top/gtsuirxrmt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cdnleiting.top/gttwkpyzhq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fengsongda.top/gtyrljuaxn.html

[B10] 遍历同时拿索引
来源：http://hz.yongpay.top/gthxgyxkkw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.fzhhl.top/gtcoeylbzf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtsytxudeb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xinyue.icu/gtruhqstqb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tian-w.cn/gtcmlyuykt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.iojbl.cn/gtdgienjfc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.gotoacloud.top/gtpzsulsrf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sxryk.cn/gtcsvakizi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sweek.top/gtzixokmvn.html

[B11] 生成数字序列 / 区间
来源：http://hz.hammf.cn/gtajyiagcw.html

Py:   list(range(0, 10, 2))
来源：http://hz.jiagoushi.top/gtdrhxbrex.html

PHP:  range(0, 10, 2);
来源：http://hz.tianlin.xyz/gtvidihcqz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gtofwtqezj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.iojbl.cn/gtgbbkspxm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.guowangkeji.top/gtctmceqlb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.pycfn.com/gtxbvejash.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hfpthk.cn/gtadjwlxcp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tanke756.top/gthqiclncx.html

[B12] 跳出多层循环
来源：http://hz.yueranfly.top/gtpbiperqv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yj20258.top/gtmrvdfaax.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cheryme.top/gtplmysgjr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtizoclxgm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtijuqgfes.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtsvfpgawy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.feifeiyinyue.top/gtqeomgypl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sufxvd.cn/gtgqaujsdk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhijiandao.cn/gtqykmcstf.html

[B13] 判断是否为数字
来源：http://hz.0kj1m.cn/gtyrnnqbcn.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhixingplan.top/gtimbzimtv.html

PHP:  is_numeric($x)
来源：http://hz.gotoacloud.top/gtazztoanq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gtttfjvfrn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tanke756.top/gtoystyezc.html

Java: x instanceof Number
来源：http://hz.9152youxi.cn/gttuqnwruu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.vqdsnc.cn/gtwmdmyygi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuxming.cn/gtogeekozf.html

C#:   x is int or double or decimal
来源：http://hz.quarkkingdee.top/gtcmkntrln.html

[B14] 判断值是否在集合内
来源：http://hz.guannengcc.top/gtykpsnzel.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yj202588.top/gtqdzhlwvw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydjk.org.cn/gtosttusnf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cqqwz.cn/gtqezpjgvh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.9152youxi.cn/gtkvuusdry.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cucudq.cn/gtecsmjdif.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ydjk.org.cn/gtjchsqcrt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ehwqpu.com/gtoofbfrfi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxinkj.top/gthnbhvpsq.html

[B15] 布尔运算与取反
来源：http://hz.bjfxy.top/gtzqsbsbfh.html

Py:   a and b or not c
来源：http://hz.aizwys.cn/gtcaqkkcfp.html

PHP:  $a && $b || !$c
来源：http://hz.yuanzhike.top/gtfuoivyit.html

JS:   a && b || !c
来源：http://hz.xylfe.cn/gtiquflair.html

TS:   a && b || !c
来源：http://hz.tianlin.xyz/gtlwywhfsa.html

Java: a && b || !c
来源：http://hz.hammf.cn/gtdlpjxkny.html

Go:   a && b || !c
来源：http://hz.sweek.top/gtujvcrjuj.html

Ruby: a && b || !c
来源：http://hz.snrcjt.cn/gtywiqddvm.html

C#:   a && b || !c
来源：http://hz.zhijiandao.cn/gtmasvlcmb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nwbrower.top/gtggmocgka.html

Py:   if not data: return
来源：http://hz.chenjidiqi.icu/gtioqhcyba.html

PHP:  if (!$data) { return; }
来源：http://hz.wangdashe.top/gtlzlrpxpi.html

JS:   if (!data) return;
来源：http://hz.dianchejie.cn/gthrmygjzh.html

TS:   if (!data) return;
来源：http://hz.andypj.xyz/gtuheetrxm.html

Java: if (data == null) return;
来源：http://hz.nwbrower.top/gtjqbszdvx.html

Go:   if data == nil { return }
来源：http://hz.dashuyun.cn/gtpzivlzgy.html

Ruby: return if data.nil?
来源：http://hz.daria6918.cn/gttbbbrtli.html

C#:   if (data == null) return;
来源：http://hz.yuanzhike.top/gtuydtkmpl.html

================================================================================
来源：http://hz.chenzaomai.com/gtkdihpqdk.html

C. 函数与作用域
来源：http://hz.hongshengwenyu.top/gtghlbvvmn.html

================================================================================
来源：http://hz.cheryme.top/gtaoiuabhi.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtkrhaanvm.html

Py:   def add(a, b): return a + b
来源：http://hz.yueranfly.top/gtooenpesf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shzxlz.cn/gtvfgihvar.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.mhx1999.top/gtmorqzkgq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtduwtbdkf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtrwhqmssg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xylfe.cn/gtfsnmydqr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daria6918.cn/gtagtlujil.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtfpqkfzki.html

[C02] 默认参数
来源：http://hz.jqgufenzy.top/gtekivqqqa.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gtukrcyusw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgfzy.top/gtwnretipe.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ppjwa.cn/gtfgcxyfdu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gttpuerlem.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhengqikj.top/gtnipuxmvx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zdqjudy.top/gtwjibdznm.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhoulong.xyz/gtvhearcue.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xuanzx.com/gtorzdpqeh.html

[C03] 可变参数
来源：http://hz.gaohongyu789.top/gtqkbvalvv.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydjk.org.cn/gthosiksre.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhaomingkeji.xyz/gttjskgqyy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cucudq.cn/gtyqihetcb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtnefuyrbd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtxwtbxowj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.redwolf501.top/gtlbvfwqxp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhongyouzk.top/gtpdknmcam.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gogol.net.cn/gtqncufaxf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gtiqvqfilv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gtswzxmbml.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gaohongyu789.top/gtxfzqbxho.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtzkhbgyzb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ydzc1.top/gtcqhdrswl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yuxming.cn/gtleeehydw.html

Go:   // 无：用配置结构体参数
来源：http://hz.feifeiyinyue.top/gthejwcsfv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.birdmap.top/gtcmtgiwhf.html

C#:   f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtyphxpjzu.html

[C05] 返回多个值
来源：http://hz.dianchejie.cn/gtxzprgqqu.html

Py:   return a, b
来源：http://hz.0kj1m.cn/gtxrxnjugw.html

PHP:  return [$a, $b];
来源：http://hz.meibo888.top/gtoevfhaza.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.snrcjt.cn/gtxwizebti.html

TS:   return { a, b };
来源：http://hz.zhoulong.xyz/gtwgygmhsu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jianghu66.top/gtjlwknizv.html

Go:   return a, b
来源：http://hz.ybcxt.top/gtrkalbmxw.html

Ruby: return a, b
来源：http://hz.xingfuxueyuan.xyz/gtbujflfdp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yongpay.top/gtnxycpzap.html

[C06] 匿名函数 / lambda
来源：http://hz.ywan-chungtsiang.top/gtzkopnaow.html

Py:   square = lambda x: x * x
来源：http://hz.9152youxi.cn/gtxvnzsqpd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.dianchejie.cn/gtcvrnyyvl.html

JS:   const square = x => x * x;
来源：http://hz.jiagoushi.top/gtqdimhqjl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhijiandao.cn/gtzjyilhuo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhixingplan.top/gtxcuezhou.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hywenlv.cn/gtfloqzmuk.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sweek.top/gtneevvhpc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.daxiang520.top/gtvrbkwivl.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangtech.top/gtlquscrgx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tianlin.xyz/gtqchtigyi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.0kj1m.cn/gtipmqwgog.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ivvv.top/gtgcjtifku.html

TS:   arr.map(String)
来源：http://hz.jyoumei.cn/gtqwhanloe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.havefunace.top/gtcvwinoyz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yvedp.cn/gtkhkrpjpx.html

Ruby: arr.map(&:upcase)
来源：http://hz.guowangkeji.top/gtpgpxhpbi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.fengsongda.top/gtulkqvedd.html

[C08] 闭包
来源：http://hz.aibaodan.cn/gtmrryijry.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yangfankeji.com/gtbapbdsmc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sysykeji.top/gtevxmevtb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtluvaipnh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.mhx1999.top/gtqbthuzri.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ehwqpu.com/gtbljtabtf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhoulong.xyz/gtmdksorpr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhongyouzk.top/gtwyarsvzr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtoazmzftl.html

[C09] 递归
来源：http://hz.hnxiangtu.top/gtruzbkppi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gtawxrazzv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenjidiqi.icu/gtovslfuxi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuanzx.com/gtaqncdwid.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtghxoctds.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sweek.top/gtfnykvnrz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yanxiufei.cn/gtfdnygoqb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangshuangyany.cn/gtcwvozdsu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinyuanbaomall.cn/gtcsuuotdi.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtiicbvjse.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.andypj.xyz/gtxtllhfwd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.aibaodan.cn/gtdrxzouye.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yongpay.top/gtnpkkahhu.html

TS:   同 JS
来源：http://hz.hfpthk.cn/gttazvhsfk.html

Java: 方法内为块级作用域
来源：http://hz.gotoacloud.top/gtwrfvqpfi.html

Go:   花括号块级作用域
来源：http://hz.hnxiangtu.top/gtkfcdvwiz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.quarkkingdee.top/gtsogricpu.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gteevgytex.html

[C11] 模块导入与导出
来源：http://hz.yuanzhike.top/gtzbeixrfx.html

Py:   from module import func
来源：http://hz.zhongyouzk.top/gtqvvfymcx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cashguo.top/gtgvqyjszj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zdqjudy.top/gtgbqmkuuy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhongyouzk.top/gtwuuvzzee.html

Java: import java.util.List;
来源：http://hz.meibo888.top/gtqjvgmkjh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hnqzz.top/gtbhfgojrv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhoulong.xyz/gteijfqfuw.html

C#:   using System.Text;
来源：http://hz.yuanzhike.top/gtqfiuxoyt.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gtfcdzqhiy.html

Py:   (lambda: print("run"))()
来源：http://hz.dashuyun.cn/gtjazwzahi.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuetiantiany.cn/gtyynkvdkb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.shzxlz.cn/gtjsxciblc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gttcvkrxoo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cdnleiting.top/gtmtfqxswi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.guannengcc.top/gtdwvpjxqp.html

Ruby: -> { puts "run" }.call
来源：http://hz.quarkkingdee.top/gtxnhysjxd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cheryme.top/gtelccaipa.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhengqikj.top/gtnkhgqbdb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.havefunace.top/gtopdhugti.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ivvv.top/gtlvwgzexx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fzhhl.top/gtwztlzhvq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtgtphtrle.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gtgwpynmla.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtqliyfdtr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.kuanghao11.cn/gtxpegfabw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cashguo.top/gtqxzzdvsr.html

[C14] 泛型函数
来源：http://hz.hfpthk.cn/gtqobdgbnc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hfpthk.cn/gtrclhskhc.html

PHP:  // 无泛型
来源：http://hz.yj20258.top/gtixmijrai.html

JS:   // 无泛型
来源：http://hz.yueranfly.top/gtmcveepwa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.daria6918.cn/gtfmnplumk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhijiandao.cn/gtfreushds.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.mhx1999.top/gtuhdqyhcy.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtisxbmdur.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hfpthk.cn/gtescamyhq.html

[C15] 解构 / 展开参数
来源：http://hz.wangdashe.top/gtuejdmeoe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj202588.top/gtjshetdvs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gtkmttgoqr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nwbrower.top/gtjvwzzxqe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xingfuxueyuan.xyz/gtnhgdtgpo.html

Java: // 无解构
来源：http://hz.ybcxt.top/gtsyvmejem.html

Go:   // 无解构
来源：http://hz.ydjk.org.cn/gturnipaye.html


<!-- 参考信息 -->