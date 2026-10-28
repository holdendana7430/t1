代发 wailian999

Ruby: a, b = b, a
来源：http://hz.chenjidiqi.icu/gtezwpcsdx.html

C#:   (a, b) = (b, a);
来源：http://hz.hysaishi.cn/gtwxayfksn.html

[A20] 读取标准输入
来源：http://hz.yuxming.cn/gtiopnpqdj.html

Py:   name = input("请输入：")
来源：http://hz.nanxuanxn.top/gtsdiagmvq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.gaohongyu789.top/gtemsxdqrh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yvedp.cn/gtumoyqdgc.html

TS:   // Node.js：readline 模块
来源：http://hz.hongshengwenyu.top/gtpcvflnac.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yj20258888.top/gtdxijwqrh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.dianchejie.cn/gtpanpgvyn.html

Ruby: gets.chomp
来源：http://hz.ehwqpu.com/gtgegkkdpl.html

C#:   Console.ReadLine();
来源：http://hz.yvedp.cn/gtxxrerfjm.html

[A21] 保留指定小数位输出
来源：http://hz.yvedp.cn/gtsnrkcwvt.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hongshengwenyu.top/gtcvmjffjy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zhaomingkeji.xyz/gtkcbdtpdu.html

JS:   (3.14159).toFixed(2)
来源：http://hz.cucudq.cn/gtlsyhkzma.html

TS:   (3.14159).toFixed(2)
来源：http://hz.hfpthk.cn/gtexameptj.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yuanzhike.top/gtsvdiykhd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hnqzz.top/gtylwzzpuv.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.pengpengdd.cyou/gtwopkoech.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhoulong.xyz/gtjhjxeysr.html

[A22] 获取字符串长度
来源：http://hz.zhijiandao.cn/gtbmmmsecn.html

Py:   len(s)
来源：http://hz.xuanzx.com/gtgnncadbl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zhengqikj.top/gtbgsrgpxj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.haohaochexian.top/gtnytwlhtp.html

TS:   s.length
来源：http://hz.hfpthk.cn/gtcjcntgyz.html

Java: s.length()
来源：http://hz.ydzc1.top/gtffmbvrwv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.fengsongda.top/gtsptnofac.html

Ruby: s.length
来源：http://hz.zhongyouzk.top/gtfepzbkoo.html

C#:   s.Length
来源：http://hz.smart0.xyz/gtyichzqxg.html

[A23] 大小写转换
来源：http://hz.kuanghao11.cn/gtqoyqbkks.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hnxiangtu.top/gtjkptwaxr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.jlsjyb.cn/gtgankmviw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ehwqpu.com/gtzgdbjbae.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.haohaochexian.top/gtyhavarpm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.svipenyu.cn/gtziwdstqx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.tianlin.xyz/gtkwizuoru.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.shanyushiyangtech.top/gtceedarrm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jyoumei.cn/gtpeaatiby.html

[A24] 去除首尾空白
来源：http://hz.cdnleiting.top/gthzatbvxp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shangyingyoupin.top/gtrtmibwbx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.52xcode.cn/gtcwcxkjoe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yanxiufei.cn/gtjlkrfxuh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.svipenyu.cn/gtfjsualdb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jinyuanbaomall.cn/gtxzdauvqv.html

Go:   strings.TrimSpace(s)
来源：http://hz.fzhhl.top/gtescxwyyi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.chenzaomai.com/gtnoyhcqtc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shangyingyoupin.top/gtadkjlzds.html

[A25] 字符串比较
来源：http://hz.guowangkeji.top/gtcgdhmeaz.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xinyue.icu/gtxewsllaf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhixingplan.top/gtekbviney.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shzxlz.cn/gtbfcgzpjy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.svipenyu.cn/gtevurmmyr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.birdmap.top/gtcghbytjp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.nanxinkj.top/gtxbbnwbjo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.dashuyun.cn/gtjojlhklz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gzhubu.top/gtmhbdthic.html

[A26] 类型转换总览
来源：http://hz.bjfxy.top/gtecbpocry.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hnxiangtu.top/gtnymyglqt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.0kj1m.cn/gtwftceias.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.chenzaomai.com/gtufirvpmw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.chenjidiqi.icu/gtorpqqhjv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xuetiantiany.cn/gtvayodtdc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.mhx1999.top/gttcjggwut.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.chenlongwang.top/gtvwwdepmi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhaomingkeji.xyz/gtcmgscqbu.html

================================================================================
来源：http://hz.jiagoushi.top/gtmmjydwfb.html

B. 流程控制
来源：http://hz.shuidangran.top/gtwbusurzr.html

================================================================================
来源：http://hz.kuanghao11.cn/gtulrngzcu.html

[B01] 条件判断 if / else
来源：http://hz.wangdashe.top/gtcgkxirdh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhongyouzk.top/gtaihzkmih.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.tian-w.cn/gtqvwomoos.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtusftvipv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zycfv.cn/gtxfbjpcck.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.daxiang520.top/gtcqwcvriq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yueranfly.top/gtbdlhhvbq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yongpay.top/gtnyxdfuqj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.feifeiyinyue.top/gtfmqewzgu.html

[B02] 多分支 else if / elif
来源：http://hz.fzhhl.top/gtsmbbuaxn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.quarkkingdee.top/gtqfabamsw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xylfe.cn/gteygvfbwy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ywan-chungtsiang.top/gtgtonfmsl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtdsrradke.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangshuangyany.cn/gtwfvueywd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.smart0.xyz/gtmjjiymqd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xuanzx.com/gtyjbcuaue.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtefgmhlyc.html

[B03] switch / match / case
来源：http://hz.jqgfzy.top/gtgzccwqyo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jianghu66.top/gttseipdlp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jqgufenzy.top/gtdostpbwj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.meibo888.top/gtitniyfnr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.52xcode.cn/gtpbpleadi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zycfv.cn/gtnyjqarbu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.tanke756.top/gtewgisqrs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.nwbrower.top/gtctpzqxzy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.pengpengdd.cyou/gtqodmcurr.html

[B04] for 计数循环
来源：http://hz.shangyingyoupin.top/gthbkdcsyp.html

Py:   for i in range(10): print(i)
来源：http://hz.xylfe.cn/gtttzfhcsg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zdqjudy.top/gtjondpupa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinghuilouyu.cn/gtyxkpfxqg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yueranfly.top/gthmnhqijd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.shanyushiyangkeji.top/gtgqisgmio.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xuanzx.com/gthyuucacd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.kuanghao11.cn/gtdqbbwdpj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tianlin.xyz/gttanuvdgv.html

[B05] 遍历数组 / 列表
来源：http://hz.yuxming.cn/gtrlgdjrav.html

Py:   for item in arr: print(item)
来源：http://hz.fengsongda.top/gtbxmwsxrq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jinqigufen.top/gtwvwyxlzo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.shanyushiyangtech.top/gtbkmznawy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.snrcjt.cn/gtdyavphix.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zdqjudy.top/gtrpnfsbom.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.vqdsnc.cn/gtyybztkfj.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ybcxt.top/gtjbacxyxd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.chenjidiqi.icu/gtqunxrdzj.html

[B06] 遍历字典 / 对象
来源：http://hz.yonumen.top/gtaxsvigib.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.nwbrower.top/gtyvpycpax.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.tanke756.top/gtgogutghv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shanyushiyangkeji.top/gtffxvwsen.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zdqjudy.top/gtjmyzvtze.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xinyue.icu/gtnaugnsll.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.dashuyun.cn/gthtknbbdc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xinyue.icu/gtkvxulxzw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jyoumei.cn/gtgmmjwllj.html

[B07] while 循环
来源：http://hz.yvedp.cn/gtjsxnafgo.html

Py:   while i < 10: i += 1
来源：http://hz.chenlongwang.top/gtrrxbkdjg.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yongpay.top/gtstbxlsxf.html

JS:   while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtxspbwgkz.html

TS:   while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtucvbeswi.html

Java: while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtmwamzqwn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.smart0.xyz/gtusaroayw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.tian-w.cn/gtufqxlmvr.html

C#:   while (i < 10) { i++; }
来源：http://hz.ehwqpu.com/gtxccgxoss.html

[B08] do-while（至少执行一次）
来源：http://hz.ehwqpu.com/gtbutoivbu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj20258888.top/gtxrgtlyol.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.daxiang520.top/gtfywkdraj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtjmyprxvh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtuccnnbxg.html

Java: do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gttyiscjho.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sxryk.cn/gtjydgrbsd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenzaomai.com/gtuehwsesu.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtbehfymnw.html

[B09] break 与 continue
来源：http://hz.quarkkingdee.top/gtkybfygym.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jinyuanbaomall.cn/gtvdriyhsf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.fzhhl.top/gtljobeptj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.kuanghao11.cn/gtvhozcqfk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtrbdezvmk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtcjcxrxnd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hammf.cn/gtfwpvcfad.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ppjwa.cn/gthjeqonih.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtgxgrwcwy.html

[B10] 遍历同时拿索引
来源：http://hz.xuanzx.com/gtqduuixhc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jiagoushi.top/gttthleymr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tanke756.top/gttknzztce.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tanke756.top/gtfhuancdy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jinqigufen.top/gtqvyxgvki.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.aibaodan.cn/gtzyyotyyk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zdqjudy.top/gtqzmzdyqx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinghuilouyu.cn/gtgbigkukj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.aizwys.cn/gtywczucue.html

[B11] 生成数字序列 / 区间
来源：http://hz.xuetiantiany.cn/gthzlmmgnh.html

Py:   list(range(0, 10, 2))
来源：http://hz.hywenlv.cn/gttulevekf.html

PHP:  range(0, 10, 2);
来源：http://hz.yonumen.top/gtfuuyesvx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtqlvuedav.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gtrohzegkw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jlsjyb.cn/gtsrepbnyh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.havefunace.top/gtnsyyrjgh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jiagoushi.top/gtetxdcwmy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zdqjudy.top/gtjvvqjrhw.html

[B12] 跳出多层循环
来源：http://hz.aibaodan.cn/gteuxgiurj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenzaomai.com/gtkfnngfmd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.meibo888.top/gtanlkcxeg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtkjkncfae.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xylfe.cn/gtgpattgod.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtluwhbdxd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.316326.xyz/gtzlfptrwe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nwbrower.top/gtcyzljsjq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ehwqpu.com/gtsajtoqya.html

[B13] 判断是否为数字
来源：http://hz.zhixingplan.top/gtyqbusnbv.html

Py:   isinstance(x, (int, float))
来源：http://hz.gaohongyu789.top/gtzvqbbnab.html

PHP:  is_numeric($x)
来源：http://hz.zhengqikj.top/gtssqszoie.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nwbrower.top/gtgxepbpfh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtzjewnhxm.html

Java: x instanceof Number
来源：http://hz.cucudq.cn/gtkypqrkoo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yj20258.top/gtwwluhadb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj202588.top/gtqmpdgkse.html

C#:   x is int or double or decimal
来源：http://hz.wangshuangyany.cn/gtzhukixzi.html

[B14] 判断值是否在集合内
来源：http://hz.ehwqpu.com/gtdmiqcboh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhoulong.xyz/gtsdnkugyx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.bjfxy.top/gttlzkxzkk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangkeji.top/gtpnwkfgap.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtkcuyddvq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.cucudq.cn/gtlyltwcqf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yj202588.top/gtcajmycfa.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gtmicaolmo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jianghu66.top/gtwgatqhdk.html

[B15] 布尔运算与取反
来源：http://hz.aibaodan.cn/gtvvukxioe.html

Py:   a and b or not c
来源：http://hz.jlsjyb.cn/gtfvmbzsth.html

PHP:  $a && $b || !$c
来源：http://hz.iojbl.cn/gtsyzqkzhu.html

JS:   a && b || !c
来源：http://hz.hnxiangtu.top/gtmnzjdofx.html

TS:   a && b || !c
来源：http://hz.hnxiangtu.top/gtmxfqoqwd.html

Java: a && b || !c
来源：http://hz.316326.xyz/gtyyagcfdp.html

Go:   a && b || !c
来源：http://hz.zdqjudy.top/gtkzusoclj.html

Ruby: a && b || !c
来源：http://hz.aizwys.cn/gtqavlaubl.html

C#:   a && b || !c
来源：http://hz.iojbl.cn/gtmqirlfrg.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ydjk.org.cn/gtbpxcownj.html

Py:   if not data: return
来源：http://hz.zhixingplan.top/gtmdbgsiqq.html

PHP:  if (!$data) { return; }
来源：http://hz.smart0.xyz/gtvecyicja.html

JS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtqgijjcyk.html

TS:   if (!data) return;
来源：http://hz.mhx1999.top/gtetignaxn.html

Java: if (data == null) return;
来源：http://hz.kuanghao11.cn/gtswylhywm.html

Go:   if data == nil { return }
来源：http://hz.ydzc1.top/gtbhqghyuo.html

Ruby: return if data.nil?
来源：http://hz.yvedp.cn/gtztrmykvw.html

C#:   if (data == null) return;
来源：http://hz.sysykeji.top/gtgdcvhhsa.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvrrzjnko.html

C. 函数与作用域
来源：http://hz.kuanghao11.cn/gtuutpgpzd.html

================================================================================
来源：http://hz.ppjwa.cn/gteyfrqfnr.html

[C01] 定义函数
来源：http://hz.vqdsnc.cn/gtagsucxrc.html

Py:   def add(a, b): return a + b
来源：http://hz.c1oappe.top/gtmilytkdj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtncvpnzam.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.bjfxy.top/gtctgrqdvt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.svipenyu.cn/gtdnsumyjc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtrltdkgge.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xuetiantiany.cn/gthbirhvih.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gzhubu.top/gtnxpterme.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtmfyhxhyx.html

[C02] 默认参数
来源：http://hz.tanke756.top/gtruyptzht.html

Py:   def greet(name="World"): return name
来源：http://hz.fzhhl.top/gtzsvwfdeq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sxryk.cn/gtebneucly.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtuaayrpbi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenzaomai.com/gtxkipvozq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.chenjidiqi.icu/gtjtljtmkv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jianghu66.top/gthuyttbxg.html

Ruby: def greet(name = "World") = name
来源：http://hz.shzxlz.cn/gtywjmppvt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.wangdashe.top/gtnfpwujtb.html

[C03] 可变参数
来源：http://hz.ppjwa.cn/gtnqofyvao.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhiwuduotai.top/gtfuflsepb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hysaishi.cn/gtqrvmnoxa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtdpririyn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ppjwa.cn/gtdtsndxro.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhengqikj.top/gtjdegyybi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigfzy.top/gtangznjkj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.andypj.xyz/gtwezlslvb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gtfokafbwh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuanzhike.top/gtrediehbg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guowangkeji.top/gtpgxvrlac.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zycfv.cn/gtjoyijxjx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ybcxt.top/gtuchdvkow.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhongyouzk.top/gtffhcqeus.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenzaomai.com/gtoovnylqp.html

Go:   // 无：用配置结构体参数
来源：http://hz.ehwqpu.com/gtdsvfyjap.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtjegrlsen.html

C#:   f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gtvmdwsscb.html

[C05] 返回多个值
来源：http://hz.0kj1m.cn/gtfvyspoum.html

Py:   return a, b
来源：http://hz.pengpengdd.cyou/gtiuvnjntd.html

PHP:  return [$a, $b];
来源：http://hz.sweek.top/gtngcbunfu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ehwqpu.com/gtfdrvglra.html

TS:   return { a, b };
来源：http://hz.yanxiufei.cn/gtlkjgnsai.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hysaishi.cn/gtrjseewaa.html

Go:   return a, b
来源：http://hz.zhiwuduotai.top/gtfntryred.html

Ruby: return a, b
来源：http://hz.snrcjt.cn/gtsxuydche.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.shanyushiyangkeji.top/gtjusjgzrz.html

[C06] 匿名函数 / lambda
来源：http://hz.jianghu66.top/gtjmanttub.html

Py:   square = lambda x: x * x
来源：http://hz.andypj.xyz/gtcbyqcmpr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yangfankeji.com/gtqdiiwxfw.html

JS:   const square = x => x * x;
来源：http://hz.pycfn.com/gticmzhxyo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sxryk.cn/gtdltugsys.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangtech.top/gtznbbcfob.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.haohaochexian.top/gtddrijjow.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gotoacloud.top/gtstdrcuiy.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtgxqhqjpn.html

[C07] 把函数作为参数传入
来源：http://hz.shuidangran.top/gtwqxcagxd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yueranfly.top/gtxaxbfttw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hnqzz.top/gtgbxqctzu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.chenzaomai.com/gtcbsxtmnl.html

TS:   arr.map(String)
来源：http://hz.ivvv.top/gtgtwotrxm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jiagoushi.top/gtbsuudtws.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yj20258.top/gtomzyujcw.html

Ruby: arr.map(&:upcase)
来源：http://hz.52xcode.cn/gtiirniiku.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gtpqdtyazo.html

[C08] 闭包
来源：http://hz.svipenyu.cn/gtxrdrhdna.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydzc1.top/gtnisfjigp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.316326.xyz/gtpknemeuo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtwgcttdsh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtagltpuux.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.svipenyu.cn/gtyatzgcuj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.smart0.xyz/gtqfirxiwb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtskmsaoru.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtkytetajw.html

[C09] 递归
来源：http://hz.xylfe.cn/gtgcdsscof.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yangfankeji.com/gtuchppona.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yuxming.cn/gthxyevksl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.cdnleiting.top/gtjqdrktjj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shanyushiyangkeji.top/gtcteoazfj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cqqwz.cn/gtkrcapuxq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zdqjudy.top/gtrmqxerai.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fengsongda.top/gtephnojsl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.haohaochexian.top/gtiwxxpzqi.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gtjirjpfms.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgfzy.top/gtpwrtraam.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhoulong.xyz/gtsshxtleq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zdqjudy.top/gtdqxkvtri.html


<!-- 参考信息 -->