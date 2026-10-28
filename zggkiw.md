代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.52xcode.cn/gtmzdpnegc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jyoumei.cn/gtxsxpdadu.html

[A24] 去除首尾空白
来源：http://hz.pycfn.com/gtveigajmt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shzxlz.cn/gtbmbxgtvw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.svipenyu.cn/gtctpqaths.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yuanzhike.top/gteayncebd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuanzx.com/gtxeepytxw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jiagoushi.top/gtcdmsgwbp.html

Go:   strings.TrimSpace(s)
来源：http://hz.dashuyun.cn/gtrwqrblsj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cqqwz.cn/gthbbtanjb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.redwolf501.top/gtttqqfhsk.html

[A25] 字符串比较
来源：http://hz.hysaishi.cn/gtnafdngtb.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhongyouzk.top/gtdvoubnje.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.meibo888.top/gtaabxenwb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.havefunace.top/gtsbbnavsx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.316326.xyz/gtgjstller.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.smart0.xyz/gtnyemnivb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hongshengwenyu.top/gteglfurhw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.tanke756.top/gtrtdlmwyj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.bjfxy.top/gtaofiegie.html

[A26] 类型转换总览
来源：http://hz.jyoumei.cn/gtxxokprkq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.9152youxi.cn/gtjpgyqejj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.nwbrower.top/gtkvlxkofs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zdqjudy.top/gtnllcupcx.html

TS:   Number() String() Boolean() x as number
来源：http://hz.vqdsnc.cn/gtgiurkhuy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jinghuilouyu.cn/gtioodftqi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.mhx1999.top/gtauirrwdd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ybcxt.top/gtfhckhouj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.0kj1m.cn/gtqczztxzb.html

================================================================================
来源：http://hz.guannengcc.top/gtligpkcwf.html

B. 流程控制
来源：http://hz.cucudq.cn/gtsrcmtvfb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtyftmegqr.html

[B01] 条件判断 if / else
来源：http://hz.jiagoushi.top/gtmtafrxam.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.xziqi.cn/gtwaohrrjq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.c1oappe.top/gtmirgzpsh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtieuhbucw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtuzqrwwhw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sufxvd.cn/gtlpmblmlq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.havefunace.top/gttxcexnxa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.tian-w.cn/gtupgdvbsh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.daria6918.cn/gtgktyggvb.html

[B02] 多分支 else if / elif
来源：http://hz.cdnleiting.top/gtjegzwddr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yanxiufei.cn/gtgfwaeeer.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.0kj1m.cn/gtorkbhngp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shuidangran.top/gtxvhsmrjk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.quarkkingdee.top/gtumayamaz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sufxvd.cn/gtahwbbrat.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.dashuyun.cn/gtzpjyuggj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hysaishi.cn/gthrceztnb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.mhx1999.top/gtqxvxhufa.html

[B03] switch / match / case
来源：http://hz.mhx1999.top/gtvmfvfhqc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.c1oappe.top/gtnzhkgscm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xuetiantiany.cn/gtkffvhunr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258.top/gtsedjdetb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jyoumei.cn/gtdqclhcql.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cashguo.top/gtocajiaee.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.shuidangran.top/gtokmovbpk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnqzz.top/gtwtkxbmhk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ywan-chungtsiang.top/gtkxlrqkty.html

[B04] for 计数循环
来源：http://hz.ydjk.org.cn/gtnxeldbfz.html

Py:   for i in range(10): print(i)
来源：http://hz.zdqjudy.top/gtvfrhwrvb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yanxiufei.cn/gthqvllkcb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shuidangran.top/gthhzmcedr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuanzhike.top/gtxlafmnhd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.52xcode.cn/gtkzqzxdai.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cucudq.cn/gtinbaasuw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.fengsongda.top/gtokhmffox.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jlsjyb.cn/gthrdphena.html

[B05] 遍历数组 / 列表
来源：http://hz.dashuyun.cn/gtmlngzfsl.html

Py:   for item in arr: print(item)
来源：http://hz.shanyushiyangkeji.top/gteobrkieu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jyoumei.cn/gtyntffixw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.redwolf501.top/gttjcvxpkg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yangfankeji.com/gtwwltmbaa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hywenlv.cn/gtadodpkqt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zhongyouzk.top/gtcwuvtvnp.html

Ruby: arr.each { |item| puts item }
来源：http://hz.316326.xyz/gtnvzqdnam.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zdqjudy.top/gtpvnbqxkj.html

[B06] 遍历字典 / 对象
来源：http://hz.xingfuxueyuan.xyz/gtsdqyzyqk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jqgufenzy.top/gtnfexhidg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.pycfn.com/gtcxjawffb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj202588.top/gtowspxthn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj202588.top/gtwysfxogc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.daxiang520.top/gtimgeveuk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jianghu66.top/gtinvbvlbf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhijiandao.cn/gtigwlprhx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.pycfn.com/gtwjdlywmc.html

[B07] while 循环
来源：http://hz.ydjk.org.cn/gtmljvotqa.html

Py:   while i < 10: i += 1
来源：http://hz.bjfxy.top/gtvnqvbvzy.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yangfankeji.com/gtbgrdexyn.html

JS:   while (i < 10) { i++; }
来源：http://hz.guowangkeji.top/gtzousauxk.html

TS:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtvzimozeq.html

Java: while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtbhadfasi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj202588.top/gtcspdzhqj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.chenlongwang.top/gtngpekwxz.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtkjzblmle.html

[B08] do-while（至少执行一次）
来源：http://hz.smart0.xyz/gtzprbtszw.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ydjk.org.cn/gtfjzxnbxn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.quarkkingdee.top/gtylxlhrvo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gtnoquvsjd.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtjvyyphqt.html

Java: do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtnfzffsyp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sufxvd.cn/gtpfkxmgvm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xylfe.cn/gtmfyzyvzl.html

C#:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gttckoxons.html

[B09] break 与 continue
来源：http://hz.yonumen.top/gttgdhfnqj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.daria6918.cn/gtmhdoicfm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.iojbl.cn/gtzqvdgnnv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtzrgqjeoy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nwbrower.top/gtfhsgzmfc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gttcbydshd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigufen.top/gtrbzhqpvj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.daxiang520.top/gtujxopwka.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gtjufwmagd.html

[B10] 遍历同时拿索引
来源：http://hz.daria6918.cn/gtwvqufhkj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sufxvd.cn/gterzukzbq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hywenlv.cn/gtmojcljde.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.wangdashe.top/gtvyyegord.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtwadbirjf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.gogol.net.cn/gtzcziodcs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.iojbl.cn/gtnicgzncr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tian-w.cn/gtwilbeuht.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.fzhhl.top/gtvnuzmbbc.html

[B11] 生成数字序列 / 区间
来源：http://hz.jiagoushi.top/gtiduhhqck.html

Py:   list(range(0, 10, 2))
来源：http://hz.shanyushiyangtech.top/gtghgmlump.html

PHP:  range(0, 10, 2);
来源：http://hz.guowangkeji.top/gtrfvyqsls.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xziqi.cn/gtmgvcagdc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtivxfunip.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.nanxinkj.top/gtfjbuojxw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.haohaochexian.top/gtbsbgciue.html

Ruby: (0...10).step(2).to_a
来源：http://hz.cucudq.cn/gtqnsrleeh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yuxming.cn/gtzopsocrw.html

[B12] 跳出多层循环
来源：http://hz.xinyue.icu/gticbjrahy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.fengsongda.top/gtoybhyuaj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.ppjwa.cn/gtswhfwiia.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pycfn.com/gtqgdtslss.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gthcjpdkol.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.svipenyu.cn/gtxawbgqgv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.gaohongyu789.top/gtpjgbgqry.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fengsongda.top/gtbdnfsbmq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinqigufen.top/gtkhmzjihn.html

[B13] 判断是否为数字
来源：http://hz.dianchejie.cn/gtessubclb.html

Py:   isinstance(x, (int, float))
来源：http://hz.mhx1999.top/gtvcyiujrv.html

PHP:  is_numeric($x)
来源：http://hz.yueranfly.top/gtjuzsgrxu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gtwxxxfehl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxuanxn.top/gtxqmldtmv.html

Java: x instanceof Number
来源：http://hz.daxiang520.top/gtgczdbhyl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cashguo.top/gtwhuygclq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhaomingkeji.xyz/gtcfgdtdpw.html

C#:   x is int or double or decimal
来源：http://hz.birdmap.top/gtiunehdwi.html

[B14] 判断值是否在集合内
来源：http://hz.smart0.xyz/gtzctftadb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.aizwys.cn/gthmbchwev.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.aibaodan.cn/gtmewqknxz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.wangshuangyany.cn/gtblvsslnp.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtlhsazqry.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ehwqpu.com/gtnljjxzby.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.nanxuanxn.top/gtdtazfiuu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhaomingkeji.xyz/gtvwmnmfse.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.316326.xyz/gttfarmowt.html

[B15] 布尔运算与取反
来源：http://hz.zhijiandao.cn/gtdclgbrmu.html

Py:   a and b or not c
来源：http://hz.ydjk.org.cn/gtscbjftpj.html

PHP:  $a && $b || !$c
来源：http://hz.yuanzhike.top/gthbndfubz.html

JS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtrthmwqmc.html

TS:   a && b || !c
来源：http://hz.hfpthk.cn/gtcdzijare.html

Java: a && b || !c
来源：http://hz.guannengcc.top/gtavifuouq.html

Go:   a && b || !c
来源：http://hz.ivvv.top/gtyqfpjbrn.html

Ruby: a && b || !c
来源：http://hz.iojbl.cn/gtavwyrczb.html

C#:   a && b || !c
来源：http://hz.cashguo.top/gtvnyvmbbl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sufxvd.cn/gtvgwyuhna.html

Py:   if not data: return
来源：http://hz.kuanghao11.cn/gtqitxtyky.html

PHP:  if (!$data) { return; }
来源：http://hz.haohaochexian.top/gtksnunqkh.html

JS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtvmpinahg.html

TS:   if (!data) return;
来源：http://hz.zhijiandao.cn/gtjnbdvaou.html

Java: if (data == null) return;
来源：http://hz.shangyingyoupin.top/gtdpgsdeks.html

Go:   if data == nil { return }
来源：http://hz.hfpthk.cn/gtfupdrtgy.html

Ruby: return if data.nil?
来源：http://hz.quarkkingdee.top/gtioyywvxq.html

C#:   if (data == null) return;
来源：http://hz.pengpengdd.cyou/gtzlzfcpyj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtavplxtep.html

C. 函数与作用域
来源：http://hz.shzxlz.cn/gtneponrhu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgrvqeckb.html

[C01] 定义函数
来源：http://hz.jinyuanbaomall.cn/gtlvngmtnp.html

Py:   def add(a, b): return a + b
来源：http://hz.ehwqpu.com/gtrihfuuvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hammf.cn/gtextblnzm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtwasmlsur.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtaahvdriv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtubxkpbfd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tanke756.top/gtbeyvvbwz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yonumen.top/gtkxvfpath.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtiupzxunm.html

[C02] 默认参数
来源：http://hz.xingfuxueyuan.xyz/gtahcbmzou.html

Py:   def greet(name="World"): return name
来源：http://hz.guowangkeji.top/gtqgkccovv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.bjfxy.top/gtqpektfzo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.havefunace.top/gtufsunpzh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yongpay.top/gtvxvnyknl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jiagoushi.top/gtbxkgkrae.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.xuetiantiany.cn/gtwbzmzfdh.html

Ruby: def greet(name = "World") = name
来源：http://hz.jyoumei.cn/gtqnzqgrlf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.c1oappe.top/gtkkpaixos.html

[C03] 可变参数
来源：http://hz.gogol.net.cn/gtymxgxwbc.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydzc1.top/gtvdvzanbv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.vqdsnc.cn/gtrfocikvz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sysykeji.top/gtmctmjbdf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yongpay.top/gtbngrnnrv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj202588.top/gtquplcgfs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgfzy.top/gtopngorse.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jianghu66.top/gthgcevjzt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dianchejie.cn/gtfftpvywt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgfzy.top/gtcnyzvifb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daria6918.cn/gtfrfvpoyn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuanzhike.top/gtqsgwzyje.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtedrfljgh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nanxinkj.top/gtjlwvptda.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.feifeiyinyue.top/gttyvooubx.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gtazskyklx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.mhx1999.top/gttoladdmp.html

C#:   f(a: 1, b: 2)
来源：http://hz.kuanghao11.cn/gtekbfccmu.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtpsilrvqk.html

Py:   return a, b
来源：http://hz.pengpengdd.cyou/gtwrgenlun.html

PHP:  return [$a, $b];
来源：http://hz.feifeiyinyue.top/gtphksbzld.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtkhhqkgpc.html

TS:   return { a, b };
来源：http://hz.cucudq.cn/gtmtatarrp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ehwqpu.com/gtwonrcabz.html

Go:   return a, b
来源：http://hz.cdnleiting.top/gtcfzsnklp.html

Ruby: return a, b
来源：http://hz.sxryk.cn/gtrirwtdpb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ivvv.top/gtdvzmnryh.html

[C06] 匿名函数 / lambda
来源：http://hz.mhx1999.top/gtyhtwglrh.html

Py:   square = lambda x: x * x
来源：http://hz.hongshengwenyu.top/gtrwiwgynh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.fengsongda.top/gtglqjgdow.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gtzajbqock.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.birdmap.top/gtsikyaefg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.daxiang520.top/gteqfrrjdc.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhongyouzk.top/gtuomdbtvg.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtdnxgbhrr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gaohongyu789.top/gtdkncacsx.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gtvgnqusyp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yuanzhike.top/gtlwfewsmr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jianghu66.top/gtfmzmlnbk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sxryk.cn/gtgcpgcndj.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gttobfkrjs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yanxiufei.cn/gtwmghidgu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xingfuxueyuan.xyz/gtlwufpzdz.html

Ruby: arr.map(&:upcase)
来源：http://hz.pycfn.com/gtchcfpubb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.smart0.xyz/gtwzgbqxxj.html

[C08] 闭包
来源：http://hz.ppjwa.cn/gthaldchep.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhengqikj.top/gteqfivbde.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.ydzc1.top/gtdstexesv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtojyibhge.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydjk.org.cn/gtzvaoldxv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinyuanbaomall.cn/gtrbocuzef.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.mhx1999.top/gtjsrcicpz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.svipenyu.cn/gtpbquzqhp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtsypqfbie.html

[C09] 递归
来源：http://hz.guowangkeji.top/gtcfayckhq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hnqzz.top/gtowujqywu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.jlsjyb.cn/gtyqpszlhv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pengpengdd.cyou/gtdohmvmhx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydjk.org.cn/gtuxbfiwju.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhengqikj.top/gtiwgozqca.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.dashuyun.cn/gtttjyvqyj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.iojbl.cn/gttsxdosbe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hammf.cn/gtqkqdvtfm.html

[C10] 变量作用域
来源：http://hz.smart0.xyz/gtvnpmmdbs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yuanzhike.top/gtsemnjswf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.aibaodan.cn/gtbtuvdtid.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenzaomai.com/gtekilamui.html

TS:   同 JS
来源：http://hz.feifeiyinyue.top/gtfdsrfycq.html

Java: 方法内为块级作用域
来源：http://hz.hysaishi.cn/gtlbktettb.html

Go:   花括号块级作用域
来源：http://hz.xziqi.cn/gtwbbrhtsq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gthxfaiunu.html

C#:   块级作用域
来源：http://hz.guannengcc.top/gtfbvmzlbw.html

[C11] 模块导入与导出
来源：http://hz.sysykeji.top/gtffoljgrd.html

Py:   from module import func
来源：http://hz.xinyue.icu/gtpecrwcdb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhiwuduotai.top/gtvhbmxwen.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.nanxuanxn.top/gtqghvosoy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yangfankeji.com/gtkljuflho.html

Java: import java.util.List;
来源：http://hz.dianchejie.cn/gtvqyvthpw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydjk.org.cn/gtncqmwjeq.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj202588.top/gtipdmtuuq.html

C#:   using System.Text;
来源：http://hz.hammf.cn/gthumxcioc.html

[C12] 立即执行函数 IIFE
来源：http://hz.smart0.xyz/gtqcuihpfd.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangkeji.top/gtouqfldiu.html

PHP:  (function () { echo "run"; })();
来源：http://hz.smart0.xyz/gtqlrsqkbs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gtkbxvlhth.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gteuppbntq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.birdmap.top/gtgpvnuxky.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.meibo888.top/gtzdoftjmk.html

Ruby: -> { puts "run" }.call
来源：http://hz.mhx1999.top/gtofcluboj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtcnsjleml.html

[C13] 类型声明 / 类型注解
来源：http://hz.yangfankeji.com/gttocewner.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.quarkkingdee.top/gtvmvnpquq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtdipuhdzr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cucudq.cn/gtuownkyft.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtbzxpcoiz.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gttsuibjxy.html

Go:   func add(a, b int) int
来源：http://hz.dianchejie.cn/gtkgytyxma.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.daria6918.cn/gttckmiimd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtyrasmhne.html

[C14] 泛型函数
来源：http://hz.dashuyun.cn/gttjysdyxh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ppjwa.cn/gttdguckuf.html

PHP:  // 无泛型
来源：http://hz.daxiang520.top/gtrqltmset.html

JS:   // 无泛型
来源：http://hz.tian-w.cn/gthkydzgnt.html


<!-- 参考信息 -->