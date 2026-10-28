代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.cucudq.cn/gtovavrjma.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cucudq.cn/gtlbkfzwsj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.fzhhl.top/gtxlpchjcm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.cqqwz.cn/gtfglgfojd.html

Go:   strings.TrimSpace(s)
来源：http://hz.hfpthk.cn/gtufcsmdrb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yangfankeji.com/gtadvjfevw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.9152youxi.cn/gtksrckdkq.html

[A25] 字符串比较
来源：http://hz.ydzc1.top/gtpiornbzf.html

Py:   s1 == s2; s1 != s2
来源：http://hz.gaohongyu789.top/gtfkuxvedl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sweek.top/gtncsgahep.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jlsjyb.cn/gthnspboub.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sxryk.cn/gtymnyynbs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.0kj1m.cn/gtfkpsmmqs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xuetiantiany.cn/gtyncmowfj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinghuilouyu.cn/gtydpsfigd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.vqdsnc.cn/gtqyhmzzzg.html

[A26] 类型转换总览
来源：http://hz.birdmap.top/gtcyhjxogc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhaomingkeji.xyz/gtjzgtwgpq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhengqikj.top/gtdhxmfbxc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.dianchejie.cn/gtaqyazgvl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cqqwz.cn/gtifkdzhpp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.hywenlv.cn/gtjtsgvuvl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenzaomai.com/gtuyuqucok.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yueranfly.top/gtnvblxpwu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.fzhhl.top/gtkioakrqi.html

================================================================================
来源：http://hz.yj20258.top/gtzkivgpcx.html

B. 流程控制
来源：http://hz.zdqjudy.top/gtouzodbne.html

================================================================================
来源：http://hz.c1oappe.top/gtpgepyjsz.html

[B01] 条件判断 if / else
来源：http://hz.smart0.xyz/gtqtcphurl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cucudq.cn/gtuwwhmekr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.feifeiyinyue.top/gtyhabjlcc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtkoqbfgpu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yuanzhike.top/gtffdhezwp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yonumen.top/gtroofeqln.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhaomingkeji.xyz/gtfxqaahsg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.fengsongda.top/gtzzvvzmzd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258.top/gtndunvivy.html

[B02] 多分支 else if / elif
来源：http://hz.jinqigfzy.top/gtvdxtmtpi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.kuanghao11.cn/gtcqaerzrd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xinyue.icu/gtzdqcumsl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gthmnsveet.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.andypj.xyz/gtzvnfczpj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtypgsombn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.tian-w.cn/gthzrqdbtm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.gzhubu.top/gtbnfsotzf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.316326.xyz/gtqbgsldoq.html

[B03] switch / match / case
来源：http://hz.9152youxi.cn/gtbdsmcudt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.haohaochexian.top/gtltifyoyh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.dianchejie.cn/gtynhlbonp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yueranfly.top/gtupvxpxxb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hysaishi.cn/gtsxzcyodh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sweek.top/gtugdbfnwz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.c1oappe.top/gttzzrxyab.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.wangshuangyany.cn/gtlddkugar.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.vqdsnc.cn/gttrvklfxo.html

[B04] for 计数循环
来源：http://hz.hysaishi.cn/gtqwvninxq.html

Py:   for i in range(10): print(i)
来源：http://hz.jinghuilouyu.cn/gtafqjymqp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.smart0.xyz/gtghqyerya.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jiagoushi.top/gtinhvuqvi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.c1oappe.top/gtihvtzqpk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xylfe.cn/gtuluokfiv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hongshengwenyu.top/gtbvjsgxxb.html

Ruby: 10.times { |i| puts i }
来源：http://hz.aibaodan.cn/gtetisqgql.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.shanyushiyangtech.top/gtcoqwchso.html

[B05] 遍历数组 / 列表
来源：http://hz.dashuyun.cn/gtxucbdvrq.html

Py:   for item in arr: print(item)
来源：http://hz.c1oappe.top/gtsvjeunup.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xuetiantiany.cn/gtemzitdtr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ppjwa.cn/gtuakmwthx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.wangshuangyany.cn/gtfmpdvmka.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xylfe.cn/gtyvzsqjit.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zycfv.cn/gtgfhvffkc.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tianlin.xyz/gtkstuynjs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shzxlz.cn/gtvzvrupoi.html

[B06] 遍历字典 / 对象
来源：http://hz.gzhubu.top/gtipgyubnv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ppjwa.cn/gtoqxqcckb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hnxiangtu.top/gtathhncag.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.wangshuangyany.cn/gtrxhnjwum.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yvedp.cn/gtdepswwja.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.aizwys.cn/gtqkenpoej.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ywan-chungtsiang.top/gtzqyfthjf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhongyouzk.top/gtnetdtsgh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.aizwys.cn/gtoemgmdlx.html

[B07] while 循环
来源：http://hz.hysaishi.cn/gtspsazvee.html

Py:   while i < 10: i += 1
来源：http://hz.ppjwa.cn/gtumairqhb.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinyuanbaomall.cn/gtaokiqory.html

JS:   while (i < 10) { i++; }
来源：http://hz.sweek.top/gttikonjmh.html

TS:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtnsddusqj.html

Java: while (i < 10) { i++; }
来源：http://hz.jiagoushi.top/gtzlpdplmp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.bjfxy.top/gthtypgefb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhengqikj.top/gtvymtuqec.html

C#:   while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtkjgkbngo.html

[B08] do-while（至少执行一次）
来源：http://hz.tianlin.xyz/gtmzzoaory.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hnxiangtu.top/gtaodlizoc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.nanxinkj.top/gtdgtvwaur.html

JS:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtwhnykjql.html

TS:   do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gtogeiahga.html

Java: do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtbligoxlk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yvedp.cn/gttwltlsjw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gogol.net.cn/gtwkqvepxz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.iojbl.cn/gtvhxapopy.html

[B09] break 与 continue
来源：http://hz.chenlongwang.top/gtmkcdhdcf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yvedp.cn/gtfbnkmkgp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jqgufenzy.top/gtgmzgjedj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtrrasdxjs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gttygtusvs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtqcpahjgq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.pengpengdd.cyou/gtzdxlflxo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgufenzy.top/gtdtoyuanj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtcjsqffpt.html

[B10] 遍历同时拿索引
来源：http://hz.yanxiufei.cn/gtufztumom.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.havefunace.top/gtlansbyub.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.aibaodan.cn/gtcxvkofvl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.fengsongda.top/gtscvsiqke.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtlgkwmspl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhaomingkeji.xyz/gtlyfzpyem.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.aizwys.cn/gtvfihqosd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinqigufen.top/gtbekqrojf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nanxinkj.top/gtpwlsxviq.html

[B11] 生成数字序列 / 区间
来源：http://hz.xziqi.cn/gtdbadixoj.html

Py:   list(range(0, 10, 2))
来源：http://hz.ywan-chungtsiang.top/gttbldfbpu.html

PHP:  range(0, 10, 2);
来源：http://hz.jinqigufen.top/gtspfsrhnj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.52xcode.cn/gtuzuaqxte.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pycfn.com/gtmnspfetw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cdnleiting.top/gtzjblmqkm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.quarkkingdee.top/gtfizsowhc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.dashuyun.cn/gtppcwzwhs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.iojbl.cn/gtsukslfio.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangtech.top/gtrpuhumck.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cqqwz.cn/gtrxquollq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yonumen.top/gtvdvwyfvi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gtxzgfhsgw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangkeji.top/gteoogfoqv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtnejyfrag.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhijiandao.cn/gtbbhwyvyi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtfzahpizg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sufxvd.cn/gtadwcuqmo.html

[B13] 判断是否为数字
来源：http://hz.zhijiandao.cn/gtemsrhhbp.html

Py:   isinstance(x, (int, float))
来源：http://hz.guannengcc.top/gttevdeoki.html

PHP:  is_numeric($x)
来源：http://hz.smart0.xyz/gtjjlhvnkw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tanke756.top/gtwtdiwurl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.birdmap.top/gtszxvhsxg.html

Java: x instanceof Number
来源：http://hz.gzhubu.top/gtmvleigda.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yuanzhike.top/gtjqexfuqn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hfpthk.cn/gtydgmfqqb.html

C#:   x is int or double or decimal
来源：http://hz.svipenyu.cn/gtoafhhyss.html

[B14] 判断值是否在集合内
来源：http://hz.jinyuanbaomall.cn/gtxctqgzet.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gogol.net.cn/gtuwmyzsmp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxuanxn.top/gtyhdxpqnp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yuanzhike.top/gtesixlcry.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.c1oappe.top/gtwuxoslzg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hongshengwenyu.top/gtymiuqgae.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.316326.xyz/gtphhhecws.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jiagoushi.top/gtfzuwjtdg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhaomingkeji.xyz/gtkbkprheh.html

[B15] 布尔运算与取反
来源：http://hz.sweek.top/gtknmkkqou.html

Py:   a and b or not c
来源：http://hz.guannengcc.top/gtpnpzdiwe.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258888.top/gtdytthhjt.html

JS:   a && b || !c
来源：http://hz.chenzaomai.com/gtbinpkbol.html

TS:   a && b || !c
来源：http://hz.52xcode.cn/gtmdidelhu.html

Java: a && b || !c
来源：http://hz.jinqigufen.top/gtmvfwkkut.html

Go:   a && b || !c
来源：http://hz.jiagoushi.top/gtajycujot.html

Ruby: a && b || !c
来源：http://hz.hammf.cn/gtscfdviak.html

C#:   a && b || !c
来源：http://hz.xylfe.cn/gtiqvfiqhf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shanyushiyangtech.top/gtqspdxbqz.html

Py:   if not data: return
来源：http://hz.gogol.net.cn/gtmxlkkggo.html

PHP:  if (!$data) { return; }
来源：http://hz.chenjidiqi.icu/gtmsszltyl.html

JS:   if (!data) return;
来源：http://hz.yanxiufei.cn/gtcrourbxv.html

TS:   if (!data) return;
来源：http://hz.sweek.top/gtctmxnmmx.html

Java: if (data == null) return;
来源：http://hz.chenzaomai.com/gttgggcswr.html

Go:   if data == nil { return }
来源：http://hz.zycfv.cn/gtxaukwjis.html

Ruby: return if data.nil?
来源：http://hz.redwolf501.top/gtygbnuidu.html

C#:   if (data == null) return;
来源：http://hz.yj20258888.top/gtcykctssj.html

================================================================================
来源：http://hz.52xcode.cn/gtiriqjcps.html

C. 函数与作用域
来源：http://hz.hammf.cn/gttzriqosm.html

================================================================================
来源：http://hz.aizwys.cn/gttrhcfyzj.html

[C01] 定义函数
来源：http://hz.jinqigufen.top/gtxvrozsoo.html

Py:   def add(a, b): return a + b
来源：http://hz.shangyingyoupin.top/gtalkitnkn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtqxbpdkqs.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.dianchejie.cn/gtuynmlolv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yonumen.top/gtfkphokrh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtrjggbjph.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.smart0.xyz/gtzomgvgqr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj20258888.top/gtsngwiaxr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gteolyuzka.html

[C02] 默认参数
来源：http://hz.chenzaomai.com/gtpjqqdyhh.html

Py:   def greet(name="World"): return name
来源：http://hz.cqqwz.cn/gtefjbnkfi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yongpay.top/gtsqanncmz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tian-w.cn/gtjvuqttfl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.iojbl.cn/gtdrgwsdyk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigfzy.top/gthbtamwmr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhengqikj.top/gtharjqbqm.html

Ruby: def greet(name = "World") = name
来源：http://hz.yvedp.cn/gtrnsbxues.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ybcxt.top/gtewhnlqcz.html

[C03] 可变参数
来源：http://hz.yuxming.cn/gtrofwfpto.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhijiandao.cn/gtswoatqgy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zdqjudy.top/gtraikfdsk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhongyouzk.top/gtvfceigxc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtlqnbudgt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hysaishi.cn/gtcymlpbsw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ybcxt.top/gtgfwtlkzn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ybcxt.top/gtfrxjfynq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yvedp.cn/gtunolhqnl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.pengpengdd.cyou/gtqyoscsnj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.tanke756.top/gtwvqbqobw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.guannengcc.top/gtytydntqc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtiasrikbf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daria6918.cn/gtpwxxubrw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnxiangtu.top/gtsfbitrjh.html

Go:   // 无：用配置结构体参数
来源：http://hz.havefunace.top/gtiosokuej.html

Ruby: f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtufkxrauh.html

C#:   f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtbwmhyznt.html

[C05] 返回多个值
来源：http://hz.guannengcc.top/gtlakqgoaf.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtsnflbkib.html

PHP:  return [$a, $b];
来源：http://hz.sysykeji.top/gtzkimiibp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.daxiang520.top/gtnobyxegx.html

TS:   return { a, b };
来源：http://hz.tianlin.xyz/gtstdjknaa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnqzz.top/gtehqzrsel.html

Go:   return a, b
来源：http://hz.nanxuanxn.top/gtxdcznwyr.html

Ruby: return a, b
来源：http://hz.9152youxi.cn/gtyiyyartc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.yj20258888.top/gtemoiystr.html

[C06] 匿名函数 / lambda
来源：http://hz.birdmap.top/gtzaidczol.html

Py:   square = lambda x: x * x
来源：http://hz.guannengcc.top/gtyrrgtbte.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xuanzx.com/gtmniymckx.html

JS:   const square = x => x * x;
来源：http://hz.jinghuilouyu.cn/gtdxxemqzg.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtocxflndn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xuanzx.com/gturofncmf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.snrcjt.cn/gtuwdbffvq.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hongshengwenyu.top/gtahgpbcow.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.svipenyu.cn/gtjhxdemdd.html

[C07] 把函数作为参数传入
来源：http://hz.aibaodan.cn/gtncgfturd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ivvv.top/gtmblqfaxy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.sxryk.cn/gtxwlnxrex.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hnxiangtu.top/gtwkhhegwj.html

TS:   arr.map(String)
来源：http://hz.daria6918.cn/gtnjueqvlt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj202588.top/gtdbozxrnx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenjidiqi.icu/gtvrkxuxbi.html

Ruby: arr.map(&:upcase)
来源：http://hz.andypj.xyz/gtckjuoaqk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gtesraiidv.html

[C08] 闭包
来源：http://hz.gzhubu.top/gtpizdrkat.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.smart0.xyz/gtzbceciyk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cucudq.cn/gtvmqeyjnu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nwbrower.top/gtpwkzhmve.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtoynylxan.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zdqjudy.top/gtohkzgnfh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gtwebbzbud.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.havefunace.top/gtxdinuuai.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zycfv.cn/gtmejnkdcq.html

[C09] 递归
来源：http://hz.jinqigufen.top/gtglehambq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinyuanbaomall.cn/gtsoanaplx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhixingplan.top/gtxcazarjv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtrzfjfqid.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtxemnmixh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hammf.cn/gtzwbphzjx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cdnleiting.top/gtuybrioxv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xziqi.cn/gtftfluape.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.dashuyun.cn/gtoovajnco.html

[C10] 变量作用域
来源：http://hz.birdmap.top/gtrwlmnqlj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj202588.top/gtfszvgois.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgufenzy.top/gtyvjlfmms.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.wangshuangyany.cn/gtwgcdsekj.html

TS:   同 JS
来源：http://hz.yj20258888.top/gtvwdoyajd.html

Java: 方法内为块级作用域
来源：http://hz.nanxuanxn.top/gtlraenxqm.html

Go:   花括号块级作用域
来源：http://hz.hnqzz.top/gtgghqphmt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yuanzhike.top/gtaizbjxcy.html

C#:   块级作用域
来源：http://hz.xziqi.cn/gtyhygphfa.html

[C11] 模块导入与导出
来源：http://hz.nwbrower.top/gtfhrsnyyf.html

Py:   from module import func
来源：http://hz.aibaodan.cn/gtqdivqapo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yonumen.top/gtdpohraqb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zhaomingkeji.xyz/gtuhffruvi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.fzhhl.top/gtfezouslh.html

Java: import java.util.List;
来源：http://hz.sxryk.cn/gtgxttyqdt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.quarkkingdee.top/gtnimvqfya.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.meibo888.top/gtdkhwpuip.html

C#:   using System.Text;
来源：http://hz.yongpay.top/gtdwbktvyw.html

[C12] 立即执行函数 IIFE
来源：http://hz.xziqi.cn/gtqypngqox.html

Py:   (lambda: print("run"))()
来源：http://hz.svipenyu.cn/gtdfkicguo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guannengcc.top/gtydiuvsbm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtcdsezmfh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yongpay.top/gtjojntjko.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.snrcjt.cn/gtsnpobqrj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zycfv.cn/gtwzclzhnr.html

Ruby: -> { puts "run" }.call
来源：http://hz.sweek.top/gtcdkttibl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.smart0.xyz/gtrfvrzvfe.html

[C13] 类型声明 / 类型注解
来源：http://hz.xinyue.icu/gtdhmwolxn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hfpthk.cn/gttfztzjjk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gthrfcwonj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gtixjyxokb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gtxbdjumyg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtgypppsel.html

Go:   func add(a, b int) int
来源：http://hz.jiagoushi.top/gtdvbqbwqx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ehwqpu.com/gtjqfxikkb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.316326.xyz/gtsvshmuay.html

[C14] 泛型函数
来源：http://hz.shanyushiyangtech.top/gtgxbxinlq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj202588.top/gtquueehll.html

PHP:  // 无泛型
来源：http://hz.bjfxy.top/gtfhgddvmu.html

JS:   // 无泛型
来源：http://hz.svipenyu.cn/gtkovehdvg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.smart0.xyz/gtrfzapmwl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.guowangkeji.top/gtgalhjjpc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gogol.net.cn/gtkwzotecn.html

Ruby: # 无泛型
来源：http://hz.tianlin.xyz/gtgxulujhy.html


<!-- 参考信息 -->