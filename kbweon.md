代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.daria6918.cn/gtudgumfbz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhongyouzk.top/gtgrjmcypn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yangfankeji.com/gtngjuyyea.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xziqi.cn/gtcalflrbh.html

Go:   strings.TrimSpace(s)
来源：http://hz.daxiang520.top/gtfhrfitsg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yonumen.top/gtpifecygb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yanxiufei.cn/gtzastidgs.html

[A25] 字符串比较
来源：http://hz.gaohongyu789.top/gtykuoqxkt.html

Py:   s1 == s2; s1 != s2
来源：http://hz.hywenlv.cn/gthucqwqws.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cqqwz.cn/gtosbbmcrb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yanxiufei.cn/gtkclhdaom.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aizwys.cn/gtvkjwkcxm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.smart0.xyz/gtthergida.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yj20258888.top/gttdfjgixr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yanxiufei.cn/gtuajqohfm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.shzxlz.cn/gtcnqdisju.html

[A26] 类型转换总览
来源：http://hz.feifeiyinyue.top/gthvslvlve.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xziqi.cn/gtuzjtsudb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ehwqpu.com/gtgsceqxjv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sxryk.cn/gtvmjszerd.html

TS:   Number() String() Boolean() x as number
来源：http://hz.gotoacloud.top/gtuzdyezka.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jinqigfzy.top/gtcaxlmazs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.tianlin.xyz/gtjaomtayz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.xingfuxueyuan.xyz/gtfiuensne.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ehwqpu.com/gtngzhysur.html

================================================================================
来源：http://hz.jyoumei.cn/gtgukzzoir.html

B. 流程控制
来源：http://hz.mhx1999.top/gtiwkwcucm.html

================================================================================
来源：http://hz.fengsongda.top/gtvcmpspch.html

[B01] 条件判断 if / else
来源：http://hz.jinghuilouyu.cn/gtsosznibg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cheryme.top/gtyvfeaobr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.redwolf501.top/gtmzopvojk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.svipenyu.cn/gtoxgtzsyt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.haohaochexian.top/gtdtfegyux.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhiwuduotai.top/gtqkbzelvq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.tian-w.cn/gtjwcuhbnc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.dianchejie.cn/gtgyukxpil.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yonumen.top/gtoabjqqgb.html

[B02] 多分支 else if / elif
来源：http://hz.gotoacloud.top/gteoxijhzh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cqqwz.cn/gtgtbevjlb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shangyingyoupin.top/gtnctzhkmq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtdyuatsew.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtlxicgaig.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtjgxppdhh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.chenlongwang.top/gtbcunfygv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhiwuduotai.top/gtyctzqzbk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtqplvjfsh.html

[B03] switch / match / case
来源：http://hz.zhongyouzk.top/gtflafnnoy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jinqigfzy.top/gtdjevkwqu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.nanxinkj.top/gtmirkfcpj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.pycfn.com/gtzxbaebba.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.dianchejie.cn/gtmxmwlkdl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.ivvv.top/gtutacimsv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yueranfly.top/gtkutkaqnd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.xingfuxueyuan.xyz/gttwmbhghc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.shuidangran.top/gtifgnefww.html

[B04] for 计数循环
来源：http://hz.nanxuanxn.top/gtcrcxqiyx.html

Py:   for i in range(10): print(i)
来源：http://hz.xylfe.cn/gtbfatfewq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shanyushiyangkeji.top/gtfusyhkhe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhongyouzk.top/gtjdxlyrwl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ydjk.org.cn/gtitoysxap.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shuidangran.top/gtustseepl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xinyue.icu/gthqxwdwgu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yuanzhike.top/gtehrwwufk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xziqi.cn/gtvpmmkccv.html

[B05] 遍历数组 / 列表
来源：http://hz.vqdsnc.cn/gtnjigfrwp.html

Py:   for item in arr: print(item)
来源：http://hz.shuidangran.top/gteyhltoyj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hywenlv.cn/gtjypuurte.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.dianchejie.cn/gtsbezkaji.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sweek.top/gtlkbkwohg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hfpthk.cn/gttmronjtm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zdqjudy.top/gtotnozdtz.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhongyouzk.top/gtgfwizhrh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.chenzaomai.com/gtwlzfovas.html

[B06] 遍历字典 / 对象
来源：http://hz.vqdsnc.cn/gtldmypjuk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.gotoacloud.top/gtiskqqsvs.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xuetiantiany.cn/gtngnvupnp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuetiantiany.cn/gthqvdoomm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinyuanbaomall.cn/gthrrvluun.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.daxiang520.top/gtijemlwub.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhiwuduotai.top/gtmpbepdbb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nanxinkj.top/gtucecitmm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hongshengwenyu.top/gtegfspppt.html

[B07] while 循环
来源：http://hz.mhx1999.top/gtnlftnblj.html

Py:   while i < 10: i += 1
来源：http://hz.daxiang520.top/gtitryyjki.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.meibo888.top/gtbasyyiig.html

JS:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtluwlbqff.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gtrzhmpzoy.html

Java: while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtsqgbruuy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.redwolf501.top/gtwbdqvzgp.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yonumen.top/gtjwpalggj.html

C#:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtlucpqvhw.html

[B08] do-while（至少执行一次）
来源：http://hz.svipenyu.cn/gteeqbxsce.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nwbrower.top/gtyfuedowi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shanyushiyangkeji.top/gtmiglnrju.html

JS:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtvpyaoetm.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hfpthk.cn/gtsbhkyoyg.html

Java: do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtlaqwfujr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shuidangran.top/gtsdphqtkk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yj20258.top/gtfopgfjdk.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtqrsmhgcn.html

[B09] break 与 continue
来源：http://hz.ywan-chungtsiang.top/gtjpzczdap.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hongshengwenyu.top/gtunaiqaiu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yuanzhike.top/gtgckmoyhy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.kuanghao11.cn/gtbkrtfgkf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtixahulub.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtbfkohnjm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cdnleiting.top/gtkgspeknj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hywenlv.cn/gtgsocharh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtlzhrmfsy.html

[B10] 遍历同时拿索引
来源：http://hz.nanxuanxn.top/gthmhhfien.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ybcxt.top/gtvodmufwj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hfpthk.cn/gtjgzaksxw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhixingplan.top/gtfprsehuu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tanke756.top/gtiamakjst.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cheryme.top/gtuyocgpeg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shanyushiyangkeji.top/gtfgzfdzln.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jqgfzy.top/gtbztjweoj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.iojbl.cn/gtgbmsuzna.html

[B11] 生成数字序列 / 区间
来源：http://hz.andypj.xyz/gtftviudkz.html

Py:   list(range(0, 10, 2))
来源：http://hz.quarkkingdee.top/gtdpvyoupv.html

PHP:  range(0, 10, 2);
来源：http://hz.yongpay.top/gtkzjtnbgo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtobprxukg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtohllcfvi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shuidangran.top/gtpbhfmfyt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.meibo888.top/gtyicgttvq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jianghu66.top/gtyoiiyvxx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenjidiqi.icu/gtuwwaspws.html

[B12] 跳出多层循环
来源：http://hz.ppjwa.cn/gtxtgqnfsm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yanxiufei.cn/gtryaukdnk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenzaomai.com/gtmeejkmti.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtsjorakdr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtgmgwalef.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhengqikj.top/gtyavvjqlr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinqigufen.top/gtganjzbfi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.xingfuxueyuan.xyz/gtuyuudbhr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnxiangtu.top/gthnfekrss.html

[B13] 判断是否为数字
来源：http://hz.bjfxy.top/gtegwcoyos.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuetiantiany.cn/gthhpitrud.html

PHP:  is_numeric($x)
来源：http://hz.zhongyouzk.top/gtlynwnjjh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yueranfly.top/gtnyaechua.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shuidangran.top/gtukrrtzzs.html

Java: x instanceof Number
来源：http://hz.cucudq.cn/gtoqxxibxf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangdashe.top/gtdzxjzuii.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sufxvd.cn/gtdcccoqlt.html

C#:   x is int or double or decimal
来源：http://hz.haohaochexian.top/gtlmanlfmk.html

[B14] 判断值是否在集合内
来源：http://hz.jiagoushi.top/gtpilocxwc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tanke756.top/gtlranozov.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xinyue.icu/gtbbciaziv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtldvayyrp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.snrcjt.cn/gtvctvjnpd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.quarkkingdee.top/gtyyvcremt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenzaomai.com/gtbngvakka.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.havefunace.top/gtiuqsrevj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yueranfly.top/gtslchocav.html

[B15] 布尔运算与取反
来源：http://hz.shangyingyoupin.top/gtwfnyfiou.html

Py:   a and b or not c
来源：http://hz.hfpthk.cn/gtvmjqjadz.html

PHP:  $a && $b || !$c
来源：http://hz.0kj1m.cn/gtplelhaub.html

JS:   a && b || !c
来源：http://hz.bjfxy.top/gtlmhywhuf.html

TS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtkbqtnrtj.html

Java: a && b || !c
来源：http://hz.jiagoushi.top/gtgyldbnzc.html

Go:   a && b || !c
来源：http://hz.cdnleiting.top/gtzxlgcgjs.html

Ruby: a && b || !c
来源：http://hz.0kj1m.cn/gtfqixluwu.html

C#:   a && b || !c
来源：http://hz.yanxiufei.cn/gtypgjjswz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinghuilouyu.cn/gttssazsst.html

Py:   if not data: return
来源：http://hz.ivvv.top/gtdbzumudl.html

PHP:  if (!$data) { return; }
来源：http://hz.zhaomingkeji.xyz/gttccqcoke.html

JS:   if (!data) return;
来源：http://hz.sysykeji.top/gtrybnuavb.html

TS:   if (!data) return;
来源：http://hz.shzxlz.cn/gtgnpcjuwl.html

Java: if (data == null) return;
来源：http://hz.c1oappe.top/gtspwnmeum.html

Go:   if data == nil { return }
来源：http://hz.zhixingplan.top/gtjhmyzvgd.html

Ruby: return if data.nil?
来源：http://hz.yangfankeji.com/gtjukjdmvx.html

C#:   if (data == null) return;
来源：http://hz.yuanzhike.top/gtopasfvir.html

================================================================================
来源：http://hz.9152youxi.cn/gtpyicfhjk.html

C. 函数与作用域
来源：http://hz.yanxiufei.cn/gtqtkrnjsw.html

================================================================================
来源：http://hz.fzhhl.top/gtfadzyqid.html

[C01] 定义函数
来源：http://hz.smart0.xyz/gtbnwmkroj.html

Py:   def add(a, b): return a + b
来源：http://hz.yj20258.top/gtwczvssnx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jiagoushi.top/gtrfgmmtlo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.birdmap.top/gtqrejfggi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigufen.top/gtwkxwuzde.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtiejwwhrd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shuidangran.top/gtgsvijvtb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenjidiqi.icu/gtvswwqybm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtkqxtevam.html

[C02] 默认参数
来源：http://hz.zycfv.cn/gtdosfqsxn.html

Py:   def greet(name="World"): return name
来源：http://hz.tianlin.xyz/gtfmmhgnza.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jiagoushi.top/gtlrtfbucl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jyoumei.cn/gtuwgblbck.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtffurbpsz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tanke756.top/gtrlheoctx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yanxiufei.cn/gtlxzeyskt.html

Ruby: def greet(name = "World") = name
来源：http://hz.tanke756.top/gtocbbubbp.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jiagoushi.top/gtitjmzxqb.html

[C03] 可变参数
来源：http://hz.wangshuangyany.cn/gthdpntjhy.html

Py:   def total(*args): return sum(args)
来源：http://hz.daria6918.cn/gtfaadhgaf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.tian-w.cn/gtcwmmedit.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtdvizmcna.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.redwolf501.top/gtnrouftpx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sysykeji.top/gtzueefrfn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangkeji.top/gttojfayju.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yuanzhike.top/gtawovzyxj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gogol.net.cn/gtejwhmqvh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.redwolf501.top/gtubnfmejz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenlongwang.top/gthtvovvgt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jiagoushi.top/gtcvxfvrfn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cashguo.top/gtrgcknppm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sweek.top/gtdoofzblo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jqgufenzy.top/gtajlkeddd.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhixingplan.top/gthkjnfsna.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtfaxdywnp.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhaomingkeji.xyz/gtynxkntgk.html

[C05] 返回多个值
来源：http://hz.yonumen.top/gteooqdswl.html

Py:   return a, b
来源：http://hz.birdmap.top/gtkqdflbam.html

PHP:  return [$a, $b];
来源：http://hz.gaohongyu789.top/gtwntyojoe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.andypj.xyz/gtdlerxkoy.html

TS:   return { a, b };
来源：http://hz.jinqigfzy.top/gtnxtjxulb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sxryk.cn/gtnfljamli.html

Go:   return a, b
来源：http://hz.pycfn.com/gtsphrwyui.html

Ruby: return a, b
来源：http://hz.shanyushiyangkeji.top/gtsfsjkcon.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtejrotcbh.html

[C06] 匿名函数 / lambda
来源：http://hz.hywenlv.cn/gtvpfnnsrv.html

Py:   square = lambda x: x * x
来源：http://hz.ivvv.top/gtsvfspiyw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jqgufenzy.top/gtichrpxlz.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtglvmwxko.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.feifeiyinyue.top/gttyxchurd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yueranfly.top/gtaciajjhg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.xylfe.cn/gtcytcxaxq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinqigfzy.top/gtufxedkfu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnqzz.top/gteqpymavl.html

[C07] 把函数作为参数传入
来源：http://hz.tianlin.xyz/gtxaasxnxb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.dianchejie.cn/gtigebhalf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangkeji.top/gtofvbwzpw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.bjfxy.top/gthvpardfl.html

TS:   arr.map(String)
来源：http://hz.yangfankeji.com/gtlrswqpir.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.cqqwz.cn/gtgbredyiw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.haohaochexian.top/gtulhkvzwq.html

Ruby: arr.map(&:upcase)
来源：http://hz.fzhhl.top/gttfjlvqoh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.snrcjt.cn/gtncazsibw.html

[C08] 闭包
来源：http://hz.316326.xyz/gtapcjhrcb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.wangdashe.top/gtqqzzscms.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ywan-chungtsiang.top/gtdhohklbe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guannengcc.top/gticiswgfa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtipgabrbh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.daria6918.cn/gtryrjnala.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yongpay.top/gtosjrldov.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hysaishi.cn/gtokcjxpxe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtxcqskpno.html

[C09] 递归
来源：http://hz.shuidangran.top/gtwzxkefvu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.daria6918.cn/gtfgurfxhi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.guannengcc.top/gtitwknhlj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtbsnekcuc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hfpthk.cn/gtspchrxzp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gzhubu.top/gtrrppzsey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zdqjudy.top/gtqutjjgpm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtqsoqlcwb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cucudq.cn/gtxouaeadt.html

[C10] 变量作用域
来源：http://hz.svipenyu.cn/gtcarmenry.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.nanxinkj.top/gtnowarvho.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtjerfpcir.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nwbrower.top/gtxxrishqn.html

TS:   同 JS
来源：http://hz.hammf.cn/gtouqfowbw.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtihywrwof.html

Go:   花括号块级作用域
来源：http://hz.kuanghao11.cn/gtvkexfoyc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.gotoacloud.top/gtzmzzslgz.html

C#:   块级作用域
来源：http://hz.chenzaomai.com/gtkoiqhgvq.html

[C11] 模块导入与导出
来源：http://hz.fzhhl.top/gtkkgrttwk.html

Py:   from module import func
来源：http://hz.sufxvd.cn/gtuazeweox.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sxryk.cn/gtdlqenmwg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jyoumei.cn/gterkswckp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.kuanghao11.cn/gtaetkqbgf.html

Java: import java.util.List;
来源：http://hz.xziqi.cn/gtzjnficoa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtitfiljog.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sweek.top/gtjqauirpf.html

C#:   using System.Text;
来源：http://hz.havefunace.top/gtgnvunjeu.html

[C12] 立即执行函数 IIFE
来源：http://hz.daxiang520.top/gtatjrhwxe.html

Py:   (lambda: print("run"))()
来源：http://hz.guannengcc.top/gtgwbxecpn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sufxvd.cn/gtfbsufhwq.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtevelikzl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.chenzaomai.com/gtvrsfhzia.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daria6918.cn/gtwkimojjv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xuanzx.com/gtvbynubfk.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtawohpryx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.redwolf501.top/gtgkeobtkc.html

[C13] 类型声明 / 类型注解
来源：http://hz.cashguo.top/gtlqajhicn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sufxvd.cn/gtoyurchqo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtwgndqbvk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.daxiang520.top/gtlybteekb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtkfhhkypg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtszretmyt.html

Go:   func add(a, b int) int
来源：http://hz.aibaodan.cn/gtjmhuiowp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenlongwang.top/gtitiwbgnu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yongpay.top/gtfccttbga.html

[C14] 泛型函数
来源：http://hz.nanxinkj.top/gtaqcfelch.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangtech.top/gtyfzhahks.html

PHP:  // 无泛型
来源：http://hz.ydzc1.top/gtqqmxyfcd.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtanirogfd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ivvv.top/gtkemktdlt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yvedp.cn/gtnyyovnam.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.bjfxy.top/gtlboazjjl.html

Ruby: # 无泛型
来源：http://hz.sysykeji.top/gtrqlsymqr.html


<!-- 参考信息 -->