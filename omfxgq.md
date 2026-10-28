代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.gaohongyu789.top/gtyymrdjle.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.52xcode.cn/gtrbxqkafs.html

[A24] 去除首尾空白
来源：http://hz.hywenlv.cn/gtjjlqffml.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.xingfuxueyuan.xyz/gtarifuvvr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.snrcjt.cn/gtkznvmujy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.c1oappe.top/gtbjcxpfwg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.316326.xyz/gttnholgxc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.quarkkingdee.top/gtgyilhjuz.html

Go:   strings.TrimSpace(s)
来源：http://hz.jyoumei.cn/gtaahorzyj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yonumen.top/gtalnzyyyv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.tanke756.top/gtiktjrrrk.html

[A25] 字符串比较
来源：http://hz.jlsjyb.cn/gtfejvpxhe.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yuxming.cn/gtwyqkfwan.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.feifeiyinyue.top/gtfdihltwc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nanxuanxn.top/gtsftyscpj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhixingplan.top/gtzhcfmwoj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.dashuyun.cn/gtixboyhuh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.svipenyu.cn/gtqyjiftdt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shuidangran.top/gtnnedairf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhixingplan.top/gtynsgcipa.html

[A26] 类型转换总览
来源：http://hz.fzhhl.top/gtdygzvswi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jqgfzy.top/gtynjryrmp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yuanzhike.top/gtmifaltmn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jyoumei.cn/gtzrhkfpbz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.dianchejie.cn/gtncmltvui.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zycfv.cn/gtmfyxhezj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.fengsongda.top/gtfsjbhsnm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zdqjudy.top/gtakgzlcxu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.bjfxy.top/gtpuegjlcs.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtpdbcykyb.html

B. 流程控制
来源：http://hz.yanxiufei.cn/gtmbtxbyjq.html

================================================================================
来源：http://hz.0kj1m.cn/gtzksczbnw.html

[B01] 条件判断 if / else
来源：http://hz.zhaomingkeji.xyz/gtheakuhwf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gzhubu.top/gtemhuhfxw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zycfv.cn/gtfufrnuoa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinyuanbaomall.cn/gtyevmxury.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhengqikj.top/gtqfomoaam.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jlsjyb.cn/gtjvkdodrk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yj20258888.top/gtlsbbgkcc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.ybcxt.top/gtskevfmpz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtulitourw.html

[B02] 多分支 else if / elif
来源：http://hz.svipenyu.cn/gtiambngwi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.xinyue.icu/gtjkyqkmvm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hysaishi.cn/gtufmhfjji.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gtwenteuiy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtvkrunlba.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtiraxvmss.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.snrcjt.cn/gtzigzvsjn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinyuanbaomall.cn/gtatgspahx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gtgypojzyk.html

[B03] switch / match / case
来源：http://hz.daxiang520.top/gthahyzrcj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hysaishi.cn/gtdvmhbgxq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hfpthk.cn/gtflhbjdss.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yvedp.cn/gtkbwlvsen.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.bjfxy.top/gtjnonrghm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jiagoushi.top/gtvfnwrvof.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yangfankeji.com/gtrmctkikp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.shzxlz.cn/gtscuekpea.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ywan-chungtsiang.top/gtmkrtalzx.html

[B04] for 计数循环
来源：http://hz.xinyue.icu/gtrwgmxakg.html

Py:   for i in range(10): print(i)
来源：http://hz.zhongyouzk.top/gtrnsfgsuh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jlsjyb.cn/gtkqgfozbh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pycfn.com/gtrxzxxtkc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ywan-chungtsiang.top/gtgepfzcwd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.dianchejie.cn/gtmuzqnxwe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jinqigfzy.top/gtdmlxylue.html

Ruby: 10.times { |i| puts i }
来源：http://hz.52xcode.cn/gtzwvgakxd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hywenlv.cn/gtjydcybki.html

[B05] 遍历数组 / 列表
来源：http://hz.hnxiangtu.top/gtdcmcogkr.html

Py:   for item in arr: print(item)
来源：http://hz.fzhhl.top/gtccfypbaz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.bjfxy.top/gtxtximedb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhijiandao.cn/gtsoklemjb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.bjfxy.top/gtbfswlifm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.bjfxy.top/gtsukctcjm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhiwuduotai.top/gtyjfrindn.html

Ruby: arr.each { |item| puts item }
来源：http://hz.mhx1999.top/gtrbiujtne.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.dianchejie.cn/gtegleecpr.html

[B06] 遍历字典 / 对象
来源：http://hz.yuxming.cn/gtvvvjydsd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.pengpengdd.cyou/gtpojjrnxk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.havefunace.top/gtadqxbsaf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jianghu66.top/gtjhygbgef.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ehwqpu.com/gtvdajngth.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zycfv.cn/gtshxkbitj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.dianchejie.cn/gtdiomqjgh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nanxuanxn.top/gtemkzmlya.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yangfankeji.com/gtpgrrwgyp.html

[B07] while 循环
来源：http://hz.jinghuilouyu.cn/gtuuimgdqd.html

Py:   while i < 10: i += 1
来源：http://hz.xuanzx.com/gthclpntek.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jlsjyb.cn/gtojwauwrk.html

JS:   while (i < 10) { i++; }
来源：http://hz.sweek.top/gtuioslvmg.html

TS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtpqavyokb.html

Java: while (i < 10) { i++; }
来源：http://hz.hnxiangtu.top/gtzpunujkp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhiwuduotai.top/gtkomvuhxf.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yueranfly.top/gtzdiftlgy.html

C#:   while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtnrekpwjg.html

[B08] do-while（至少执行一次）
来源：http://hz.xylfe.cn/gtdoefvqkt.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yuanzhike.top/gteeuafgeg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ehwqpu.com/gtpxjubxyh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hongshengwenyu.top/gtpagfmofu.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtjquetjfv.html

Java: do { i++; } while (i < 10);
来源：http://hz.quarkkingdee.top/gtwvedcgsd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.aibaodan.cn/gtyytqatyd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.snrcjt.cn/gtrffvlhuk.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtdahtlktk.html

[B09] break 与 continue
来源：http://hz.jyoumei.cn/gtfajkkiqi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yongpay.top/gtkqrrbldj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jianghu66.top/gtspronmnx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtdgdrylqr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtiglsgjdq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtgtyonnvg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yuanzhike.top/gthmoxbcyo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.svipenyu.cn/gtakptnhge.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtuuqtmsgs.html

[B10] 遍历同时拿索引
来源：http://hz.zhongyouzk.top/gthimpaepl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gaohongyu789.top/gtxclywnwd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinqigufen.top/gtpxdyzzwr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hnqzz.top/gtwepdpeie.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.pengpengdd.cyou/gtcvoznezr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.wangdashe.top/gtvnqqxhtu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhongyouzk.top/gtoypihmcu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jlsjyb.cn/gttqcpyhza.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tian-w.cn/gtlbsifevt.html

[B11] 生成数字序列 / 区间
来源：http://hz.birdmap.top/gtcluvbmhm.html

Py:   list(range(0, 10, 2))
来源：http://hz.zdqjudy.top/gtedbzgfen.html

PHP:  range(0, 10, 2);
来源：http://hz.sysykeji.top/gtguucmtcv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yuanzhike.top/gthkecgulp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.daxiang520.top/gtavobzqov.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhoulong.xyz/gtunelaojm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ybcxt.top/gtujgecstr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yuxming.cn/gtenvsyjdx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ivvv.top/gtxpycbtie.html

[B12] 跳出多层循环
来源：http://hz.jinghuilouyu.cn/gtuuwnjjoi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hysaishi.cn/gtbgjswngf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shzxlz.cn/gteaoullyu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtlvsfwlgq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtsjvubmtd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hfpthk.cn/gtzgidyvwx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jlsjyb.cn/gtnqpzwlqw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.feifeiyinyue.top/gttupgglun.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.smart0.xyz/gtnpwsgiha.html

[B13] 判断是否为数字
来源：http://hz.nanxuanxn.top/gttyokmhge.html

Py:   isinstance(x, (int, float))
来源：http://hz.snrcjt.cn/gtoexwuqls.html

PHP:  is_numeric($x)
来源：http://hz.ivvv.top/gtigufmehs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gtepquzpru.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtfgvadxtr.html

Java: x instanceof Number
来源：http://hz.ppjwa.cn/gtyottfndn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.pengpengdd.cyou/gtpfhbozin.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hysaishi.cn/gtaslweeqi.html

C#:   x is int or double or decimal
来源：http://hz.xuetiantiany.cn/gtfbklglzk.html

[B14] 判断值是否在集合内
来源：http://hz.pycfn.com/gtamftfptz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.andypj.xyz/gteanzenei.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhongyouzk.top/gtacvmdjwk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gtcvqsqvob.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.daria6918.cn/gttxkofpxa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shzxlz.cn/gtgojeftfg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hongshengwenyu.top/gtorkzlfck.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xinyue.icu/gtggrfhsdc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenjidiqi.icu/gtodfusimw.html

[B15] 布尔运算与取反
来源：http://hz.gzhubu.top/gtplggueil.html

Py:   a and b or not c
来源：http://hz.chenjidiqi.icu/gthwrokbbx.html

PHP:  $a && $b || !$c
来源：http://hz.hammf.cn/gtezsipeco.html

JS:   a && b || !c
来源：http://hz.xinyue.icu/gthrjhtrdf.html

TS:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtvastrybg.html

Java: a && b || !c
来源：http://hz.smart0.xyz/gtstynmoxd.html

Go:   a && b || !c
来源：http://hz.dianchejie.cn/gthmpjgdcp.html

Ruby: a && b || !c
来源：http://hz.gotoacloud.top/gtnyacwyqz.html

C#:   a && b || !c
来源：http://hz.hammf.cn/gtodtuqjis.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gtdafhpmjw.html

Py:   if not data: return
来源：http://hz.zdqjudy.top/gtuwuvfgvy.html

PHP:  if (!$data) { return; }
来源：http://hz.hysaishi.cn/gtqykvreoz.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gtlzilaekt.html

TS:   if (!data) return;
来源：http://hz.andypj.xyz/gtxiuynjuo.html

Java: if (data == null) return;
来源：http://hz.ppjwa.cn/gtqjyzyhev.html

Go:   if data == nil { return }
来源：http://hz.ydzc1.top/gtnxcljidu.html

Ruby: return if data.nil?
来源：http://hz.yj202588.top/gtpehwetle.html

C#:   if (data == null) return;
来源：http://hz.hywenlv.cn/gtngluqlvo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gterhkwkcr.html

C. 函数与作用域
来源：http://hz.ywan-chungtsiang.top/gtqadoapny.html

================================================================================
来源：http://hz.yj20258888.top/gtavxkvrcu.html

[C01] 定义函数
来源：http://hz.316326.xyz/gtgaqpbxio.html

Py:   def add(a, b): return a + b
来源：http://hz.nwbrower.top/gtmcxwgbkl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nwbrower.top/gtsfdmamzh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.sufxvd.cn/gtdrgghtfr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtcjzpvfbj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtecybvzgo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.vqdsnc.cn/gtnispgdch.html

Ruby: def add(a, b); a + b; end
来源：http://hz.ybcxt.top/gtdbhlxhhh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhongyouzk.top/gtbafmjekq.html

[C02] 默认参数
来源：http://hz.ybcxt.top/gtcjonappf.html

Py:   def greet(name="World"): return name
来源：http://hz.zdqjudy.top/gtomneddps.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhoulong.xyz/gtiutuwjfw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinghuilouyu.cn/gttogzsbio.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhoulong.xyz/gtmkvtwfnb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jlsjyb.cn/gtufsrvrzb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gzhubu.top/gtzgiqomuy.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtqzooztjz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenzaomai.com/gtsntlwgee.html

[C03] 可变参数
来源：http://hz.svipenyu.cn/gtuywtdnwn.html

Py:   def total(*args): return sum(args)
来源：http://hz.guowangkeji.top/gtggeoguwg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yangfankeji.com/gtfxqhdzhz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gtrtkxfgeb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtdzwhxisz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtiuahdcfz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.guowangkeji.top/gtmnfpnhab.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinghuilouyu.cn/gtaunmyaxp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aizwys.cn/gtsfpvvere.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sysykeji.top/gtiormimht.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.wangdashe.top/gtchbmlvan.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yueranfly.top/gttqozmsfg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.shangyingyoupin.top/gtatrqiwys.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gtuuxivmty.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guannengcc.top/gtpzgkdlwj.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gtrdueobks.html

Ruby: f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtpdwtsdbr.html

C#:   f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtrdzyagfx.html

[C05] 返回多个值
来源：http://hz.jlsjyb.cn/gttdbrbwkd.html

Py:   return a, b
来源：http://hz.kuanghao11.cn/gtkakkrrpb.html

PHP:  return [$a, $b];
来源：http://hz.redwolf501.top/gtbttsszrz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guowangkeji.top/gtqduwdsbf.html

TS:   return { a, b };
来源：http://hz.zycfv.cn/gtrsynlxro.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnxiangtu.top/gtuahervqv.html

Go:   return a, b
来源：http://hz.nanxuanxn.top/gtuhconbum.html

Ruby: return a, b
来源：http://hz.cdnleiting.top/gtzlaerhog.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jianghu66.top/gtxvdlzoqw.html

[C06] 匿名函数 / lambda
来源：http://hz.mhx1999.top/gttrmmvebb.html

Py:   square = lambda x: x * x
来源：http://hz.svipenyu.cn/gtxweulewq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.mhx1999.top/gtolyouvoc.html

JS:   const square = x => x * x;
来源：http://hz.jiagoushi.top/gtnrevqvkg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xuanzx.com/gtxldebyaw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.smart0.xyz/gtffwnrizh.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tian-w.cn/gtogzefavo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tian-w.cn/gtcndykcis.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.chenjidiqi.icu/gtjkldhwok.html

[C07] 把函数作为参数传入
来源：http://hz.dianchejie.cn/gttkeiumrx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.guannengcc.top/gtgrdpztev.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xinyue.icu/gtuzojvsck.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.smart0.xyz/gtafjgjbor.html

TS:   arr.map(String)
来源：http://hz.andypj.xyz/gtfcdprzgm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.9152youxi.cn/gtqhwovjus.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cqqwz.cn/gtkjbpkewg.html

Ruby: arr.map(&:upcase)
来源：http://hz.ppjwa.cn/gtoehupdok.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gogol.net.cn/gtbpdygdmz.html

[C08] 闭包
来源：http://hz.hammf.cn/gtqhwvaduy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gtysofiiqr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.redwolf501.top/gtrexuccoo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtsvatuxih.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtqcjyfbrx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.havefunace.top/gtrqhwvpby.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.xylfe.cn/gtquwyndzj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sxryk.cn/gtpnyeyxvy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtstezqobi.html

[C09] 递归
来源：http://hz.tian-w.cn/gtscdrhjpl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ydjk.org.cn/gtvxvgdeuy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jiagoushi.top/gtlcxcjtts.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gotoacloud.top/gtiicnkecp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhoulong.xyz/gtantjyzvn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgfzy.top/gtoprqofiz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fzhhl.top/gteocmxuva.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.c1oappe.top/gtggwxrwvs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ywan-chungtsiang.top/gteyiysezj.html

[C10] 变量作用域
来源：http://hz.nwbrower.top/gteqpiqdxa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.quarkkingdee.top/gtaoomjcuu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.daria6918.cn/gtkrrnsanw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.haohaochexian.top/gtbuebcabg.html

TS:   同 JS
来源：http://hz.snrcjt.cn/gtadxjifmp.html

Java: 方法内为块级作用域
来源：http://hz.wangdashe.top/gtvdzmfaoe.html

Go:   花括号块级作用域
来源：http://hz.ybcxt.top/gtrebqolui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xziqi.cn/gtdzukflxo.html

C#:   块级作用域
来源：http://hz.xuetiantiany.cn/gtvyokedad.html

[C11] 模块导入与导出
来源：http://hz.shzxlz.cn/gtetbntffw.html

Py:   from module import func
来源：http://hz.dashuyun.cn/gtctktwelp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shanyushiyangtech.top/gthiycyhbs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.mhx1999.top/gtsvhribai.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.meibo888.top/gtjpkwgqed.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtdwvsdhkb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.havefunace.top/gtlaevyznx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pengpengdd.cyou/gtveggkycr.html

C#:   using System.Text;
来源：http://hz.yanxiufei.cn/gtqrkgsoqg.html

[C12] 立即执行函数 IIFE
来源：http://hz.gzhubu.top/gtfwpdiili.html

Py:   (lambda: print("run"))()
来源：http://hz.zhixingplan.top/gtsccuxfbx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ydjk.org.cn/gtrrjbygca.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gtdmzyukkg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenjidiqi.icu/gtxvsnrrwb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinqigufen.top/gtoaskyexp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yonumen.top/gtlzllnpvf.html

Ruby: -> { puts "run" }.call
来源：http://hz.pycfn.com/gtmkmdjqtg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.birdmap.top/gtdzqxvpxu.html

[C13] 类型声明 / 类型注解
来源：http://hz.shzxlz.cn/gttmicgyyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xinyue.icu/gtnexxpbjo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gthhhbjkbx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnxiangtu.top/gtzmogsals.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hfpthk.cn/gtujoknztk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtlxlvdzul.html

Go:   func add(a, b int) int
来源：http://hz.ppjwa.cn/gtknwjssmq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenzaomai.com/gtisvgizlg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.cdnleiting.top/gtlajomkek.html

[C14] 泛型函数
来源：http://hz.cucudq.cn/gtgctqadkd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sweek.top/gthgwwpfff.html

PHP:  // 无泛型
来源：http://hz.xylfe.cn/gtcgpddygx.html

JS:   // 无泛型
来源：http://hz.zhaomingkeji.xyz/gtfgtvzydx.html


<!-- 参考信息 -->