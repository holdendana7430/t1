代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hfpthk.cn/gtpkvnnfym.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.guowangkeji.top/gtxbpzptay.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yvedp.cn/gtkfympdrq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yj202588.top/gtygyttqyw.html

Go:   strings.TrimSpace(s)
来源：http://hz.yueranfly.top/gtrywnacog.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.shangyingyoupin.top/gtqazkvwlq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cheryme.top/gtxhehyyga.html

[A25] 字符串比较
来源：http://hz.cdnleiting.top/gtkzrqjbjw.html

Py:   s1 == s2; s1 != s2
来源：http://hz.chenlongwang.top/gthyxbsray.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.gzhubu.top/gtxxaxjvvn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ybcxt.top/gtwcfnariw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhoulong.xyz/gtytxfdcoe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xuanzx.com/gtgdmyzadb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hnxiangtu.top/gtnjfuhohg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sxryk.cn/gtqulxbuyj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.redwolf501.top/gtxgmjlfbv.html

[A26] 类型转换总览
来源：http://hz.yueranfly.top/gtsqfeopjh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yuanzhike.top/gtbwutduvi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.fengsongda.top/gtzakqdhwt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yonumen.top/gtcuizfzft.html

TS:   Number() String() Boolean() x as number
来源：http://hz.fzhhl.top/gtqcwicmvo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cdnleiting.top/gtgahyudud.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.quarkkingdee.top/gtekrulmwd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.vqdsnc.cn/gtagmfhknt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shangyingyoupin.top/gtjcxabsgu.html

================================================================================
来源：http://hz.yj20258.top/gtqykcfiwy.html

B. 流程控制
来源：http://hz.pycfn.com/gtefnfpqnm.html

================================================================================
来源：http://hz.guannengcc.top/gtmzxiqame.html

[B01] 条件判断 if / else
来源：http://hz.sysykeji.top/gtrxjwxkcw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.chenzaomai.com/gtfkiurahy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.316326.xyz/gtbmuccocl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.snrcjt.cn/gtclzrkvxr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gotoacloud.top/gtdgvhjyhb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zdqjudy.top/gtaesvukyc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhongyouzk.top/gtkumylyix.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.aizwys.cn/gtrburoepr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.wangdashe.top/gtzgghfdpu.html

[B02] 多分支 else if / elif
来源：http://hz.zhiwuduotai.top/gtalmlyyot.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zycfv.cn/gtohrciyff.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj202588.top/gtzbidxwgm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtmcvkekqc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sxryk.cn/gtmqrekhka.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gtqutuacst.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.birdmap.top/gtmylzuhkq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.chenlongwang.top/gtbqawepnn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.haohaochexian.top/gtlptkaidm.html

[B03] switch / match / case
来源：http://hz.c1oappe.top/gtdmrcpppb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jlsjyb.cn/gtxbtyklwh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jiagoushi.top/gthaosobgo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenjidiqi.icu/gtbllbiujk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nwbrower.top/gtgtdizsfk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sxryk.cn/gtbmavkmla.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.pengpengdd.cyou/gteoylfbag.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnxiangtu.top/gtglsvfyew.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ywan-chungtsiang.top/gtzbkmmyni.html

[B04] for 计数循环
来源：http://hz.yj202588.top/gtbjphalyj.html

Py:   for i in range(10): print(i)
来源：http://hz.ehwqpu.com/gtsawrbwsj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shuidangran.top/gtsehfpube.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuanzx.com/gtmdhkivod.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.0kj1m.cn/gtjyhebrpg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xylfe.cn/gtuurwpdsp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xuanzx.com/gtdistrebd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cqqwz.cn/gtthwewveg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.daria6918.cn/gtbckpvxjm.html

[B05] 遍历数组 / 列表
来源：http://hz.haohaochexian.top/gtctrxhlqo.html

Py:   for item in arr: print(item)
来源：http://hz.nanxinkj.top/gtykejohdf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.andypj.xyz/gtejoucrwo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhixingplan.top/gtakivneft.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.daria6918.cn/gtzxpdplgu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.snrcjt.cn/gtaobudtnp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cdnleiting.top/gtknhawsvb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jlsjyb.cn/gtkushhgov.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.fzhhl.top/gteegojzll.html

[B06] 遍历字典 / 对象
来源：http://hz.gogol.net.cn/gtcvyxidfh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hywenlv.cn/gtjdhfigyc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.daxiang520.top/gtipxufyhe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yonumen.top/gtmxseclea.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydzc1.top/gtlrpxyiks.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sxryk.cn/gtimhewuvv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yj20258888.top/gtytbrexoq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nanxinkj.top/gtqykclhaa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sxryk.cn/gtcwwaynmr.html

[B07] while 循环
来源：http://hz.aibaodan.cn/gtiddsvyus.html

Py:   while i < 10: i += 1
来源：http://hz.zdqjudy.top/gtqckthmky.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhoulong.xyz/gtbiatgdbq.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtfooxeqns.html

TS:   while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gtvhrkwkhh.html

Java: while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtlifsygwt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hysaishi.cn/gtyyfmvcmu.html

Ruby: while i < 10; i += 1; end
来源：http://hz.fzhhl.top/gtqalkhufs.html

C#:   while (i < 10) { i++; }
来源：http://hz.cqqwz.cn/gtmxzgdjfv.html

[B08] do-while（至少执行一次）
来源：http://hz.gogol.net.cn/gtktornber.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.wangdashe.top/gtdzstijic.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.iojbl.cn/gtlzfvofou.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtqewwgcyy.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtlqbarypv.html

Java: do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtlugalzih.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jyoumei.cn/gtyiajpksg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hywenlv.cn/gtjohftbhi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yongpay.top/gtcuwpmljd.html

[B09] break 与 continue
来源：http://hz.birdmap.top/gtxcgozhhk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aizwys.cn/gteyqypqis.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj202588.top/gtsthmevxv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtujcaadpw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtqiqracqb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtssmzebsd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.daria6918.cn/gtjsodzjck.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cdnleiting.top/gtrnaeeiht.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gteapwjwqj.html

[B10] 遍历同时拿索引
来源：http://hz.kuanghao11.cn/gtrcbfxxjn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gotoacloud.top/gtjnhuqnrm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cqqwz.cn/gtvqpjykzw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nwbrower.top/gtwtlchjuw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ydzc1.top/gtdrvkcvay.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.ppjwa.cn/gtovprnxki.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shanyushiyangtech.top/gtftfdfzew.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.fzhhl.top/gtnwxxtdrx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.chenlongwang.top/gtqqplvsly.html

[B11] 生成数字序列 / 区间
来源：http://hz.cdnleiting.top/gtqbtkphqc.html

Py:   list(range(0, 10, 2))
来源：http://hz.quarkkingdee.top/gtaajgfsmq.html

PHP:  range(0, 10, 2);
来源：http://hz.haohaochexian.top/gtummzwabg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gtlqyatiql.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gtkiupxweb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hysaishi.cn/gtxnbxugqr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.52xcode.cn/gtuvbsywwe.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yangfankeji.com/gtbsgfrcow.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.pycfn.com/gtzkoksbdy.html

[B12] 跳出多层循环
来源：http://hz.yonumen.top/gtjhzwbxzm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jyoumei.cn/gtolyotnxw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ivvv.top/gtejqznwpv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tianlin.xyz/gtvnjpvbrr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtxeglksdp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hfpthk.cn/gtkheokrqy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hammf.cn/gtmcnybeye.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sweek.top/gtqjlwqnfv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zdqjudy.top/gtvdvxtrqx.html

[B13] 判断是否为数字
来源：http://hz.guowangkeji.top/gtithepokx.html

Py:   isinstance(x, (int, float))
来源：http://hz.sxryk.cn/gtwkwbklha.html

PHP:  is_numeric($x)
来源：http://hz.jyoumei.cn/gtczwixjvo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tian-w.cn/gtthxheliz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhijiandao.cn/gtkgmaeezy.html

Java: x instanceof Number
来源：http://hz.yuxming.cn/gttdacpnma.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xylfe.cn/gtayrnmrph.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xylfe.cn/gtvgjswwlh.html

C#:   x is int or double or decimal
来源：http://hz.cucudq.cn/gtbhylatfx.html

[B14] 判断值是否在集合内
来源：http://hz.ydzc1.top/gtykntvhdf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.0kj1m.cn/gthbngrdmc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhiwuduotai.top/gttmmzlufu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtxxprizng.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shzxlz.cn/gtceyknrep.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.smart0.xyz/gtkbbducyq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gaohongyu789.top/gtcdmhkqru.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hnqzz.top/gtecfxzxat.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.xziqi.cn/gttrezlmwk.html

[B15] 布尔运算与取反
来源：http://hz.52xcode.cn/gttqcvtqqg.html

Py:   a and b or not c
来源：http://hz.andypj.xyz/gtreejadyt.html

PHP:  $a && $b || !$c
来源：http://hz.sysykeji.top/gtgvaclztx.html

JS:   a && b || !c
来源：http://hz.tianlin.xyz/gtxdunqkco.html

TS:   a && b || !c
来源：http://hz.cdnleiting.top/gtprzuxlbc.html

Java: a && b || !c
来源：http://hz.cashguo.top/gtolcqvtbq.html

Go:   a && b || !c
来源：http://hz.sweek.top/gtkvpcuytx.html

Ruby: a && b || !c
来源：http://hz.yj202588.top/gtowzscfgg.html

C#:   a && b || !c
来源：http://hz.xinyue.icu/gtgwnxxsza.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.smart0.xyz/gtfqmsjxcb.html

Py:   if not data: return
来源：http://hz.tianlin.xyz/gtfsnozplh.html

PHP:  if (!$data) { return; }
来源：http://hz.jinghuilouyu.cn/gtiadhhplp.html

JS:   if (!data) return;
来源：http://hz.pengpengdd.cyou/gtzjjsvkhb.html

TS:   if (!data) return;
来源：http://hz.sxryk.cn/gtotybudjg.html

Java: if (data == null) return;
来源：http://hz.shzxlz.cn/gtolpypmwg.html

Go:   if data == nil { return }
来源：http://hz.haohaochexian.top/gtstfjjyue.html

Ruby: return if data.nil?
来源：http://hz.yueranfly.top/gtbqlhuila.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtxxsehdxt.html

================================================================================
来源：http://hz.daxiang520.top/gtmigvbrih.html

C. 函数与作用域
来源：http://hz.aizwys.cn/gtxfwybmdt.html

================================================================================
来源：http://hz.gogol.net.cn/gtkipbwqau.html

[C01] 定义函数
来源：http://hz.yj20258888.top/gtyyvmkalx.html

Py:   def add(a, b): return a + b
来源：http://hz.jlsjyb.cn/gtliiwmrhn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jyoumei.cn/gtylikjdnd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtuuugtnpf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtlaimlgrg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtzhsyveza.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gtiajkidpc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinghuilouyu.cn/gttjmygofi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtmtflvkjn.html

[C02] 默认参数
来源：http://hz.cqqwz.cn/gtxyazrwxk.html

Py:   def greet(name="World"): return name
来源：http://hz.xuanzx.com/gttuxqhlow.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.daxiang520.top/gtimyeiujx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhengqikj.top/gtoqulvrfm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj202588.top/gtxzxmpffp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hnxiangtu.top/gtdzdwyxja.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhiwuduotai.top/gtwdoivqtr.html

Ruby: def greet(name = "World") = name
来源：http://hz.smart0.xyz/gthghkwptl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.kuanghao11.cn/gtgzzhuoht.html

[C03] 可变参数
来源：http://hz.quarkkingdee.top/gtfbbiatem.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhongyouzk.top/gtuhjziwap.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtmlnuspiq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.snrcjt.cn/gtekzcdpfy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gtusxgzavy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.52xcode.cn/gtnwiyohcw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.guannengcc.top/gtrukdzhkl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pycfn.com/gtxiiwepay.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.haohaochexian.top/gtdwlwalmp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtxdimlkkn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jinyuanbaomall.cn/gtldauhgjg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xziqi.cn/gttltnelni.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtadqtdxtr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yvedp.cn/gtprmjgewf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhongyouzk.top/gtcbgaqmvx.html

Go:   // 无：用配置结构体参数
来源：http://hz.52xcode.cn/gtxhzfadcn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xylfe.cn/gtwbpwczks.html

C#:   f(a: 1, b: 2)
来源：http://hz.andypj.xyz/gtgvmvfrnc.html

[C05] 返回多个值
来源：http://hz.jianghu66.top/gtcuamajyl.html

Py:   return a, b
来源：http://hz.yueranfly.top/gtdelogcpt.html

PHP:  return [$a, $b];
来源：http://hz.nanxinkj.top/gtpmyjzsxl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.smart0.xyz/gtvkjhhwun.html

TS:   return { a, b };
来源：http://hz.zdqjudy.top/gtlhwrbggz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yongpay.top/gtverfzflw.html

Go:   return a, b
来源：http://hz.vqdsnc.cn/gtzhymknba.html

Ruby: return a, b
来源：http://hz.ppjwa.cn/gteovyeqfw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xuetiantiany.cn/gthnrwzabv.html

[C06] 匿名函数 / lambda
来源：http://hz.gaohongyu789.top/gtgfvxqhxi.html

Py:   square = lambda x: x * x
来源：http://hz.hnqzz.top/gtbvwydbjq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangshuangyany.cn/gtipoclzhe.html

JS:   const square = x => x * x;
来源：http://hz.yj20258888.top/gtqukftizt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pycfn.com/gtobmobyiq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ehwqpu.com/gtobdfvrfz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hysaishi.cn/gtgalbhmzl.html

Ruby: square = ->(x) { x * x }
来源：http://hz.xuanzx.com/gtrfucwugv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.cdnleiting.top/gtjhqspnms.html

[C07] 把函数作为参数传入
来源：http://hz.yonumen.top/gtwblxxtdi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.c1oappe.top/gtdwjczwwn.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jlsjyb.cn/gtsbwpwoqy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangshuangyany.cn/gtspwmwbuz.html

TS:   arr.map(String)
来源：http://hz.bjfxy.top/gtsnxbgzyt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dashuyun.cn/gtyafijnpf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.fzhhl.top/gtgzwbzotx.html

Ruby: arr.map(&:upcase)
来源：http://hz.cashguo.top/gtmqwuzxav.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zdqjudy.top/gtkwvlimkc.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtusqtkxxh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.kuanghao11.cn/gtphiomaja.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shanyushiyangtech.top/gtmxiipnze.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gtkqrdseng.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtegkibiez.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.0kj1m.cn/gtjlxhfula.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cashguo.top/gtnptgzkic.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydjk.org.cn/gtjobsorex.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtpqcgzajk.html

[C09] 递归
来源：http://hz.haohaochexian.top/gtdlzeltdt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuanzx.com/gtjcqhqxtv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.dianchejie.cn/gtjjwsfctu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jyoumei.cn/gtdwydnhru.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.snrcjt.cn/gtoqmkmgvz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtvgrvtzbv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yonumen.top/gtvcercbao.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shanyushiyangkeji.top/gtgygeqluf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gttdhlccoe.html

[C10] 变量作用域
来源：http://hz.feifeiyinyue.top/gtzkeecpni.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yangfankeji.com/gttznnajmi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hammf.cn/gtlnugnftj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sxryk.cn/gtwyjoxxsl.html

TS:   同 JS
来源：http://hz.shangyingyoupin.top/gtiqdawdcc.html

Java: 方法内为块级作用域
来源：http://hz.yvedp.cn/gtedynslpo.html

Go:   花括号块级作用域
来源：http://hz.yj20258.top/gtywktfifj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yvedp.cn/gtrgxcxavf.html

C#:   块级作用域
来源：http://hz.yj20258888.top/gtkeyfmekr.html

[C11] 模块导入与导出
来源：http://hz.kuanghao11.cn/gtanrmxxxq.html

Py:   from module import func
来源：http://hz.guannengcc.top/gtjouutbhs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dashuyun.cn/gtlhzhonim.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.c1oappe.top/gtpzumottk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yvedp.cn/gtpaecgqtk.html

Java: import java.util.List;
来源：http://hz.cashguo.top/gtcxrxabzj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xingfuxueyuan.xyz/gtkgknqcki.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gotoacloud.top/gtmgahxdkg.html

C#:   using System.Text;
来源：http://hz.pycfn.com/gtkmcsnlya.html

[C12] 立即执行函数 IIFE
来源：http://hz.hfpthk.cn/gtbiecrusm.html

Py:   (lambda: print("run"))()
来源：http://hz.tian-w.cn/gtbpsaqlwn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhongyouzk.top/gtlbscxcqx.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinghuilouyu.cn/gtdwkralxq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tianlin.xyz/gtxexiuwil.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gogol.net.cn/gticbondbu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hysaishi.cn/gtzaumgmdl.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhaomingkeji.xyz/gtsuzrvijc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sysykeji.top/gtnhcyzkaq.html

[C13] 类型声明 / 类型注解
来源：http://hz.birdmap.top/gttejwndtc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gtayclqvrm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtdlypadvq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gtzfdcckdd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtpiwndbnz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtdtyhhmdu.html

Go:   func add(a, b int) int
来源：http://hz.zhijiandao.cn/gtpzfiyujh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yj20258.top/gthtdzspxi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.pengpengdd.cyou/gtkgyqbpsn.html

[C14] 泛型函数
来源：http://hz.nanxinkj.top/gtpizfntyf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.guannengcc.top/gtujujnchh.html

PHP:  // 无泛型
来源：http://hz.hnxiangtu.top/gtsqmrelyr.html

JS:   // 无泛型
来源：http://hz.jqgfzy.top/gthogmtgmn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hnxiangtu.top/gtfgtcxdfm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cucudq.cn/gtieivxhgl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtymyenojz.html

Ruby: # 无泛型
来源：http://hz.tanke756.top/gtcyauhuou.html


<!-- 参考信息 -->