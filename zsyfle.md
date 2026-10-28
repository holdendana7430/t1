代发 wailian999

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hfpthk.cn/gtbdsvierf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tian-w.cn/gtyunkbelu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuanzx.com/gtplpxqydt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.shzxlz.cn/gtznjmggge.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yueranfly.top/gtyvsbujeo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.nanxinkj.top/gtwehhcebg.html

[A24] 去除首尾空白
来源：http://hz.xylfe.cn/gtebrgprqc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yj20258888.top/gtzhajtlbx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.smart0.xyz/gtkqolrzwm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shanyushiyangtech.top/gtmmmahvan.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yonumen.top/gtfmoujoxs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.0kj1m.cn/gtrabqqeql.html

Go:   strings.TrimSpace(s)
来源：http://hz.xuetiantiany.cn/gtugeecxln.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xuetiantiany.cn/gtyicmafct.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.nwbrower.top/gtmrpxbwnm.html

[A25] 字符串比较
来源：http://hz.smart0.xyz/gtofpdammr.html

Py:   s1 == s2; s1 != s2
来源：http://hz.9152youxi.cn/gtygogylna.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.daxiang520.top/gtvcubmzlt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhengqikj.top/gtmansalrz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.c1oappe.top/gtuwfoglud.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xinyue.icu/gtvrdsbtlk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.0kj1m.cn/gtnnphtrki.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.tian-w.cn/gttnxoitqn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jlsjyb.cn/gtfsipxpyp.html

[A26] 类型转换总览
来源：http://hz.tianlin.xyz/gtdznbcwkm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.9152youxi.cn/gtonkmzhgy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cashguo.top/gthcwhupbi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.mhx1999.top/gtkhuxwujw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yj202588.top/gtvvrcwzqi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shanyushiyangtech.top/gtpyxnlfst.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.bjfxy.top/gthzvjlprx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jinqigufen.top/gtwtynbmtn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shangyingyoupin.top/gtccijqoli.html

================================================================================
来源：http://hz.jinqigufen.top/gtieqjjxmv.html

B. 流程控制
来源：http://hz.xuetiantiany.cn/gtstfhplda.html

================================================================================
来源：http://hz.hfpthk.cn/gtljgbdpji.html

[B01] 条件判断 if / else
来源：http://hz.nwbrower.top/gthkybfgyi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.xuetiantiany.cn/gthlkmaeyf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hywenlv.cn/gtuozlzdmk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.dianchejie.cn/gtjpoxvqzm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hysaishi.cn/gttgixpgwg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.nwbrower.top/gtgtdvrtdb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yuanzhike.top/gtxfhsjbkk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhengqikj.top/gtksclkuxq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhiwuduotai.top/gtdzmggwel.html

[B02] 多分支 else if / elif
来源：http://hz.ydzc1.top/gtajncqgnk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zycfv.cn/gtipfhhzrs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.aizwys.cn/gtirvudcfd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtohdjpuuw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtesplnuyg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtpssacepz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jqgufenzy.top/gtinmchogt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.nanxinkj.top/gtgbhjybzi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtodauvwbi.html

[B03] switch / match / case
来源：http://hz.gogol.net.cn/gtpotjluko.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cqqwz.cn/gttydmeiqk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yuanzhike.top/gtztncfoka.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ybcxt.top/gtjtougkda.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigufen.top/gtssmwlcxy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj20258.top/gttsndaqgp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ydjk.org.cn/gtmkqyrtdb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.xinyue.icu/gtgbvpxase.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hammf.cn/gtgesftsgd.html

[B04] for 计数循环
来源：http://hz.hnxiangtu.top/gtxhvnlzrc.html

Py:   for i in range(10): print(i)
来源：http://hz.ywan-chungtsiang.top/gtpufxuukc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.52xcode.cn/gtljxrzyeg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hnqzz.top/gtvkumlwyc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuetiantiany.cn/gttbsomghk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.tianlin.xyz/gtsjsojkxp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.meibo888.top/gtgzmllpve.html

Ruby: 10.times { |i| puts i }
来源：http://hz.sxryk.cn/gtgrhcibfz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.9152youxi.cn/gtpcogcygs.html

[B05] 遍历数组 / 列表
来源：http://hz.andypj.xyz/gtlspkyuaq.html

Py:   for item in arr: print(item)
来源：http://hz.hnxiangtu.top/gtrmmdxdxx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.fzhhl.top/gtqpjhsxpl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.quarkkingdee.top/gtgmcwfrnb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.havefunace.top/gtykfymiqy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ywan-chungtsiang.top/gtmvcxsedm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.aibaodan.cn/gtucoudyhq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj20258.top/gttormxzuf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.sxryk.cn/gtiidvmcms.html

[B06] 遍历字典 / 对象
来源：http://hz.havefunace.top/gtqcqbvkjr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.birdmap.top/gtxstqbwny.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.redwolf501.top/gtgmfmydmk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shanyushiyangtech.top/gtfesiqycf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cashguo.top/gtpgfywiji.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.birdmap.top/gtqiimegrw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.52xcode.cn/gtfakdrwcb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.smart0.xyz/gtkyhqjrmh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hywenlv.cn/gtnpjhkrbb.html

[B07] while 循环
来源：http://hz.kuanghao11.cn/gtgunitdvh.html

Py:   while i < 10: i += 1
来源：http://hz.bjfxy.top/gtgboaarrz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xziqi.cn/gtshpgwecs.html

JS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtqmhowgxy.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtwvyudtmb.html

Java: while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtppfmzoqp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhongyouzk.top/gtupawowee.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hysaishi.cn/gtdxcyhnxz.html

C#:   while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtthctmifl.html

[B08] do-while（至少执行一次）
来源：http://hz.52xcode.cn/gtuaqlcxym.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hongshengwenyu.top/gtjzfclwjc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shangyingyoupin.top/gtvrfghiwv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtfxnsjvmz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtmjjseqql.html

Java: do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtqyxbsxmg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhongyouzk.top/gtowtrzpor.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhixingplan.top/gtmgrbuuoc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangkeji.top/gtzjawshch.html

[B09] break 与 continue
来源：http://hz.ehwqpu.com/gthqajixjc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.birdmap.top/gtdeylegff.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.redwolf501.top/gtuzskwnuq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtithpesvj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtohtfrriv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtdxtmpbep.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.wangdashe.top/gtbumghhdv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.nwbrower.top/gtwwjdumid.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gtafyjnght.html

[B10] 遍历同时拿索引
来源：http://hz.hywenlv.cn/gtekxvedmb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dashuyun.cn/gtxkfufsin.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yonumen.top/gtjtahnjdl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.fzhhl.top/gttpqncuwr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ydzc1.top/gtdbxglyzy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhongyouzk.top/gtjueszded.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.chenzaomai.com/gtbgexneyx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hammf.cn/gtqpddfxzy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jyoumei.cn/gtfbsksnpk.html

[B11] 生成数字序列 / 区间
来源：http://hz.yj20258.top/gtnwivbvps.html

Py:   list(range(0, 10, 2))
来源：http://hz.shuidangran.top/gtpymwbrrf.html

PHP:  range(0, 10, 2);
来源：http://hz.guowangkeji.top/gtuoqcjuwi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gthjeqyrrv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gtsyxynhdt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.aibaodan.cn/gtjijppqhj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ehwqpu.com/gtyaqbfffp.html

Ruby: (0...10).step(2).to_a
来源：http://hz.nanxinkj.top/gtfeebrcmw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.kuanghao11.cn/gtkzntpvbn.html

[B12] 跳出多层循环
来源：http://hz.feifeiyinyue.top/gtpynywzcj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yvedp.cn/gtqothnkss.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhengqikj.top/gtzzguxxnw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.iojbl.cn/gtskmiiszu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gthdgfglfo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtsrbekfjl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.tianlin.xyz/gtncwugeyt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yangfankeji.com/gtntfapuai.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yj20258.top/gtrlzadvka.html

[B13] 判断是否为数字
来源：http://hz.jinghuilouyu.cn/gthtvcbkkf.html

Py:   isinstance(x, (int, float))
来源：http://hz.52xcode.cn/gtclykalhg.html

PHP:  is_numeric($x)
来源：http://hz.jqgufenzy.top/gtsalydetn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gtaffaynxd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtpqblpjkv.html

Java: x instanceof Number
来源：http://hz.gotoacloud.top/gtpnymeies.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ybcxt.top/gthrtkjhwd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ydzc1.top/gtzycdfrjc.html

C#:   x is int or double or decimal
来源：http://hz.chenzaomai.com/gtnyqxvjmm.html

[B14] 判断值是否在集合内
来源：http://hz.gogol.net.cn/gtfclcvhrp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.chenlongwang.top/gtutelbjpy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydjk.org.cn/gtfvzdqblb.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhaomingkeji.xyz/gtlipmthed.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.hywenlv.cn/gtqqmqgovs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinqigufen.top/gtpdlfsjxh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cheryme.top/gtvxtlvpar.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuetiantiany.cn/gtgqgnehfo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.quarkkingdee.top/gtjzrztuft.html

[B15] 布尔运算与取反
来源：http://hz.yj20258.top/gttwidmyyi.html

Py:   a and b or not c
来源：http://hz.nanxuanxn.top/gtksgtwlpo.html

PHP:  $a && $b || !$c
来源：http://hz.yvedp.cn/gtabmguton.html

JS:   a && b || !c
来源：http://hz.havefunace.top/gtrintecyn.html

TS:   a && b || !c
来源：http://hz.jqgfzy.top/gtlapexozp.html

Java: a && b || !c
来源：http://hz.yanxiufei.cn/gtlnomgmof.html

Go:   a && b || !c
来源：http://hz.gzhubu.top/gtwjbdrwxg.html

Ruby: a && b || !c
来源：http://hz.shangyingyoupin.top/gtlwppixpd.html

C#:   a && b || !c
来源：http://hz.daria6918.cn/gtnwslocpe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gtzqponevl.html

Py:   if not data: return
来源：http://hz.jqgufenzy.top/gtqhxwbwnf.html

PHP:  if (!$data) { return; }
来源：http://hz.shangyingyoupin.top/gtwojecuuq.html

JS:   if (!data) return;
来源：http://hz.xingfuxueyuan.xyz/gtfnwkuiim.html

TS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtlcpbmuct.html

Java: if (data == null) return;
来源：http://hz.zhongyouzk.top/gtepjlrrue.html

Go:   if data == nil { return }
来源：http://hz.jiagoushi.top/gtiyxxeqls.html

Ruby: return if data.nil?
来源：http://hz.hammf.cn/gtecvknmrc.html

C#:   if (data == null) return;
来源：http://hz.ehwqpu.com/gtgwdkzoqw.html

================================================================================
来源：http://hz.snrcjt.cn/gtixtaerwr.html

C. 函数与作用域
来源：http://hz.sufxvd.cn/gtgnufyngy.html

================================================================================
来源：http://hz.52xcode.cn/gtbwtusfaa.html

[C01] 定义函数
来源：http://hz.yongpay.top/gthmsjszuo.html

Py:   def add(a, b): return a + b
来源：http://hz.ywan-chungtsiang.top/gtlizcwtss.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtkpthhjhp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenzaomai.com/gtnnjmxird.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtkikagrvz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtpeezgjrs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenjidiqi.icu/gtguqxldie.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daxiang520.top/gtxrddqszd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hysaishi.cn/gtphpbxzvt.html

[C02] 默认参数
来源：http://hz.fengsongda.top/gtewxqnumt.html

Py:   def greet(name="World"): return name
来源：http://hz.shzxlz.cn/gtztofoabg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydjk.org.cn/gtmiylfecj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtjowdoyun.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aizwys.cn/gtohiqrqbr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.andypj.xyz/gtihbinqwk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hywenlv.cn/gtkwykphye.html

Ruby: def greet(name = "World") = name
来源：http://hz.ivvv.top/gtuinegvjd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.daria6918.cn/gtfauqwuxe.html

[C03] 可变参数
来源：http://hz.snrcjt.cn/gtbzuxkkbk.html

Py:   def total(*args): return sum(args)
来源：http://hz.xziqi.cn/gtgyqirwvk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.redwolf501.top/gtiqdtvhmp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtjaectlyb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hnxiangtu.top/gtwsrflrvr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cdnleiting.top/gtakgcrffk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.bjfxy.top/gticqndlag.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.feifeiyinyue.top/gtfacjheqw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.c1oappe.top/gtafjtvyej.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtnqugvpxy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cucudq.cn/gtnsmqollb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yuanzhike.top/gtfjjyirta.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.wangdashe.top/gtljivphsh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhengqikj.top/gtjlungarh.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sysykeji.top/gthiykhtzr.html

Go:   // 无：用配置结构体参数
来源：http://hz.fengsongda.top/gtpvanosza.html

Ruby: f(a: 1, b: 2)
来源：http://hz.dianchejie.cn/gtucaegxwj.html

C#:   f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtogwavfqq.html

[C05] 返回多个值
来源：http://hz.shuidangran.top/gtvlyxhdrd.html

Py:   return a, b
来源：http://hz.gaohongyu789.top/gtnggzrbpi.html

PHP:  return [$a, $b];
来源：http://hz.nwbrower.top/gtahvykcxf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.316326.xyz/gtzkirsgmd.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtavmweybq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.birdmap.top/gttednciru.html

Go:   return a, b
来源：http://hz.aibaodan.cn/gtexojysqy.html

Ruby: return a, b
来源：http://hz.tianlin.xyz/gtdtqywgns.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shzxlz.cn/gtlotjthqa.html

[C06] 匿名函数 / lambda
来源：http://hz.guannengcc.top/gtvnbqifca.html

Py:   square = lambda x: x * x
来源：http://hz.gzhubu.top/gthsoidhrc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jqgufenzy.top/gtwcbtnsce.html

JS:   const square = x => x * x;
来源：http://hz.hnxiangtu.top/gtboraxuwd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yueranfly.top/gtctumrexb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.smart0.xyz/gtulrtseax.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shangyingyoupin.top/gtnsdogaup.html

Ruby: square = ->(x) { x * x }
来源：http://hz.316326.xyz/gtfeoyzttl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtmijekpik.html

[C07] 把函数作为参数传入
来源：http://hz.gaohongyu789.top/gteeojylho.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hywenlv.cn/gtnjxgkgug.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangtech.top/gtvbbilldb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.svipenyu.cn/gtkgtqadib.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtikmdnjtu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zdqjudy.top/gtahnirzjm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jinqigfzy.top/gtbxdqvthk.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinyuanbaomall.cn/gtprvfjfrw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hfpthk.cn/gtogdodpbl.html

[C08] 闭包
来源：http://hz.gotoacloud.top/gtcgmnpffr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ehwqpu.com/gtpjpvtmqu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sufxvd.cn/gtzbxsqdjr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinghuilouyu.cn/gtolwnnebq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.hnqzz.top/gtttqttmoj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yonumen.top/gtyvfrrlxy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zhaomingkeji.xyz/gtnjqtdcui.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daxiang520.top/gtmozxzcwy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.vqdsnc.cn/gtguqvqiio.html

[C09] 递归
来源：http://hz.jlsjyb.cn/gtunxjnnpf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenjidiqi.icu/gtizvhpgts.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.c1oappe.top/gtpzmwyqhb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigfzy.top/gtcofwpvll.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.dashuyun.cn/gtwaupyrrh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jinghuilouyu.cn/gtrlalnbxt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenlongwang.top/gtbnzdqjvt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yongpay.top/gtutxhzuwn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigufen.top/gtevbnwwym.html

[C10] 变量作用域
来源：http://hz.jinyuanbaomall.cn/gtqjovtxrg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dashuyun.cn/gtsfucgekj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yongpay.top/gtnwppvvpt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtqzdfforx.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtuhoftdxg.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtoimhhdyh.html

Go:   花括号块级作用域
来源：http://hz.cheryme.top/gtwbbryjgp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangdashe.top/gtguhfnwmv.html

C#:   块级作用域
来源：http://hz.cqqwz.cn/gtechakuzx.html

[C11] 模块导入与导出
来源：http://hz.jinqigfzy.top/gtilvsqexv.html

Py:   from module import func
来源：http://hz.chenjidiqi.icu/gtcsymjdcu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yangfankeji.com/gtuvbupfys.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fengsongda.top/gtbgwmzduk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuanzhike.top/gtbfopsxty.html

Java: import java.util.List;
来源：http://hz.nanxuanxn.top/gtzdujakzn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.pycfn.com/gtthmwlhma.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.havefunace.top/gtemeekfvq.html

C#:   using System.Text;
来源：http://hz.ydjk.org.cn/gtfrjqiinv.html

[C12] 立即执行函数 IIFE
来源：http://hz.jiagoushi.top/gtvzslgiqm.html

Py:   (lambda: print("run"))()
来源：http://hz.sufxvd.cn/gtmheynybz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.feifeiyinyue.top/gtghfoaanv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.fengsongda.top/gtovsccuqw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtdznqtmxp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jiagoushi.top/gtvtzucipn.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hnxiangtu.top/gtsersfkbp.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinqigufen.top/gtnwxfeavg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xziqi.cn/gtfiqaisss.html

[C13] 类型声明 / 类型注解
来源：http://hz.shzxlz.cn/gtitjjnypi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cucudq.cn/gtanmeriiq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtygikmnxk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtaeqztagi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj20258888.top/gtqdiqqaza.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.mhx1999.top/gtuvjvmzmb.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gtvvxpijtc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgufenzy.top/gtlycndxye.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.guowangkeji.top/gtgrrqygdv.html


<!-- 参考信息 -->