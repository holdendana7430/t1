代发 wailian999

[A22] 获取字符串长度
来源：http://hz.dashuyun.cn/gtypxlxpvq.html

Py:   len(s)
来源：http://hz.hywenlv.cn/gtdewsfvsx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yueranfly.top/gtrpyfmyov.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jianghu66.top/gtdlezlcdu.html

TS:   s.length
来源：http://hz.gotoacloud.top/gtveklzsey.html

Java: s.length()
来源：http://hz.jinghuilouyu.cn/gtzrnijwve.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jinqigfzy.top/gtloqyqdbh.html

Ruby: s.length
来源：http://hz.sweek.top/gthqojoyhn.html

C#:   s.Length
来源：http://hz.daria6918.cn/gtbrkpkagc.html

[A23] 大小写转换
来源：http://hz.sysykeji.top/gtaotobxld.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.havefunace.top/gtfzuvtnmc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ydzc1.top/gtrqfxhszm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigfzy.top/gtjxnfntep.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhijiandao.cn/gtsctmczam.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.redwolf501.top/gtwzuxuwoq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ehwqpu.com/gtkpzwiaqr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.birdmap.top/gtugavtrjv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.hywenlv.cn/gtqgeuetkj.html

[A24] 去除首尾空白
来源：http://hz.pengpengdd.cyou/gtatzfgdkl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yj20258888.top/gtosurzrfr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.tanke756.top/gtmweecxpj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xylfe.cn/gtiisykhjc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.mhx1999.top/gtyhsddpev.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shanyushiyangtech.top/gtndhjxbeg.html

Go:   strings.TrimSpace(s)
来源：http://hz.xinyue.icu/gtkvpffmtp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xylfe.cn/gtenrpfvlb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cheryme.top/gtiivgqdnu.html

[A25] 字符串比较
来源：http://hz.c1oappe.top/gtmazzspaz.html

Py:   s1 == s2; s1 != s2
来源：http://hz.daria6918.cn/gtosogesqj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yueranfly.top/gttgsnqjmb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.guannengcc.top/gtlqzbmewg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.316326.xyz/gtzwsqixlh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ppjwa.cn/gtyabubiax.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jinghuilouyu.cn/gtxbokrhmn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.gaohongyu789.top/gtkqrahjlt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.feifeiyinyue.top/gtdwlaprcl.html

[A26] 类型转换总览
来源：http://hz.fengsongda.top/gttnopgbqd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jinqigfzy.top/gthzhzeuvd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gotoacloud.top/gtxhzorhpp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sweek.top/gtyvdghyjp.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sysykeji.top/gtvybuleuz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zdqjudy.top/gtxbcuejue.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.bjfxy.top/gtxatnfcmx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.sufxvd.cn/gtvpwrfavz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xuetiantiany.cn/gtuymnvhzl.html

================================================================================
来源：http://hz.gogol.net.cn/gtroohaiyn.html

B. 流程控制
来源：http://hz.yuanzhike.top/gtfhnspjii.html

================================================================================
来源：http://hz.jlsjyb.cn/gtxwywqkqt.html

[B01] 条件判断 if / else
来源：http://hz.zhongyouzk.top/gtsijfkjwc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jlsjyb.cn/gtkqxyrabk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yuxming.cn/gtcbatfoem.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtityuiqhn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtjyopzivr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gtyyqqwnun.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jyoumei.cn/gtpdbyekgd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.0kj1m.cn/gtmunhyivq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.kuanghao11.cn/gtlqhscdqj.html

[B02] 多分支 else if / elif
来源：http://hz.feifeiyinyue.top/gtudrwttsd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.sxryk.cn/gtxrhrcisj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gaohongyu789.top/gtghwulaqd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jianghu66.top/gtqgnladoo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtrioqsnps.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtzpvwgrvj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.smart0.xyz/gteyhzptqv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.iojbl.cn/gtyewrgrsr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gtnozoqeri.html

[B03] switch / match / case
来源：http://hz.redwolf501.top/gtqxmgoqes.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.guowangkeji.top/gtuuggxvbm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daxiang520.top/gtcqgjnhnt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.dianchejie.cn/gtblrxgmey.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgfzy.top/gtfmxbgzvj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.9152youxi.cn/gtwvwkcefr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jiagoushi.top/gtisqgqusp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.pengpengdd.cyou/gtnsanhmss.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yonumen.top/gtyicsbbtj.html

[B04] for 计数循环
来源：http://hz.vqdsnc.cn/gtqoktjpei.html

Py:   for i in range(10): print(i)
来源：http://hz.daxiang520.top/gtngkwiwyk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.kuanghao11.cn/gtrfpcjhvh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sysykeji.top/gtjyhjsjsf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhiwuduotai.top/gtevdvzthm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yangfankeji.com/gtthmfswef.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.svipenyu.cn/gtygrccfxk.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhiwuduotai.top/gtzgjtohsf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.sysykeji.top/gtkudyvzdy.html

[B05] 遍历数组 / 列表
来源：http://hz.yvedp.cn/gtudjeffvw.html

Py:   for item in arr: print(item)
来源：http://hz.ppjwa.cn/gtvggqgpbl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zycfv.cn/gtfcacgxrj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tanke756.top/gthdljqxtg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.gzhubu.top/gtdutwhvwd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ydzc1.top/gtrzusjfzy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yj202588.top/gtbvqlrgwg.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yvedp.cn/gtpvoupvez.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yuxming.cn/gtamvdfqcl.html

[B06] 遍历字典 / 对象
来源：http://hz.fengsongda.top/gtkrweuvcy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuanzhike.top/gtalqygqmk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.iojbl.cn/gtyisvuitl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj202588.top/gtwbnktsna.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.haohaochexian.top/gtuzkatgcm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.pengpengdd.cyou/gtnnhqjgwo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yangfankeji.com/gtbllamocz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jianghu66.top/gtdrcqttjv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cdnleiting.top/gtstuztrrp.html

[B07] while 循环
来源：http://hz.jqgfzy.top/gtyanpvkfu.html

Py:   while i < 10: i += 1
来源：http://hz.jianghu66.top/gtpfygkvna.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sweek.top/gtoidkwtuk.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtqcbdwuty.html

TS:   while (i < 10) { i++; }
来源：http://hz.tianlin.xyz/gtobgukfxr.html

Java: while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtnrzfhygo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jianghu66.top/gtfewzxttk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhixingplan.top/gtvtkbzudm.html

C#:   while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gtboiuzqob.html

[B08] do-while（至少执行一次）
来源：http://hz.xingfuxueyuan.xyz/gtjthuzjwr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hammf.cn/gtqdkwnffe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhiwuduotai.top/gtibpymjsv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtzaskyfnw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtofvdfxio.html

Java: do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtqnhrjjyl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.snrcjt.cn/gtmyyduqdc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.cheryme.top/gtofrwxmao.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtlsegdqst.html

[B09] break 与 continue
来源：http://hz.yj202588.top/gtydhlpvta.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.daria6918.cn/gthclnztkf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj20258.top/gtrqehwrzd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtevtvnnds.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yvedp.cn/gtyguoelir.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtvcddxtji.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.svipenyu.cn/gtuilsurwl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.haohaochexian.top/gtxyutmbfc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtfvvsnrtu.html

[B10] 遍历同时拿索引
来源：http://hz.zdqjudy.top/gtmkwgswgs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.redwolf501.top/gtcanpkntf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shzxlz.cn/gtldjnbmmh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.chenlongwang.top/gtfuyxkmfc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gtcjyvvxsn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zdqjudy.top/gtenrhpnxs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.iojbl.cn/gtnxbuldng.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.nanxinkj.top/gtzhelcygm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shangyingyoupin.top/gtibfmfekj.html

[B11] 生成数字序列 / 区间
来源：http://hz.cqqwz.cn/gtxpbprzlr.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtbpidwpmn.html

PHP:  range(0, 10, 2);
来源：http://hz.gotoacloud.top/gtflujsdat.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sweek.top/gtmpeldhpg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yueranfly.top/gtngalhaov.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yuxming.cn/gtakyhwerx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.nwbrower.top/gtyjsgeodo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenjidiqi.icu/gtkfrxbimf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jianghu66.top/gttebyvwpo.html

[B12] 跳出多层循环
来源：http://hz.jiagoushi.top/gtlhmwikkt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhongyouzk.top/gtqgvgfdci.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yj202588.top/gtsxiiefjc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtxkqinpcx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtskgicueh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigfzy.top/gtusszglna.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zdqjudy.top/gtsclsmnel.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhixingplan.top/gtaecabmvi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ivvv.top/gtxnxakqbu.html

[B13] 判断是否为数字
来源：http://hz.hfpthk.cn/gtuwdllkhe.html

Py:   isinstance(x, (int, float))
来源：http://hz.zycfv.cn/gtpbqbsana.html

PHP:  is_numeric($x)
来源：http://hz.aizwys.cn/gtinnrhcuy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtkrqlistg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xylfe.cn/gthnmtcasq.html

Java: x instanceof Number
来源：http://hz.aibaodan.cn/gtgkideeqf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jqgfzy.top/gtljvvzzfo.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cqqwz.cn/gtnjnsyqbk.html

C#:   x is int or double or decimal
来源：http://hz.ppjwa.cn/gtknmbqmvt.html

[B14] 判断值是否在集合内
来源：http://hz.iojbl.cn/gtmnfdoggr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ywan-chungtsiang.top/gttyvevhtm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydjk.org.cn/gtcwqnnexp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangdashe.top/gtdxulnouz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guowangkeji.top/gtzjryzxri.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuanzhike.top/gtugvsnvpy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sxryk.cn/gtoronosys.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhixingplan.top/gtxjbgkxum.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.meibo888.top/gtbqnblvbw.html

[B15] 布尔运算与取反
来源：http://hz.chenlongwang.top/gtspxiunhj.html

Py:   a and b or not c
来源：http://hz.havefunace.top/gtdumgulhu.html

PHP:  $a && $b || !$c
来源：http://hz.zdqjudy.top/gtnchyoujz.html

JS:   a && b || !c
来源：http://hz.zhengqikj.top/gtnnpfqmep.html

TS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtzcyakhoq.html

Java: a && b || !c
来源：http://hz.tianlin.xyz/gtpnevfnsd.html

Go:   a && b || !c
来源：http://hz.iojbl.cn/gtocrixkou.html

Ruby: a && b || !c
来源：http://hz.yangfankeji.com/gtqfndwxgx.html

C#:   a && b || !c
来源：http://hz.daxiang520.top/gtjraoxdzr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.52xcode.cn/gttzdhwjtb.html

Py:   if not data: return
来源：http://hz.kuanghao11.cn/gtvzjleezs.html

PHP:  if (!$data) { return; }
来源：http://hz.hfpthk.cn/gtacpebspr.html

JS:   if (!data) return;
来源：http://hz.dashuyun.cn/gtbzlujssv.html

TS:   if (!data) return;
来源：http://hz.wangdashe.top/gtehabkgpx.html

Java: if (data == null) return;
来源：http://hz.chenlongwang.top/gthzzidtzi.html

Go:   if data == nil { return }
来源：http://hz.andypj.xyz/gtoywbqlxq.html

Ruby: return if data.nil?
来源：http://hz.jinghuilouyu.cn/gtzvcfwrnb.html

C#:   if (data == null) return;
来源：http://hz.iojbl.cn/gtaodhkmmh.html

================================================================================
来源：http://hz.yonumen.top/gtvdbrkbwn.html

C. 函数与作用域
来源：http://hz.ivvv.top/gtyxnqrloo.html

================================================================================
来源：http://hz.havefunace.top/gtukkrudwp.html

[C01] 定义函数
来源：http://hz.c1oappe.top/gtrfuxrzgq.html

Py:   def add(a, b): return a + b
来源：http://hz.hysaishi.cn/gtqxhfvssw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yanxiufei.cn/gtybqtxlee.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gterwqinli.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtrzuuqcnc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtcajgxojv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cqqwz.cn/gtaelybogo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yj202588.top/gtbwdnpfme.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtebaqftei.html

[C02] 默认参数
来源：http://hz.shanyushiyangtech.top/gtmmhnnvqt.html

Py:   def greet(name="World"): return name
来源：http://hz.cashguo.top/gtdbzptwhr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhijiandao.cn/gtetmdiqwv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dianchejie.cn/gtokfwrqqt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ehwqpu.com/gtwagroszz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xylfe.cn/gtpxfdsnjl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.bjfxy.top/gtmxlvoxss.html

Ruby: def greet(name = "World") = name
来源：http://hz.ehwqpu.com/gthzfnawqn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258888.top/gtvckzdoef.html

[C03] 可变参数
来源：http://hz.yongpay.top/gtcyxmlxeu.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuetiantiany.cn/gtfswrmbww.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangdashe.top/gtiaanxaou.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtplipmwum.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pycfn.com/gtpzbhxykc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.gotoacloud.top/gtqiyiwuoe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgfzy.top/gtrticuyxq.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zdqjudy.top/gthsblrhmb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nwbrower.top/gthduyfhjk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sxryk.cn/gtsewgihqp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fengsongda.top/gtaygfmlyz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinyuanbaomall.cn/gtmeyajadn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtvgelkqis.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinqigfzy.top/gtbhmunhhe.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shuidangran.top/gtlvfhslfz.html

Go:   // 无：用配置结构体参数
来源：http://hz.bjfxy.top/gtpxpbjizj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtcwhkuybl.html

C#:   f(a: 1, b: 2)
来源：http://hz.gaohongyu789.top/gtlstmncms.html

[C05] 返回多个值
来源：http://hz.chenjidiqi.icu/gtdmrjvweu.html

Py:   return a, b
来源：http://hz.zhoulong.xyz/gtwueigknw.html

PHP:  return [$a, $b];
来源：http://hz.52xcode.cn/gtxpsoqhqy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hammf.cn/gtovimfnkx.html

TS:   return { a, b };
来源：http://hz.zhoulong.xyz/gteptdoaqr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shangyingyoupin.top/gtdcwkqdoy.html

Go:   return a, b
来源：http://hz.chenlongwang.top/gtpmzmrxuo.html

Ruby: return a, b
来源：http://hz.guannengcc.top/gtpjyogkbm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangdashe.top/gtijqlagqr.html

[C06] 匿名函数 / lambda
来源：http://hz.zhaomingkeji.xyz/gtojaptpwo.html

Py:   square = lambda x: x * x
来源：http://hz.haohaochexian.top/gtwnrsgfod.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhiwuduotai.top/gtwwyqmufd.html

JS:   const square = x => x * x;
来源：http://hz.wangdashe.top/gtdngueope.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cdnleiting.top/gtozwzfamz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hfpthk.cn/gtrutsdtfn.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yongpay.top/gtizqjzjgt.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yj202588.top/gtcgogtnag.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tianlin.xyz/gtnwnyvguy.html

[C07] 把函数作为参数传入
来源：http://hz.xziqi.cn/gtchyuwcpc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ppjwa.cn/gtjfizvuwa.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.316326.xyz/gtxrwmrvdn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daxiang520.top/gteivuitlt.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangkeji.top/gtzkwsfwaz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.316326.xyz/gtphplvnae.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aizwys.cn/gtitzvnnht.html

Ruby: arr.map(&:upcase)
来源：http://hz.tianlin.xyz/gtxqvmlwxu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.tianlin.xyz/gtdhgcvpkx.html

[C08] 闭包
来源：http://hz.ehwqpu.com/gtaebjnpzo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258.top/gtvntrhair.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhongyouzk.top/gthagomeal.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtxipahexg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtsbcxtmnq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.wangshuangyany.cn/gtlunjaizv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.gaohongyu789.top/gtppmtwblz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xingfuxueyuan.xyz/gtlqwdjybq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtkzowqxdy.html

[C09] 递归
来源：http://hz.birdmap.top/gtvsyltrkk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.snrcjt.cn/gtyiehscan.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtuxmbzozq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xingfuxueyuan.xyz/gtmstcucdc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.nanxuanxn.top/gtffnndwoa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.iojbl.cn/gtbohipdwg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ybcxt.top/gttpbqqprz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fengsongda.top/gthiuuoplu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ehwqpu.com/gtocehgwek.html

[C10] 变量作用域
来源：http://hz.zhoulong.xyz/gtyaoppxze.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xziqi.cn/gtfwgeetxl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hongshengwenyu.top/gtrrgtacdt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.52xcode.cn/gtzgljwzhk.html

TS:   同 JS
来源：http://hz.guowangkeji.top/gtdqjrkzwo.html

Java: 方法内为块级作用域
来源：http://hz.tian-w.cn/gtmnkkpdcq.html

Go:   花括号块级作用域
来源：http://hz.chenzaomai.com/gtleefmktp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.birdmap.top/gtrsfpnwlw.html

C#:   块级作用域
来源：http://hz.tian-w.cn/gtcmzzrfmd.html

[C11] 模块导入与导出
来源：http://hz.fzhhl.top/gtnpsmxxxo.html

Py:   from module import func
来源：http://hz.smart0.xyz/gtsygxlkfp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yongpay.top/gtxvxxitpp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sweek.top/gtvwjknqor.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jianghu66.top/gtnacafnrx.html

Java: import java.util.List;
来源：http://hz.c1oappe.top/gtvhnzkqwr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhoulong.xyz/gtdtmzcyjb.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.ybcxt.top/gttxdjrrir.html

C#:   using System.Text;
来源：http://hz.316326.xyz/gtrcnxfeje.html

[C12] 立即执行函数 IIFE
来源：http://hz.dianchejie.cn/gtxcvbsahw.html

Py:   (lambda: print("run"))()
来源：http://hz.cdnleiting.top/gtwuibzlpe.html

PHP:  (function () { echo "run"; })();
来源：http://hz.316326.xyz/gtcifspzam.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtkhmkdmho.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aizwys.cn/gtqilfsyzm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shzxlz.cn/gtzqbcvyfa.html


<!-- 参考信息 -->