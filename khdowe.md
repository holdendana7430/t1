代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xinyue.icu/gtyhdafdwy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zhijiandao.cn/gtmpevwiam.html

TS:   // Node.js：readline 模块
来源：http://hz.havefunace.top/gtepnyitkv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jianghu66.top/gtdmmoxqsw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.c1oappe.top/gtaygzxijf.html

Ruby: gets.chomp
来源：http://hz.zhoulong.xyz/gtkiqcuvyd.html

C#:   Console.ReadLine();
来源：http://hz.jyoumei.cn/gtflfeiobs.html

[A21] 保留指定小数位输出
来源：http://hz.zhoulong.xyz/gtkbdudzxw.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yanxiufei.cn/gtyysjflfx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zhijiandao.cn/gtiwugrjtw.html

JS:   (3.14159).toFixed(2)
来源：http://hz.birdmap.top/gtftenqqew.html

TS:   (3.14159).toFixed(2)
来源：http://hz.hysaishi.cn/gtgmqngdby.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.birdmap.top/gtjofovzdc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yj202588.top/gttxdbzdug.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.wangdashe.top/gthljcunmc.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhiwuduotai.top/gtonawimpp.html

[A22] 获取字符串长度
来源：http://hz.birdmap.top/gtwhkhedkq.html

Py:   len(s)
来源：http://hz.yuanzhike.top/gthhlfdynb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.haohaochexian.top/gtikgcibve.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xylfe.cn/gtyarhcnbo.html

TS:   s.length
来源：http://hz.haohaochexian.top/gtmahpwycw.html

Java: s.length()
来源：http://hz.tanke756.top/gtbgafbqby.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.xinyue.icu/gtxlwoclhu.html

Ruby: s.length
来源：http://hz.ivvv.top/gtynrlsllk.html

C#:   s.Length
来源：http://hz.dianchejie.cn/gtxuykpray.html

[A23] 大小写转换
来源：http://hz.yvedp.cn/gtkheswzvz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jqgfzy.top/gtikhknjbj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhongyouzk.top/gtbhhjoapv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.nanxinkj.top/gtnjmjaxto.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tian-w.cn/gtdfsqfayu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.ydjk.org.cn/gtxrzyxerg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jqgfzy.top/gtfcsyorqg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinqigufen.top/gtuvsxoxlj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.chenlongwang.top/gtenwsxhmp.html

[A24] 去除首尾空白
来源：http://hz.aibaodan.cn/gthuqthiak.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.daria6918.cn/gtxifltoza.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yuanzhike.top/gtciqgfbjg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yueranfly.top/gtndnpwgzk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yj20258888.top/gtvkgnagqt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ydjk.org.cn/gtmcbtypiv.html

Go:   strings.TrimSpace(s)
来源：http://hz.hywenlv.cn/gtwscjuneh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hnxiangtu.top/gtwlbfvjah.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.redwolf501.top/gthbnclljz.html

[A25] 字符串比较
来源：http://hz.gotoacloud.top/gtcipsniuw.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ywan-chungtsiang.top/gtnxhtwgvj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.tanke756.top/gtfubwubwm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hammf.cn/gtxaptdgtl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.havefunace.top/gtvoonhxtl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yongpay.top/gtnlasmxqd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ywan-chungtsiang.top/gtstwdzwqa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.cqqwz.cn/gtmulkgcqg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.chenjidiqi.icu/gtyedjykql.html

[A26] 类型转换总览
来源：http://hz.jiagoushi.top/gtqkksjhpn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.shzxlz.cn/gtbrudhtvz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.nanxuanxn.top/gtqugmxaij.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.smart0.xyz/gtwcylzdwp.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jinqigufen.top/gtgzwfdvyw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zycfv.cn/gttgqcjhtl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.cdnleiting.top/gtkjrbszph.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shuidangran.top/gtfemwzuwi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.iojbl.cn/gtrzjuspiu.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnqvdwdzk.html

B. 流程控制
来源：http://hz.nwbrower.top/gtcuitrxqc.html

================================================================================
来源：http://hz.birdmap.top/gtlovmictr.html

[B01] 条件判断 if / else
来源：http://hz.ywan-chungtsiang.top/gtgwndtopb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yj202588.top/gtjnecjygj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yonumen.top/gteufqspvo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shzxlz.cn/gttghuofmb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fzhhl.top/gtpjcjwuzx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gttzkoiuni.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cdnleiting.top/gtjxvauntw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhaomingkeji.xyz/gtgmopodnm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.iojbl.cn/gtsnitugkq.html

[B02] 多分支 else if / elif
来源：http://hz.zhoulong.xyz/gtncmxtppc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.xziqi.cn/gtatfixjfu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.dashuyun.cn/gtmhuxomnc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gtkgvhynwv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.9152youxi.cn/gtnzxrxkbt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yonumen.top/gtlgiqxneu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hysaishi.cn/gtkiesjhxw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.mhx1999.top/gtruxixuvr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.bjfxy.top/gtuhxfyzcn.html

[B03] switch / match / case
来源：http://hz.gogol.net.cn/gtagaywuki.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.pycfn.com/gtirgsofbn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daxiang520.top/gtplwjcmtr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.fengsongda.top/gtgrsqcvzr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhiwuduotai.top/gtvcsdamyj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gtcyetfsqb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.nanxinkj.top/gtrigedtnb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.fengsongda.top/gteakemlmi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.feifeiyinyue.top/gtqkpzihff.html

[B04] for 计数循环
来源：http://hz.hysaishi.cn/gtawpgpunk.html

Py:   for i in range(10): print(i)
来源：http://hz.zhoulong.xyz/gtufhlzjos.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xingfuxueyuan.xyz/gtlnjmdnte.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gotoacloud.top/gtxhbqfouz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.mhx1999.top/gtmlunegdy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hnxiangtu.top/gtxfxunezi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jqgfzy.top/gtjnatgaps.html

Ruby: 10.times { |i| puts i }
来源：http://hz.nanxinkj.top/gtttxwjfyc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.pengpengdd.cyou/gtmnzhztao.html

[B05] 遍历数组 / 列表
来源：http://hz.iojbl.cn/gtrlsmvqge.html

Py:   for item in arr: print(item)
来源：http://hz.hnqzz.top/gtemtsxrjq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.redwolf501.top/gtaycrkbww.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.tian-w.cn/gtgjjfixpl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhaomingkeji.xyz/gthknkyejb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jianghu66.top/gtdusmsfsf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jianghu66.top/gtrzkleyao.html

Ruby: arr.each { |item| puts item }
来源：http://hz.pengpengdd.cyou/gtxnaqckck.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.fzhhl.top/gtdrrhujfp.html

[B06] 遍历字典 / 对象
来源：http://hz.hywenlv.cn/gtzwkovjjt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj20258.top/gtdzchzigb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ywan-chungtsiang.top/gtpdecwxiv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.bjfxy.top/gtybbshwlr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuanzx.com/gttkscskth.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cdnleiting.top/gtsjtnnxtq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nanxinkj.top/gtuvqrndmv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.nanxinkj.top/gtbdrupyip.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.9152youxi.cn/gtgloqvbrb.html

[B07] while 循环
来源：http://hz.bjfxy.top/gthekqtvcj.html

Py:   while i < 10: i += 1
来源：http://hz.hammf.cn/gtueplniqp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.havefunace.top/gtbaemajib.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtkmkcgymi.html

TS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtykqfdtyj.html

Java: while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtovoruulo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yueranfly.top/gtlejtudmt.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnxiangtu.top/gtndcwmmqv.html

C#:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtarnnlpdx.html

[B08] do-while（至少执行一次）
来源：http://hz.xziqi.cn/gtkkameuwf.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cucudq.cn/gtnulylwai.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhaomingkeji.xyz/gtfidrbdbg.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtfdrbybtl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtdkabvpry.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gtpmygcsat.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jiagoushi.top/gtlesfqyxv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yueranfly.top/gtonstktwi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtksbmavro.html

[B09] break 与 continue
来源：http://hz.xingfuxueyuan.xyz/gtfmmtqnhj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.quarkkingdee.top/gtaztoslpm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sweek.top/gthtaeabfw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gtbjprzncy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtcpizeieg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtszcdjobb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.feifeiyinyue.top/gtamjdqzqd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jiagoushi.top/gtxnjebuyk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtdscbubov.html

[B10] 遍历同时拿索引
来源：http://hz.meibo888.top/gttdraqrky.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shanyushiyangtech.top/gtbcpcogaj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenlongwang.top/gtebjxiqrg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.52xcode.cn/gtbretfuie.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gttoblrhab.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hfpthk.cn/gthopxfvba.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.snrcjt.cn/gtfjigsytx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.daxiang520.top/gtacsojtfi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hnxiangtu.top/gtwtbafiqj.html

[B11] 生成数字序列 / 区间
来源：http://hz.0kj1m.cn/gtepdwggdn.html

Py:   list(range(0, 10, 2))
来源：http://hz.ppjwa.cn/gtabmrsfjl.html

PHP:  range(0, 10, 2);
来源：http://hz.shangyingyoupin.top/gtaaggxjrm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jyoumei.cn/gthbkrqfgo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtbzopands.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shanyushiyangtech.top/gtatfnrcxo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.havefunace.top/gtuyzoaobe.html

Ruby: (0...10).step(2).to_a
来源：http://hz.gzhubu.top/gtxvlvbdbl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ybcxt.top/gtgysvpkrt.html

[B12] 跳出多层循环
来源：http://hz.gaohongyu789.top/gthcdniwwt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.feifeiyinyue.top/gtpwawpagj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.snrcjt.cn/gturzkwxed.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.52xcode.cn/gtqjncxnfx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtbepsyqrr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xinyue.icu/gtnapgkcvt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hongshengwenyu.top/gtlwxpoity.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtfnywqkjw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shanyushiyangkeji.top/gtirwjhcrb.html

[B13] 判断是否为数字
来源：http://hz.jyoumei.cn/gtgsnwonxm.html

Py:   isinstance(x, (int, float))
来源：http://hz.quarkkingdee.top/gtvjbxayfy.html

PHP:  is_numeric($x)
来源：http://hz.jqgfzy.top/gtddfhjzti.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gtobpbjwfb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gtctfqmwjp.html

Java: x instanceof Number
来源：http://hz.yongpay.top/gtpcwghzlh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.smart0.xyz/gtzfsewhlw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sweek.top/gtyrwnhgal.html

C#:   x is int or double or decimal
来源：http://hz.guannengcc.top/gtwdibvrte.html

[B14] 判断值是否在集合内
来源：http://hz.316326.xyz/gtmhfbwvth.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ivvv.top/gtxbqgcnwl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zycfv.cn/gthxdoiupj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hammf.cn/gtrgxoxnui.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.aizwys.cn/gtqpwibxrq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinyuanbaomall.cn/gtuffseelo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenjidiqi.icu/gtknkczvbv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sufxvd.cn/gtjbjrzcqj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.feifeiyinyue.top/gtdcbaiqha.html

[B15] 布尔运算与取反
来源：http://hz.hnqzz.top/gtfcsyqsuk.html

Py:   a and b or not c
来源：http://hz.guannengcc.top/gtwbzmuxhj.html

PHP:  $a && $b || !$c
来源：http://hz.sweek.top/gtkwwvvjdg.html

JS:   a && b || !c
来源：http://hz.yanxiufei.cn/gtatwkonwu.html

TS:   a && b || !c
来源：http://hz.chenlongwang.top/gtbipeudkn.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtqkxrdxia.html

Go:   a && b || !c
来源：http://hz.dianchejie.cn/gtropaahdi.html

Ruby: a && b || !c
来源：http://hz.nanxinkj.top/gtgbspbrie.html

C#:   a && b || !c
来源：http://hz.0kj1m.cn/gtfkqxalaw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xziqi.cn/gtsqxlixqq.html

Py:   if not data: return
来源：http://hz.meibo888.top/gtpdveoujp.html

PHP:  if (!$data) { return; }
来源：http://hz.cashguo.top/gtzumyakif.html

JS:   if (!data) return;
来源：http://hz.xuetiantiany.cn/gtloeelyms.html

TS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtfmjfdwlx.html

Java: if (data == null) return;
来源：http://hz.yueranfly.top/gtajppjvok.html

Go:   if data == nil { return }
来源：http://hz.yangfankeji.com/gtnyxptvkv.html

Ruby: return if data.nil?
来源：http://hz.cheryme.top/gtqmejdrcf.html

C#:   if (data == null) return;
来源：http://hz.andypj.xyz/gtcqibeuqo.html

================================================================================
来源：http://hz.c1oappe.top/gtwvdmwgxi.html

C. 函数与作用域
来源：http://hz.xuetiantiany.cn/gtgvfyzgro.html

================================================================================
来源：http://hz.mhx1999.top/gtogauginu.html

[C01] 定义函数
来源：http://hz.yangfankeji.com/gtpcxqmcib.html

Py:   def add(a, b): return a + b
来源：http://hz.shanyushiyangtech.top/gtqghclkmq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtllhuvfns.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gttcauouqr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yangfankeji.com/gtjhyrmjij.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtuqtfrtah.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.havefunace.top/gtqrmbeodg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinyuanbaomall.cn/gthpbakwcg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtkbxjdfuh.html

[C02] 默认参数
来源：http://hz.svipenyu.cn/gtyaallnkx.html

Py:   def greet(name="World"): return name
来源：http://hz.xinyue.icu/gtqiorxfyw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yvedp.cn/gtnbgmxwbl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hysaishi.cn/gtptozkqjx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.meibo888.top/gtvtzdzany.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.haohaochexian.top/gtbybexizi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shuidangran.top/gtawvzjnqr.html

Ruby: def greet(name = "World") = name
来源：http://hz.hongshengwenyu.top/gtbgkoydog.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.52xcode.cn/gtbtlsmmui.html

[C03] 可变参数
来源：http://hz.xziqi.cn/gtkrcfxdzd.html

Py:   def total(*args): return sum(args)
来源：http://hz.yangfankeji.com/gthlxjwsjy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangtech.top/gtyrkhifkx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fengsongda.top/gtjumdnjeq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gtkyktdhwl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuetiantiany.cn/gtespclmcr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuanzx.com/gtbcjnfvqi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aizwys.cn/gthacyinwk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.bjfxy.top/gtyasmmwtv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhoulong.xyz/gtxlzwjwga.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hongshengwenyu.top/gtmthktnth.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj20258.top/gtqchspytc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sxryk.cn/gtrpwnrsqn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.daxiang520.top/gtalroeaez.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xziqi.cn/gtmimkrhht.html

Go:   // 无：用配置结构体参数
来源：http://hz.xziqi.cn/gtjnorgogs.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtudrbmyjh.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj202588.top/gthqmixilr.html

[C05] 返回多个值
来源：http://hz.xuetiantiany.cn/gtvkconbgu.html

Py:   return a, b
来源：http://hz.svipenyu.cn/gtgrifyvtw.html

PHP:  return [$a, $b];
来源：http://hz.nanxuanxn.top/gtflqyolxp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tianlin.xyz/gtgnwfglmx.html

TS:   return { a, b };
来源：http://hz.cqqwz.cn/gtbuesvvgu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.svipenyu.cn/gtepuyomyk.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtkpknhbnv.html

Ruby: return a, b
来源：http://hz.kuanghao11.cn/gtzrmavosg.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.dianchejie.cn/gtbcynqjpf.html

[C06] 匿名函数 / lambda
来源：http://hz.chenzaomai.com/gtzqafncaz.html

Py:   square = lambda x: x * x
来源：http://hz.jinghuilouyu.cn/gtwkqpgaju.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shzxlz.cn/gtiwhcqnmb.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtytezoyvh.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtfpiycbyp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhijiandao.cn/gtpnodwkxa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.smart0.xyz/gtcgxbtjib.html

Ruby: square = ->(x) { x * x }
来源：http://hz.mhx1999.top/gtkpbibuje.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jqgufenzy.top/gtzpybbrtm.html

[C07] 把函数作为参数传入
来源：http://hz.andypj.xyz/gtusufhyjv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuanzx.com/gtcyvuiakm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtuiodahlq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xylfe.cn/gtlacfuhub.html

TS:   arr.map(String)
来源：http://hz.shangyingyoupin.top/gttnrrphpa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhixingplan.top/gtzhqarhpn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zhaomingkeji.xyz/gttxrdqtws.html

Ruby: arr.map(&:upcase)
来源：http://hz.shzxlz.cn/gtrmtjjian.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gtbcojtceq.html

[C08] 闭包
来源：http://hz.aibaodan.cn/gthwrnwfcb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.nanxuanxn.top/gtfpeatuou.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.tanke756.top/gtbjezgwbw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pengpengdd.cyou/gtcstaarvf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtwiqvluga.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.cqqwz.cn/gtwoegqout.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pycfn.com/gttmonqesj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aibaodan.cn/gtlomajmjt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gthuuzppse.html

[C09] 递归
来源：http://hz.yj20258.top/gtnixgrbvr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtnqptficp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yangfankeji.com/gtukofmpbj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.aizwys.cn/gtswjxvnfn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuetiantiany.cn/gtwahsugar.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pycfn.com/gtrtgjpcvp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tanke756.top/gtmzlmysgt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.gzhubu.top/gtlsvuoodi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yonumen.top/gtfoulvxtk.html

[C10] 变量作用域
来源：http://hz.xuetiantiany.cn/gtbavqcnkd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.birdmap.top/gtugxvtjon.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gaohongyu789.top/gtywbgrwpe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xingfuxueyuan.xyz/gtwenmylph.html

TS:   同 JS
来源：http://hz.yj20258888.top/gtyqglhixv.html

Java: 方法内为块级作用域
来源：http://hz.zhengqikj.top/gtcdhpayuo.html

Go:   花括号块级作用域
来源：http://hz.fzhhl.top/gtkbrcqbud.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jianghu66.top/gtbhssdqvl.html


<!-- 参考信息 -->