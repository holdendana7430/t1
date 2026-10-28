代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shanyushiyangtech.top/gtzdbznrgp.html

Java: (int) 'A'; (char) 65
来源：http://hz.cashguo.top/gtptkbtafy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.cdnleiting.top/gtjvuiewkf.html

Ruby: "A".ord; 65.chr
来源：http://hz.ywan-chungtsiang.top/gtrmtkjmxb.html

C#:   (int)'A'; (char)65
来源：http://hz.jianghu66.top/gtjtwkakdp.html

[A19] 交换两个变量
来源：http://hz.hammf.cn/gtrwrkieqt.html

Py:   a, b = b, a
来源：http://hz.yj202588.top/gtrbgrizxh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yanxiufei.cn/gtehwrudgc.html

JS:   [a, b] = [b, a];
来源：http://hz.gogol.net.cn/gtfzjeelot.html

TS:   [a, b] = [b, a];
来源：http://hz.kuanghao11.cn/gtqjhmmwkd.html

Java: int t = a; a = b; b = t;
来源：http://hz.guannengcc.top/gtgmbtgbdu.html

Go:   a, b = b, a
来源：http://hz.jinqigfzy.top/gtomzmacug.html

Ruby: a, b = b, a
来源：http://hz.tian-w.cn/gttsijishh.html

C#:   (a, b) = (b, a);
来源：http://hz.yangfankeji.com/gtpzzudxuy.html

[A20] 读取标准输入
来源：http://hz.yj20258888.top/gtcyydiefc.html

Py:   name = input("请输入：")
来源：http://hz.jianghu66.top/gtxwisdoyl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xuetiantiany.cn/gtupaknmbv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.iojbl.cn/gtfyejzhjc.html

TS:   // Node.js：readline 模块
来源：http://hz.jqgufenzy.top/gtzzwzqtkp.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yvedp.cn/gtjshtpcgq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jinqigufen.top/gtrdsqfzge.html

Ruby: gets.chomp
来源：http://hz.aizwys.cn/gtqmmokjpx.html

C#:   Console.ReadLine();
来源：http://hz.shuidangran.top/gtqepwryox.html

[A21] 保留指定小数位输出
来源：http://hz.nwbrower.top/gtdlcwhjpf.html

Py:   f"{3.14159:.2f}"
来源：http://hz.hammf.cn/gtigeeccpm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.wangshuangyany.cn/gtwaluaabi.html

JS:   (3.14159).toFixed(2)
来源：http://hz.redwolf501.top/gtgycktlda.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zycfv.cn/gtldqwuvgy.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.chenzaomai.com/gtpqtxdqpz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yvedp.cn/gtdgzdkpcy.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.kuanghao11.cn/gtajoaxniu.html

C#:   3.14159.ToString("F2")
来源：http://hz.52xcode.cn/gtkacqnhkc.html

[A22] 获取字符串长度
来源：http://hz.jlsjyb.cn/gtchjyxiyw.html

Py:   len(s)
来源：http://hz.redwolf501.top/gtjhzgykgx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zycfv.cn/gtexptsxhi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xinyue.icu/gtohpwtptg.html

TS:   s.length
来源：http://hz.cashguo.top/gtylhbssig.html

Java: s.length()
来源：http://hz.svipenyu.cn/gtouhzyomn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.0kj1m.cn/gtoznlksbl.html

Ruby: s.length
来源：http://hz.jyoumei.cn/gtpuyewuut.html

C#:   s.Length
来源：http://hz.gogol.net.cn/gtytpcjstj.html

[A23] 大小写转换
来源：http://hz.cdnleiting.top/gtpphuqkqa.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.xingfuxueyuan.xyz/gttiptkzfr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhongyouzk.top/gtipqiyitg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenlongwang.top/gtmsepzneb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuxming.cn/gtkhfrjhmh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shangyingyoupin.top/gtdoavdkml.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.daxiang520.top/gtjhmssjpu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yueranfly.top/gtaocydppk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhongyouzk.top/gtkxmskydu.html

[A24] 去除首尾空白
来源：http://hz.sxryk.cn/gtagmoicbf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.daxiang520.top/gthrliuzfn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.52xcode.cn/gtygjhbeev.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinyuanbaomall.cn/gttrbexsaf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cqqwz.cn/gtrrpahnmw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.nanxuanxn.top/gtpccuqnqx.html

Go:   strings.TrimSpace(s)
来源：http://hz.yueranfly.top/gtdfkusvfj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinyuanbaomall.cn/gtuqivzhwj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhengqikj.top/gtkbjgupkf.html

[A25] 字符串比较
来源：http://hz.zhengqikj.top/gtrmcduwbe.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ybcxt.top/gthaylhsny.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.redwolf501.top/gtfpzibftl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xuanzx.com/gtzlvtrdza.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yuxming.cn/gticoapsdx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xuetiantiany.cn/gthxisueyg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.mhx1999.top/gtyxfuxtyq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.snrcjt.cn/gtpbqpvwcr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.shuidangran.top/gtonfvdyfu.html

[A26] 类型转换总览
来源：http://hz.kuanghao11.cn/gtedcrnyld.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.gaohongyu789.top/gtrudxxjos.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gaohongyu789.top/gtjdqmuufz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.daxiang520.top/gtnsirbxih.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zdqjudy.top/gtcbkzkcpg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shangyingyoupin.top/gthjifalwd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ybcxt.top/gtncgptxwc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.pycfn.com/gtiiphwgcb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.dashuyun.cn/gtecfldeiz.html

================================================================================
来源：http://hz.yuxming.cn/gtkqdlouap.html

B. 流程控制
来源：http://hz.zhaomingkeji.xyz/gttlyjngic.html

================================================================================
来源：http://hz.hysaishi.cn/gtacmbusml.html

[B01] 条件判断 if / else
来源：http://hz.snrcjt.cn/gtscasmhcu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cashguo.top/gtlhwxiepl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xingfuxueyuan.xyz/gtklowocbo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtjhxzsgyv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtmdlnbysf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zdqjudy.top/gtbyqvmwmj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.wangshuangyany.cn/gtapzkjlft.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.ppjwa.cn/gthymrkwqy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtsvzztooi.html

[B02] 多分支 else if / elif
来源：http://hz.xingfuxueyuan.xyz/gtltfpkbqc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.snrcjt.cn/gtrnsqbdpb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhiwuduotai.top/gtqowdeeck.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtrqascwld.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtcmzgdbly.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gtdsxkixbj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.c1oappe.top/gtmjraepyq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yuanzhike.top/gtgxxtbrfm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.birdmap.top/gtwtnlzyih.html

[B03] switch / match / case
来源：http://hz.cdnleiting.top/gtmqatzgya.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jinqigfzy.top/gtxzjobqwc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daxiang520.top/gtondmiegl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jianghu66.top/gtohqxtque.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hammf.cn/gtmqxxxjsh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj202588.top/gtebosscnm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cqqwz.cn/gtqdymxmza.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.vqdsnc.cn/gtswrppjda.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.birdmap.top/gtznfhsnhr.html

[B04] for 计数循环
来源：http://hz.hongshengwenyu.top/gtivrddvuu.html

Py:   for i in range(10): print(i)
来源：http://hz.redwolf501.top/gtngdchatj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ehwqpu.com/gthcdymdyb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ppjwa.cn/gtjmkoywpr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.birdmap.top/gttctprmte.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhaomingkeji.xyz/gtnegbbmjx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cheryme.top/gtlkoaooto.html

Ruby: 10.times { |i| puts i }
来源：http://hz.chenlongwang.top/gtgaxbuxgm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yueranfly.top/gtfkasqihj.html

[B05] 遍历数组 / 列表
来源：http://hz.zhaomingkeji.xyz/gtemgnddoq.html

Py:   for item in arr: print(item)
来源：http://hz.shanyushiyangtech.top/gtdqpqqrat.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yuanzhike.top/gtlhuknegq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ppjwa.cn/gtrmyoxyta.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.snrcjt.cn/gtkrhheial.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.dashuyun.cn/gtktlzikfd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yongpay.top/gtwxsmmuhl.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hnqzz.top/gtnfutdsok.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yangfankeji.com/gtixpcoblb.html

[B06] 遍历字典 / 对象
来源：http://hz.ybcxt.top/gtscmaqfkr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhijiandao.cn/gtlmqkrlci.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.havefunace.top/gtxujtnyie.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shuidangran.top/gtvkvchkhk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinghuilouyu.cn/gtqijxwiue.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.haohaochexian.top/gtojsnhlku.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hysaishi.cn/gtpzkkijst.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xinyue.icu/gtsonosbrs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yuanzhike.top/gtzzwftrsm.html

[B07] while 循环
来源：http://hz.chenjidiqi.icu/gtiqvkizri.html

Py:   while i < 10: i += 1
来源：http://hz.gzhubu.top/gtehyubjsu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zycfv.cn/gtdopezeyz.html

JS:   while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gtsklmoqvn.html

TS:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtlmtlgoce.html

Java: while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtiaypzghf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xinyue.icu/gtlaloyvso.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yj20258.top/gtbghvptwq.html

C#:   while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtjwobjgwj.html

[B08] do-while（至少执行一次）
来源：http://hz.snrcjt.cn/gtesnafkad.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenzaomai.com/gteuiincml.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.cdnleiting.top/gtajvzwysa.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtvzfblzxj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gtnphjqzez.html

Java: do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtqlwavxzr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.aizwys.cn/gtgrrjmbib.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hnqzz.top/gtstkzvfzo.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gteokjhkfe.html

[B09] break 与 continue
来源：http://hz.zhiwuduotai.top/gtoohfxden.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.iojbl.cn/gtktwpapiv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.quarkkingdee.top/gtguyhljkq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aizwys.cn/gttcmrhokv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtbndltjbx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtawgtoisd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jiagoushi.top/gtlcewyxrg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xingfuxueyuan.xyz/gtaipfnebq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtxpwenuww.html

[B10] 遍历同时拿索引
来源：http://hz.yonumen.top/gtbsavzvnj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinqigfzy.top/gtgubsbezu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.andypj.xyz/gtkdmitcph.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhoulong.xyz/gtiwadhisx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtztmsbjbe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.birdmap.top/gtmdfmtqwx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cucudq.cn/gtwyfhadtf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.316326.xyz/gtpjfmrajk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhongyouzk.top/gtxhalmnnv.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinyuanbaomall.cn/gtcgbdwmoq.html

Py:   list(range(0, 10, 2))
来源：http://hz.aibaodan.cn/gtpypzngqd.html

PHP:  range(0, 10, 2);
来源：http://hz.yonumen.top/gtgonqbwgf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tian-w.cn/gtghqntnbq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinghuilouyu.cn/gtdmyiyjxl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.birdmap.top/gtsiaclrff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinyuanbaomall.cn/gtcbqgkvyk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.birdmap.top/gthirewbgg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ehwqpu.com/gthnydgofu.html

[B12] 跳出多层循环
来源：http://hz.xuanzx.com/gtmmjflgza.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tian-w.cn/gtfagezsvq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hysaishi.cn/gtyfxxslth.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gtukxkhrnr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtgnclkncz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gtnhbvyblx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.sxryk.cn/gtoctxbzxd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.pycfn.com/gtykmqggxm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.fengsongda.top/gtjwfbqdoh.html

[B13] 判断是否为数字
来源：http://hz.tanke756.top/gtlqpatpux.html

Py:   isinstance(x, (int, float))
来源：http://hz.aizwys.cn/gtrvhfhzma.html

PHP:  is_numeric($x)
来源：http://hz.zhijiandao.cn/gtwrawuoge.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jlsjyb.cn/gtpnjkihat.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gteouidxpd.html

Java: x instanceof Number
来源：http://hz.fengsongda.top/gtasgozvmz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ywan-chungtsiang.top/gtgoalhuyu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yueranfly.top/gtvyucnoor.html

C#:   x is int or double or decimal
来源：http://hz.shuidangran.top/gtodamdjen.html

[B14] 判断值是否在集合内
来源：http://hz.kuanghao11.cn/gtdaqccryr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yongpay.top/gtnvbgbiuu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtkjltjnsl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtthpaklqb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtjosjbutz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.nwbrower.top/gtbcavpzqo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hysaishi.cn/gtsefelwto.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xylfe.cn/gtafpvstkr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.guannengcc.top/gtizbapbrh.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangtech.top/gtxhrlhqzu.html

Py:   a and b or not c
来源：http://hz.wangshuangyany.cn/gtquynwcnj.html

PHP:  $a && $b || !$c
来源：http://hz.mhx1999.top/gtjgbxnjpc.html

JS:   a && b || !c
来源：http://hz.yj20258888.top/gtkdsyyivi.html

TS:   a && b || !c
来源：http://hz.guannengcc.top/gtvgvpqpcy.html

Java: a && b || !c
来源：http://hz.zhengqikj.top/gtczolqerv.html

Go:   a && b || !c
来源：http://hz.xziqi.cn/gtwwgpoxmz.html

Ruby: a && b || !c
来源：http://hz.0kj1m.cn/gtzwicznfa.html

C#:   a && b || !c
来源：http://hz.snrcjt.cn/gtfhtbphsz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jyoumei.cn/gtymegrkez.html

Py:   if not data: return
来源：http://hz.vqdsnc.cn/gtkipbmfzk.html

PHP:  if (!$data) { return; }
来源：http://hz.haohaochexian.top/gtdjwaqmot.html

JS:   if (!data) return;
来源：http://hz.daria6918.cn/gtjbanyzxf.html

TS:   if (!data) return;
来源：http://hz.hammf.cn/gtngveyoho.html

Java: if (data == null) return;
来源：http://hz.zhijiandao.cn/gtwpgzixwj.html

Go:   if data == nil { return }
来源：http://hz.birdmap.top/gtjbtfxefp.html

Ruby: return if data.nil?
来源：http://hz.yanxiufei.cn/gtrjmmafvw.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangkeji.top/gtpswtmfjx.html

================================================================================
来源：http://hz.cdnleiting.top/gtieqfsafb.html

C. 函数与作用域
来源：http://hz.hammf.cn/gtpshyongj.html

================================================================================
来源：http://hz.yanxiufei.cn/gttjwxnhxb.html

[C01] 定义函数
来源：http://hz.ydjk.org.cn/gtkxfzqjva.html

Py:   def add(a, b): return a + b
来源：http://hz.pengpengdd.cyou/gthmsndijp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigfzy.top/gtjnuiiwcd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ydzc1.top/gtzosdxalf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gtgtvyvpyv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtmcnrexra.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pycfn.com/gtewlswbsw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.pengpengdd.cyou/gtcpmqztjq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtkebxkorw.html

[C02] 默认参数
来源：http://hz.hammf.cn/gtjdjccrka.html

Py:   def greet(name="World"): return name
来源：http://hz.mhx1999.top/gtrxchkutw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnqzz.top/gtlwhfhwzt.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tian-w.cn/gtvanvshhr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yvedp.cn/gtjkgvmgrf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinyuanbaomall.cn/gthclfjeap.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhongyouzk.top/gtazjpxkjk.html

Ruby: def greet(name = "World") = name
来源：http://hz.hysaishi.cn/gtzqbpzvzl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258.top/gtxbphxrcv.html

[C03] 可变参数
来源：http://hz.xuetiantiany.cn/gtxonejxrg.html

Py:   def total(*args): return sum(args)
来源：http://hz.jiagoushi.top/gtsjfkoxbh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangtech.top/gtpkmjuohx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hywenlv.cn/gteszfrjbb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.smart0.xyz/gtxojvudut.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sxryk.cn/gtagugphcz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ehwqpu.com/gtugypfacr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xuanzx.com/gtpcguugeh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenlongwang.top/gtkhxjgznr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.haohaochexian.top/gtrumcskzr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.feifeiyinyue.top/gtnwqvoazy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.vqdsnc.cn/gtpxxisbqj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtxkacoktb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.birdmap.top/gtdwahokqy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.316326.xyz/gtfeypplpl.html

Go:   // 无：用配置结构体参数
来源：http://hz.yueranfly.top/gtmwatwcjv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.9152youxi.cn/gtvfymgink.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtdrjethhz.html

[C05] 返回多个值
来源：http://hz.tian-w.cn/gtyaxgmbff.html

Py:   return a, b
来源：http://hz.xingfuxueyuan.xyz/gtutkonwgo.html

PHP:  return [$a, $b];
来源：http://hz.kuanghao11.cn/gthphqcuvh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yuxming.cn/gtnvtzsvnb.html

TS:   return { a, b };
来源：http://hz.cheryme.top/gtstdajmco.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jinghuilouyu.cn/gtpbkmsljm.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtedlscblz.html

Ruby: return a, b
来源：http://hz.yangfankeji.com/gtjjxurwbq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.pengpengdd.cyou/gthseunuue.html

[C06] 匿名函数 / lambda
来源：http://hz.pengpengdd.cyou/gtmenizcln.html

Py:   square = lambda x: x * x
来源：http://hz.hnxiangtu.top/gtfkxrfdpm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhongyouzk.top/gtpbjgvkjy.html

JS:   const square = x => x * x;
来源：http://hz.yueranfly.top/gteanuyxma.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cashguo.top/gtewcqyein.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guannengcc.top/gtwpfhirrg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.9152youxi.cn/gtchrbbtho.html

Ruby: square = ->(x) { x * x }
来源：http://hz.iojbl.cn/gtjhkbelsk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jlsjyb.cn/gtrqprykau.html

[C07] 把函数作为参数传入
来源：http://hz.gzhubu.top/gttjvnfxnc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ehwqpu.com/gtpysrnxkh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.mhx1999.top/gteuyfsasx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sysykeji.top/gtscwhwvfi.html

TS:   arr.map(String)
来源：http://hz.sufxvd.cn/gtdvwcdnsw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgfzy.top/gtuhqvezeu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ydzc1.top/gtuaoaachd.html

Ruby: arr.map(&:upcase)
来源：http://hz.gogol.net.cn/gtxmdqekuh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.gogol.net.cn/gtloqdivqi.html

[C08] 闭包
来源：http://hz.cucudq.cn/gtsnsmzsvv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zdqjudy.top/gtlrfmkcjo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.wangshuangyany.cn/gtjjqyxsod.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.chenlongwang.top/gtogvnsino.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gthepfxjzf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xylfe.cn/gtmswufkzr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jqgufenzy.top/gtbnrcbvsu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhixingplan.top/gtbqroueer.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtyasipbwr.html

[C09] 递归
来源：http://hz.iojbl.cn/gtdirebkwe.html


<!-- 参考信息 -->