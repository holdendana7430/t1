代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daria6918.cn/gtfdhhamku.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhiwuduotai.top/gtigauvmgd.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zycfv.cn/gtbyetkxzw.html

Ruby: "A".ord; 65.chr
来源：http://hz.guannengcc.top/gtxvasaxjn.html

C#:   (int)'A'; (char)65
来源：http://hz.nwbrower.top/gtugzdoxvt.html

[A19] 交换两个变量
来源：http://hz.9152youxi.cn/gtrxknsoeu.html

Py:   a, b = b, a
来源：http://hz.316326.xyz/gtwghrprrr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jqgufenzy.top/gtthskexzx.html

JS:   [a, b] = [b, a];
来源：http://hz.snrcjt.cn/gtardggjid.html

TS:   [a, b] = [b, a];
来源：http://hz.daxiang520.top/gtdneyzvkw.html

Java: int t = a; a = b; b = t;
来源：http://hz.xinyue.icu/gtkunbmlwp.html

Go:   a, b = b, a
来源：http://hz.sxryk.cn/gtakfedleo.html

Ruby: a, b = b, a
来源：http://hz.jinqigufen.top/gtvoelrsfw.html

C#:   (a, b) = (b, a);
来源：http://hz.ybcxt.top/gtqqesmsxn.html

[A20] 读取标准输入
来源：http://hz.hywenlv.cn/gtaewqvbdy.html

Py:   name = input("请输入：")
来源：http://hz.zdqjudy.top/gtwwafgghu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.svipenyu.cn/gtuqxukxrj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.gogol.net.cn/gtsodsbqwq.html

TS:   // Node.js：readline 模块
来源：http://hz.ybcxt.top/gtdsgaugld.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.daxiang520.top/gtigqhmxyj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.haohaochexian.top/gtrhcuuzrr.html

Ruby: gets.chomp
来源：http://hz.jyoumei.cn/gtpvpbecqj.html

C#:   Console.ReadLine();
来源：http://hz.yj20258888.top/gtzzbdxdmc.html

[A21] 保留指定小数位输出
来源：http://hz.zhixingplan.top/gtmtuesupk.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hnqzz.top/gtutrzeuoy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.mhx1999.top/gtzvrbnqmb.html

JS:   (3.14159).toFixed(2)
来源：http://hz.9152youxi.cn/gtmtlxjnjc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.nwbrower.top/gtpghxqiue.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yanxiufei.cn/gtoixhfivo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.zhixingplan.top/gtlmnyazvh.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.daria6918.cn/gtwyrwwhed.html

C#:   3.14159.ToString("F2")
来源：http://hz.guannengcc.top/gtxabexxqs.html

[A22] 获取字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtoqvrfqji.html

Py:   len(s)
来源：http://hz.daria6918.cn/gtytwnygpp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.dashuyun.cn/gtwxjizbci.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.svipenyu.cn/gtvtdllrbq.html

TS:   s.length
来源：http://hz.xingfuxueyuan.xyz/gtxhdneztm.html

Java: s.length()
来源：http://hz.pycfn.com/gtyhpdqbck.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.sufxvd.cn/gtwwbqncxs.html

Ruby: s.length
来源：http://hz.gotoacloud.top/gtddfaanim.html

C#:   s.Length
来源：http://hz.0kj1m.cn/gtsuikemzr.html

[A23] 大小写转换
来源：http://hz.jqgufenzy.top/gtxluuypzi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.sysykeji.top/gttcpdsdar.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cucudq.cn/gtcxbuxagk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.wangdashe.top/gtrusjftvn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.snrcjt.cn/gtjbhjwybo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.cashguo.top/gtqiweuuko.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zhongyouzk.top/gtsvjaoezo.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhengqikj.top/gttpxtbpai.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.chenjidiqi.icu/gtjyerpunj.html

[A24] 去除首尾空白
来源：http://hz.guowangkeji.top/gtflycpkzh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.guowangkeji.top/gtaabsxrvt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zdqjudy.top/gtffkvrnka.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.fengsongda.top/gtlvwmvygu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yanxiufei.cn/gtrudyrhhf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ivvv.top/gtzookpdid.html

Go:   strings.TrimSpace(s)
来源：http://hz.xingfuxueyuan.xyz/gtribninbn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.fzhhl.top/gtypocpkid.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.kuanghao11.cn/gthsruufto.html

[A25] 字符串比较
来源：http://hz.smart0.xyz/gtxodacvez.html

Py:   s1 == s2; s1 != s2
来源：http://hz.guannengcc.top/gtbfqvkbyo.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yj20258888.top/gtxvubunjr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.kuanghao11.cn/gthjjwhxrz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nanxinkj.top/gtxyxfqaxt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.guowangkeji.top/gtsdlhytfh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.wangdashe.top/gtbaggzxru.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yj20258.top/gtfbqasdop.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xylfe.cn/gtecepkobz.html

[A26] 类型转换总览
来源：http://hz.sysykeji.top/gtdusurfzg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.tian-w.cn/gttbyanfzz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jlsjyb.cn/gtdbnxucdi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sweek.top/gtjtetfgwv.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jinqigufen.top/gtixynsixb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.sweek.top/gtdxdhwbkj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.smart0.xyz/gtfpvygvin.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.gaohongyu789.top/gtmhgzweuv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.aizwys.cn/gttxiohtsr.html

================================================================================
来源：http://hz.zhengqikj.top/gtxzdjgwck.html

B. 流程控制
来源：http://hz.yuanzhike.top/gtmfbxzott.html

================================================================================
来源：http://hz.jqgfzy.top/gtbhwuejhn.html

[B01] 条件判断 if / else
来源：http://hz.bjfxy.top/gtjwjgdqjr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.dashuyun.cn/gtkofwjsxz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gogol.net.cn/gtdjidcswr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtjwuugttm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yueranfly.top/gttjciiilh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtlczpuuvo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.chenjidiqi.icu/gtuxetskbi.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhijiandao.cn/gtzeqaasma.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.tanke756.top/gtivjlufvs.html

[B02] 多分支 else if / elif
来源：http://hz.gaohongyu789.top/gtvopcwiwf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.svipenyu.cn/gtehxbunpc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhixingplan.top/gtgiskcilr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtblgtdgnx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtgrmwhwir.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangshuangyany.cn/gtajuyxtxa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xylfe.cn/gtydkfstcn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.chenjidiqi.icu/gtgxalllxy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtcizjvnrb.html

[B03] switch / match / case
来源：http://hz.shangyingyoupin.top/gtlasdanfs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jyoumei.cn/gtayuksale.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ppjwa.cn/gtrnihtten.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cheryme.top/gtiwawvnuz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aibaodan.cn/gtwormkmjq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.tanke756.top/gtjtpgedfe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yangfankeji.com/gtcrxljwkf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhijiandao.cn/gtrvupgksk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.chenjidiqi.icu/gtupgsiuml.html

[B04] for 计数循环
来源：http://hz.ydjk.org.cn/gtedbzpypf.html

Py:   for i in range(10): print(i)
来源：http://hz.xuanzx.com/gtpxiljerh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jqgufenzy.top/gtdahvvajl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.daxiang520.top/gtattqsdnv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.quarkkingdee.top/gtcpajdjjz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.nwbrower.top/gthjsilxhb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhijiandao.cn/gtchezodvu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shanyushiyangtech.top/gthjznzpfl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhijiandao.cn/gtyeyomsei.html

[B05] 遍历数组 / 列表
来源：http://hz.hfpthk.cn/gtoilloxvr.html

Py:   for item in arr: print(item)
来源：http://hz.sufxvd.cn/gtfzkzgeot.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yj20258.top/gtndgbpmoa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.guannengcc.top/gttuakbesg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xingfuxueyuan.xyz/gtbttzyzjv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sxryk.cn/gtqqulahcq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cdnleiting.top/gtsdgtvebo.html

Ruby: arr.each { |item| puts item }
来源：http://hz.andypj.xyz/gtubuxzrvg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.nanxuanxn.top/gtiivgeyfx.html

[B06] 遍历字典 / 对象
来源：http://hz.chenjidiqi.icu/gtjftahsfu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.birdmap.top/gtfjqrfnyf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yuxming.cn/gtyripmvbc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sysykeji.top/gtayoqauzf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.mhx1999.top/gtopdpjbcy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hammf.cn/gttldhtvpr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ywan-chungtsiang.top/gtvcmigsog.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.sufxvd.cn/gthaqwxrrf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shuidangran.top/gtgmighacq.html

[B07] while 循环
来源：http://hz.jiagoushi.top/gtjlfjrzvk.html

Py:   while i < 10: i += 1
来源：http://hz.yj20258888.top/gtfyuzjded.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cucudq.cn/gtnjreynfn.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gtlqkjhzek.html

TS:   while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtawjrcoqb.html

Java: while (i < 10) { i++; }
来源：http://hz.xuanzx.com/gturblrgpb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.haohaochexian.top/gttflpukts.html

Ruby: while i < 10; i += 1; end
来源：http://hz.snrcjt.cn/gtrorbzlth.html

C#:   while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gthfbxaxuc.html

[B08] do-while（至少执行一次）
来源：http://hz.yuanzhike.top/gtxbnufvbl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yueranfly.top/gtaalhuukk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xingfuxueyuan.xyz/gtaruiovmp.html

JS:   do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtqwtyrvdm.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtuddhjmxf.html

Java: do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtwplinwgu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jyoumei.cn/gtucqpuiff.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.svipenyu.cn/gtzhxddehx.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aizwys.cn/gtpemofsic.html

[B09] break 与 continue
来源：http://hz.pycfn.com/gtafyayrvu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jlsjyb.cn/gtikafipaq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtbvhrwidw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtmjmsxxwq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sweek.top/gtyrmtmwmk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gthhzvbvtl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.dianchejie.cn/gtoccsejul.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shanyushiyangkeji.top/gtpqytnwjz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnqzz.top/gtdoxnzoqr.html

[B10] 遍历同时拿索引
来源：http://hz.hysaishi.cn/gtenegbclo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.svipenyu.cn/gtmrxiymzy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.smart0.xyz/gtinhwwjhh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtehgnaiyu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.redwolf501.top/gtiaqksheu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yongpay.top/gteaglcorm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ivvv.top/gtadqazeoj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guowangkeji.top/gttykdahqw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.c1oappe.top/gteyuseazv.html

[B11] 生成数字序列 / 区间
来源：http://hz.xingfuxueyuan.xyz/gtauahoxxu.html

Py:   list(range(0, 10, 2))
来源：http://hz.jyoumei.cn/gteswsvgpa.html

PHP:  range(0, 10, 2);
来源：http://hz.zhaomingkeji.xyz/gtyyiarcdo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.aizwys.cn/gtbwktborp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtqjxvcejr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xinyue.icu/gtcqkiqydb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yonumen.top/gtnoveqmch.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yangfankeji.com/gtpmbsuewa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenlongwang.top/gtxusprspc.html

[B12] 跳出多层循环
来源：http://hz.fengsongda.top/gtuuoykokn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cqqwz.cn/gtamxjbqzm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shuidangran.top/gtvugeicih.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtyujlyyhf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtnhvqoixf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhaomingkeji.xyz/gtbhosyabr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jyoumei.cn/gtaayttwap.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hammf.cn/gtqkfzbbtb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yj202588.top/gtiylweelt.html

[B13] 判断是否为数字
来源：http://hz.zdqjudy.top/gtmlmqtpgi.html

Py:   isinstance(x, (int, float))
来源：http://hz.shanyushiyangtech.top/gteovepjde.html

PHP:  is_numeric($x)
来源：http://hz.mhx1999.top/gtklprikbf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtbyhfqykt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ywan-chungtsiang.top/gtytchdjpe.html

Java: x instanceof Number
来源：http://hz.meibo888.top/gtbcpejycc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shanyushiyangkeji.top/gtrqeacxrd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuxming.cn/gtqbhrbrjz.html

C#:   x is int or double or decimal
来源：http://hz.hammf.cn/gthsmvqhna.html

[B14] 判断值是否在集合内
来源：http://hz.ydjk.org.cn/gtwoxoezll.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.bjfxy.top/gtutxfhano.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.feifeiyinyue.top/gtlepbvnvu.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jlsjyb.cn/gtvagevsth.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zycfv.cn/gtybtoufhx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hammf.cn/gtgfqezfky.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hongshengwenyu.top/gtzgdanhrb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.meibo888.top/gtyjhccqyn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.quarkkingdee.top/gtyzwqlhup.html

[B15] 布尔运算与取反
来源：http://hz.pengpengdd.cyou/gtyuomnnvs.html

Py:   a and b or not c
来源：http://hz.shzxlz.cn/gtuxestbpc.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258.top/gthluytswm.html

JS:   a && b || !c
来源：http://hz.zycfv.cn/gtxtgdylvd.html

TS:   a && b || !c
来源：http://hz.xylfe.cn/gtrnplsioe.html

Java: a && b || !c
来源：http://hz.shzxlz.cn/gtlnjyxxpf.html

Go:   a && b || !c
来源：http://hz.yuxming.cn/gtpfxmeogq.html

Ruby: a && b || !c
来源：http://hz.9152youxi.cn/gtsuyetyvn.html

C#:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtxvaujnje.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.pycfn.com/gtyfugwxgt.html

Py:   if not data: return
来源：http://hz.fengsongda.top/gtolfqccwl.html

PHP:  if (!$data) { return; }
来源：http://hz.ywan-chungtsiang.top/gtecwqbqmr.html

JS:   if (!data) return;
来源：http://hz.ivvv.top/gtlrtkuzam.html

TS:   if (!data) return;
来源：http://hz.hfpthk.cn/gtwngylkih.html

Java: if (data == null) return;
来源：http://hz.gaohongyu789.top/gtbnovixwe.html

Go:   if data == nil { return }
来源：http://hz.yvedp.cn/gteiqctmox.html

Ruby: return if data.nil?
来源：http://hz.gogol.net.cn/gtaowayimw.html

C#:   if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtrjwupncj.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmnxogaul.html

C. 函数与作用域
来源：http://hz.cqqwz.cn/gtgqzktexu.html

================================================================================
来源：http://hz.smart0.xyz/gtnrcmvaql.html

[C01] 定义函数
来源：http://hz.chenzaomai.com/gteqdvltlu.html

Py:   def add(a, b): return a + b
来源：http://hz.316326.xyz/gtnfgktdcs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pycfn.com/gtxptzadfl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtvurbzcnc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtccdxgtct.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gtzejuivfy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sxryk.cn/gtzcejomgu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hysaishi.cn/gtczydsjia.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtpffsxcnx.html

[C02] 默认参数
来源：http://hz.guannengcc.top/gtihoyjaem.html

Py:   def greet(name="World"): return name
来源：http://hz.quarkkingdee.top/gtwdljncmk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sufxvd.cn/gtzcnduspz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jlsjyb.cn/gtnjroyfkc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cdnleiting.top/gthfpyacuc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhijiandao.cn/gtyrtlhydg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jlsjyb.cn/gtxccgxdqv.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinghuilouyu.cn/gtmbhqniow.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hysaishi.cn/gtfgdoasyw.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtfckqzxda.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhengqikj.top/gtginebvck.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xinyue.icu/gtyxaskhfg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtkqesztvx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtkpylncjh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ivvv.top/gtcxssgvue.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yvedp.cn/gtgxiujbbz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yvedp.cn/gttwkpxeer.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cheryme.top/gtfmgqirvg.html

[C04] 命名参数 / 关键字参数
来源：http://hz.havefunace.top/gtrlebzdyq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daxiang520.top/gtfvcmhyxd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gtsgngpoqq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtyaejkkcj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yonumen.top/gtabuopxwx.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daria6918.cn/gtwaymmbgq.html

Go:   // 无：用配置结构体参数
来源：http://hz.jiagoushi.top/gtyyhjaoyy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtvstjbmag.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtrnttfwdi.html

[C05] 返回多个值
来源：http://hz.pengpengdd.cyou/gtuuepyvse.html

Py:   return a, b
来源：http://hz.yonumen.top/gtejmhfuoa.html

PHP:  return [$a, $b];
来源：http://hz.jlsjyb.cn/gthprlqlry.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xuanzx.com/gtzhtkqseh.html

TS:   return { a, b };
来源：http://hz.wangdashe.top/gtsvvwjczq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ehwqpu.com/gtgugzejmc.html

Go:   return a, b
来源：http://hz.ydjk.org.cn/gtmuvzsdpj.html

Ruby: return a, b
来源：http://hz.pycfn.com/gtioxfnatm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hywenlv.cn/gtifpcqkrx.html

[C06] 匿名函数 / lambda
来源：http://hz.birdmap.top/gtvgdwpakh.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258888.top/gtxejsuphq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenzaomai.com/gtugwuvdkv.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangkeji.top/gtavtxhmvi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jqgufenzy.top/gtgnbjcwrr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.chenzaomai.com/gtjqvktait.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tanke756.top/gteuqssvke.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gogol.net.cn/gtnadmnktw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinyuanbaomall.cn/gtupacwkmk.html

[C07] 把函数作为参数传入
来源：http://hz.c1oappe.top/gtypcmalza.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.jinyuanbaomall.cn/gtgkpbnfgl.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yuxming.cn/gtxebjkozt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.birdmap.top/gtkcvvybhv.html

TS:   arr.map(String)
来源：http://hz.smart0.xyz/gtcbzrnuwk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.sweek.top/gtuclzdqum.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.xziqi.cn/gtgcmnbext.html

Ruby: arr.map(&:upcase)
来源：http://hz.aizwys.cn/gticzwmqbf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnqzz.top/gtrzdorvph.html

[C08] 闭包
来源：http://hz.wangshuangyany.cn/gtjjcughpk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jlsjyb.cn/gtqfxoqvup.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj202588.top/gtqsnhwoqv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtfbrixnar.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtogwfedtg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuanzx.com/gtkohujoaj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtlzasqngd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenlongwang.top/gtarhxfksg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gteqjkcmee.html

[C09] 递归
来源：http://hz.aibaodan.cn/gthfebkwpb.html


<!-- 参考信息 -->