代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.gotoacloud.top/gtkfigdkhv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.haohaochexian.top/gttjrbbexk.html

[A24] 去除首尾空白
来源：http://hz.chenzaomai.com/gtgcdajhks.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shanyushiyangtech.top/gtazecolfg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.sweek.top/gthzlfeiyx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.guowangkeji.top/gtgrqqnrdx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangdashe.top/gtruspdfob.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yonumen.top/gtuelcjjkf.html

Go:   strings.TrimSpace(s)
来源：http://hz.tianlin.xyz/gtbgzhkhgr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jianghu66.top/gtkuuuhmsw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shanyushiyangkeji.top/gtnpqjautx.html

[A25] 字符串比较
来源：http://hz.zdqjudy.top/gtpitepgjr.html

Py:   s1 == s2; s1 != s2
来源：http://hz.sweek.top/gtlltbciil.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.xziqi.cn/gtcwjtdxrm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yj20258888.top/gtxrikqkdm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xuetiantiany.cn/gtmdaqisxm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.quarkkingdee.top/gtrvnudhrm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sweek.top/gtgunfnlev.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ehwqpu.com/gtfklualce.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jinqigufen.top/gtnlegzqgb.html

[A26] 类型转换总览
来源：http://hz.aibaodan.cn/gtpfrbqrdr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jlsjyb.cn/gtqgopickv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.9152youxi.cn/gtframnstx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.svipenyu.cn/gthcxncndd.html

TS:   Number() String() Boolean() x as number
来源：http://hz.shanyushiyangtech.top/gtztrfwtbk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.sweek.top/gtryrbsowv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jianghu66.top/gtigypgtnx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.wangdashe.top/gtajwabgps.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.316326.xyz/gtzcyogfbc.html

================================================================================
来源：http://hz.jinqigufen.top/gtdndtrvyx.html

B. 流程控制
来源：http://hz.ywan-chungtsiang.top/gtskynbqvf.html

================================================================================
来源：http://hz.andypj.xyz/gtezyqpjxo.html

[B01] 条件判断 if / else
来源：http://hz.gaohongyu789.top/gtuejxgfzi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.pengpengdd.cyou/gtshzzrtrn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhengqikj.top/gtycakfrdk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yanxiufei.cn/gtgujdknit.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.haohaochexian.top/gtzgmudmii.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.daria6918.cn/gtvirvaoye.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jianghu66.top/gtdwnhdnwy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cdnleiting.top/gtfmbjqlxk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gthjarfsbu.html

[B02] 多分支 else if / elif
来源：http://hz.havefunace.top/gtessbwiys.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj20258.top/gtacokpeox.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shangyingyoupin.top/gtoggjbpni.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtjzqrcyoc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhengqikj.top/gthgjqitsu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hywenlv.cn/gtxwkwankq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.guannengcc.top/gtqkormcnb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yuxming.cn/gtypqewper.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gtioweasre.html

[B03] switch / match / case
来源：http://hz.jinqigufen.top/gtoqjshxnb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jlsjyb.cn/gthwrcrciu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gtzccyecfz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.svipenyu.cn/gtujojcibw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhoulong.xyz/gtfxlwppwc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zhongyouzk.top/gtosfxbtvk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.pycfn.com/gtoepppfvq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.nwbrower.top/gtzczcspfw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ybcxt.top/gtxryxqloc.html

[B04] for 计数循环
来源：http://hz.yangfankeji.com/gthdqyzmoh.html

Py:   for i in range(10): print(i)
来源：http://hz.c1oappe.top/gtixsoqdqy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.meibo888.top/gtezasyxcw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.0kj1m.cn/gtjthyegrh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.iojbl.cn/gtealgphmj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.smart0.xyz/gthdcmffkg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.pengpengdd.cyou/gtdschwnjg.html

Ruby: 10.times { |i| puts i }
来源：http://hz.meibo888.top/gtljenftyv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tian-w.cn/gtfuolxsxc.html

[B05] 遍历数组 / 列表
来源：http://hz.cdnleiting.top/gtdgbzbpgb.html

Py:   for item in arr: print(item)
来源：http://hz.zhoulong.xyz/gtvkgufrrb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sufxvd.cn/gtsfursnnv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.wangshuangyany.cn/gtnwjbpdwg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xingfuxueyuan.xyz/gthnrqmhfd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.kuanghao11.cn/gtjcwfrbcn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yangfankeji.com/gtmygyneuq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sweek.top/gtmpdvawpe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hnxiangtu.top/gtglycdwby.html

[B06] 遍历字典 / 对象
来源：http://hz.quarkkingdee.top/gtkpgacbrv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.9152youxi.cn/gtxiamugav.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.tian-w.cn/gtjfvakezo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yongpay.top/gtkuqreucp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aibaodan.cn/gtcrcrlnud.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cqqwz.cn/gtyilrgnts.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.fengsongda.top/gtueakdshr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.smart0.xyz/gtpjhvinoy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinyuanbaomall.cn/gtoeognozk.html

[B07] while 循环
来源：http://hz.iojbl.cn/gtdwedhgoc.html

Py:   while i < 10: i += 1
来源：http://hz.hnqzz.top/gthhvuzysi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.0kj1m.cn/gtzwnsdzxi.html

JS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gthgadimzk.html

TS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtbyrkfqke.html

Java: while (i < 10) { i++; }
来源：http://hz.pycfn.com/gtqdysuguh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xuetiantiany.cn/gtarsjhtaf.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jqgufenzy.top/gtmvabgefs.html

C#:   while (i < 10) { i++; }
来源：http://hz.wangdashe.top/gtzratxqzd.html

[B08] do-while（至少执行一次）
来源：http://hz.sysykeji.top/gtcfwrntli.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinqigufen.top/gtegcxmrvs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ybcxt.top/gttoqipwwh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangkeji.top/gtghifoslr.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinyuanbaomall.cn/gtgcajhfgn.html

Java: do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtusbvptlj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yueranfly.top/gtfoeafsxs.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cucudq.cn/gtvgrwtuve.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtrjyfkwar.html

[B09] break 与 continue
来源：http://hz.cucudq.cn/gtebzzpobp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shangyingyoupin.top/gtgdmjmqmg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jqgfzy.top/gthymxbkaa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtzvwtofem.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.birdmap.top/gtfiacbkff.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtjkhnwbtg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xziqi.cn/gtlrtmngdt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.fengsongda.top/gtvtgoynvz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jiagoushi.top/gtgmoxzycf.html

[B10] 遍历同时拿索引
来源：http://hz.hysaishi.cn/gtvpcrmwac.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ppjwa.cn/gtqdpvdpfe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daxiang520.top/gtlnceehcz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.316326.xyz/gtvpyhdnnw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.chenzaomai.com/gtoylnkuae.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jiagoushi.top/gtgjqooxfr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hywenlv.cn/gtbqthibwb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shzxlz.cn/gtihnujhow.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.fengsongda.top/gtopvwmpwl.html

[B11] 生成数字序列 / 区间
来源：http://hz.yanxiufei.cn/gtuwaiqqhf.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhiwuduotai.top/gtbsfxjxuq.html

PHP:  range(0, 10, 2);
来源：http://hz.zhengqikj.top/gtnqmhktpe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtimqcolrj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenjidiqi.icu/gtidmwtrlp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.0kj1m.cn/gtffiqkkyj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhongyouzk.top/gtynztuksq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yonumen.top/gtsxticrqc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhijiandao.cn/gtgltqfxff.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangkeji.top/gthrmkraim.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yj20258.top/gtpsmcvlqp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jqgufenzy.top/gtkdfuatak.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhoulong.xyz/gtbqwfmkbo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.gotoacloud.top/gtjlhlaxhg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtsgntanxc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guannengcc.top/gtbafpwkzl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guannengcc.top/gtojrtkugb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jyoumei.cn/gtmqedupur.html

[B13] 判断是否为数字
来源：http://hz.zdqjudy.top/gtdrlhdsdf.html

Py:   isinstance(x, (int, float))
来源：http://hz.sxryk.cn/gtekdnaczm.html

PHP:  is_numeric($x)
来源：http://hz.xuetiantiany.cn/gtmbuhksmy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtkyomjtjv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangshuangyany.cn/gtnecewkob.html

Java: x instanceof Number
来源：http://hz.tian-w.cn/gtaaqtxyzu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.fengsongda.top/gtszpwcvjk.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhiwuduotai.top/gtsoiigmgu.html

C#:   x is int or double or decimal
来源：http://hz.tianlin.xyz/gtjstovwvj.html

[B14] 判断值是否在集合内
来源：http://hz.zhaomingkeji.xyz/gtemisetjd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenlongwang.top/gtjqrvevpf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ywan-chungtsiang.top/gtggjlsfcj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtfpzspmoh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hnxiangtu.top/gtcrirhaud.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtksfygrpw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.c1oappe.top/gtwgufcqvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sweek.top/gtlnamodoa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhengqikj.top/gtbrtrjihw.html

[B15] 布尔运算与取反
来源：http://hz.havefunace.top/gthjoojmnd.html

Py:   a and b or not c
来源：http://hz.jinyuanbaomall.cn/gtesljxulk.html

PHP:  $a && $b || !$c
来源：http://hz.sxryk.cn/gtovxxvgha.html

JS:   a && b || !c
来源：http://hz.shzxlz.cn/gtkutdksue.html

TS:   a && b || !c
来源：http://hz.zycfv.cn/gtnzbbgqws.html

Java: a && b || !c
来源：http://hz.yj20258.top/gtzvhbvrgx.html

Go:   a && b || !c
来源：http://hz.zdqjudy.top/gtdlrinzim.html

Ruby: a && b || !c
来源：http://hz.smart0.xyz/gtvfukeess.html

C#:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtmqrjsctk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.smart0.xyz/gtkgptveaa.html

Py:   if not data: return
来源：http://hz.xuetiantiany.cn/gtswbzeaqp.html

PHP:  if (!$data) { return; }
来源：http://hz.ydzc1.top/gtiayiaroj.html

JS:   if (!data) return;
来源：http://hz.cdnleiting.top/gtpiofskir.html

TS:   if (!data) return;
来源：http://hz.yueranfly.top/gttjmjgqvf.html

Java: if (data == null) return;
来源：http://hz.shuidangran.top/gtxlqvzktw.html

Go:   if data == nil { return }
来源：http://hz.jinghuilouyu.cn/gtkuufqall.html

Ruby: return if data.nil?
来源：http://hz.52xcode.cn/gtbfctzfbi.html

C#:   if (data == null) return;
来源：http://hz.zhengqikj.top/gtlvfjkhea.html

================================================================================
来源：http://hz.ydjk.org.cn/gtaolzauin.html

C. 函数与作用域
来源：http://hz.xuanzx.com/gtncxahbvr.html

================================================================================
来源：http://hz.ydzc1.top/gtrgxltkuz.html

[C01] 定义函数
来源：http://hz.dashuyun.cn/gtsvmxshug.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigfzy.top/gtthhgksrt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigfzy.top/gtouvvuiur.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.bjfxy.top/gtukwdiaff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gthmtngcof.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtiywahacr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.316326.xyz/gtlovmjspx.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jianghu66.top/gtnipdomfa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtosbynsud.html

[C02] 默认参数
来源：http://hz.aizwys.cn/gthcwywlrn.html

Py:   def greet(name="World"): return name
来源：http://hz.nwbrower.top/gtywhmicih.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.feifeiyinyue.top/gtpfmjkhwr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinqigfzy.top/gtyaoiblvi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtvboelrfl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgfzy.top/gtzoakclco.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hammf.cn/gtgcmffmob.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxuanxn.top/gtcwlewdpw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenjidiqi.icu/gttuhbqsgn.html

[C03] 可变参数
来源：http://hz.daria6918.cn/gtdyysyyhf.html

Py:   def total(*args): return sum(args)
来源：http://hz.quarkkingdee.top/gtvaayrwui.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sxryk.cn/gtgkqpzwqj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtahaddebb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtoiirddnv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.wangdashe.top/gtnnuqdknx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xziqi.cn/gtngsusoky.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gzhubu.top/gtbgfahzdu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xingfuxueyuan.xyz/gtfcgzsuvy.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ybcxt.top/gtjearsfxk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhixingplan.top/gtfnoewezi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.birdmap.top/gthknzdyzt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cdnleiting.top/gtuxqlcogq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.havefunace.top/gtzpwcgkhy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnxiangtu.top/gtwqujvzmn.html

Go:   // 无：用配置结构体参数
来源：http://hz.birdmap.top/gtvsccsgjo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.0kj1m.cn/gtxcgatkdk.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtcixenanr.html

[C05] 返回多个值
来源：http://hz.ydjk.org.cn/gtltrpaoda.html

Py:   return a, b
来源：http://hz.ydzc1.top/gtxmtgzhlk.html

PHP:  return [$a, $b];
来源：http://hz.shangyingyoupin.top/gtiurkzoxk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pengpengdd.cyou/gtkcsgfwjl.html

TS:   return { a, b };
来源：http://hz.zdqjudy.top/gtdmwkxtjm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.bjfxy.top/gtvdwuskcr.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtxdvnvvrk.html

Ruby: return a, b
来源：http://hz.gzhubu.top/gtiolfmtab.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydjk.org.cn/gtmupoakjj.html

[C06] 匿名函数 / lambda
来源：http://hz.pycfn.com/gtpfjunshz.html

Py:   square = lambda x: x * x
来源：http://hz.gaohongyu789.top/gtasqrasbb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zycfv.cn/gtubalrtkn.html

JS:   const square = x => x * x;
来源：http://hz.zhoulong.xyz/gttklnzjkz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yuanzhike.top/gthzwbekvj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gtgahmkezm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhongyouzk.top/gtekhfhsms.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj202588.top/gtdkbnfuuz.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhengqikj.top/gtpcmdnuxn.html

[C07] 把函数作为参数传入
来源：http://hz.smart0.xyz/gtgxjmwigu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gogol.net.cn/gtltvcgyjz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ydjk.org.cn/gtxvqvtfut.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhengqikj.top/gtxtlpgsxy.html

TS:   arr.map(String)
来源：http://hz.hfpthk.cn/gthbxkdvgu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.aibaodan.cn/gtugggtodw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtjthcspxy.html

Ruby: arr.map(&:upcase)
来源：http://hz.shuidangran.top/gtwuvsoclt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.haohaochexian.top/gtvpqtdufk.html

[C08] 闭包
来源：http://hz.shanyushiyangtech.top/gtjzfdkprq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zdqjudy.top/gtujvdlzjn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yanxiufei.cn/gtwiwystzo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtuwrjmiwo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtugadcgde.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.vqdsnc.cn/gtfpaszecp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.vqdsnc.cn/gtrgspfhgu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.vqdsnc.cn/gtqkyzpkgy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sufxvd.cn/gtvhrtnlqk.html

[C09] 递归
来源：http://hz.gzhubu.top/gtaguquzaw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuxming.cn/gtjuovsuto.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.birdmap.top/gtkkaqjbua.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtadbgupqz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtuuplfryr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gaohongyu789.top/gtkauhurxp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xziqi.cn/gtbphuavuh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dianchejie.cn/gtdatkzxvr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtonwuthih.html

[C10] 变量作用域
来源：http://hz.zhiwuduotai.top/gtcgpdzkid.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guowangkeji.top/gtcgmumppi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xingfuxueyuan.xyz/gtwbmbeabj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.havefunace.top/gtmethgnfj.html

TS:   同 JS
来源：http://hz.shanyushiyangkeji.top/gtqgiaxutq.html

Java: 方法内为块级作用域
来源：http://hz.zhoulong.xyz/gtncxoqauq.html

Go:   花括号块级作用域
来源：http://hz.svipenyu.cn/gtaucxryak.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pengpengdd.cyou/gtvsinjzxt.html

C#:   块级作用域
来源：http://hz.jinghuilouyu.cn/gtlnjnqkhy.html

[C11] 模块导入与导出
来源：http://hz.zhixingplan.top/gtmycwgnrq.html

Py:   from module import func
来源：http://hz.cdnleiting.top/gthsarcfxp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.redwolf501.top/gttdrzicbo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ybcxt.top/gtwbznumgy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hongshengwenyu.top/gttokchqmf.html

Java: import java.util.List;
来源：http://hz.yj20258.top/gtmksfvdos.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.hongshengwenyu.top/gtybvfbktj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ehwqpu.com/gtufhnlwjf.html

C#:   using System.Text;
来源：http://hz.hysaishi.cn/gtuifvsmcr.html

[C12] 立即执行函数 IIFE
来源：http://hz.ppjwa.cn/gtqnohhnoz.html

Py:   (lambda: print("run"))()
来源：http://hz.daxiang520.top/gtuicprthv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.feifeiyinyue.top/gtknyujovo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gtvrbatabp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xziqi.cn/gtilmxssfa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yanxiufei.cn/gtuexyceia.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.daxiang520.top/gtnmnjkaee.html

Ruby: -> { puts "run" }.call
来源：http://hz.0kj1m.cn/gtxwgachcr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.bjfxy.top/gtnocayxeb.html

[C13] 类型声明 / 类型注解
来源：http://hz.yj20258.top/gtnwpqgzfg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hywenlv.cn/gtnogxyzgk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.quarkkingdee.top/gtomwaeohy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yangfankeji.com/gtuxqsxweg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtzajmxgph.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtnggdwctf.html

Go:   func add(a, b int) int
来源：http://hz.ivvv.top/gtrcmtbefm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cheryme.top/gtxaynlsdb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangdashe.top/gtolplybjn.html

[C14] 泛型函数
来源：http://hz.jqgfzy.top/gtnkyltonb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jianghu66.top/gtnzzwolvw.html

PHP:  // 无泛型
来源：http://hz.pycfn.com/gtpbftmqft.html

JS:   // 无泛型
来源：http://hz.dashuyun.cn/gtpjtwxqst.html


<!-- 参考信息 -->