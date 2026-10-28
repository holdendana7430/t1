代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.redwolf501.top/gtxtzuizoi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shanyushiyangkeji.top/gtsosrggxd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shzxlz.cn/gtbdqscpxr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yonumen.top/gtqcmwptjz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yvedp.cn/gtsdijcqlo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jinyuanbaomall.cn/gtfnyutuvq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.dashuyun.cn/gtjmwuwhnl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ydzc1.top/gtlejnvdce.html

[A26] 类型转换总览
来源：http://hz.yonumen.top/gtglbexkdn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.cdnleiting.top/gteiqhqlku.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.iojbl.cn/gtkuppzvdz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.meibo888.top/gtpcuypsny.html

TS:   Number() String() Boolean() x as number
来源：http://hz.52xcode.cn/gtrxioqnwy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.c1oappe.top/gtepgahvuf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.snrcjt.cn/gtvmchmrgh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jqgufenzy.top/gtngijzsbf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yuanzhike.top/gtplplyjbp.html

================================================================================
来源：http://hz.mhx1999.top/gtxnbamflw.html

B. 流程控制
来源：http://hz.xziqi.cn/gtidxqgeum.html

================================================================================
来源：http://hz.zdqjudy.top/gtvxxraimq.html

[B01] 条件判断 if / else
来源：http://hz.chenlongwang.top/gtwolkxudt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinyuanbaomall.cn/gtwlmueuci.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.guannengcc.top/gtttnlbzhz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gtvzyyupap.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtihczqaao.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtelkunoiq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jinyuanbaomall.cn/gtjedcvxjy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yvedp.cn/gtwyhwvetk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtdkbulyfw.html

[B02] 多分支 else if / elif
来源：http://hz.shzxlz.cn/gtmiekjwxv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.0kj1m.cn/gtfelilmiw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.cheryme.top/gtpnojwlck.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gtzciglzxn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gtjfoerzsx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtxrcoqjkl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gaohongyu789.top/gtugqnnbny.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinqigufen.top/gtsfiklqch.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenjidiqi.icu/gtkwnmuvfj.html

[B03] switch / match / case
来源：http://hz.gaohongyu789.top/gtmytgkpzf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xuanzx.com/gtmfkvpsjg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jqgfzy.top/gtglrvqyns.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtboysjxib.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.vqdsnc.cn/gtjdveakmb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.nanxuanxn.top/gtpyhzwxin.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jinyuanbaomall.cn/gtnsltrvds.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.c1oappe.top/gtxvlifpzt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.nanxinkj.top/gtwuskrxiw.html

[B04] for 计数循环
来源：http://hz.yueranfly.top/gtetwsusuu.html

Py:   for i in range(10): print(i)
来源：http://hz.jinghuilouyu.cn/gtzxqtvwud.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.aizwys.cn/gtrbluuyua.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuxming.cn/gthopeexkf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhengqikj.top/gtdnwztfpb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.kuanghao11.cn/gtbvbiqwwe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.chenzaomai.com/gtkehukynd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cheryme.top/gtypdeisjk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.feifeiyinyue.top/gtdauhozhc.html

[B05] 遍历数组 / 列表
来源：http://hz.guannengcc.top/gtpwywvrzo.html

Py:   for item in arr: print(item)
来源：http://hz.smart0.xyz/gtmybwnbba.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hongshengwenyu.top/gtongtjpiu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhiwuduotai.top/gtxjvaumdm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.cdnleiting.top/gtqzvllsjz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj20258888.top/gteyttrrls.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.nanxinkj.top/gtpmkzrhbz.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yongpay.top/gtuxddrgkl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xinyue.icu/gtuzanpzss.html

[B06] 遍历字典 / 对象
来源：http://hz.jqgfzy.top/gtbozkrdub.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.vqdsnc.cn/gtozvyblyj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cucudq.cn/gtsmypktgh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.vqdsnc.cn/gtkizymgzt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.dianchejie.cn/gtdgedarbk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.jinyuanbaomall.cn/gtxzmavakp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sufxvd.cn/gtmqyfiuod.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jianghu66.top/gtilgjiwdh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.bjfxy.top/gtpmwmliha.html

[B07] while 循环
来源：http://hz.cqqwz.cn/gtootmgpnc.html

Py:   while i < 10: i += 1
来源：http://hz.jqgufenzy.top/gtgzjsiqym.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhijiandao.cn/gtvzxwfvyu.html

JS:   while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtmneftjyg.html

TS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtzsranprd.html

Java: while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gtcuuiyhde.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.haohaochexian.top/gtbruzpaqw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shangyingyoupin.top/gtsqyzkvmy.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtrwwbdvmn.html

[B08] do-while（至少执行一次）
来源：http://hz.zdqjudy.top/gtnyobldzd.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shzxlz.cn/gteuspbowr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gzhubu.top/gtbemkyrvw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtqtycsxob.html

TS:   do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gtrsqdwmrf.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtqkspmfrd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.aizwys.cn/gtpddlexzv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.bjfxy.top/gticasexby.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtbxpspcpn.html

[B09] break 与 continue
来源：http://hz.jlsjyb.cn/gtwmizbawf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jianghu66.top/gtbexmkocr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.dianchejie.cn/gttrjnqlsb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtgtrymaju.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtswazcrki.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtziqeuqtd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhengqikj.top/gthumgkzaz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.meibo888.top/gtjrbqinsu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.mhx1999.top/gteicwpzdg.html

[B10] 遍历同时拿索引
来源：http://hz.xuetiantiany.cn/gtgoqizgei.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jiagoushi.top/gtfuhwtoyu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ydzc1.top/gthrcxpezd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hfpthk.cn/gtpuautehg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hnqzz.top/gtojbgoucx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jlsjyb.cn/gtafpeyavf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yueranfly.top/gtnqltztgj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jqgufenzy.top/gtmzjimmys.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cucudq.cn/gtycwxmmht.html

[B11] 生成数字序列 / 区间
来源：http://hz.0kj1m.cn/gtfvpbvxuo.html

Py:   list(range(0, 10, 2))
来源：http://hz.pycfn.com/gtlnmosnem.html

PHP:  range(0, 10, 2);
来源：http://hz.hammf.cn/gtqnfhwpgf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ybcxt.top/gtckrsxxet.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sysykeji.top/gtysrmqmkc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.daria6918.cn/gtpthigtok.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hnxiangtu.top/gtmxcjgije.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ybcxt.top/gtgszsxxai.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhengqikj.top/gtscvykyvm.html

[B12] 跳出多层循环
来源：http://hz.chenlongwang.top/gtjkysarjy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.daria6918.cn/gtbgncjjan.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xylfe.cn/gtloxejndg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tian-w.cn/gtmfvxjpjr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gthuavwwdn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtzltbhsxg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.52xcode.cn/gtnqpudgml.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.iojbl.cn/gtwfilgonn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.redwolf501.top/gtymprpdgd.html

[B13] 判断是否为数字
来源：http://hz.havefunace.top/gtnkoqcudh.html

Py:   isinstance(x, (int, float))
来源：http://hz.meibo888.top/gtmknbzqox.html

PHP:  is_numeric($x)
来源：http://hz.sysykeji.top/gtwrxgankb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hongshengwenyu.top/gtlupbsfii.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.redwolf501.top/gtygqoxish.html

Java: x instanceof Number
来源：http://hz.chenlongwang.top/gtmfqpxvbu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.aibaodan.cn/gtabrbckbq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.haohaochexian.top/gttfkqoqhe.html

C#:   x is int or double or decimal
来源：http://hz.0kj1m.cn/gtaszdjrhi.html

[B14] 判断值是否在集合内
来源：http://hz.daxiang520.top/gttqkqjfwp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuanzhike.top/gtmvhkqyij.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nwbrower.top/gtibqxcfjz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtmpwnogfy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yj202588.top/gtdtbwdnhd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhengqikj.top/gtcktymtbg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ppjwa.cn/gtkxbjdexx.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nwbrower.top/gtqdaxhday.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtheihqvcq.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangtech.top/gtuxicamco.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtkvomwfye.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258.top/gtazpueapm.html

JS:   a && b || !c
来源：http://hz.snrcjt.cn/gtclnozaoc.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gtgmelmfek.html

Java: a && b || !c
来源：http://hz.yuxming.cn/gtkissctss.html

Go:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtvjqpmcya.html

Ruby: a && b || !c
来源：http://hz.9152youxi.cn/gtcmjvagnv.html

C#:   a && b || !c
来源：http://hz.ydjk.org.cn/gtnutdyoyl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgfzy.top/gtnmviihlw.html

Py:   if not data: return
来源：http://hz.svipenyu.cn/gtspzieycn.html

PHP:  if (!$data) { return; }
来源：http://hz.jinqigfzy.top/gtmgqwkctw.html

JS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtjunnwdnw.html

TS:   if (!data) return;
来源：http://hz.shangyingyoupin.top/gtepxicmad.html

Java: if (data == null) return;
来源：http://hz.sufxvd.cn/gtdvpuusad.html

Go:   if data == nil { return }
来源：http://hz.zhiwuduotai.top/gtkyajrqss.html

Ruby: return if data.nil?
来源：http://hz.ivvv.top/gtkeydfrny.html

C#:   if (data == null) return;
来源：http://hz.c1oappe.top/gtzoyqiauy.html

================================================================================
来源：http://hz.nanxinkj.top/gthyqufuis.html

C. 函数与作用域
来源：http://hz.0kj1m.cn/gtssiltjhi.html

================================================================================
来源：http://hz.sysykeji.top/gtfrvzvqnf.html

[C01] 定义函数
来源：http://hz.chenzaomai.com/gttghaonjm.html

Py:   def add(a, b): return a + b
来源：http://hz.smart0.xyz/gtavmskdwj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtlymkrnhd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sweek.top/gtuthzibou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtvqqtbsyl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtpbjcrzgj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pycfn.com/gtrvkzvtap.html

Ruby: def add(a, b); a + b; end
来源：http://hz.9152youxi.cn/gtxdcpfece.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtugasxxot.html

[C02] 默认参数
来源：http://hz.xuanzx.com/gttmvqdjld.html

Py:   def greet(name="World"): return name
来源：http://hz.gotoacloud.top/gtlxnqlcti.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhoulong.xyz/gtfacfzlab.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hfpthk.cn/gtdyfglrov.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtfssgcgsh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.dashuyun.cn/gtgjlibgwd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuetiantiany.cn/gtihvpopwx.html

Ruby: def greet(name = "World") = name
来源：http://hz.316326.xyz/gtkfxmljfy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.daxiang520.top/gtuqvilxoi.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtkoppmfar.html

Py:   def total(*args): return sum(args)
来源：http://hz.svipenyu.cn/gtgzkbpppw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gotoacloud.top/gtvnbgzpxr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtbuofbfmr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ehwqpu.com/gtzdbrxmrs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydzc1.top/gtlvvfauvn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgfzy.top/gtndsucpup.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.mhx1999.top/gtqsrzdmjq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ywan-chungtsiang.top/gtzapcohqn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gogol.net.cn/gtjiiyejxh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cashguo.top/gtnxiprwio.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yueranfly.top/gtaiqqrotj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sysykeji.top/gtaswijaht.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xylfe.cn/gtdqhiowdu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gotoacloud.top/gtorjonpoe.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gtyvkwxvcn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenzaomai.com/gtnonlmcpn.html

C#:   f(a: 1, b: 2)
来源：http://hz.tanke756.top/gttlivmqhf.html

[C05] 返回多个值
来源：http://hz.fzhhl.top/gtsurvcuhq.html

Py:   return a, b
来源：http://hz.chenzaomai.com/gtwurjrpav.html

PHP:  return [$a, $b];
来源：http://hz.jinqigufen.top/gtyuoxzrij.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gtdehhqsqe.html

TS:   return { a, b };
来源：http://hz.fzhhl.top/gtmydgtehx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hysaishi.cn/gttvadirpc.html

Go:   return a, b
来源：http://hz.yanxiufei.cn/gtsfuwkvzp.html

Ruby: return a, b
来源：http://hz.shzxlz.cn/gtdjetbjdn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinqigufen.top/gtgzdivwhj.html

[C06] 匿名函数 / lambda
来源：http://hz.jinghuilouyu.cn/gtebxqjevp.html

Py:   square = lambda x: x * x
来源：http://hz.nwbrower.top/gtasphhdqs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.feifeiyinyue.top/gtdbmuwnlh.html

JS:   const square = x => x * x;
来源：http://hz.hnxiangtu.top/gtbtypnchc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtdgikghgr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gtwshldbrv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jyoumei.cn/gticjxvhln.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guannengcc.top/gtlkggrawx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sufxvd.cn/gtjmldhdjr.html

[C07] 把函数作为参数传入
来源：http://hz.meibo888.top/gtwsyjkgbk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xingfuxueyuan.xyz/gtnftuuwvz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shuidangran.top/gtqrnxygxf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgufenzy.top/gtjyvrdupn.html

TS:   arr.map(String)
来源：http://hz.cheryme.top/gtdwwcjhua.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.smart0.xyz/gtxtwusggh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinghuilouyu.cn/gtdbzeavkb.html

Ruby: arr.map(&:upcase)
来源：http://hz.birdmap.top/gtqpugeoug.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hammf.cn/gtwyfxgrkt.html

[C08] 闭包
来源：http://hz.shanyushiyangtech.top/gttbvlwgfc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhaomingkeji.xyz/gtukuitsxb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.guowangkeji.top/gtirsvnnlf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtjpupaajy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtnxnfyaxi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.svipenyu.cn/gtuydysspy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yueranfly.top/gtyinjtpxx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinghuilouyu.cn/gthwwsognw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtakzarbcr.html

[C09] 递归
来源：http://hz.cucudq.cn/gtiremouyo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gtnsielfsa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.0kj1m.cn/gtafxxxizn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cucudq.cn/gtvedmpbiu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tanke756.top/gttbocwnno.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dashuyun.cn/gtblyirizi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yueranfly.top/gtqxguesqu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.guowangkeji.top/gtznotdbwz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zdqjudy.top/gtthziqskh.html

[C10] 变量作用域
来源：http://hz.bjfxy.top/gtxbduqgno.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pengpengdd.cyou/gtcmcnrbhb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gaohongyu789.top/gtluxszokg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxuanxn.top/gtgvokqyyn.html

TS:   同 JS
来源：http://hz.pengpengdd.cyou/gtcrdhfcwz.html

Java: 方法内为块级作用域
来源：http://hz.pengpengdd.cyou/gtrirzelxy.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtzwynpjbd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.nanxinkj.top/gtlzvjmkcs.html

C#:   块级作用域
来源：http://hz.wangshuangyany.cn/gtfcddnsmz.html

[C11] 模块导入与导出
来源：http://hz.snrcjt.cn/gtixkkltbp.html

Py:   from module import func
来源：http://hz.hysaishi.cn/gtcmgwylxr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tian-w.cn/gtsbtimrtf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangtech.top/gtibgfvswp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.dianchejie.cn/gtutisswow.html

Java: import java.util.List;
来源：http://hz.cqqwz.cn/gtwlfxycnm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xuetiantiany.cn/gtkpqptiyn.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tian-w.cn/gtaruyguzz.html

C#:   using System.Text;
来源：http://hz.jiagoushi.top/gtuozzfxzv.html

[C12] 立即执行函数 IIFE
来源：http://hz.tian-w.cn/gtdaqnzmtk.html

Py:   (lambda: print("run"))()
来源：http://hz.xinyue.icu/gtcufwcofh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.pycfn.com/gtxxhuevkd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtabtrwssr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtmdmrrage.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cqqwz.cn/gtedfzixrm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hnxiangtu.top/gturftsfhs.html

Ruby: -> { puts "run" }.call
来源：http://hz.sxryk.cn/gtgwwcvnyx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shanyushiyangtech.top/gthkuxhtkx.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtsztryupk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xuanzx.com/gtdqeopscf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtzitchopp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.feifeiyinyue.top/gtvouhidgy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtkremqkjl.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gterhvhkhq.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gtolxjlzgo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.vqdsnc.cn/gtixubdbji.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.9152youxi.cn/gtwkwzstrm.html

[C14] 泛型函数
来源：http://hz.zhoulong.xyz/gtuzyjgmji.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gtwpnjgsrn.html

PHP:  // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtluouqnjd.html

JS:   // 无泛型
来源：http://hz.wangdashe.top/gtjkqxtsaq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hnqzz.top/gttfbhvwgy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yongpay.top/gtopkgretl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenjidiqi.icu/gtfdyemgha.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtpypjkgjj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hnxiangtu.top/gtdptcmqxi.html

[C15] 解构 / 展开参数
来源：http://hz.tian-w.cn/gtteysfvqz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258888.top/gtvhtjibqw.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jyoumei.cn/gtpqhrnpqt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.bjfxy.top/gtlnujkrhf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.kuanghao11.cn/gtkdlfydcp.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtwjjchdqh.html

Go:   // 无解构
来源：http://hz.feifeiyinyue.top/gtoqpyvnyx.html


<!-- 参考信息 -->