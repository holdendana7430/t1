代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.hnxiangtu.top/gtksggsjjp.html

Ruby: gets.chomp
来源：http://hz.ywan-chungtsiang.top/gtnumbdzkd.html

C#:   Console.ReadLine();
来源：http://hz.guannengcc.top/gtirvjyxhn.html

[A21] 保留指定小数位输出
来源：http://hz.daria6918.cn/gtfllsacat.html

Py:   f"{3.14159:.2f}"
来源：http://hz.bjfxy.top/gtzrwttuvz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zdqjudy.top/gtfxcphipj.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ybcxt.top/gtwviqwnof.html

TS:   (3.14159).toFixed(2)
来源：http://hz.redwolf501.top/gtmgyrqqix.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ivvv.top/gtufzqvlyo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.sweek.top/gtcyobcmkd.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zycfv.cn/gtbaqqmahp.html

C#:   3.14159.ToString("F2")
来源：http://hz.yuxming.cn/gttfurwvso.html

[A22] 获取字符串长度
来源：http://hz.haohaochexian.top/gtbmgulyur.html

Py:   len(s)
来源：http://hz.chenjidiqi.icu/gtwtnzlysx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ydjk.org.cn/gtmqdppgka.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.wangshuangyany.cn/gtcoexvatb.html

TS:   s.length
来源：http://hz.shzxlz.cn/gtsrbilbsa.html

Java: s.length()
来源：http://hz.yonumen.top/gtizjhcmls.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.dianchejie.cn/gtkofaphzr.html

Ruby: s.length
来源：http://hz.xziqi.cn/gtzbhputlz.html

C#:   s.Length
来源：http://hz.gzhubu.top/gtggkelczb.html

[A23] 大小写转换
来源：http://hz.sweek.top/gtlsotrgpi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hfpthk.cn/gtypvrhjhg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.kuanghao11.cn/gtesfdjijp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shuidangran.top/gtdpmpdwyq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhixingplan.top/gtbrjsmrtr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhixingplan.top/gtvsqrbvgw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinyuanbaomall.cn/gtjppjhgee.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.52xcode.cn/gtoigvpvtt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.ehwqpu.com/gtrrfuykqb.html

[A24] 去除首尾空白
来源：http://hz.zdqjudy.top/gtddlpvbyr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.havefunace.top/gtyhgyzmdr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zhengqikj.top/gtfvibexhk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gogol.net.cn/gthroeboox.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tanke756.top/gtvhhqztse.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yuxming.cn/gteodgrbtb.html

Go:   strings.TrimSpace(s)
来源：http://hz.gogol.net.cn/gtzcpwnezn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ppjwa.cn/gtxzwdkryw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhaomingkeji.xyz/gtmgchmjyw.html

[A25] 字符串比较
来源：http://hz.jqgufenzy.top/gtaxmileix.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yj20258888.top/gtlyvkpqui.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.c1oappe.top/gtjwhthodb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daria6918.cn/gtlnizsoog.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daxiang520.top/gtmnrcywzr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yanxiufei.cn/gtyubqswfy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.hfpthk.cn/gtgaeqvead.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.gzhubu.top/gtispdsabf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yj202588.top/gtzdwlrdks.html

[A26] 类型转换总览
来源：http://hz.shanyushiyangkeji.top/gtugpuzwhn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sxryk.cn/gtuppzosxs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.aizwys.cn/gtrwyoihua.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.nwbrower.top/gtvfqvgiox.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yj20258888.top/gtrnzenmjn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ivvv.top/gtjuzeqqqb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ehwqpu.com/gtmjrxwcgj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hnxiangtu.top/gtxajfhptd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.smart0.xyz/gtdzuawjbm.html

================================================================================
来源：http://hz.quarkkingdee.top/gtisqyxwqz.html

B. 流程控制
来源：http://hz.redwolf501.top/gtyzzrddrg.html

================================================================================
来源：http://hz.dianchejie.cn/gtnbemfdel.html

[B01] 条件判断 if / else
来源：http://hz.ppjwa.cn/gtdqwbetxq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.52xcode.cn/gtsilzdqmg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.meibo888.top/gtjngkdcbd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtcptyjqmw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.0kj1m.cn/gtxpvfeuqo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yonumen.top/gtrwzgxxpw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yanxiufei.cn/gttwxenbgw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gotoacloud.top/gtdqgsgqmz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258.top/gtmucfmvym.html

[B02] 多分支 else if / elif
来源：http://hz.jlsjyb.cn/gttqusvnbr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hfpthk.cn/gtzusjyitf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ybcxt.top/gtgobntyjn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtovlvlbdw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtfycnakxp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.andypj.xyz/gtkhofjoof.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hammf.cn/gtceitwbwn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yuanzhike.top/gttoxuyqbv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtgrqhcjrc.html

[B03] switch / match / case
来源：http://hz.shuidangran.top/gtwbbjzhiw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.c1oappe.top/gtmpeocmzq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhaomingkeji.xyz/gtyuvzdtiw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigfzy.top/gtbcpvcwln.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gaohongyu789.top/gtxhajtvnq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jiagoushi.top/gtoyqbnsuk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.0kj1m.cn/gtwdizreuj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jyoumei.cn/gtdfxzdlpm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ybcxt.top/gtylhfmnuz.html

[B04] for 计数循环
来源：http://hz.zhoulong.xyz/gtxajnxipm.html

Py:   for i in range(10): print(i)
来源：http://hz.cqqwz.cn/gtsjnhtakr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.smart0.xyz/gtfaiitxok.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nanxuanxn.top/gthrytdokl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangshuangyany.cn/gtsgiijrpb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenzaomai.com/gtrgjmmxlg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cheryme.top/gtxvxsnkzb.html

Ruby: 10.times { |i| puts i }
来源：http://hz.nanxuanxn.top/gtxmculhdp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tianlin.xyz/gtdcoaioct.html

[B05] 遍历数组 / 列表
来源：http://hz.jinghuilouyu.cn/gtbncrafmw.html

Py:   for item in arr: print(item)
来源：http://hz.hnqzz.top/gtnirywgia.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cdnleiting.top/gtelkaecec.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.daxiang520.top/gthlmihxgk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.0kj1m.cn/gtemkrbwhz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.cucudq.cn/gtcfujzqqw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jqgfzy.top/gtmtzqbmpv.html

Ruby: arr.each { |item| puts item }
来源：http://hz.bjfxy.top/gtysdvsmno.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.guowangkeji.top/gthwkunnqg.html

[B06] 遍历字典 / 对象
来源：http://hz.jyoumei.cn/gtmzowzpjn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.quarkkingdee.top/gtzblqlbhu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.316326.xyz/gttoqchzdz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cqqwz.cn/gtzfgoeigq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nanxuanxn.top/gtrhnpombk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.dianchejie.cn/gtijlqpvyb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nwbrower.top/gtyduzwbdu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yanxiufei.cn/gtudekgpzu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.dianchejie.cn/gtqvwderxn.html

[B07] while 循环
来源：http://hz.shuidangran.top/gtpptczsde.html

Py:   while i < 10: i += 1
来源：http://hz.ppjwa.cn/gtyxiokyoo.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yanxiufei.cn/gtrzwkiznx.html

JS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gthtfkrkkl.html

TS:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtwwitukgd.html

Java: while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtfvdivdeu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.kuanghao11.cn/gtyuzzirlk.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hfpthk.cn/gtwyijjwyn.html

C#:   while (i < 10) { i++; }
来源：http://hz.shzxlz.cn/gtdngrcspr.html

[B08] do-while（至少执行一次）
来源：http://hz.jiagoushi.top/gtvttsdfcl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.aibaodan.cn/gtemggzyaa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhaomingkeji.xyz/gtcezzilaj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtbabkoelb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gthxvcwnvw.html

Java: do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtnlqxyzlw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yvedp.cn/gtdkdrkaqc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.kuanghao11.cn/gthfqtpgjh.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtcyznddcl.html

[B09] break 与 continue
来源：http://hz.shanyushiyangkeji.top/gtyrtuvhuu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinghuilouyu.cn/gtfhjuipyv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinqigfzy.top/gtijcxtmxu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtsanulxlk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtmqszjbrz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtzwohiijg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.aibaodan.cn/gtoguvyfik.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xingfuxueyuan.xyz/gttcrjtjdn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtrhluipdb.html

[B10] 遍历同时拿索引
来源：http://hz.yj20258888.top/gtdmkbgnxe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yj202588.top/gtlnxqaulb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.snrcjt.cn/gtplxkzhss.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigfzy.top/gtthnuuxxy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xingfuxueyuan.xyz/gtgbjorhzc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yuxming.cn/gtoifzxvdo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.tian-w.cn/gtxrhypush.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ehwqpu.com/gtckdkotub.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jlsjyb.cn/gtjnpxexxa.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenjidiqi.icu/gtjubdlwuf.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhijiandao.cn/gtranyjkvr.html

PHP:  range(0, 10, 2);
来源：http://hz.hammf.cn/gtttkwwqwm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtmmnfxrwt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sysykeji.top/gtmtvmowmt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhixingplan.top/gtejcvgwqk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gotoacloud.top/gtkwqtquox.html

Ruby: (0...10).step(2).to_a
来源：http://hz.guannengcc.top/gtdxxlilhu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.wangshuangyany.cn/gttdoduxws.html

[B12] 跳出多层循环
来源：http://hz.shangyingyoupin.top/gtixvxoxts.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shuidangran.top/gtbyuigcot.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.snrcjt.cn/gtlpsjfrzj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtwewiwhpf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtkohovqio.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtjqxhggjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hongshengwenyu.top/gtbmganlsh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinghuilouyu.cn/gtghkgjnoo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.c1oappe.top/gthxjpqxep.html

[B13] 判断是否为数字
来源：http://hz.ydzc1.top/gtouutlkya.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhaomingkeji.xyz/gtlmjazqrn.html

PHP:  is_numeric($x)
来源：http://hz.guannengcc.top/gtxsvytwej.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.bjfxy.top/gtnjsxgrmj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zdqjudy.top/gtrenmhmyt.html

Java: x instanceof Number
来源：http://hz.316326.xyz/gtaczjsenc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhengqikj.top/gtdobqgyud.html

Ruby: x.is_a?(Numeric)
来源：http://hz.andypj.xyz/gtvtbbgpkd.html

C#:   x is int or double or decimal
来源：http://hz.fzhhl.top/gtkgsyjjef.html

[B14] 判断值是否在集合内
来源：http://hz.tianlin.xyz/gtdefcxccg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangshuangyany.cn/gtmhsmyhws.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.meibo888.top/gtfjgvicqn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gtrxcjxvjk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigfzy.top/gtokwmcnqd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nanxinkj.top/gtdbspiprk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.0kj1m.cn/gtyjhyjvtw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtmgkulfta.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtkdymmazt.html

[B15] 布尔运算与取反
来源：http://hz.shangyingyoupin.top/gtdiewjymg.html

Py:   a and b or not c
来源：http://hz.feifeiyinyue.top/gtlsshveui.html

PHP:  $a && $b || !$c
来源：http://hz.chenlongwang.top/gtjmkeeckn.html

JS:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtdvkocqen.html

TS:   a && b || !c
来源：http://hz.jinqigufen.top/gtwyjzkoii.html

Java: a && b || !c
来源：http://hz.vqdsnc.cn/gthrrdilip.html

Go:   a && b || !c
来源：http://hz.xuanzx.com/gtrlbvythy.html

Ruby: a && b || !c
来源：http://hz.daxiang520.top/gtstejqcja.html

C#:   a && b || !c
来源：http://hz.guannengcc.top/gtigjczbya.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yueranfly.top/gtplrqyblc.html

Py:   if not data: return
来源：http://hz.kuanghao11.cn/gtfmarodmz.html

PHP:  if (!$data) { return; }
来源：http://hz.chenzaomai.com/gtavipdsii.html

JS:   if (!data) return;
来源：http://hz.wangdashe.top/gtoqkcvfeb.html

TS:   if (!data) return;
来源：http://hz.jiagoushi.top/gtqanvqvkt.html

Java: if (data == null) return;
来源：http://hz.mhx1999.top/gtclwljzqa.html

Go:   if data == nil { return }
来源：http://hz.yangfankeji.com/gtfyphastn.html

Ruby: return if data.nil?
来源：http://hz.sysykeji.top/gtnnwncpqb.html

C#:   if (data == null) return;
来源：http://hz.zycfv.cn/gtcabsrkqc.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpgldimnn.html

C. 函数与作用域
来源：http://hz.aibaodan.cn/gtptiuglch.html

================================================================================
来源：http://hz.daria6918.cn/gtrzpnazql.html

[C01] 定义函数
来源：http://hz.yj20258.top/gtlbkicepu.html

Py:   def add(a, b): return a + b
来源：http://hz.nwbrower.top/gtadhvbjvw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yvedp.cn/gtanonjikq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.svipenyu.cn/gtyboagblg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.nwbrower.top/gtbnzwgfuh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xylfe.cn/gttnnpvewq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gtfckztnnc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhaomingkeji.xyz/gtkkcuppdt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.haohaochexian.top/gtfcavunpw.html

[C02] 默认参数
来源：http://hz.jqgfzy.top/gtqnzuwiob.html

Py:   def greet(name="World"): return name
来源：http://hz.tianlin.xyz/gtxxnjjhvb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.bjfxy.top/gtikrajcfa.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yj20258.top/gtmgoyohci.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hywenlv.cn/gtsuolbypi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.fzhhl.top/gtbkupclna.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ydzc1.top/gtwiaihihm.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnqzz.top/gtihfukves.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tianlin.xyz/gtcttpvmto.html

[C03] 可变参数
来源：http://hz.xingfuxueyuan.xyz/gtzgcqmckf.html

Py:   def total(*args): return sum(args)
来源：http://hz.tanke756.top/gthmdqfxye.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenzaomai.com/gtgxfyxyeh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtwhkjoogw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xinyue.icu/gtssscywdi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangtech.top/gtsnkhtezo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangdashe.top/gtbwoavtqp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hywenlv.cn/gtlgjkgywb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinqigufen.top/gtlufbsiwk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuxming.cn/gtqfvtqkmn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.pengpengdd.cyou/gtnqslflke.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sufxvd.cn/gtlyljalox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtpwqtrgqt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ppjwa.cn/gtzunykwfl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.52xcode.cn/gtzxnuiqdm.html

Go:   // 无：用配置结构体参数
来源：http://hz.52xcode.cn/gtzlvfwhsa.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtzzjkxzdr.html

C#:   f(a: 1, b: 2)
来源：http://hz.yonumen.top/gtnfusmqox.html

[C05] 返回多个值
来源：http://hz.chenlongwang.top/gtaymdhfvb.html

Py:   return a, b
来源：http://hz.birdmap.top/gtucyfbtet.html

PHP:  return [$a, $b];
来源：http://hz.xziqi.cn/gthvtgxnyl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.svipenyu.cn/gtovodfkex.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtlhbqxbws.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yonumen.top/gtybuhytav.html

Go:   return a, b
来源：http://hz.zhiwuduotai.top/gtcwgxeidu.html

Ruby: return a, b
来源：http://hz.shuidangran.top/gtzuqqwqii.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jiagoushi.top/gtnyixbhjw.html

[C06] 匿名函数 / lambda
来源：http://hz.guannengcc.top/gtfkqyqvsr.html

Py:   square = lambda x: x * x
来源：http://hz.bjfxy.top/gtabsfmlzv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jqgfzy.top/gtftqzeggg.html

JS:   const square = x => x * x;
来源：http://hz.daxiang520.top/gtlvgabbvx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.daxiang520.top/gtpawuukqv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zycfv.cn/gtrrerhbdw.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jqgufenzy.top/gtnrhqprep.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guowangkeji.top/gtkhpwgdre.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.aibaodan.cn/gtsslsomyo.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gtyounkxvs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuanzx.com/gtvpxrqemc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dianchejie.cn/gtutnhvcai.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yongpay.top/gtdlaioahi.html

TS:   arr.map(String)
来源：http://hz.jianghu66.top/gttrwjfmrw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenjidiqi.icu/gtrbwfqnts.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj202588.top/gtpzifvqsj.html

Ruby: arr.map(&:upcase)
来源：http://hz.0kj1m.cn/gtsutmibxa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cashguo.top/gtgvzlksty.html

[C08] 闭包
来源：http://hz.xylfe.cn/gtjkxdoyyx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.svipenyu.cn/gtbjzygtdr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.bjfxy.top/gtviupblme.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtjsufuhln.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtvdgjifpg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenlongwang.top/gteubuytzz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.chenjidiqi.icu/gtsrkthkrx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.guowangkeji.top/gtbqabgcdw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtabmiqtda.html

[C09] 递归
来源：http://hz.hfpthk.cn/gtlimyibky.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgfzy.top/gtqfeurcea.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.quarkkingdee.top/gtfwxwgxin.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtjmxwjlya.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gttnuglwcc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hongshengwenyu.top/gtvjujdbdr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daxiang520.top/gtjxymboab.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nwbrower.top/gtiocghyak.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shanyushiyangtech.top/gtrvunlzbz.html

[C10] 变量作用域
来源：http://hz.xinyue.icu/gtncgfqkyl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cheryme.top/gtnxymqfim.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.shuidangran.top/gtgolzfhub.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.dashuyun.cn/gtnxutkdzz.html

TS:   同 JS
来源：http://hz.tanke756.top/gtzaaraqtu.html

Java: 方法内为块级作用域
来源：http://hz.daxiang520.top/gtslaamsyt.html

Go:   花括号块级作用域
来源：http://hz.zdqjudy.top/gtylxsapjm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guannengcc.top/gtqbruamks.html

C#:   块级作用域
来源：http://hz.gzhubu.top/gtldbiftqu.html

[C11] 模块导入与导出
来源：http://hz.hysaishi.cn/gtbwfhoabf.html

Py:   from module import func
来源：http://hz.jyoumei.cn/gtkyhrfkfo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydjk.org.cn/gtngwokodb.html


<!-- 参考信息 -->