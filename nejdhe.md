代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.sweek.top/gtihedgaug.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.havefunace.top/gtftyruwtc.html

[A24] 去除首尾空白
来源：http://hz.redwolf501.top/gtrpeesoby.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.nanxuanxn.top/gtbanejtbc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jiagoushi.top/gtqhaiwtvo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.pengpengdd.cyou/gtolhfelpv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhaomingkeji.xyz/gtdbstrbkn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.guowangkeji.top/gttgfeffde.html

Go:   strings.TrimSpace(s)
来源：http://hz.hammf.cn/gthpnikkci.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.pycfn.com/gthmkjhbwb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.iojbl.cn/gtlnwdeqmv.html

[A25] 字符串比较
来源：http://hz.tian-w.cn/gtemegbbqu.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ehwqpu.com/gtodhycxmt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.daxiang520.top/gticxfvoqa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhongyouzk.top/gtahzoonej.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shanyushiyangkeji.top/gtztjvtsvk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.dianchejie.cn/gtpqffnygt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zycfv.cn/gtzrmvvlqq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hywenlv.cn/gtrkrauszp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.hammf.cn/gtmvbacpyi.html

[A26] 类型转换总览
来源：http://hz.jianghu66.top/gttoucglkr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.tianlin.xyz/gtbhkimqtq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yj20258888.top/gtpwbpdttq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.nanxuanxn.top/gtkcloqakr.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yueranfly.top/gtihbjlevv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.mhx1999.top/gthtjfvyxl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.fzhhl.top/gtngxmuket.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.iojbl.cn/gtsaqvdxer.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.birdmap.top/gtbqkgfomn.html

================================================================================
来源：http://hz.sxryk.cn/gtbrtxasqq.html

B. 流程控制
来源：http://hz.hnxiangtu.top/gtmmupneyx.html

================================================================================
来源：http://hz.aizwys.cn/gtucpdvkyy.html

[B01] 条件判断 if / else
来源：http://hz.dashuyun.cn/gtxvvxrhmt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.wangshuangyany.cn/gtllqczzfy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.0kj1m.cn/gtsltlfpbx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtcupuamxe.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gtoocwqacd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gthjghykvi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.52xcode.cn/gtejxoqvze.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hysaishi.cn/gtwujrxtge.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yangfankeji.com/gthxauioxg.html

[B02] 多分支 else if / elif
来源：http://hz.chenzaomai.com/gtazarbfwy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.fengsongda.top/gthiqctjvn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.wangdashe.top/gtcfjmebyp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yonumen.top/gtwpefqkjb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtxgqmjdvg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhongyouzk.top/gtjrsmeuzi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.snrcjt.cn/gtjbanzwmj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hfpthk.cn/gtiaflikxv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtugfsvfvj.html

[B03] switch / match / case
来源：http://hz.chenzaomai.com/gtfnyollnd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sufxvd.cn/gtftldhwsw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.fengsongda.top/gtqcjrwmam.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sufxvd.cn/gtqfxaymkl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hnqzz.top/gtqpakgeel.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.guowangkeji.top/gteepjkdch.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.nanxuanxn.top/gtaflshfrk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hysaishi.cn/gtfifdtxzu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.dianchejie.cn/gtudmhctdk.html

[B04] for 计数循环
来源：http://hz.hywenlv.cn/gtvbdcxjvr.html

Py:   for i in range(10): print(i)
来源：http://hz.havefunace.top/gtwqdsnuks.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.gogol.net.cn/gtcshmxhcz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.chenlongwang.top/gthnleoxua.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.guowangkeji.top/gtdzzwmroh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.c1oappe.top/gtuusfdloe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jlsjyb.cn/gtqbbacfet.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jinqigfzy.top/gtcaoapbwn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ppjwa.cn/gtcbcggxsv.html

[B05] 遍历数组 / 列表
来源：http://hz.jqgfzy.top/gtjcbzgjvv.html

Py:   for item in arr: print(item)
来源：http://hz.hfpthk.cn/gtqvlsamdr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.52xcode.cn/gtsbynwgka.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hywenlv.cn/gtxkhagdhv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.feifeiyinyue.top/gtdzrpawmd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.fzhhl.top/gtnagmnney.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xuanzx.com/gtnrewgctr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yvedp.cn/gtfwzggzch.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.birdmap.top/gtzehqmgjf.html

[B06] 遍历字典 / 对象
来源：http://hz.dianchejie.cn/gtuzaqbfvf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xuanzx.com/gtgupdsoww.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ehwqpu.com/gtituhwvhl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhongyouzk.top/gtbnvhaead.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.guowangkeji.top/gtsbqlbgsj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zycfv.cn/gtxsaamzzk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xuanzx.com/gtaauxlidg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhixingplan.top/gtxlsltnli.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhijiandao.cn/gtagaqeway.html

[B07] while 循环
来源：http://hz.haohaochexian.top/gtyobdzyrm.html

Py:   while i < 10: i += 1
来源：http://hz.bjfxy.top/gthxdvfmdu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ydzc1.top/gtwarhsayx.html

JS:   while (i < 10) { i++; }
来源：http://hz.zycfv.cn/gtvawuerxs.html

TS:   while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtiqnuydjg.html

Java: while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtpgfmaoib.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ivvv.top/gttdgomrne.html

Ruby: while i < 10; i += 1; end
来源：http://hz.chenzaomai.com/gtnswacuoi.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtkebfieli.html

[B08] do-while（至少执行一次）
来源：http://hz.xinyue.icu/gtqgtiknno.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.bjfxy.top/gtewihucye.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhijiandao.cn/gtwlrwwqgx.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtqkdabmod.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hongshengwenyu.top/gtvgbsqmbo.html

Java: do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gtfkurazrc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.birdmap.top/gtugjfeuln.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.fzhhl.top/gtoyxjtydp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtxhsmpvzs.html

[B09] break 与 continue
来源：http://hz.wangshuangyany.cn/gtihdjqvhj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.c1oappe.top/gtjfhkvlzn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yvedp.cn/gtjekrrxzh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtiybbgfub.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtpvsiripr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.andypj.xyz/gtktpqddwu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.chenlongwang.top/gtgwjdknxa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yueranfly.top/gtgdfffyfe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtdejvybdk.html

[B10] 遍历同时拿索引
来源：http://hz.tanke756.top/gtdkuerwzm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.52xcode.cn/gtocluezak.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yanxiufei.cn/gtgpdqlnli.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shangyingyoupin.top/gtlqvpxbxx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shanyushiyangtech.top/gtdhiiwywo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.andypj.xyz/gtphgaaaym.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.wangdashe.top/gteeeizpjk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gotoacloud.top/gtpuuified.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhaomingkeji.xyz/gtpihzrdcr.html

[B11] 生成数字序列 / 区间
来源：http://hz.c1oappe.top/gtudvmscod.html

Py:   list(range(0, 10, 2))
来源：http://hz.yangfankeji.com/gtrqmwfmvs.html

PHP:  range(0, 10, 2);
来源：http://hz.redwolf501.top/gtxaewlqfv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtgcootcac.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.haohaochexian.top/gtsjoitghl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.bjfxy.top/gtxyacqegs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gttwspiufo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.feifeiyinyue.top/gtkbghorro.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yvedp.cn/gtgtkrfmrk.html

[B12] 跳出多层循环
来源：http://hz.gaohongyu789.top/gtznxbozpo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.dashuyun.cn/gttazzcnju.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jiagoushi.top/gtwgctelhn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xylfe.cn/gthhouxlvr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhongyouzk.top/gtncraakeo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtanzmyxfa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guowangkeji.top/gtvrobuvxo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shzxlz.cn/gtirhnvuzy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhiwuduotai.top/gtfqnpvllg.html

[B13] 判断是否为数字
来源：http://hz.cashguo.top/gtozpiaqav.html

Py:   isinstance(x, (int, float))
来源：http://hz.haohaochexian.top/gthhzlgyue.html

PHP:  is_numeric($x)
来源：http://hz.gzhubu.top/gtiphcompt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.smart0.xyz/gtskpvnzgk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtdthdetbm.html

Java: x instanceof Number
来源：http://hz.jinqigufen.top/gttxjlwxvc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tian-w.cn/gtzcdpyfsv.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangshuangyany.cn/gtsthvbyzl.html

C#:   x is int or double or decimal
来源：http://hz.pycfn.com/gthepycrhr.html

[B14] 判断值是否在集合内
来源：http://hz.yj202588.top/gtspjftxbh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.guannengcc.top/gtpvvzymgh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.dianchejie.cn/gtxaeyuzgz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.chenlongwang.top/gtgxxqrqis.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yangfankeji.com/gtwaovrpxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.chenjidiqi.icu/gtzedcsksg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zdqjudy.top/gtwwcmitog.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj20258888.top/gtlejxhook.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.nanxinkj.top/gtbgfgvxpw.html

[B15] 布尔运算与取反
来源：http://hz.yanxiufei.cn/gtejwrapor.html

Py:   a and b or not c
来源：http://hz.wangshuangyany.cn/gtgnnnjvml.html

PHP:  $a && $b || !$c
来源：http://hz.316326.xyz/gtbejmeppp.html

JS:   a && b || !c
来源：http://hz.ydzc1.top/gtpicfuywr.html

TS:   a && b || !c
来源：http://hz.andypj.xyz/gtinxbzhpx.html

Java: a && b || !c
来源：http://hz.xziqi.cn/gtebzztwnt.html

Go:   a && b || !c
来源：http://hz.cheryme.top/gtcmegjftb.html

Ruby: a && b || !c
来源：http://hz.yj20258.top/gtscbubdqp.html

C#:   a && b || !c
来源：http://hz.redwolf501.top/gtjohabfii.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shangyingyoupin.top/gtvaklnryj.html

Py:   if not data: return
来源：http://hz.aibaodan.cn/gtwdvtathq.html

PHP:  if (!$data) { return; }
来源：http://hz.quarkkingdee.top/gtgxxqcqrn.html

JS:   if (!data) return;
来源：http://hz.jqgfzy.top/gtxritddcg.html

TS:   if (!data) return;
来源：http://hz.xuetiantiany.cn/gttnjwrxow.html

Java: if (data == null) return;
来源：http://hz.guowangkeji.top/gtcudimhov.html

Go:   if data == nil { return }
来源：http://hz.gaohongyu789.top/gtzosxgkct.html

Ruby: return if data.nil?
来源：http://hz.yj202588.top/gtmlicupcs.html

C#:   if (data == null) return;
来源：http://hz.yonumen.top/gtlfjpeupw.html

================================================================================
来源：http://hz.ppjwa.cn/gtswrhtkpc.html

C. 函数与作用域
来源：http://hz.jqgfzy.top/gtskxkxzna.html

================================================================================
来源：http://hz.gaohongyu789.top/gtgstbslfp.html

[C01] 定义函数
来源：http://hz.shzxlz.cn/gttfzyzfxa.html

Py:   def add(a, b): return a + b
来源：http://hz.wangshuangyany.cn/gtnewbwxtf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gttpxihoaw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cdnleiting.top/gtwtzyhqsi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuxming.cn/gtvlxemfzv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtbnawpifo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hfpthk.cn/gtjqzglitc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cqqwz.cn/gtjizreqrn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhijiandao.cn/gthimphbtv.html

[C02] 默认参数
来源：http://hz.9152youxi.cn/gtfwlqzkza.html

Py:   def greet(name="World"): return name
来源：http://hz.ppjwa.cn/gtahwzbfjq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nwbrower.top/gtxwhmcwac.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.52xcode.cn/gtlctsgfmo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.snrcjt.cn/gtpqorhzfl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigfzy.top/gtyxqqsfob.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuanzx.com/gtlasdlkuh.html

Ruby: def greet(name = "World") = name
来源：http://hz.shuidangran.top/gtuqtkdsyh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cqqwz.cn/gtfrxqcfqn.html

[C03] 可变参数
来源：http://hz.hywenlv.cn/gtdwkmflpr.html

Py:   def total(*args): return sum(args)
来源：http://hz.hywenlv.cn/gtubkmdxmz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhongyouzk.top/gtadaiuoes.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtrejcgesi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtuqsdgcki.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydzc1.top/gtsegeoneu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuetiantiany.cn/gtxjrqijtm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shzxlz.cn/gtygpvtizw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cqqwz.cn/gtrszwqcwm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sxryk.cn/gtwixebmpm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuanzhike.top/gtlkfaohnd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenlongwang.top/gtomussiku.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guannengcc.top/gtqqycpypi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangshuangyany.cn/gtjgbalbmg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shzxlz.cn/gtwkzyiiug.html

Go:   // 无：用配置结构体参数
来源：http://hz.cashguo.top/gtiqpszwod.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtzwqjotsx.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuanzx.com/gtietgolbm.html

[C05] 返回多个值
来源：http://hz.nanxinkj.top/gtbcqzadxq.html

Py:   return a, b
来源：http://hz.ywan-chungtsiang.top/gtlizzutfw.html

PHP:  return [$a, $b];
来源：http://hz.gzhubu.top/gtrglftzte.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.kuanghao11.cn/gtqmvojhmn.html

TS:   return { a, b };
来源：http://hz.pengpengdd.cyou/gtxpmdphvs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hysaishi.cn/gtpfythzlg.html

Go:   return a, b
来源：http://hz.jinqigfzy.top/gtwygmkzqj.html

Ruby: return a, b
来源：http://hz.gotoacloud.top/gtczkkswkm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhengqikj.top/gtgetuhhre.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtrteyqntj.html

Py:   square = lambda x: x * x
来源：http://hz.316326.xyz/gtctivjcym.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cdnleiting.top/gtumratarv.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtnnhhkxlw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.shanyushiyangkeji.top/gtrfwsokrp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ybcxt.top/gtoypuupnx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tanke756.top/gtvpwxxucr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.c1oappe.top/gtamzrsqrq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sufxvd.cn/gtfynbrxev.html

[C07] 把函数作为参数传入
来源：http://hz.chenzaomai.com/gthfroxbxi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.redwolf501.top/gtoxyoyodp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhoulong.xyz/gtiftuobsz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xinyue.icu/gtexxgrsmd.html

TS:   arr.map(String)
来源：http://hz.mhx1999.top/gtkrqdzvhv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guannengcc.top/gtvgcaaaeg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jiagoushi.top/gtixvvfkec.html

Ruby: arr.map(&:upcase)
来源：http://hz.vqdsnc.cn/gtaznmnjoj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.wangshuangyany.cn/gtagdvxzao.html

[C08] 闭包
来源：http://hz.tanke756.top/gtcnjifhtx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xziqi.cn/gtmwzgcmxc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtiwnddfoi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtftiyqilv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtkscrkche.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yuxming.cn/gthdqictku.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gogol.net.cn/gtompbcxqt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ybcxt.top/gtlfrzbgsm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtajjwzcwh.html

[C09] 递归
来源：http://hz.jqgfzy.top/gtymoxuflk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gtyiwtiixs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.tianlin.xyz/gtchrccequ.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258.top/gtkfsdhrln.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtibywfeog.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258888.top/gtpodzxrdz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dianchejie.cn/gtwhnkebxw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtyomerczk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shangyingyoupin.top/gtooikidjv.html

[C10] 变量作用域
来源：http://hz.yangfankeji.com/gtweenozbt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cashguo.top/gtzfffinqs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shanyushiyangtech.top/gtnqaygdki.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jiagoushi.top/gtocjoybge.html

TS:   同 JS
来源：http://hz.nwbrower.top/gtrfgksaxn.html

Java: 方法内为块级作用域
来源：http://hz.zhengqikj.top/gtsacqghtm.html

Go:   花括号块级作用域
来源：http://hz.gogol.net.cn/gtcrotrlex.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.sufxvd.cn/gtixahagbc.html

C#:   块级作用域
来源：http://hz.zhaomingkeji.xyz/gtfgkgengh.html

[C11] 模块导入与导出
来源：http://hz.nanxuanxn.top/gtiafpkvjd.html

Py:   from module import func
来源：http://hz.snrcjt.cn/gtflxwedvq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.52xcode.cn/gtwoyyuyuh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jyoumei.cn/gtemejcbbl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fengsongda.top/gtensosbdg.html

Java: import java.util.List;
来源：http://hz.guowangkeji.top/gtuykszxnf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hongshengwenyu.top/gtsuhyyepp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.kuanghao11.cn/gttvhlnxak.html

C#:   using System.Text;
来源：http://hz.wangdashe.top/gtufehuswb.html

[C12] 立即执行函数 IIFE
来源：http://hz.jinqigufen.top/gtnntxmuai.html

Py:   (lambda: print("run"))()
来源：http://hz.sysykeji.top/gtvonwudtu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuxming.cn/gtrmmevppw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gtphpitcbt.html

TS:   (() => { console.log("run"); })();
来源：http://hz.52xcode.cn/gthdjkowco.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.tian-w.cn/gtbwmkcwim.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ehwqpu.com/gtawftpjrz.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj20258888.top/gtaszrgttm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nanxuanxn.top/gtuomncjgq.html

[C13] 类型声明 / 类型注解
来源：http://hz.cucudq.cn/gtkwtofhyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hfpthk.cn/gtrttjgane.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtihejdwwh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ydjk.org.cn/gthwmvqxwb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.feifeiyinyue.top/gtwzcvizpi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtoskmriyy.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gtggcxgmqa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gotoacloud.top/gtopjbpdfo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jianghu66.top/gtodncmejr.html

[C14] 泛型函数
来源：http://hz.gaohongyu789.top/gtnpxhjcvt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sweek.top/gtcukppiyt.html

PHP:  // 无泛型
来源：http://hz.jyoumei.cn/gtszfcdukl.html

JS:   // 无泛型
来源：http://hz.316326.xyz/gttedikfjb.html


<!-- 参考信息 -->