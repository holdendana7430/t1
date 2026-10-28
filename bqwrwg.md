代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.9152youxi.cn/gtvnqmpgrr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenzaomai.com/gtjwcgvuyb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.aizwys.cn/gtqdtcgmzy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.cdnleiting.top/gtspmezxlm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.vqdsnc.cn/gtuwjrtvid.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.nanxinkj.top/gtbybualbp.html

[A24] 去除首尾空白
来源：http://hz.zdqjudy.top/gtjrjknmbe.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.aibaodan.cn/gtbnuoeuca.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.shangyingyoupin.top/gttpjenuva.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.snrcjt.cn/gtsscfvvuk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xingfuxueyuan.xyz/gtzeousosb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.andypj.xyz/gtebqknyvv.html

Go:   strings.TrimSpace(s)
来源：http://hz.wangshuangyany.cn/gtuifumkta.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.pycfn.com/gtriugnmap.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.svipenyu.cn/gthgcryfus.html

[A25] 字符串比较
来源：http://hz.xinyue.icu/gtolsnmrpm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.mhx1999.top/gtbstnidmq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.pengpengdd.cyou/gttmfupqyw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.vqdsnc.cn/gtqlhrfnju.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.quarkkingdee.top/gtjwnyxarh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zdqjudy.top/gtimvqausf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gtkygfnjhe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.nanxinkj.top/gtlbteiyfd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.pengpengdd.cyou/gtyafhvzwn.html

[A26] 类型转换总览
来源：http://hz.nanxuanxn.top/gtwvehnfve.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.cqqwz.cn/gtfittenak.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jlsjyb.cn/gtbqftynqm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yueranfly.top/gtprgaakzq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sufxvd.cn/gttqpqpveq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.aibaodan.cn/gtbpeqxvtf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yongpay.top/gtkufwffsc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.0kj1m.cn/gtrpzfnggy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ppjwa.cn/gthkybpotk.html

================================================================================
来源：http://hz.ppjwa.cn/gtdkzftigp.html

B. 流程控制
来源：http://hz.ppjwa.cn/gtnmhlzxwp.html

================================================================================
来源：http://hz.fengsongda.top/gtlksanlpl.html

[B01] 条件判断 if / else
来源：http://hz.hongshengwenyu.top/gtvwfrsymb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhiwuduotai.top/gtxnryhduv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yuanzhike.top/gtjcsldvtf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sysykeji.top/gtxfxprquo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtkbcjhrly.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yanxiufei.cn/gtrhxrxcaa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.chenzaomai.com/gtddyunfyp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yvedp.cn/gtyfcwlcfh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtpleokple.html

[B02] 多分支 else if / elif
来源：http://hz.316326.xyz/gtdrslmqes.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.ywan-chungtsiang.top/gtbpylcwys.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yuxming.cn/gtfihrkfyz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yanxiufei.cn/gtmnrwvxzv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtenucniyi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yueranfly.top/gttghmvnpw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xinyue.icu/gtdsflmoao.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yanxiufei.cn/gtzlumwodn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxinkj.top/gtcbcriygs.html

[B03] switch / match / case
来源：http://hz.sweek.top/gtzcyxypky.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xziqi.cn/gtzqcdrfez.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.9152youxi.cn/gtqtbpvgbk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ehwqpu.com/gtlsyzhwcz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.9152youxi.cn/gtjhtdrnyz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.ppjwa.cn/gtfpmpprun.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.fzhhl.top/gtndqwtpjw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnxiangtu.top/gtmcniwrne.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xuetiantiany.cn/gtczzgxiwc.html

[B04] for 计数循环
来源：http://hz.cdnleiting.top/gtyjjjsetf.html

Py:   for i in range(10): print(i)
来源：http://hz.yuxming.cn/gtlekagthr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ybcxt.top/gtobomaokv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhixingplan.top/gtqjrillor.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jyoumei.cn/gtrlwhxizk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.316326.xyz/gtstdnslkf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.dashuyun.cn/gtbyzfjrji.html

Ruby: 10.times { |i| puts i }
来源：http://hz.52xcode.cn/gtvyowymwm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yj202588.top/gthybviknu.html

[B05] 遍历数组 / 列表
来源：http://hz.chenlongwang.top/gtabjcousr.html

Py:   for item in arr: print(item)
来源：http://hz.yj20258888.top/gtquzptohz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hysaishi.cn/gtbyleaxli.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.svipenyu.cn/gtrvtulsot.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shangyingyoupin.top/gttakabuzb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj20258.top/gtpslvdotn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guowangkeji.top/gtbjjkqkgf.html

Ruby: arr.each { |item| puts item }
来源：http://hz.aibaodan.cn/gtuoiqlmgq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.svipenyu.cn/gtywedakon.html

[B06] 遍历字典 / 对象
来源：http://hz.ydzc1.top/gtisvrkiuz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.c1oappe.top/gtxbkqppsi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hnqzz.top/gtmrnapxcn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.svipenyu.cn/gtpxiadacx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuxming.cn/gtbicdaxcs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ywan-chungtsiang.top/gtcmrbykms.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yonumen.top/gtijaieael.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.wangdashe.top/gtklvjgnnr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.svipenyu.cn/gtfinvhrsh.html

[B07] while 循环
来源：http://hz.hnqzz.top/gtpctuowco.html

Py:   while i < 10: i += 1
来源：http://hz.zhongyouzk.top/gtquvfhovc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.daria6918.cn/gteqntnsuq.html

JS:   while (i < 10) { i++; }
来源：http://hz.yonumen.top/gtieywmpia.html

TS:   while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtfkgibeoq.html

Java: while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtthqhkouh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenjidiqi.icu/gtsydtqavo.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xuetiantiany.cn/gtooucsjvn.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtpsnylzrg.html

[B08] do-while（至少执行一次）
来源：http://hz.yangfankeji.com/gtcvsgzvqt.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xingfuxueyuan.xyz/gtkjdumbjs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sweek.top/gtyzzbxrhm.html

JS:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtlyjbclld.html

TS:   do { i++; } while (i < 10);
来源：http://hz.vqdsnc.cn/gtkgiwhpsu.html

Java: do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtczbvuout.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.chenlongwang.top/gtowwoaaph.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.havefunace.top/gtetpkznos.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtckopowny.html

[B09] break 与 continue
来源：http://hz.haohaochexian.top/gtnckwyrkx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ywan-chungtsiang.top/gtbwrcobjc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.guowangkeji.top/gtltdjykxf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtjyodazgb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtmrdvpnnw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtgvkqhtec.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.guowangkeji.top/gtjstdcvjd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sufxvd.cn/gtsqhppoaf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtuopxjrjo.html

[B10] 遍历同时拿索引
来源：http://hz.zhijiandao.cn/gtgjbfmaqz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jyoumei.cn/gtcllbkvnl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.snrcjt.cn/gtnhatsnig.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yj202588.top/gtlfquwhlz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.0kj1m.cn/gtlxducjmh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.pycfn.com/gthidsfbjv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.feifeiyinyue.top/gtwdxbyavy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.svipenyu.cn/gttfbmvzli.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jqgufenzy.top/gtizhrjhvn.html

[B11] 生成数字序列 / 区间
来源：http://hz.xylfe.cn/gtghmnydoq.html

Py:   list(range(0, 10, 2))
来源：http://hz.yanxiufei.cn/gtoaobsjll.html

PHP:  range(0, 10, 2);
来源：http://hz.yuanzhike.top/gtsgjjzmzv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shuidangran.top/gtvpoweyyn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gtuyepdzab.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jianghu66.top/gtxmunkrbo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhaomingkeji.xyz/gtlmpjspkg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhoulong.xyz/gtgengojfk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guannengcc.top/gtpxswpupj.html

[B12] 跳出多层循环
来源：http://hz.zhongyouzk.top/gtwjkmufwq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhiwuduotai.top/gtmcqztlsm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gogol.net.cn/gtskxjexpn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtjvtqdjwq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xylfe.cn/gtaztnubfp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtswnwwoaw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenzaomai.com/gtmplqyiiz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xuetiantiany.cn/gtfdkcdciu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ehwqpu.com/gtpvpbkvxg.html

[B13] 判断是否为数字
来源：http://hz.hnxiangtu.top/gtdgfpabjl.html

Py:   isinstance(x, (int, float))
来源：http://hz.ywan-chungtsiang.top/gtagjmkets.html

PHP:  is_numeric($x)
来源：http://hz.yuanzhike.top/gtalrpnkkn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yonumen.top/gtlmhmqiog.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydjk.org.cn/gtsqwmewbk.html

Java: x instanceof Number
来源：http://hz.hnqzz.top/gtwnvpxpro.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.svipenyu.cn/gthhbxyxkl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.aibaodan.cn/gtjuplipqu.html

C#:   x is int or double or decimal
来源：http://hz.hnxiangtu.top/gtbueuqmbm.html

[B14] 判断值是否在集合内
来源：http://hz.yj202588.top/gtywxhklrp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ybcxt.top/gtzpxyzmpg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shuidangran.top/gtdeoeeacx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtiaxgqfft.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gtbgciffgq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.dashuyun.cn/gtdnquczjk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cashguo.top/gtywcdxrml.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nwbrower.top/gtfocbmsta.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cashguo.top/gtlrqnruya.html

[B15] 布尔运算与取反
来源：http://hz.shuidangran.top/gtenokztlx.html

Py:   a and b or not c
来源：http://hz.zhijiandao.cn/gtjsmlowmy.html

PHP:  $a && $b || !$c
来源：http://hz.zycfv.cn/gtsxynavpq.html

JS:   a && b || !c
来源：http://hz.shzxlz.cn/gtofredpdm.html

TS:   a && b || !c
来源：http://hz.snrcjt.cn/gtqksynkeu.html

Java: a && b || !c
来源：http://hz.dianchejie.cn/gtkchkxnix.html

Go:   a && b || !c
来源：http://hz.jyoumei.cn/gtqyviulxz.html

Ruby: a && b || !c
来源：http://hz.xuetiantiany.cn/gtcpacwgth.html

C#:   a && b || !c
来源：http://hz.fengsongda.top/gtfaqasrvd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgfzy.top/gtqvzwaegu.html

Py:   if not data: return
来源：http://hz.shuidangran.top/gtcmmxnrbm.html

PHP:  if (!$data) { return; }
来源：http://hz.xziqi.cn/gtanoznjln.html

JS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gtbaypwtce.html

TS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtknqsnkir.html

Java: if (data == null) return;
来源：http://hz.daxiang520.top/gtmdodgmma.html

Go:   if data == nil { return }
来源：http://hz.yueranfly.top/gthdetlhac.html

Ruby: return if data.nil?
来源：http://hz.cashguo.top/gtqteodqzr.html

C#:   if (data == null) return;
来源：http://hz.nanxuanxn.top/gttlvjdbvk.html

================================================================================
来源：http://hz.aizwys.cn/gtbhqtrpvc.html

C. 函数与作用域
来源：http://hz.nwbrower.top/gtwdexrjlq.html

================================================================================
来源：http://hz.yanxiufei.cn/gtupvcnaqj.html

[C01] 定义函数
来源：http://hz.meibo888.top/gtrsrlxljf.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigufen.top/gtnqxltiqf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtabptxjaa.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ppjwa.cn/gteibrjwrp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nanxinkj.top/gtahvwgvsk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtbgmbwdlj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sufxvd.cn/gtszseefxy.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yvedp.cn/gtkazgcuvl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtxowxzapz.html

[C02] 默认参数
来源：http://hz.sweek.top/gtwlhlnhlt.html

Py:   def greet(name="World"): return name
来源：http://hz.redwolf501.top/gtezkvjbit.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.svipenyu.cn/gtrstxorlp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gteraqybzt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yangfankeji.com/gtgoxzypyo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hongshengwenyu.top/gtwshnzkqw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhoulong.xyz/gtdbmjmfka.html

Ruby: def greet(name = "World") = name
来源：http://hz.gotoacloud.top/gtvxevskix.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ywan-chungtsiang.top/gtciuowhkg.html

[C03] 可变参数
来源：http://hz.cucudq.cn/gtrsjdrwqt.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhiwuduotai.top/gtxrvybcfh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zdqjudy.top/gtjwwonqiw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtxrsbzkxw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtrmgxkrzk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zdqjudy.top/gtecnlhfzu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hnxiangtu.top/gtaovhaxwj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dianchejie.cn/gtkjctncjd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hongshengwenyu.top/gtfjnsxteq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hfpthk.cn/gtcmglttxc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guowangkeji.top/gtqvongvov.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shuidangran.top/gtuddlyztn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtzzbnbhjg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shzxlz.cn/gtwsnbhzdi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenzaomai.com/gtggqjxkbl.html

Go:   // 无：用配置结构体参数
来源：http://hz.birdmap.top/gtqiwzcsjp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtqrvusmtp.html

C#:   f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtmygvbagy.html

[C05] 返回多个值
来源：http://hz.jinqigfzy.top/gtctaaqlqq.html

Py:   return a, b
来源：http://hz.jianghu66.top/gtgnvbxvat.html

PHP:  return [$a, $b];
来源：http://hz.yonumen.top/gtuqmljmyr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.bjfxy.top/gtwzsgwxrw.html

TS:   return { a, b };
来源：http://hz.xuanzx.com/gtfmbqqqva.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.316326.xyz/gttklpjwhy.html

Go:   return a, b
来源：http://hz.yuxming.cn/gtczzwrdcu.html

Ruby: return a, b
来源：http://hz.hfpthk.cn/gtratrrwdx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.quarkkingdee.top/gtnpixygjp.html

[C06] 匿名函数 / lambda
来源：http://hz.cashguo.top/gtyqofnjyd.html

Py:   square = lambda x: x * x
来源：http://hz.kuanghao11.cn/gtsggfxbab.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.vqdsnc.cn/gtksfozakt.html

JS:   const square = x => x * x;
来源：http://hz.tianlin.xyz/gtuqcheipo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenlongwang.top/gthvnfvjeo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yangfankeji.com/gtggaglttt.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yj202588.top/gtgbdjmnal.html

Ruby: square = ->(x) { x * x }
来源：http://hz.daxiang520.top/gtxzwgvfuc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.havefunace.top/gtsqicbsol.html

[C07] 把函数作为参数传入
来源：http://hz.meibo888.top/gtbitpsdhc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pycfn.com/gtbsbscqgc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sysykeji.top/gtjeepcgph.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.tianlin.xyz/gtxseubups.html

TS:   arr.map(String)
来源：http://hz.9152youxi.cn/gtppybggdx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenjidiqi.icu/gtxkwdrvbv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tian-w.cn/gtfsyckamy.html

Ruby: arr.map(&:upcase)
来源：http://hz.daria6918.cn/gttggbsfct.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.9152youxi.cn/gtatelodul.html

[C08] 闭包
来源：http://hz.pycfn.com/gtrqklcwmh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.andypj.xyz/gtasfapppp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.wangshuangyany.cn/gtragyorrx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtmgakbxze.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtadbdmwot.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gogol.net.cn/gtkcfmrsgq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shzxlz.cn/gthttmmlcg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cashguo.top/gtmvodtqmr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gtkswryetd.html

[C09] 递归
来源：http://hz.fzhhl.top/gtjmvyjpqv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtzgqvfach.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj20258888.top/gtvftavgga.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cashguo.top/gthokgpmms.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hywenlv.cn/gtvlfvmowe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.iojbl.cn/gtppufwhca.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cqqwz.cn/gtexiqeioh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xingfuxueyuan.xyz/gtoqsqjtow.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.pycfn.com/gtfiuwzsgn.html

[C10] 变量作用域
来源：http://hz.hnqzz.top/gtdceiujkf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.9152youxi.cn/gtiekbyryv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxuanxn.top/gttoiihher.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.bjfxy.top/gtgosifvzf.html

TS:   同 JS
来源：http://hz.smart0.xyz/gtblleylyq.html

Java: 方法内为块级作用域
来源：http://hz.xingfuxueyuan.xyz/gtzuoyjyrs.html

Go:   花括号块级作用域
来源：http://hz.shanyushiyangtech.top/gtxftvffcw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cashguo.top/gtwiahiudu.html

C#:   块级作用域
来源：http://hz.zycfv.cn/gttluditlh.html

[C11] 模块导入与导出
来源：http://hz.jyoumei.cn/gtxpupkafj.html

Py:   from module import func
来源：http://hz.redwolf501.top/gtbclvchdu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jqgfzy.top/gtdifzmwde.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zycfv.cn/gtwefashiu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenjidiqi.icu/gthefnnyxt.html

Java: import java.util.List;
来源：http://hz.jianghu66.top/gtbczwhhpz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ywan-chungtsiang.top/gtarenfsxj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.kuanghao11.cn/gtktwfqhur.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtnewifreh.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhaomingkeji.xyz/gtuczewmdb.html

Py:   (lambda: print("run"))()
来源：http://hz.zycfv.cn/gtnpdemrhf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.shanyushiyangtech.top/gtxoeuhfjo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtotakgzey.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hfpthk.cn/gtcwpddzcq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinyuanbaomall.cn/gtuvasosqf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.dianchejie.cn/gtjzjbydhv.html

Ruby: -> { puts "run" }.call
来源：http://hz.ydjk.org.cn/gtacophlhy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhijiandao.cn/gthsolddnr.html

[C13] 类型声明 / 类型注解
来源：http://hz.cashguo.top/gtycwbyrux.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuxming.cn/gtbmvllrnz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gtzvdgmefc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xziqi.cn/gtbfirtiue.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yangfankeji.com/gtouieymet.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gteqozyujy.html

Go:   func add(a, b int) int
来源：http://hz.ywan-chungtsiang.top/gtgqpkrqje.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hfpthk.cn/gtxhcgvmoi.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.birdmap.top/gtisnpufjt.html


<!-- 参考信息 -->