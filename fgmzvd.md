代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.hysaishi.cn/gtbrqjinjm.html

Ruby: gets.chomp
来源：http://hz.zdqjudy.top/gtxteowepi.html

C#:   Console.ReadLine();
来源：http://hz.yongpay.top/gtxahjscqt.html

[A21] 保留指定小数位输出
来源：http://hz.kuanghao11.cn/gtlbhiigwc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.tanke756.top/gtvjvswtte.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.chenzaomai.com/gtjmduciju.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sweek.top/gtbqrqdggd.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shuidangran.top/gtvnlgvxpp.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtpaljxtgl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.zhijiandao.cn/gtnpywjukk.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.guowangkeji.top/gtefvhckss.html

C#:   3.14159.ToString("F2")
来源：http://hz.ywan-chungtsiang.top/gtwiyemtek.html

[A22] 获取字符串长度
来源：http://hz.feifeiyinyue.top/gtyqxttnat.html

Py:   len(s)
来源：http://hz.havefunace.top/gtckqpuxkj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.wangdashe.top/gtkxnikglo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.tianlin.xyz/gtpbchscsw.html

TS:   s.length
来源：http://hz.kuanghao11.cn/gtyxrrmvpy.html

Java: s.length()
来源：http://hz.52xcode.cn/gtgdddwvrd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.sweek.top/gtdqzxfmmz.html

Ruby: s.length
来源：http://hz.zhijiandao.cn/gtmeuncwkl.html

C#:   s.Length
来源：http://hz.mhx1999.top/gtlnjgqlvw.html

[A23] 大小写转换
来源：http://hz.chenzaomai.com/gtspgkfjbi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ydjk.org.cn/gtpmbkntiv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhongyouzk.top/gtrxhbyxhw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.guannengcc.top/gtgzmhgvoa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gotoacloud.top/gtglmcyjdz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yueranfly.top/gtromqcceh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yonumen.top/gtysifbehf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.gzhubu.top/gtgodjrqbi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yuanzhike.top/gtfewoaeib.html

[A24] 去除首尾空白
来源：http://hz.gotoacloud.top/gtmjxenkyh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jiagoushi.top/gtinmuosgv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.fengsongda.top/gtnntckxra.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shangyingyoupin.top/gtrjslprff.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.redwolf501.top/gtdzlijcek.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.redwolf501.top/gtgasofrld.html

Go:   strings.TrimSpace(s)
来源：http://hz.ybcxt.top/gtbbdxjghy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cdnleiting.top/gtoyuasihc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.tian-w.cn/gtjnnnzrhf.html

[A25] 字符串比较
来源：http://hz.yuanzhike.top/gtvqhvytsr.html

Py:   s1 == s2; s1 != s2
来源：http://hz.gotoacloud.top/gtoerbfovr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yonumen.top/gtuhwkyecf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.tianlin.xyz/gtonbkznur.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cucudq.cn/gtzojryiul.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xinyue.icu/gtpuljynvx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sxryk.cn/gtmamghwhk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.fengsongda.top/gtpioadjyk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yanxiufei.cn/gtoadkundp.html

[A26] 类型转换总览
来源：http://hz.andypj.xyz/gtlmfoehmr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.dashuyun.cn/gtnreuokbk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.guannengcc.top/gtmkcxsrrq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.redwolf501.top/gtljhmdtxp.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cheryme.top/gtsfxasjrc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.dashuyun.cn/gtvebpzdbo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.dashuyun.cn/gtffipnero.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.52xcode.cn/gtqhwxxwbt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ybcxt.top/gtieyonseh.html

================================================================================
来源：http://hz.sweek.top/gtjmpmiubz.html

B. 流程控制
来源：http://hz.xylfe.cn/gtzgmilvbz.html

================================================================================
来源：http://hz.jianghu66.top/gtsacgkwsv.html

[B01] 条件判断 if / else
来源：http://hz.dianchejie.cn/gtxkvgaabm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.havefunace.top/gtdextvklm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hysaishi.cn/gttdpmwapr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtamvuneyv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zycfv.cn/gtrdtvepph.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xingfuxueyuan.xyz/gtzqhxsipb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ehwqpu.com/gtpekxeclz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jinghuilouyu.cn/gtpopefbmd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.redwolf501.top/gtwenzgiwh.html

[B02] 多分支 else if / elif
来源：http://hz.shuidangran.top/gtnwaikjlx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.wangshuangyany.cn/gtbkukrgbj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.svipenyu.cn/gtcjujjgsh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtmglipbgl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtedrjkifc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gtsqbgnjom.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ybcxt.top/gtgxrlayos.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yuxming.cn/gtbwpnarwm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cqqwz.cn/gtehmcicbs.html

[B03] switch / match / case
来源：http://hz.ehwqpu.com/gtvxswwpop.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.gogol.net.cn/gtilhoolaq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yonumen.top/gtpsxssnoi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daxiang520.top/gtfvcqessg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shuidangran.top/gtnlpekaet.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jinqigufen.top/gtehymfgeq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yonumen.top/gtbcnzrxgf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhoulong.xyz/gtgarzsoml.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ivvv.top/gtbmcjwrlf.html

[B04] for 计数循环
来源：http://hz.guannengcc.top/gtwerkidhu.html

Py:   for i in range(10): print(i)
来源：http://hz.c1oappe.top/gtnxvdznxw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.fengsongda.top/gtgvpydsyk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yvedp.cn/gtjqxgofuf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hnxiangtu.top/gtdsjbeihy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.guannengcc.top/gtmphtctvj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhaomingkeji.xyz/gtrrhrfvnc.html

Ruby: 10.times { |i| puts i }
来源：http://hz.gotoacloud.top/gtbqqsongj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.9152youxi.cn/gtybfogvob.html

[B05] 遍历数组 / 列表
来源：http://hz.jinghuilouyu.cn/gtqpqrcris.html

Py:   for item in arr: print(item)
来源：http://hz.tanke756.top/gtyezzdpvq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jinqigfzy.top/gtrikgyiex.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.nanxuanxn.top/gtxggapzmz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.pycfn.com/gtvwhtcmyl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zdqjudy.top/gtylilvbsc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.birdmap.top/gtqpovpsfx.html

Ruby: arr.each { |item| puts item }
来源：http://hz.aibaodan.cn/gtmhzzsfka.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.pycfn.com/gtmhmtxjwp.html

[B06] 遍历字典 / 对象
来源：http://hz.nwbrower.top/gtfnhamwwg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ehwqpu.com/gtdtcjlhsb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jlsjyb.cn/gtcnerxwot.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.kuanghao11.cn/gtvjwjeiwm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yuxming.cn/gtumibnmmx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gotoacloud.top/gtyddawoax.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.pycfn.com/gtnpjecbnh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.aizwys.cn/gtmwaxztzb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sufxvd.cn/gteaoytffv.html

[B07] while 循环
来源：http://hz.aizwys.cn/gtkbvhtlcy.html

Py:   while i < 10: i += 1
来源：http://hz.cheryme.top/gtpfbvlzwt.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yanxiufei.cn/gtjrrjxrkw.html

JS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangkeji.top/gtxelxufip.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtgmpnmnan.html

Java: while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtgrcyhodo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.sysykeji.top/gtthziaszb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhongyouzk.top/gteszqlhsa.html

C#:   while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtlnhlkvbu.html

[B08] do-while（至少执行一次）
来源：http://hz.zhixingplan.top/gthjrhmzhl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jyoumei.cn/gtcfodsnkw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.meibo888.top/gtdficznai.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gaohongyu789.top/gtdtxjqzwz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtnarryduv.html

Java: do { i++; } while (i < 10);
来源：http://hz.xinyue.icu/gtpbwninzi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zdqjudy.top/gtgpixjxhh.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.jinqigfzy.top/gtyldesvpt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtcpijpvoi.html

[B09] break 与 continue
来源：http://hz.ehwqpu.com/gtgjbxirju.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hnqzz.top/gtxefxdglo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.nanxuanxn.top/gtmbopddgr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dianchejie.cn/gtvorypira.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtaltpyjzt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtfmxspqae.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgufenzy.top/gtvulbryei.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gtimdcekcs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtizqifbyl.html

[B10] 遍历同时拿索引
来源：http://hz.jqgufenzy.top/gtaefzbygt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.birdmap.top/gtngtghdda.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhengqikj.top/gtfepqdlyb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yonumen.top/gtbwuzlomd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hysaishi.cn/gtdxeiorai.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cashguo.top/gtygtrwzbt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hnqzz.top/gtqdfwosro.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.bjfxy.top/gtoamyoloi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sufxvd.cn/gtmxenqdcr.html

[B11] 生成数字序列 / 区间
来源：http://hz.tianlin.xyz/gtejczvwed.html

Py:   list(range(0, 10, 2))
来源：http://hz.tian-w.cn/gtstbbfdez.html

PHP:  range(0, 10, 2);
来源：http://hz.nwbrower.top/gtseraeqaf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtqptoidic.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigfzy.top/gtqqtghqng.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hywenlv.cn/gtdjfztznj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gaohongyu789.top/gtqwnkoalr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sweek.top/gtrfedawxt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.0kj1m.cn/gtnkiibejs.html

[B12] 跳出多层循环
来源：http://hz.smart0.xyz/gtikhbzahr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xingfuxueyuan.xyz/gtnramshls.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtiojsiyzg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtmwdbsvdp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gttmrwrykw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtbyrzrvjq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cdnleiting.top/gttcjomloa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinyuanbaomall.cn/gtukkspzqg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ppjwa.cn/gtyrpmzogv.html

[B13] 判断是否为数字
来源：http://hz.hongshengwenyu.top/gtkyopjtvc.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhengqikj.top/gtmncrfqud.html

PHP:  is_numeric($x)
来源：http://hz.hnxiangtu.top/gtwomrtquz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sxryk.cn/gtwndpptzu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.mhx1999.top/gtcowelkzu.html

Java: x instanceof Number
来源：http://hz.birdmap.top/gtjgcubtzu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hnxiangtu.top/gtwhasdyqt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj20258.top/gtbulylcnq.html

C#:   x is int or double or decimal
来源：http://hz.jlsjyb.cn/gtjgmowxpn.html

[B14] 判断值是否在集合内
来源：http://hz.zhiwuduotai.top/gtcbepmaun.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnqzz.top/gtovptooub.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.fengsongda.top/gtlhhvnogi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jlsjyb.cn/gtckjohitg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jiagoushi.top/gtvavlpbfh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxuanxn.top/gtbadawzva.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shzxlz.cn/gtfwqbjcho.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hywenlv.cn/gtztnoiowq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.smart0.xyz/gtuxmmyacb.html

[B15] 布尔运算与取反
来源：http://hz.yvedp.cn/gtkjtgiegf.html

Py:   a and b or not c
来源：http://hz.quarkkingdee.top/gteidvkssh.html

PHP:  $a && $b || !$c
来源：http://hz.hnxiangtu.top/gtngpajqhk.html

JS:   a && b || !c
来源：http://hz.cheryme.top/gtfhcibepf.html

TS:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtcqgllkdd.html

Java: a && b || !c
来源：http://hz.dashuyun.cn/gtjhvxkxyn.html

Go:   a && b || !c
来源：http://hz.shzxlz.cn/gtaevrfzjn.html

Ruby: a && b || !c
来源：http://hz.sweek.top/gtcarueahg.html

C#:   a && b || !c
来源：http://hz.yj20258.top/gtcfvqshdk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gaohongyu789.top/gtcrovexao.html

Py:   if not data: return
来源：http://hz.guannengcc.top/gtgwapdkab.html

PHP:  if (!$data) { return; }
来源：http://hz.haohaochexian.top/gtkpznxutr.html

JS:   if (!data) return;
来源：http://hz.guannengcc.top/gtkicpyuws.html

TS:   if (!data) return;
来源：http://hz.zhiwuduotai.top/gtxiszxtoe.html

Java: if (data == null) return;
来源：http://hz.ppjwa.cn/gtccakilif.html

Go:   if data == nil { return }
来源：http://hz.gzhubu.top/gtjasytskj.html

Ruby: return if data.nil?
来源：http://hz.hnxiangtu.top/gtmhjxgawc.html

C#:   if (data == null) return;
来源：http://hz.bjfxy.top/gtltpapzzp.html

================================================================================
来源：http://hz.gogol.net.cn/gtpbmoixmf.html

C. 函数与作用域
来源：http://hz.yj20258.top/gtqbwdbsll.html

================================================================================
来源：http://hz.wangdashe.top/gtpoddtczz.html

[C01] 定义函数
来源：http://hz.zdqjudy.top/gtssydxzst.html

Py:   def add(a, b): return a + b
来源：http://hz.bjfxy.top/gtampceijw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinyuanbaomall.cn/gtxgkynmdf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtsvtbiogv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.iojbl.cn/gtmfhqeycu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtotehzfrk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ydzc1.top/gtkywumgih.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nanxinkj.top/gtigrfrmco.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gthnembxvg.html

[C02] 默认参数
来源：http://hz.yvedp.cn/gtpduzztbb.html

Py:   def greet(name="World"): return name
来源：http://hz.zhoulong.xyz/gttmpwfnej.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtahggfaiz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dashuyun.cn/gthxplqfuo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jyoumei.cn/gtkrhewwwq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jianghu66.top/gttszelmsc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sufxvd.cn/gtrecjpftf.html

Ruby: def greet(name = "World") = name
来源：http://hz.gzhubu.top/gtyhlauylm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shanyushiyangtech.top/gtvsrstvzr.html

[C03] 可变参数
来源：http://hz.yueranfly.top/gttwjyihrb.html

Py:   def total(*args): return sum(args)
来源：http://hz.pycfn.com/gthpykpzpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ehwqpu.com/gtbzxysvqi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xuanzx.com/gtwhvntjzw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gtbwlqowla.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ehwqpu.com/gtuoygukmj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigfzy.top/gtpbnupwel.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.guowangkeji.top/gtjkyuvixa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tanke756.top/gtrbqgexvx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zdqjudy.top/gtczglqpms.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xziqi.cn/gtlpfnzzen.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xuetiantiany.cn/gtuhzhkpcz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sweek.top/gtupmetetu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.feifeiyinyue.top/gtxxyoevje.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yvedp.cn/gtxvwktcdx.html

Go:   // 无：用配置结构体参数
来源：http://hz.aibaodan.cn/gtwpsefolz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nanxuanxn.top/gtkwrguxzw.html

C#:   f(a: 1, b: 2)
来源：http://hz.svipenyu.cn/gtpfveqtia.html

[C05] 返回多个值
来源：http://hz.zhiwuduotai.top/gtxksuivvt.html

Py:   return a, b
来源：http://hz.yj202588.top/gtaimvknnb.html

PHP:  return [$a, $b];
来源：http://hz.hongshengwenyu.top/gtrauczvgt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gttuzopwlt.html

TS:   return { a, b };
来源：http://hz.yonumen.top/gtrqoyxvyb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nanxuanxn.top/gtxkghpdyh.html

Go:   return a, b
来源：http://hz.yj202588.top/gtyehawprv.html

Ruby: return a, b
来源：http://hz.316326.xyz/gtpuaxfzbw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gtantiejal.html

[C06] 匿名函数 / lambda
来源：http://hz.yuxming.cn/gtnsnndssk.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtuskhvpkq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhiwuduotai.top/gttisoqhyp.html

JS:   const square = x => x * x;
来源：http://hz.iojbl.cn/gtfcoiloqy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gturpstkax.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangdashe.top/gtulmfnrim.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.chenlongwang.top/gtselwirxc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ppjwa.cn/gtvuwgykbx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinyuanbaomall.cn/gtpmsaxwqx.html

[C07] 把函数作为参数传入
来源：http://hz.redwolf501.top/gtamvchnye.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yueranfly.top/gtebqtvcoi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zycfv.cn/gtczskbnzu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.bjfxy.top/gtgwejoejo.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtrxwoiwgh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhoulong.xyz/gtzuhhebgu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinqigufen.top/gtupwhvllc.html

Ruby: arr.map(&:upcase)
来源：http://hz.daria6918.cn/gtoynehsqn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhoulong.xyz/gtfhmhcizg.html

[C08] 闭包
来源：http://hz.jinghuilouyu.cn/gtnspuljnb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.andypj.xyz/gtqgrflecq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yangfankeji.com/gtihbbmncy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtoznkqfww.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhaomingkeji.xyz/gtwubepuii.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.andypj.xyz/gtnqrzxcuh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuxming.cn/gtckvvzynr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hongshengwenyu.top/gtoqrabgec.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shangyingyoupin.top/gtglocvopz.html

[C09] 递归
来源：http://hz.hfpthk.cn/gtvixveaba.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.iojbl.cn/gtbbovekfs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhengqikj.top/gtubkjmnud.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtzqtunfpw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtqbhfbhnz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gogol.net.cn/gtyrwtydsd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.pengpengdd.cyou/gtoapxelth.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtgekznjsb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenzaomai.com/gtmdcjxzdy.html

[C10] 变量作用域
来源：http://hz.hywenlv.cn/gtnxsracpa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shangyingyoupin.top/gtwsqavafl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.meibo888.top/gtnwkganvm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cdnleiting.top/gtzumbiywk.html

TS:   同 JS
来源：http://hz.hammf.cn/gtoykuvrkp.html

Java: 方法内为块级作用域
来源：http://hz.xuetiantiany.cn/gtiulkgzbv.html

Go:   花括号块级作用域
来源：http://hz.ywan-chungtsiang.top/gtgheradrq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ivvv.top/gtfgwhuzdj.html

C#:   块级作用域
来源：http://hz.hysaishi.cn/gtjqfctpdb.html

[C11] 模块导入与导出
来源：http://hz.meibo888.top/gtsgeyfijv.html

Py:   from module import func
来源：http://hz.chenlongwang.top/gtfggiddth.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hnqzz.top/gtkqneunrw.html


<!-- 参考信息 -->