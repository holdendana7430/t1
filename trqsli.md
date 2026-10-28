代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.guowangkeji.top/gtujjgcubs.html

Py:   ord("A"); chr(65)
来源：http://hz.jinqigufen.top/gtnaicyliz.html

PHP:  ord("A"); chr(65)
来源：http://hz.ybcxt.top/gttfhwunbb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.haohaochexian.top/gtwmgdpelf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shzxlz.cn/gtyaznwrjd.html

Java: (int) 'A'; (char) 65
来源：http://hz.chenzaomai.com/gtzltxlvtz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jinghuilouyu.cn/gtqrscyido.html

Ruby: "A".ord; 65.chr
来源：http://hz.cdnleiting.top/gtnedggocm.html

C#:   (int)'A'; (char)65
来源：http://hz.9152youxi.cn/gthzdhupyy.html

[A19] 交换两个变量
来源：http://hz.andypj.xyz/gtwbcamyfu.html

Py:   a, b = b, a
来源：http://hz.daxiang520.top/gtmtgjvexj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jinqigufen.top/gtnwlnpkvm.html

JS:   [a, b] = [b, a];
来源：http://hz.316326.xyz/gtfvczpfup.html

TS:   [a, b] = [b, a];
来源：http://hz.ivvv.top/gthkocojnh.html

Java: int t = a; a = b; b = t;
来源：http://hz.kuanghao11.cn/gtnufjlfft.html

Go:   a, b = b, a
来源：http://hz.ppjwa.cn/gtftfkqlns.html

Ruby: a, b = b, a
来源：http://hz.zhijiandao.cn/gtocioghcz.html

C#:   (a, b) = (b, a);
来源：http://hz.kuanghao11.cn/gtlbktlfrj.html

[A20] 读取标准输入
来源：http://hz.redwolf501.top/gtjnwhzvcv.html

Py:   name = input("请输入：")
来源：http://hz.tanke756.top/gtrusqlefz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.sweek.top/gtdgezuiwq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yueranfly.top/gtdusgkpcb.html

TS:   // Node.js：readline 模块
来源：http://hz.yuxming.cn/gtumlvqvjd.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.cheryme.top/gtwfotzrvh.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.cucudq.cn/gtehetvbei.html

Ruby: gets.chomp
来源：http://hz.zhixingplan.top/gtnplgabmr.html

C#:   Console.ReadLine();
来源：http://hz.yj20258.top/gtoszofccr.html

[A21] 保留指定小数位输出
来源：http://hz.shangyingyoupin.top/gtmnpgffsd.html

Py:   f"{3.14159:.2f}"
来源：http://hz.xuetiantiany.cn/gtdzieropd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cdnleiting.top/gttcdyhqrb.html

JS:   (3.14159).toFixed(2)
来源：http://hz.cucudq.cn/gtudjmbmke.html

TS:   (3.14159).toFixed(2)
来源：http://hz.sweek.top/gtzdgphfmu.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.gzhubu.top/gtziwnntwz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.dashuyun.cn/gtubguqbqc.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.guowangkeji.top/gtweacgcsh.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj20258.top/gtihmbfxoe.html

[A22] 获取字符串长度
来源：http://hz.shanyushiyangkeji.top/gtqampvgup.html

Py:   len(s)
来源：http://hz.yvedp.cn/gtqrkkcfhc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jinqigfzy.top/gtpvvptbgu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yj20258888.top/gtdxnrxkfx.html

TS:   s.length
来源：http://hz.yuanzhike.top/gtrtkssozj.html

Java: s.length()
来源：http://hz.sweek.top/gttycqnzrx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.c1oappe.top/gtntwkvpvp.html

Ruby: s.length
来源：http://hz.cheryme.top/gtbgarovzx.html

C#:   s.Length
来源：http://hz.chenjidiqi.icu/gtmjfriidt.html

[A23] 大小写转换
来源：http://hz.chenzaomai.com/gtzxcrkmss.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jinyuanbaomall.cn/gtihaalwif.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xinyue.icu/gtlaghjkyf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shzxlz.cn/gthmrdjcrz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuanzhike.top/gtswbaqzvi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shzxlz.cn/gtstfjlvrx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.kuanghao11.cn/gtpsypjnkf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xuetiantiany.cn/gtknhdqnti.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.havefunace.top/gtvysetohj.html

[A24] 去除首尾空白
来源：http://hz.zhaomingkeji.xyz/gtejhyipke.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.pycfn.com/gtuhyyoczb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jlsjyb.cn/gtuwgdypgv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hfpthk.cn/gtzodxgslr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cdnleiting.top/gtayebyubz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yj20258888.top/gtioloaqll.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhaomingkeji.xyz/gtrxivbmub.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.c1oappe.top/gtqwfgqpwy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.chenjidiqi.icu/gtbwxkzfvp.html

[A25] 字符串比较
来源：http://hz.nanxinkj.top/gtznogfmbd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhixingplan.top/gtdjmursgd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.dashuyun.cn/gtpmwhbquh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aizwys.cn/gtwmvqwbin.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigfzy.top/gtliqznoox.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shangyingyoupin.top/gtbofktvse.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.wangshuangyany.cn/gttuzhensj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ppjwa.cn/gtqfgwgtdr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.daxiang520.top/gtbspcdymr.html

[A26] 类型转换总览
来源：http://hz.316326.xyz/gtemazrxgf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sysykeji.top/gthhjmuokx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.c1oappe.top/gthliyzafl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.tanke756.top/gtxoxsutti.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jqgfzy.top/gtuxvuumct.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ppjwa.cn/gttsjsqrhz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.smart0.xyz/gtmmifeaqg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.kuanghao11.cn/gtsnhwbhgm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.gotoacloud.top/gtthficdrh.html

================================================================================
来源：http://hz.cashguo.top/gtodcqiivs.html

B. 流程控制
来源：http://hz.aibaodan.cn/gtejvtchiv.html

================================================================================
来源：http://hz.hfpthk.cn/gthiqfvgmr.html

[B01] 条件判断 if / else
来源：http://hz.feifeiyinyue.top/gtnxiqwcum.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gaohongyu789.top/gtogaqiend.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.aibaodan.cn/gtohtyjrpp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtvgpmgsvn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shangyingyoupin.top/gtijxcyqzu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.vqdsnc.cn/gtjtiyljxz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gzhubu.top/gtltaahjwo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.havefunace.top/gttqqaunio.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hammf.cn/gtbskgtnhd.html

[B02] 多分支 else if / elif
来源：http://hz.yuxming.cn/gtlgobqykw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yuxming.cn/gthyazvgow.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.316326.xyz/gtvzwappdp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtsnvbrolz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtauertbyi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtddgrznqk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yanxiufei.cn/gtcnciauvr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.nanxuanxn.top/gtfjdjrtut.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.redwolf501.top/gtbvljblme.html

[B03] switch / match / case
来源：http://hz.yongpay.top/gtqvjkieax.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.havefunace.top/gtsbomsikn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.aibaodan.cn/gtkccxboon.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yuxming.cn/gtsbrrjwin.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cucudq.cn/gthzxlirpy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.guowangkeji.top/gtrnttkqjl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jlsjyb.cn/gtzozfdedr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jianghu66.top/gtyulwjxso.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.bjfxy.top/gtycdvhsik.html

[B04] for 计数循环
来源：http://hz.aibaodan.cn/gtsqqbviia.html

Py:   for i in range(10): print(i)
来源：http://hz.shangyingyoupin.top/gtxdzlwqsb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yj20258888.top/gtsajtxegs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shanyushiyangkeji.top/gtzzgdpxaa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuetiantiany.cn/gtjdhhvhuv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jinqigufen.top/gtzmozdaog.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jiagoushi.top/gtaqsmydbl.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hnqzz.top/gtlazmetpi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.shuidangran.top/gthjwibigl.html

[B05] 遍历数组 / 列表
来源：http://hz.sxryk.cn/gteaekmuws.html

Py:   for item in arr: print(item)
来源：http://hz.zhongyouzk.top/gtkwwpzxzc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ivvv.top/gtpqwrszab.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.quarkkingdee.top/gtoptmlgag.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sweek.top/gtwfhvzpig.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinyuanbaomall.cn/gtjuykowra.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnxiangtu.top/gtzvfplqks.html

Ruby: arr.each { |item| puts item }
来源：http://hz.mhx1999.top/gtfsfalyuv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yonumen.top/gtkiynqybn.html

[B06] 遍历字典 / 对象
来源：http://hz.cqqwz.cn/gtapuuwugk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuxming.cn/gtremjjuan.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.quarkkingdee.top/gtfiaaomng.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhijiandao.cn/gtphxeajcv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhengqikj.top/gtrecjxcoq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gotoacloud.top/gtbgslovfm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.nwbrower.top/gtzguyiztq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jinghuilouyu.cn/gtyxezdifz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinghuilouyu.cn/gtvienfbbz.html

[B07] while 循环
来源：http://hz.jianghu66.top/gttxisnyax.html

Py:   while i < 10: i += 1
来源：http://hz.chenlongwang.top/gtliqkirgv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.c1oappe.top/gtcshrwfip.html

JS:   while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtktfsnbwo.html

TS:   while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtrnltzkty.html

Java: while (i < 10) { i++; }
来源：http://hz.jinqigfzy.top/gtjititwgd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ydjk.org.cn/gtdawlzyxi.html

Ruby: while i < 10; i += 1; end
来源：http://hz.svipenyu.cn/gtdetratfy.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhengqikj.top/gtpsqnozpj.html

[B08] do-while（至少执行一次）
来源：http://hz.sysykeji.top/gtfnewwlml.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yuxming.cn/gtpsfktowy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gzhubu.top/gtsvglqwhl.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinghuilouyu.cn/gtvcuabryn.html

TS:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtjfarkjpf.html

Java: do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gttsmhdxno.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ehwqpu.com/gtmmwjusfw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yj20258.top/gtklnsanyw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhengqikj.top/gtbdwbatlr.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gtuhodvsgm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cdnleiting.top/gtmgmbqaak.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xuanzx.com/gtxlvcoyzp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtgubtebdh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtglxatsqf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtoqpockei.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.tianlin.xyz/gtxyouxbgs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhengqikj.top/gtyynktwcp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtwtbxosmr.html

[B10] 遍历同时拿索引
来源：http://hz.hywenlv.cn/gtaxlemfxe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gotoacloud.top/gtxwxkcchu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.birdmap.top/gthjjqjwra.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtrmxusfsb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.daria6918.cn/gtlthnkeqa.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigfzy.top/gtpysowajj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yueranfly.top/gtclscntmc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinghuilouyu.cn/gtvbeyqtyr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.pengpengdd.cyou/gtnkakadek.html

[B11] 生成数字序列 / 区间
来源：http://hz.shuidangran.top/gtlfaehgpw.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gthtkjjntc.html

PHP:  range(0, 10, 2);
来源：http://hz.kuanghao11.cn/gtkqkyninn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tian-w.cn/gtneknhkjm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydjk.org.cn/gtkudvoatk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yongpay.top/gtsfqusnbt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhongyouzk.top/gtuqgvoywq.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xinyue.icu/gtqaqajgmn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xziqi.cn/gtrauvmidd.html

[B12] 跳出多层循环
来源：http://hz.chenlongwang.top/gtjanytrfb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.52xcode.cn/gtubjjuuen.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.nanxinkj.top/gtealvlibn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gthwnuayvi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtccqeymtf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinyuanbaomall.cn/gtvqpusivn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jqgfzy.top/gtokdfftpe.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.kuanghao11.cn/gtrhtbwnhi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhaomingkeji.xyz/gtexrmjehz.html

[B13] 判断是否为数字
来源：http://hz.xziqi.cn/gtznkfnfdq.html

Py:   isinstance(x, (int, float))
来源：http://hz.yj202588.top/gtsmwmjfoo.html

PHP:  is_numeric($x)
来源：http://hz.gzhubu.top/gtoygwuhya.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cqqwz.cn/gtxlfsvjvh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.c1oappe.top/gtoykfnzco.html

Java: x instanceof Number
来源：http://hz.hammf.cn/gtumwwmipn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sweek.top/gtjcqxicgy.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangtech.top/gtwdmqshud.html

C#:   x is int or double or decimal
来源：http://hz.hnqzz.top/gtkvoafybm.html

[B14] 判断值是否在集合内
来源：http://hz.zhoulong.xyz/gtmivirbzr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xingfuxueyuan.xyz/gtkjlanywv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yvedp.cn/gtevflxprt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.bjfxy.top/gtuzdkbydl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zdqjudy.top/gtrecyqtot.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shangyingyoupin.top/gtaazfyaix.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ywan-chungtsiang.top/gthpieptcn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gaohongyu789.top/gtobzzxovs.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jqgufenzy.top/gtxysgxbbi.html

[B15] 布尔运算与取反
来源：http://hz.9152youxi.cn/gthpngtcpd.html

Py:   a and b or not c
来源：http://hz.zhengqikj.top/gtzecaknji.html

PHP:  $a && $b || !$c
来源：http://hz.yuanzhike.top/gtjzddefnp.html

JS:   a && b || !c
来源：http://hz.meibo888.top/gtudidreip.html

TS:   a && b || !c
来源：http://hz.daria6918.cn/gtidnfayyb.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtifztryvs.html

Go:   a && b || !c
来源：http://hz.daria6918.cn/gtsutxgatl.html

Ruby: a && b || !c
来源：http://hz.guannengcc.top/gtsmyynxeu.html

C#:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtdjcohinf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ehwqpu.com/gtbxhbfrxt.html

Py:   if not data: return
来源：http://hz.svipenyu.cn/gtaeffbnaw.html

PHP:  if (!$data) { return; }
来源：http://hz.c1oappe.top/gttxlnrfcy.html

JS:   if (!data) return;
来源：http://hz.yj202588.top/gtjbhjasnv.html

TS:   if (!data) return;
来源：http://hz.yueranfly.top/gtdynxbxfo.html

Java: if (data == null) return;
来源：http://hz.daxiang520.top/gtnoigpkpw.html

Go:   if data == nil { return }
来源：http://hz.cashguo.top/gtqwsqqjun.html

Ruby: return if data.nil?
来源：http://hz.cqqwz.cn/gtynecbyly.html

C#:   if (data == null) return;
来源：http://hz.hfpthk.cn/gtkhivnrdi.html

================================================================================
来源：http://hz.yongpay.top/gtrwfswzgq.html

C. 函数与作用域
来源：http://hz.feifeiyinyue.top/gtwucmtswg.html

================================================================================
来源：http://hz.hywenlv.cn/gtgvfihqvd.html

[C01] 定义函数
来源：http://hz.redwolf501.top/gteiojjhcc.html

Py:   def add(a, b): return a + b
来源：http://hz.birdmap.top/gtwmujduzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gthcrnhcdw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ppjwa.cn/gtgdaaxvuw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenjidiqi.icu/gtspovlsac.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtedcnprgm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtoklqmxow.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zdqjudy.top/gttcuejhuh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtglauzggy.html

[C02] 默认参数
来源：http://hz.daria6918.cn/gtbhgmcvds.html

Py:   def greet(name="World"): return name
来源：http://hz.jqgufenzy.top/gtlsocpgnx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yangfankeji.com/gtuxnzhmpr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.shanyushiyangtech.top/gtksoxghzk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ppjwa.cn/gtrfzcngep.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangshuangyany.cn/gtmvvilqsf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.svipenyu.cn/gttgfpqzux.html

Ruby: def greet(name = "World") = name
来源：http://hz.zdqjudy.top/gtpqzterjk.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhengqikj.top/gtzbxhejwq.html

[C03] 可变参数
来源：http://hz.iojbl.cn/gtrtngflgw.html

Py:   def total(*args): return sum(args)
来源：http://hz.shzxlz.cn/gteqdxmcvf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cucudq.cn/gtrozvzxyy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gtnbydopxi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtawiognrh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xylfe.cn/gtcvbbxgux.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sweek.top/gttbscbpvn.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xylfe.cn/gtmrcncxwo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.quarkkingdee.top/gtcjnlroll.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhixingplan.top/gtaqaqugme.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuxming.cn/gtuvewztbc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xingfuxueyuan.xyz/gtydytgztk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.fzhhl.top/gtlaeelcmi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ehwqpu.com/gtwxhpemcv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xinyue.icu/gtkknnqmbt.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinghuilouyu.cn/gtlcyuxgck.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtdogefrkp.html

C#:   f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtsdlamzdi.html

[C05] 返回多个值
来源：http://hz.andypj.xyz/gtzwsmtati.html

Py:   return a, b
来源：http://hz.wangdashe.top/gtndtjamas.html

PHP:  return [$a, $b];
来源：http://hz.pengpengdd.cyou/gtheugdvbu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yuxming.cn/gtlgasqmrt.html

TS:   return { a, b };
来源：http://hz.shanyushiyangtech.top/gtyjvfkhki.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhoulong.xyz/gtbogthwtz.html

Go:   return a, b
来源：http://hz.hywenlv.cn/gtxbosdxjh.html

Ruby: return a, b
来源：http://hz.jinqigufen.top/gtvpriatez.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhengqikj.top/gtdlindknk.html

[C06] 匿名函数 / lambda
来源：http://hz.zycfv.cn/gtjqhsuqjj.html

Py:   square = lambda x: x * x
来源：http://hz.birdmap.top/gtodgebamy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jiagoushi.top/gtuisabrfo.html

JS:   const square = x => x * x;
来源：http://hz.nanxuanxn.top/gtiwagmpwq.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.haohaochexian.top/gtlfriekil.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gaohongyu789.top/gtlgmpwiwi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinghuilouyu.cn/gtehdhdcju.html

Ruby: square = ->(x) { x * x }
来源：http://hz.guowangkeji.top/gtufcdydsg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.iojbl.cn/gtlccqsxym.html

[C07] 把函数作为参数传入
来源：http://hz.guowangkeji.top/gtvhgqwscu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zycfv.cn/gtiqjycdoh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.redwolf501.top/gtkugvzwzu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinyuanbaomall.cn/gtsxjuopud.html

TS:   arr.map(String)
来源：http://hz.c1oappe.top/gtrvbgyqad.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.pycfn.com/gthaqqpera.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.chenlongwang.top/gtouqhngmd.html

Ruby: arr.map(&:upcase)
来源：http://hz.gaohongyu789.top/gtnzuwgigh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.quarkkingdee.top/gtcwlmlitn.html

[C08] 闭包
来源：http://hz.xziqi.cn/gtfuzayvuj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhongyouzk.top/gteccmxnwl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.daxiang520.top/gtfkxhpssd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtuewcoxmx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtvmovoxkc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gaohongyu789.top/gtxhofqssq.html


<!-- 参考信息 -->