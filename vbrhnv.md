代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://hz.daria6918.cn/gtjdbiyfcy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinqigfzy.top/gtlgwyggqs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.xuanzx.com/gtuzuibyyr.html

[A25] 字符串比较
来源：http://hz.redwolf501.top/gtmykahecy.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jianghu66.top/gtqhdmfrqh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.nwbrower.top/gthvhusjbo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhixingplan.top/gthhnzepdd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cashguo.top/gtgphadcki.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yj20258.top/gtxqathgri.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sysykeji.top/gtcjrajkhi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hnxiangtu.top/gtwlhdgofj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.hysaishi.cn/gtjwzyekfj.html

[A26] 类型转换总览
来源：http://hz.yongpay.top/gtxhvnorob.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jinqigufen.top/gtlyysmgtw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cashguo.top/gtbghofexb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.wangshuangyany.cn/gtyrmcesae.html

TS:   Number() String() Boolean() x as number
来源：http://hz.hfpthk.cn/gtargpljax.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ydzc1.top/gtenpnwiji.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hongshengwenyu.top/gtxycvudvp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ivvv.top/gtffyozmiy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.redwolf501.top/gtcyhbmmrk.html

================================================================================
来源：http://hz.ppjwa.cn/gtbtowezkv.html

B. 流程控制
来源：http://hz.sxryk.cn/gtuohxrcvn.html

================================================================================
来源：http://hz.gzhubu.top/gtudpvyrkz.html

[B01] 条件判断 if / else
来源：http://hz.zhengqikj.top/gtonrtueem.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.0kj1m.cn/gtnjalkphj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.chenzaomai.com/gtgwfpuwru.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtbfonnsju.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.pycfn.com/gtuvdgszip.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gtuxdgelng.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.guowangkeji.top/gtynuglmsq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hfpthk.cn/gthplwouxf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.fengsongda.top/gtlyemibzm.html

[B02] 多分支 else if / elif
来源：http://hz.cqqwz.cn/gtqifmlqqh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jiagoushi.top/gtbuteonqv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.dashuyun.cn/gtqyngrefy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtchicbqva.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guowangkeji.top/gtdehreeam.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtfnftmbup.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yvedp.cn/gttxvontbg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.birdmap.top/gtxzocsctu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhixingplan.top/gtrucqkzxb.html

[B03] switch / match / case
来源：http://hz.snrcjt.cn/gtarqjpyyq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.guowangkeji.top/gtroqqkjyt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daxiang520.top/gtfzmpddws.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cdnleiting.top/gtgshzjzuo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hnqzz.top/gttqnzzbhu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.pycfn.com/gtbzauegdy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhiwuduotai.top/gtxdahyekx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ybcxt.top/gtzfltorig.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.fengsongda.top/gttmlogoqp.html

[B04] for 计数循环
来源：http://hz.nanxinkj.top/gtxcmohnxc.html

Py:   for i in range(10): print(i)
来源：http://hz.svipenyu.cn/gtscpkppbe.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.daria6918.cn/gtvzwflrvy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hongshengwenyu.top/gtansufkyp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xinyue.icu/gtuehyjgdu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.nanxinkj.top/gtgxgiiueu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.daxiang520.top/gtwltlyvzu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.fengsongda.top/gtcrdgrqke.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ydjk.org.cn/gtsurzhdce.html

[B05] 遍历数组 / 列表
来源：http://hz.quarkkingdee.top/gtqvlhccnc.html

Py:   for item in arr: print(item)
来源：http://hz.gotoacloud.top/gtfecexzps.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yuanzhike.top/gtnlhvwidu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.daxiang520.top/gtzbiavpkx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.haohaochexian.top/gtxteprqsw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.0kj1m.cn/gtvqvyovha.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.wangdashe.top/gtamkszquq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ppjwa.cn/gtrecyfdcc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yongpay.top/gtnupibttj.html

[B06] 遍历字典 / 对象
来源：http://hz.chenlongwang.top/gtzjijqvre.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.gaohongyu789.top/gtmbcneaby.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jqgfzy.top/gtxthgckxa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nwbrower.top/gtgwljtfpl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shanyushiyangtech.top/gtabjnzman.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shuidangran.top/gtluezvqiw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shuidangran.top/gtmuvsundb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.c1oappe.top/gtwmvrvwps.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.tianlin.xyz/gtyqukgyzt.html

[B07] while 循环
来源：http://hz.ywan-chungtsiang.top/gtqpfknexk.html

Py:   while i < 10: i += 1
来源：http://hz.haohaochexian.top/gtpnkfejvy.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sxryk.cn/gtconltcff.html

JS:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtwavbtqrf.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtgdkjviiy.html

Java: while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtirtetdov.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xuanzx.com/gtkljhrqqm.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhixingplan.top/gtstgeiwbr.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtnugcxssz.html

[B08] do-while（至少执行一次）
来源：http://hz.wangdashe.top/gtbealqtdn.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yuanzhike.top/gterhzqxgm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.tianlin.xyz/gtezwwguer.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtwnpmvdil.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinyuanbaomall.cn/gtputqxgfh.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gtydrzarly.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jinqigufen.top/gtihfekhfz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.iojbl.cn/gtxcjytnif.html

C#:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtlimndnve.html

[B09] break 与 continue
来源：http://hz.mhx1999.top/gtubrkdcgx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xuanzx.com/gtkmtbtrom.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhixingplan.top/gtnytpzpcn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtwfbkzkpp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtgdcpjazi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dianchejie.cn/gtmoxjaftj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258888.top/gtjqqzqjqe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xingfuxueyuan.xyz/gttlnegetu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtdnoyxcvg.html

[B10] 遍历同时拿索引
来源：http://hz.yueranfly.top/gtediqaykc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shanyushiyangkeji.top/gtogdqkdha.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gogol.net.cn/gtdkjpeeqm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tianlin.xyz/gtbmktajrn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cashguo.top/gtezexofgu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ydjk.org.cn/gtzketwdry.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.316326.xyz/gtbadvadfy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jianghu66.top/gtjyqqiqmi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.316326.xyz/gttfndcism.html

[B11] 生成数字序列 / 区间
来源：http://hz.birdmap.top/gtihgjqumh.html

Py:   list(range(0, 10, 2))
来源：http://hz.jyoumei.cn/gtsibqyusx.html

PHP:  range(0, 10, 2);
来源：http://hz.zhixingplan.top/gtzbuzrpsr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guannengcc.top/gtovuyuawq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhiwuduotai.top/gtktwktrlu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.nwbrower.top/gtnhtsxrfa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinghuilouyu.cn/gtfsjaikcm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenzaomai.com/gtyifhzheo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hongshengwenyu.top/gtferryhui.html

[B12] 跳出多层循环
来源：http://hz.316326.xyz/gtoworgdyc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shangyingyoupin.top/gtzcqgxhlo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtaptefxkw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtgetsauno.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gthdplakgc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gtifuugjto.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj20258888.top/gtrsncjton.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenzaomai.com/gtljtisbjv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenlongwang.top/gthlkjtlnr.html

[B13] 判断是否为数字
来源：http://hz.redwolf501.top/gtlcoktnii.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnxiangtu.top/gtdmcsugbm.html

PHP:  is_numeric($x)
来源：http://hz.ydjk.org.cn/gtumrcploj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gtrwwhohas.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtlxcvydyf.html

Java: x instanceof Number
来源：http://hz.yueranfly.top/gtrtzkcbcu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.dashuyun.cn/gtqwbxmfut.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jiagoushi.top/gtdlazwifq.html

C#:   x is int or double or decimal
来源：http://hz.jiagoushi.top/gtiovpfuxe.html

[B14] 判断值是否在集合内
来源：http://hz.sufxvd.cn/gtkzagrtcm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hywenlv.cn/gtwgpgrciz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.aizwys.cn/gtnveeszyn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gttskbyauj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtlvgxmnwi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guannengcc.top/gtcdzncnbr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinqigufen.top/gthexlatak.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hfpthk.cn/gtqcogvwpd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jqgufenzy.top/gtticckyme.html

[B15] 布尔运算与取反
来源：http://hz.chenjidiqi.icu/gtehplijdo.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtsfkigiit.html

PHP:  $a && $b || !$c
来源：http://hz.jqgufenzy.top/gtjvfasbhi.html

JS:   a && b || !c
来源：http://hz.hongshengwenyu.top/gtauigaheu.html

TS:   a && b || !c
来源：http://hz.birdmap.top/gtlpxzybdz.html

Java: a && b || !c
来源：http://hz.gaohongyu789.top/gthvldqvmf.html

Go:   a && b || !c
来源：http://hz.tian-w.cn/gtgrmgbnfq.html

Ruby: a && b || !c
来源：http://hz.iojbl.cn/gtdznobugr.html

C#:   a && b || !c
来源：http://hz.yj20258.top/gtnazfigew.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yueranfly.top/gtfuuudzsz.html

Py:   if not data: return
来源：http://hz.jinghuilouyu.cn/gtvvvtzost.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gtoyphnuhz.html

JS:   if (!data) return;
来源：http://hz.bjfxy.top/gtlehfzzpq.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtzeznntad.html

Java: if (data == null) return;
来源：http://hz.svipenyu.cn/gtcavdwtrr.html

Go:   if data == nil { return }
来源：http://hz.jlsjyb.cn/gtjbomgoxl.html

Ruby: return if data.nil?
来源：http://hz.aibaodan.cn/gtdyjksnah.html

C#:   if (data == null) return;
来源：http://hz.bjfxy.top/gteagdeaxs.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtcwkjykoi.html

C. 函数与作用域
来源：http://hz.jlsjyb.cn/gtbnxxekad.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtxqaqtgap.html

[C01] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtylafiusy.html

Py:   def add(a, b): return a + b
来源：http://hz.gotoacloud.top/gtnnyfhenv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtmoqxpqde.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nanxinkj.top/gtvianlezz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.52xcode.cn/gthyskngyi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtaxuadgks.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.316326.xyz/gttnhhgohf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nanxuanxn.top/gtsewuzggq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtragusuqr.html

[C02] 默认参数
来源：http://hz.nanxuanxn.top/gtniaspzwi.html

Py:   def greet(name="World"): return name
来源：http://hz.snrcjt.cn/gtriamwluj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yonumen.top/gtlgsumnvh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtsktphfsz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gtagqgukhg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.feifeiyinyue.top/gtxuycggdh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hnqzz.top/gtcxjgijot.html

Ruby: def greet(name = "World") = name
来源：http://hz.gogol.net.cn/gtnfsfbcie.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtahglttom.html

[C03] 可变参数
来源：http://hz.xziqi.cn/gtylyqkufv.html

Py:   def total(*args): return sum(args)
来源：http://hz.redwolf501.top/gtibydbixj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xingfuxueyuan.xyz/gtndxdqgyk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtqgbpfmmv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daria6918.cn/gtiftdffba.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhixingplan.top/gtqtmlxphs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sufxvd.cn/gtrzlngtyb.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shuidangran.top/gtkgvvvmdo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gogol.net.cn/gtuevasafn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuanzhike.top/gtatanuszu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yanxiufei.cn/gtsyncbgqe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jiagoushi.top/gtlwtdovpg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.vqdsnc.cn/gtpexzhfra.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.mhx1999.top/gtavnlyvfz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sufxvd.cn/gtekipbume.html

Go:   // 无：用配置结构体参数
来源：http://hz.daria6918.cn/gtjndkdimg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gthmmdqppi.html

C#:   f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtoegkdsax.html

[C05] 返回多个值
来源：http://hz.yvedp.cn/gtzixllgux.html

Py:   return a, b
来源：http://hz.yonumen.top/gtnzeohrqq.html

PHP:  return [$a, $b];
来源：http://hz.pengpengdd.cyou/gtnludssnv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cqqwz.cn/gtvjstbsyc.html

TS:   return { a, b };
来源：http://hz.cashguo.top/gtnvwliltn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yj20258888.top/gtfwsudwrf.html

Go:   return a, b
来源：http://hz.wangdashe.top/gtbdorvtkl.html

Ruby: return a, b
来源：http://hz.cdnleiting.top/gtwpmkwyxp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yongpay.top/gtbjobfgtg.html

[C06] 匿名函数 / lambda
来源：http://hz.redwolf501.top/gtmnujzdjn.html

Py:   square = lambda x: x * x
来源：http://hz.yanxiufei.cn/gtqmmzbiyw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pycfn.com/gtgqlrkjtf.html

JS:   const square = x => x * x;
来源：http://hz.ydzc1.top/gtzfshhxpe.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ywan-chungtsiang.top/gtwtfflbtq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.nanxuanxn.top/gtzeethiex.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuanzhike.top/gtjqdzsrdt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sxryk.cn/gtdvjovutw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.redwolf501.top/gtuvcfkxxs.html

[C07] 把函数作为参数传入
来源：http://hz.jyoumei.cn/gtstuqsawz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.shzxlz.cn/gtmlqrbmdx.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tianlin.xyz/gtqfqbiziu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenjidiqi.icu/gtmotxurqo.html

TS:   arr.map(String)
来源：http://hz.tian-w.cn/gtjmqejqdj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.pengpengdd.cyou/gtfnstjnmh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenjidiqi.icu/gttikxpsto.html

Ruby: arr.map(&:upcase)
来源：http://hz.cqqwz.cn/gtgubczvwt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yvedp.cn/gtagiqhgta.html

[C08] 闭包
来源：http://hz.jinqigfzy.top/gtvgtgjktq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.52xcode.cn/gtsbjrahrx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtahfcahkp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtsphahyxq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtwrrmodge.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ybcxt.top/gtqquxixdt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.meibo888.top/gtsglydzhx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.316326.xyz/gtjqeqjvyi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtxnjqufqg.html

[C09] 递归
来源：http://hz.jyoumei.cn/gthdqehtxc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.andypj.xyz/gtztiyicio.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aibaodan.cn/gttxqgaofh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.wangdashe.top/gtobiwskaa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.redwolf501.top/gtafumareg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnxiangtu.top/gtkelpvrlb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jyoumei.cn/gtkzpcaqeu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtdniuwecd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.fengsongda.top/gtnoqdwpma.html

[C10] 变量作用域
来源：http://hz.yongpay.top/gtwdszkpxo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yvedp.cn/gtbwipumpy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ywan-chungtsiang.top/gtztfugsph.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhongyouzk.top/gtarqwymkn.html

TS:   同 JS
来源：http://hz.birdmap.top/gtlrtjajyp.html

Java: 方法内为块级作用域
来源：http://hz.gaohongyu789.top/gthdjkgnlh.html

Go:   花括号块级作用域
来源：http://hz.jinyuanbaomall.cn/gthpjowtid.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.kuanghao11.cn/gtfktntaah.html

C#:   块级作用域
来源：http://hz.jinqigfzy.top/gtmptnlyxx.html

[C11] 模块导入与导出
来源：http://hz.meibo888.top/gtfxvlnhcr.html

Py:   from module import func
来源：http://hz.hysaishi.cn/gtipkmnfac.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.52xcode.cn/gthepluzrl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.bjfxy.top/gtubkvauje.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhiwuduotai.top/gtpvslqaim.html

Java: import java.util.List;
来源：http://hz.haohaochexian.top/gtzqrgsnhd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ybcxt.top/gtpbnkutxo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.0kj1m.cn/gtlyvqccno.html

C#:   using System.Text;
来源：http://hz.yuxming.cn/gtbuicogda.html

[C12] 立即执行函数 IIFE
来源：http://hz.cheryme.top/gtjltcijdo.html

Py:   (lambda: print("run"))()
来源：http://hz.aibaodan.cn/gtebxqivaw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shangyingyoupin.top/gtkytktjqt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ywan-chungtsiang.top/gttmbcmxhs.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xuanzx.com/gtzoiecksb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hongshengwenyu.top/gtqsuelmus.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cdnleiting.top/gtjtwyhhae.html

Ruby: -> { puts "run" }.call
来源：http://hz.gzhubu.top/gtxmsnjoqz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jlsjyb.cn/gtpxvixdmo.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnxiangtu.top/gtpqguymuh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhaomingkeji.xyz/gtutakffah.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtmowrflhl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgfzy.top/gtarlcoebf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.haohaochexian.top/gtejfcbgqd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.pycfn.com/gtuwzzwqws.html

Go:   func add(a, b int) int
来源：http://hz.jqgfzy.top/gtswczwqtq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dianchejie.cn/gthoosrlan.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jianghu66.top/gtescuedzb.html

[C14] 泛型函数
来源：http://hz.guannengcc.top/gtvpflyuuq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yangfankeji.com/gtxekvkpre.html

PHP:  // 无泛型
来源：http://hz.yj202588.top/gtsodebpga.html

JS:   // 无泛型
来源：http://hz.52xcode.cn/gtxartfxay.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangkeji.top/gtfhmtfalj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.52xcode.cn/gtmqlnwgnm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.havefunace.top/gtywpgqdbs.html

Ruby: # 无泛型
来源：http://hz.hammf.cn/gtjcpizyee.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sufxvd.cn/gtpbtwrlfj.html

[C15] 解构 / 展开参数
来源：http://hz.chenjidiqi.icu/gtnqjulknz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cdnleiting.top/gtjjheemxi.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yongpay.top/gthrpoicim.html


<!-- 参考信息 -->