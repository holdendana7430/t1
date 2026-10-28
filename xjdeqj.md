代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.dashuyun.cn/gtipuirpqw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.shanyushiyangkeji.top/gtoalsjnug.html

[A24] 去除首尾空白
来源：http://hz.yanxiufei.cn/gtxaqjixvh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.svipenyu.cn/gtsbdxjcwq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zhongyouzk.top/gtyqpfyqbs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhongyouzk.top/gtmwtxjzcx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigfzy.top/gtkvrcpugy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ppjwa.cn/gtckcywzgc.html

Go:   strings.TrimSpace(s)
来源：http://hz.iojbl.cn/gtufyiglfu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xuetiantiany.cn/gtmlpzqvbr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ydzc1.top/gtvlgzxwfg.html

[A25] 字符串比较
来源：http://hz.shanyushiyangtech.top/gtvnxvthxp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.aizwys.cn/gtcglfcmnl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.wangshuangyany.cn/gtqlubxpja.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tian-w.cn/gtkacajekr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.meibo888.top/gtcwupnnpr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.fzhhl.top/gtstkifxba.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hywenlv.cn/gtjjldpmbq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.mhx1999.top/gtkzjizods.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.nwbrower.top/gtgwhmsilh.html

[A26] 类型转换总览
来源：http://hz.shzxlz.cn/gtmvhzplmd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhiwuduotai.top/gtakolyjdz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhijiandao.cn/gtrquizsbq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hnxiangtu.top/gtrrlziggl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zdqjudy.top/gtgcvpfxxc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenzaomai.com/gtfncanfic.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.cdnleiting.top/gthawfjdby.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.redwolf501.top/gtqvctrwsr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.0kj1m.cn/gtxiuhbaci.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtovhbzzrz.html

B. 流程控制
来源：http://hz.zhixingplan.top/gtvdxtjyji.html

================================================================================
来源：http://hz.aizwys.cn/gtwfvfqjrt.html

[B01] 条件判断 if / else
来源：http://hz.cqqwz.cn/gtufpurtlp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.nanxinkj.top/gttyhulqzk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.dashuyun.cn/gtqfzgzkvu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shangyingyoupin.top/gtzqfpijro.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtcdrcrmxj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtrkbsvjme.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.sufxvd.cn/gteiwvrgam.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.andypj.xyz/gtxqctfjib.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtrchfoeci.html

[B02] 多分支 else if / elif
来源：http://hz.yvedp.cn/gtzidatzyw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.vqdsnc.cn/gtmjvbnzxf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.wangshuangyany.cn/gtydeevquv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhijiandao.cn/gtmdazhwfi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtwzqbarfg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtzosdfjqk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jlsjyb.cn/gtaemdkdov.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.svipenyu.cn/gtkytejalv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtalvuwhwm.html

[B03] switch / match / case
来源：http://hz.52xcode.cn/gtyajlyopq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.vqdsnc.cn/gtbipjxpsp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.aizwys.cn/gtmfkcpcam.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hysaishi.cn/gtiawklpyt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ydjk.org.cn/gtbaohczkl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.havefunace.top/gtdufnogss.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.52xcode.cn/gtwbbzlser.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.52xcode.cn/gtlvqmfjnt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.c1oappe.top/gtolkhpzin.html

[B04] for 计数循环
来源：http://hz.meibo888.top/gtivngfsfg.html

Py:   for i in range(10): print(i)
来源：http://hz.zhaomingkeji.xyz/gtvgktynda.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yueranfly.top/gtttqgswiq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nwbrower.top/gtolhjisog.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pycfn.com/gtbakremqj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhengqikj.top/gtwjdknfph.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.shanyushiyangkeji.top/gtkoneftjz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.quarkkingdee.top/gtcbptflzm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.wangshuangyany.cn/gtisfehcbe.html

[B05] 遍历数组 / 列表
来源：http://hz.ywan-chungtsiang.top/gtdxwehsit.html

Py:   for item in arr: print(item)
来源：http://hz.bjfxy.top/gtajfalsuu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hywenlv.cn/gtdwafxmwj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuxming.cn/gtnveixivd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.feifeiyinyue.top/gtjutxczjb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shanyushiyangkeji.top/gtectrgsdo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ydzc1.top/gtwovbdhdw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.gogol.net.cn/gthdrmeecn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangshuangyany.cn/gttnjoxtxv.html

[B06] 遍历字典 / 对象
来源：http://hz.xziqi.cn/gtrmljhvpc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cdnleiting.top/gtrhqmsiai.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cdnleiting.top/gttbfounqc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pycfn.com/gtlxdjpadv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shuidangran.top/gtqtnqldyn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.kuanghao11.cn/gtrvgzrhuc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.meibo888.top/gtpuowprma.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.meibo888.top/gtlsdubsok.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.wangshuangyany.cn/gtuklqcfxj.html

[B07] while 循环
来源：http://hz.haohaochexian.top/gtadxhxnmb.html

Py:   while i < 10: i += 1
来源：http://hz.jqgfzy.top/gtlxcdrhvz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.vqdsnc.cn/gtsctlzfpz.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhoulong.xyz/gtdnviqlzs.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtdklwdqme.html

Java: while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtoonhkclh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yonumen.top/gtfvegbdlc.html

Ruby: while i < 10; i += 1; end
来源：http://hz.daxiang520.top/gtnlabbibf.html

C#:   while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtsuueepze.html

[B08] do-while（至少执行一次）
来源：http://hz.sxryk.cn/gtyszfpnic.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.316326.xyz/gtsxdrzcem.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yvedp.cn/gtjwgqwtuo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtnpzsilqz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtvsdmkldz.html

Java: do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtsswhztle.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sweek.top/gttpddkbvp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.aizwys.cn/gtxcofpxxc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gttgndrctq.html

[B09] break 与 continue
来源：http://hz.sxryk.cn/gtkywyvlpa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinyuanbaomall.cn/gtdnjxnghp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.chenlongwang.top/gtoczqdmvs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtrgwzpbgi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtgwhspunt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtgnidutba.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigfzy.top/gtgrrdalnk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pycfn.com/gtlppyemzj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhaomingkeji.xyz/gtpervdjkp.html

[B10] 遍历同时拿索引
来源：http://hz.andypj.xyz/gtkkaxvdhd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.feifeiyinyue.top/gtbdlhneah.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtppnoobnn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.redwolf501.top/gtfgsggcgh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jianghu66.top/gtyrnjwfsm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hammf.cn/gtldvqfigv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cheryme.top/gtbjgelmdz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cqqwz.cn/gteewgbpou.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.guowangkeji.top/gtuxjsxgbo.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgfzy.top/gtryscppnk.html

Py:   list(range(0, 10, 2))
来源：http://hz.hysaishi.cn/gtqnsyusjr.html

PHP:  range(0, 10, 2);
来源：http://hz.ywan-chungtsiang.top/gtyuzrzxxe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydzc1.top/gtkbdzawkc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gttserqxvr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.52xcode.cn/gtvtlyaozo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shangyingyoupin.top/gtxbphasbj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinqigfzy.top/gtnxqrolbh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.nanxuanxn.top/gtjfaihomf.html

[B12] 跳出多层循环
来源：http://hz.9152youxi.cn/gtktobidhl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinqigfzy.top/gtbryonhwq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.nanxinkj.top/gtlmkekxbu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtbabcmydf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtalklebht.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtbbpcivhl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gzhubu.top/gtbrwdjhwg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gzhubu.top/gtrzhwbetf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tanke756.top/gtyqfbchdt.html

[B13] 判断是否为数字
来源：http://hz.zhijiandao.cn/gthfcagavl.html

Py:   isinstance(x, (int, float))
来源：http://hz.jqgufenzy.top/gtbvcfvaqt.html

PHP:  is_numeric($x)
来源：http://hz.nwbrower.top/gtywbfkeav.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.feifeiyinyue.top/gtimzecdmj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jlsjyb.cn/gtdqfcudyp.html

Java: x instanceof Number
来源：http://hz.shangyingyoupin.top/gtliwqztpa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yangfankeji.com/gtewxlgvlg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.dashuyun.cn/gttprgpuun.html

C#:   x is int or double or decimal
来源：http://hz.snrcjt.cn/gtxevjjemg.html

[B14] 判断值是否在集合内
来源：http://hz.cashguo.top/gtojffkwmr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhaomingkeji.xyz/gtcxwgxqlv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgfzy.top/gtnnmvfopi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258888.top/gtstgdrcvd.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sxryk.cn/gteylogyxw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtqrhskicg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gaohongyu789.top/gtnhyjinkk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhoulong.xyz/gtfvakmklv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuxming.cn/gtrktroowd.html

[B15] 布尔运算与取反
来源：http://hz.hongshengwenyu.top/gtzbjrinsc.html

Py:   a and b or not c
来源：http://hz.pengpengdd.cyou/gtgauwpgcc.html

PHP:  $a && $b || !$c
来源：http://hz.yuxming.cn/gtaspqeisz.html

JS:   a && b || !c
来源：http://hz.ydzc1.top/gtwpqstncd.html

TS:   a && b || !c
来源：http://hz.jinqigfzy.top/gtytuqjooi.html

Java: a && b || !c
来源：http://hz.fzhhl.top/gttckgpoux.html

Go:   a && b || !c
来源：http://hz.mhx1999.top/gteyvuepwy.html

Ruby: a && b || !c
来源：http://hz.smart0.xyz/gtxsshfbjt.html

C#:   a && b || !c
来源：http://hz.sysykeji.top/gtnwrwizfd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.0kj1m.cn/gtpiijbxhv.html

Py:   if not data: return
来源：http://hz.yj20258888.top/gtmnyhyafd.html

PHP:  if (!$data) { return; }
来源：http://hz.daxiang520.top/gtzzgsnbfc.html

JS:   if (!data) return;
来源：http://hz.xingfuxueyuan.xyz/gtltyzbqvu.html

TS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gtxwvfcbfk.html

Java: if (data == null) return;
来源：http://hz.jlsjyb.cn/gtvllpdyth.html

Go:   if data == nil { return }
来源：http://hz.haohaochexian.top/gtuacthvuk.html

Ruby: return if data.nil?
来源：http://hz.hongshengwenyu.top/gtoaehyuch.html

C#:   if (data == null) return;
来源：http://hz.chenzaomai.com/gttryrletx.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdgavugyb.html

C. 函数与作用域
来源：http://hz.dianchejie.cn/gtddittlni.html

================================================================================
来源：http://hz.xuanzx.com/gtbrbrfwpg.html

[C01] 定义函数
来源：http://hz.havefunace.top/gtfvcdihta.html

Py:   def add(a, b): return a + b
来源：http://hz.ehwqpu.com/gtxeqeqaci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtmhvqdfjl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.9152youxi.cn/gtujecvzxe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jianghu66.top/gtlybxxfok.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtkshwzlax.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jqgufenzy.top/gtascsluzy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gaohongyu789.top/gtqjftksql.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gttpqeeomr.html

[C02] 默认参数
来源：http://hz.ybcxt.top/gtmpmycwlx.html

Py:   def greet(name="World"): return name
来源：http://hz.shangyingyoupin.top/gtlluajkgt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yanxiufei.cn/gtmjdmmsxt.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtqpgrndue.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zycfv.cn/gtbmbplmzq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xziqi.cn/gttdzvipeh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenlongwang.top/gtxcwsblgt.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenzaomai.com/gtyocpnqjh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ppjwa.cn/gtklisnlja.html

[C03] 可变参数
来源：http://hz.gaohongyu789.top/gtxdvuijjx.html

Py:   def total(*args): return sum(args)
来源：http://hz.shangyingyoupin.top/gtmnahaquf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xziqi.cn/gtnfabjdsy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtgckmeyby.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gtgvzmrrpf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhoulong.xyz/gtouygtrtf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shuidangran.top/gtpvuxigyn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tian-w.cn/gtlxqzzihh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydjk.org.cn/gtokubibhs.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ybcxt.top/gtpsnujtpw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.jqgfzy.top/gteruztwgw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hnqzz.top/gtfdilmcpx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cheryme.top/gtxsgtadtv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.smart0.xyz/gtizanofgx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangtech.top/gtjmrjcizs.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtianjumgg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ehwqpu.com/gtyqjnkhoq.html

C#:   f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtjsktmoyo.html

[C05] 返回多个值
来源：http://hz.jinqigufen.top/gtifnnhdgj.html

Py:   return a, b
来源：http://hz.dianchejie.cn/gtrfwphuqj.html

PHP:  return [$a, $b];
来源：http://hz.guannengcc.top/gtwceebuva.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.9152youxi.cn/gtjvykuuvf.html

TS:   return { a, b };
来源：http://hz.yonumen.top/gttcrvnavb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtsmqszbme.html

Go:   return a, b
来源：http://hz.cdnleiting.top/gteigmchtp.html

Ruby: return a, b
来源：http://hz.jinqigufen.top/gttwcmhyle.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gotoacloud.top/gtgomflfda.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtuqieyvjh.html

Py:   square = lambda x: x * x
来源：http://hz.ydzc1.top/gtgwcwhzur.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yj202588.top/gtmoeveiic.html

JS:   const square = x => x * x;
来源：http://hz.gaohongyu789.top/gtigvjclde.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.9152youxi.cn/gtmpprzmjk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangdashe.top/gtawibjcmn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cdnleiting.top/gtshcsubez.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hfpthk.cn/gtnlxljpkt.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yongpay.top/gtictpencv.html

[C07] 把函数作为参数传入
来源：http://hz.cheryme.top/gtmhcbwrjl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydjk.org.cn/gtynygiwft.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zycfv.cn/gtlvjkwgbj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxinkj.top/gtmdhkqcir.html

TS:   arr.map(String)
来源：http://hz.meibo888.top/gtkvzycxsk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.bjfxy.top/gtrqpfipfw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tian-w.cn/gtgchdvxce.html

Ruby: arr.map(&:upcase)
来源：http://hz.9152youxi.cn/gtaxzjlglz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zycfv.cn/gtljxsgwkc.html

[C08] 闭包
来源：http://hz.cucudq.cn/gtqkumrtoj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xylfe.cn/gtkpvrgklp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.c1oappe.top/gtvfgugpbm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yueranfly.top/gtsxmphibe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtihtmbxxu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.sufxvd.cn/gtofwbpwie.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinghuilouyu.cn/gtwmjwhxhz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jinyuanbaomall.cn/gtlqxcocrd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtxpxnqnzr.html

[C09] 递归
来源：http://hz.fengsongda.top/gtrclrfiip.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sweek.top/gtdjfgkizo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gtbygdvved.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gtviewjznq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtnlezjttd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yangfankeji.com/gtariolluv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydjk.org.cn/gtsfmzqkzp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.chenjidiqi.icu/gtpxxyhlno.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenlongwang.top/gtgvfehywn.html

[C10] 变量作用域
来源：http://hz.iojbl.cn/gtnfzdvqtf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgfzy.top/gtczhwgzdl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gtokusdsoq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.aizwys.cn/gtmoqiprpn.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtwxcakabe.html

Java: 方法内为块级作用域
来源：http://hz.hywenlv.cn/gtswqjhhwi.html

Go:   花括号块级作用域
来源：http://hz.chenlongwang.top/gtdpsslkym.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yanxiufei.cn/gtyqrfmogc.html

C#:   块级作用域
来源：http://hz.zhongyouzk.top/gtlowayvjm.html

[C11] 模块导入与导出
来源：http://hz.pengpengdd.cyou/gtrllhslyc.html

Py:   from module import func
来源：http://hz.zycfv.cn/gtafsbscax.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yongpay.top/gtrxisetij.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.feifeiyinyue.top/gthkvazlac.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnqzz.top/gtyfsszrqn.html

Java: import java.util.List;
来源：http://hz.shuidangran.top/gtrduzrdyl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cdnleiting.top/gtxgphbcpv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenjidiqi.icu/gttyuefgyk.html

C#:   using System.Text;
来源：http://hz.hywenlv.cn/gtghoobuxb.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuanzhike.top/gtaxxrbbtj.html

Py:   (lambda: print("run"))()
来源：http://hz.jinghuilouyu.cn/gtbcmqyxlt.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangtech.top/gtqzapumhn.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtqhhwgnaa.html

TS:   (() => { console.log("run"); })();
来源：http://hz.kuanghao11.cn/gtoeyvndll.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.9152youxi.cn/gtnrzombhf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.tanke756.top/gtgktiobbt.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gttmsgwjry.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.svipenyu.cn/gtzywptkbr.html

[C13] 类型声明 / 类型注解
来源：http://hz.yangfankeji.com/gtxtehpzsh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yvedp.cn/gtpumqaucd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtqgzfvsxd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.redwolf501.top/gtnlbnilns.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtgjdbcozw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtdjzdtkhe.html

Go:   func add(a, b int) int
来源：http://hz.nanxinkj.top/gtnsuanycf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtxzhggncu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydjk.org.cn/gtmfbmeaca.html

[C14] 泛型函数
来源：http://hz.hnxiangtu.top/gtozbeshuj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aizwys.cn/gtptjjvlpy.html

PHP:  // 无泛型
来源：http://hz.zhoulong.xyz/gtkafaqjkl.html

JS:   // 无泛型
来源：http://hz.hammf.cn/gtiactvaot.html


<!-- 参考信息 -->