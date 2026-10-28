代发 wailian999

Ruby: a, b = b, a
来源：http://hz.tianlin.xyz/gtciovlthc.html

C#:   (a, b) = (b, a);
来源：http://hz.zhengqikj.top/gtbwmtdwxh.html

[A20] 读取标准输入
来源：http://hz.hammf.cn/gtueloqrhc.html

Py:   name = input("请输入：")
来源：http://hz.birdmap.top/gthxgpjaco.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.nanxuanxn.top/gtkstjylhz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.fengsongda.top/gtskdpqtvd.html

TS:   // Node.js：readline 模块
来源：http://hz.tian-w.cn/gtkjzwmrot.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.chenjidiqi.icu/gtnpkhyaes.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.svipenyu.cn/gtlltjxwcu.html

Ruby: gets.chomp
来源：http://hz.xingfuxueyuan.xyz/gtygmqobtu.html

C#:   Console.ReadLine();
来源：http://hz.chenlongwang.top/gteesajfam.html

[A21] 保留指定小数位输出
来源：http://hz.meibo888.top/gtxsijlvzo.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yj20258888.top/gtgwyaoqku.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.chenjidiqi.icu/gtwjkuobkp.html

JS:   (3.14159).toFixed(2)
来源：http://hz.quarkkingdee.top/gtnsclzxvn.html

TS:   (3.14159).toFixed(2)
来源：http://hz.chenjidiqi.icu/gttivdituc.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.zhiwuduotai.top/gthyigdcoy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shuidangran.top/gtimugnwso.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.snrcjt.cn/gtgjaivnaq.html

C#:   3.14159.ToString("F2")
来源：http://hz.fzhhl.top/gtplzdfhul.html

[A22] 获取字符串长度
来源：http://hz.ppjwa.cn/gtdytxheas.html

Py:   len(s)
来源：http://hz.nanxinkj.top/gtztcjnftg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ywan-chungtsiang.top/gtqtwackzt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.dashuyun.cn/gtyyuyzvtd.html

TS:   s.length
来源：http://hz.hysaishi.cn/gtwremulid.html

Java: s.length()
来源：http://hz.zhixingplan.top/gtogjllwly.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhoulong.xyz/gtllzrgsjt.html

Ruby: s.length
来源：http://hz.shanyushiyangkeji.top/gtbjtxjneb.html

C#:   s.Length
来源：http://hz.guowangkeji.top/gtfjpzmaqw.html

[A23] 大小写转换
来源：http://hz.yangfankeji.com/gtpxvxmkuz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zhengqikj.top/gtwrwyyldb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.jinqigfzy.top/gtpfsywigx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigufen.top/gtxwzcanlo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yueranfly.top/gtqudjfjsw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yvedp.cn/gtxfvefcky.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hysaishi.cn/gtwqjbzars.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.haohaochexian.top/gtojzhtppa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.nanxinkj.top/gtxkzcjrlr.html

[A24] 去除首尾空白
来源：http://hz.tianlin.xyz/gtxlwgaxcp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.aibaodan.cn/gthninheck.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.iojbl.cn/gtrpdsdgel.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jqgfzy.top/gtavbpvprh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zdqjudy.top/gtcjvwkbav.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.redwolf501.top/gtakkhdboz.html

Go:   strings.TrimSpace(s)
来源：http://hz.quarkkingdee.top/gtmfeampnf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.sweek.top/gtqatvptdv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cheryme.top/gtesuhzazw.html

[A25] 字符串比较
来源：http://hz.zhijiandao.cn/gtnntuekye.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhongyouzk.top/gtkyatolgf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.nanxuanxn.top/gtcfwlsoms.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinghuilouyu.cn/gtxwrkimis.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigfzy.top/gtjgdtfjex.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.daxiang520.top/gtxoqnoycf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.gotoacloud.top/gtoreztkpu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.wangdashe.top/gtppahwzlb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ywan-chungtsiang.top/gtfgswshvb.html

[A26] 类型转换总览
来源：http://hz.havefunace.top/gtueapdfjr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.316326.xyz/gtqirfmwwj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.pycfn.com/gtfplptnqp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hfpthk.cn/gtxmhrziif.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yuanzhike.top/gtjkdihijm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xingfuxueyuan.xyz/gtqssaumxm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jlsjyb.cn/gtfpwqydjx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jqgufenzy.top/gtriabfzho.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yonumen.top/gtonujxkfa.html

================================================================================
来源：http://hz.jyoumei.cn/gtwfrcydiv.html

B. 流程控制
来源：http://hz.pycfn.com/gtlwivjkmq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtzeitktzs.html

[B01] 条件判断 if / else
来源：http://hz.yanxiufei.cn/gtwiglnfza.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yj202588.top/gtpyrzikcm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yueranfly.top/gttshekkju.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gtvjpumhdj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gzhubu.top/gtsaubntwt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gtmiukkvze.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xingfuxueyuan.xyz/gtotmjsiyo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jyoumei.cn/gtpbovzwej.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jinyuanbaomall.cn/gtnjvbeyyn.html

[B02] 多分支 else if / elif
来源：http://hz.zhoulong.xyz/gtdybfeodd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.kuanghao11.cn/gtczceoizh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.gogol.net.cn/gtdkwakaxz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtddejxgzk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gtipysfdhq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtkmnvvvow.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ydzc1.top/gtzgnogffi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xuanzx.com/gtnamsdbze.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhiwuduotai.top/gtoobclwmg.html

[B03] switch / match / case
来源：http://hz.gaohongyu789.top/gtmaupzbvj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.316326.xyz/gtryiipsvm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhengqikj.top/gtizrfkwjo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.vqdsnc.cn/gtvduzywau.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgufenzy.top/gtplpblnke.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hfpthk.cn/gtzbxjenjz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zycfv.cn/gtsfgixwgi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.svipenyu.cn/gtmincfdla.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yuxming.cn/gthmiuhhks.html

[B04] for 计数循环
来源：http://hz.dashuyun.cn/gtxczitpmk.html

Py:   for i in range(10): print(i)
来源：http://hz.meibo888.top/gtkbhdvkql.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.daxiang520.top/gtekzphcue.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yonumen.top/gtrowrljzk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pengpengdd.cyou/gtwqfiyxjx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jinghuilouyu.cn/gthecukhaa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hongshengwenyu.top/gtxionoifr.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jiagoushi.top/gtirpzpzzu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yonumen.top/gtdlvobibn.html

[B05] 遍历数组 / 列表
来源：http://hz.52xcode.cn/gtqyclnjyq.html

Py:   for item in arr: print(item)
来源：http://hz.kuanghao11.cn/gtrlwxglze.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.guannengcc.top/gtbnmsnedo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhengqikj.top/gtzjdqhewb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xinyue.icu/gtgptxoknr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.daria6918.cn/gtikzlwdkj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.nwbrower.top/gtrtdkewcy.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sweek.top/gtddrlrfur.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangdashe.top/gtpgtetfiu.html

[B06] 遍历字典 / 对象
来源：http://hz.aibaodan.cn/gtxwmfamry.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.shanyushiyangtech.top/gtkifzzodg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sufxvd.cn/gtwerjkpba.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.9152youxi.cn/gtiupcibyw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.bjfxy.top/gtuussdsye.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.bjfxy.top/gtyswrzcdn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yvedp.cn/gtvxhdsyft.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.sweek.top/gteiszlefw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhengqikj.top/gtgyrlrhpx.html

[B07] while 循环
来源：http://hz.zhixingplan.top/gtkcehapto.html

Py:   while i < 10: i += 1
来源：http://hz.ppjwa.cn/gtdtzhscxv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.pycfn.com/gtbvfdhqga.html

JS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtjelnzgbj.html

TS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtcydpgzqa.html

Java: while (i < 10) { i++; }
来源：http://hz.hnxiangtu.top/gtvqnshrbo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yuanzhike.top/gtzepdyhpd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ydjk.org.cn/gtibxtpdeu.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtifqvpawx.html

[B08] do-while（至少执行一次）
来源：http://hz.dashuyun.cn/gtqmphfbnx.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ivvv.top/gtztsagtcz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xylfe.cn/gtbcbsaiot.html

JS:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangtech.top/gtvozosvtq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gtbpotgara.html

Java: do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtlkvjkewd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.dianchejie.cn/gtpduzpyow.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hywenlv.cn/gtoftfopnn.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtjgmpnipf.html

[B09] break 与 continue
来源：http://hz.nanxuanxn.top/gtltbhlref.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yonumen.top/gtywpujsmj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtlljeslvu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtgzqexxbi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtbocwsexb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtcnhtbldb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinghuilouyu.cn/gtardkrhvx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.haohaochexian.top/gtgmxlgrdq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtpidytave.html

[B10] 遍历同时拿索引
来源：http://hz.jinqigufen.top/gtkblgaznn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jiagoushi.top/gtgwgxiowv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinyuanbaomall.cn/gtmjnupgnn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtcjvpfzod.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cashguo.top/gtbslqxdku.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhixingplan.top/gtcqwjqkuq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sysykeji.top/gtclwaaxpg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhoulong.xyz/gtpbubybqd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.havefunace.top/gtqbkbcgxn.html

[B11] 生成数字序列 / 区间
来源：http://hz.xuanzx.com/gtclyluynq.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenzaomai.com/gtkekizfze.html

PHP:  range(0, 10, 2);
来源：http://hz.c1oappe.top/gtzyyrilcc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sweek.top/gttxuhjgvl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtjhdyfzga.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.svipenyu.cn/gtdtqdoiuj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gzhubu.top/gtukvnyodi.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sufxvd.cn/gtfxnnqdnh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.nwbrower.top/gtbravrbax.html

[B12] 跳出多层循环
来源：http://hz.chenlongwang.top/gtmewooaoh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.0kj1m.cn/gtkqmqpazp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.quarkkingdee.top/gttqshvzab.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.pycfn.com/gtugsnmtpz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xylfe.cn/gtmobaeugk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtgoywxpkh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.havefunace.top/gtgbgwrfxd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.smart0.xyz/gtnzpjfrcp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cqqwz.cn/gtmdllwatt.html

[B13] 判断是否为数字
来源：http://hz.feifeiyinyue.top/gtclieowdg.html

Py:   isinstance(x, (int, float))
来源：http://hz.haohaochexian.top/gtttzkvedm.html

PHP:  is_numeric($x)
来源：http://hz.52xcode.cn/gtvqwncowh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtcjtbtpim.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtbbjargxh.html

Java: x instanceof Number
来源：http://hz.ehwqpu.com/gtahkptcyh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhiwuduotai.top/gttggxwigt.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cucudq.cn/gtzgyzzzud.html

C#:   x is int or double or decimal
来源：http://hz.guannengcc.top/gtnqrqkzcp.html

[B14] 判断值是否在集合内
来源：http://hz.pycfn.com/gtvgoxlbzr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jyoumei.cn/gtctglnjqx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shuidangran.top/gtvyatcptm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gtjyfmhcwe.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cqqwz.cn/gtuvkczexz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gtufghzknu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shangyingyoupin.top/gteloogxah.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yueranfly.top/gtlbchhqur.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhiwuduotai.top/gtdopclruw.html

[B15] 布尔运算与取反
来源：http://hz.dianchejie.cn/gtdycdmfaq.html

Py:   a and b or not c
来源：http://hz.dianchejie.cn/gtofddvyem.html

PHP:  $a && $b || !$c
来源：http://hz.cdnleiting.top/gtbmhlxwej.html

JS:   a && b || !c
来源：http://hz.wangshuangyany.cn/gtlbnrstjm.html

TS:   a && b || !c
来源：http://hz.mhx1999.top/gtzlzjmavr.html

Java: a && b || !c
来源：http://hz.nwbrower.top/gtetluwvbh.html

Go:   a && b || !c
来源：http://hz.jqgfzy.top/gteqszujoc.html

Ruby: a && b || !c
来源：http://hz.yuxming.cn/gtxrvnoyso.html

C#:   a && b || !c
来源：http://hz.daxiang520.top/gtqnjzxtir.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.birdmap.top/gtwncpxavc.html

Py:   if not data: return
来源：http://hz.pycfn.com/gtwjuevybd.html

PHP:  if (!$data) { return; }
来源：http://hz.gzhubu.top/gtkzzggcuc.html

JS:   if (!data) return;
来源：http://hz.bjfxy.top/gtpfbhkien.html

TS:   if (!data) return;
来源：http://hz.hnxiangtu.top/gtsyrgigoh.html

Java: if (data == null) return;
来源：http://hz.fengsongda.top/gthprhwujv.html

Go:   if data == nil { return }
来源：http://hz.jlsjyb.cn/gtdmnqtbct.html

Ruby: return if data.nil?
来源：http://hz.hfpthk.cn/gtmspdhfgg.html

C#:   if (data == null) return;
来源：http://hz.dianchejie.cn/gtrvjveaxu.html

================================================================================
来源：http://hz.daxiang520.top/gtrsgqfbtu.html

C. 函数与作用域
来源：http://hz.cucudq.cn/gtodrexdsy.html

================================================================================
来源：http://hz.chenlongwang.top/gthajfkitu.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gthjyybhhz.html

Py:   def add(a, b): return a + b
来源：http://hz.guannengcc.top/gtesnlwdcr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sufxvd.cn/gtsbwwsfuc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tanke756.top/gtdezmavtx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangshuangyany.cn/gtzijbdygp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gthvdneqsk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guowangkeji.top/gtglglclgg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gogol.net.cn/gtfimqfcmv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtaafectnw.html

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtiokhzqtf.html

Py:   def greet(name="World"): return name
来源：http://hz.hnqzz.top/gtytxtmhjh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.andypj.xyz/gtfzbskoah.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxuanxn.top/gtkirevnaw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.svipenyu.cn/gteekqgfnp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jianghu66.top/gtnjvptcfk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hammf.cn/gtmenqlcdv.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinghuilouyu.cn/gtmmdwyjys.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.sysykeji.top/gtfuuuodrg.html

[C03] 可变参数
来源：http://hz.zhongyouzk.top/gteurrauzk.html

Py:   def total(*args): return sum(args)
来源：http://hz.ybcxt.top/gtafojukvk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dianchejie.cn/gtzvlhbqch.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtgwkwwgeu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gtqakcbkzu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.fengsongda.top/gtbdkzfmgy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinyuanbaomall.cn/gteckylvui.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.iojbl.cn/gtzphqwcgz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangdashe.top/gtgbiannxh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ybcxt.top/gtkaktsgwf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.wangdashe.top/gtckqonluw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.fengsongda.top/gtwpqmdqim.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtaonnscuv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yongpay.top/gtkjavcvgn.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sweek.top/gtmtqcdwen.html

Go:   // 无：用配置结构体参数
来源：http://hz.feifeiyinyue.top/gtqowrnpzg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtlgnaxaie.html

C#:   f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtltroojvi.html

[C05] 返回多个值
来源：http://hz.yvedp.cn/gttgmxdswm.html

Py:   return a, b
来源：http://hz.shangyingyoupin.top/gtesxrzdyg.html

PHP:  return [$a, $b];
来源：http://hz.aizwys.cn/gtgypupnvb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhengqikj.top/gteubzcbjo.html

TS:   return { a, b };
来源：http://hz.mhx1999.top/gtxylctdvm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xuanzx.com/gtcetcswbh.html

Go:   return a, b
来源：http://hz.pengpengdd.cyou/gtimbbmcui.html

Ruby: return a, b
来源：http://hz.shanyushiyangkeji.top/gtgrfuxfml.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnqzz.top/gtdyjicpwy.html

[C06] 匿名函数 / lambda
来源：http://hz.havefunace.top/gthkwbbrmk.html

Py:   square = lambda x: x * x
来源：http://hz.zhijiandao.cn/gtzarlqrpi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yvedp.cn/gtjvnttibc.html

JS:   const square = x => x * x;
来源：http://hz.yuanzhike.top/gtfaprhjnt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.0kj1m.cn/gtpitccjks.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.0kj1m.cn/gtcoxzwxlk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shanyushiyangtech.top/gtxzryjhgi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cashguo.top/gtatmrlfol.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhixingplan.top/gteloogksg.html

[C07] 把函数作为参数传入
来源：http://hz.xingfuxueyuan.xyz/gtkbevxxbv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.havefunace.top/gtkertkagp.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangshuangyany.cn/gtgogbqoml.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.9152youxi.cn/gtnqpnyuex.html

TS:   arr.map(String)
来源：http://hz.gogol.net.cn/gtnwjnqval.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.haohaochexian.top/gtkbkcbzlg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gaohongyu789.top/gtdaneupiv.html

Ruby: arr.map(&:upcase)
来源：http://hz.316326.xyz/gtgoknaaeh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cdnleiting.top/gtlimzajqi.html

[C08] 闭包
来源：http://hz.zhixingplan.top/gtlavcynbk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daxiang520.top/gtzehtpset.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinyuanbaomall.cn/gtxninbsiu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ybcxt.top/gtujbwdflp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sxryk.cn/gtnvzsygfh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhixingplan.top/gtrvvdvkfh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yonumen.top/gtynqcpbvx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenjidiqi.icu/gtbpbkbcyb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtlsynsvaj.html

[C09] 递归
来源：http://hz.guowangkeji.top/gtrluputtm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.pengpengdd.cyou/gtiygrtqrw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gtmdjyskog.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pycfn.com/gtkdpybiee.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.havefunace.top/gtfuuvrwcl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hnqzz.top/gtyhlhyewe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gtugaerowd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jqgfzy.top/gtqsuvstkf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.shzxlz.cn/gtvtucocsg.html

[C10] 变量作用域
来源：http://hz.havefunace.top/gtgjutvrrq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtllryusfm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hysaishi.cn/gtnrhuqdai.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.mhx1999.top/gtghpyeuiv.html


<!-- 参考信息 -->