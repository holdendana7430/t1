代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinqigufen.top/gttkuvjhwu.html

Java: (int) 'A'; (char) 65
来源：http://hz.birdmap.top/gtcjlmnzya.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zhixingplan.top/gtkqinxctl.html

Ruby: "A".ord; 65.chr
来源：http://hz.hnxiangtu.top/gtrpbyofel.html

C#:   (int)'A'; (char)65
来源：http://hz.jyoumei.cn/gteprswtuj.html

[A19] 交换两个变量
来源：http://hz.c1oappe.top/gtjyviajyw.html

Py:   a, b = b, a
来源：http://hz.zhiwuduotai.top/gtzarhgtmh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hywenlv.cn/gtqoywzbin.html

JS:   [a, b] = [b, a];
来源：http://hz.chenjidiqi.icu/gtrlubisbr.html

TS:   [a, b] = [b, a];
来源：http://hz.gogol.net.cn/gtoexcmidj.html

Java: int t = a; a = b; b = t;
来源：http://hz.xinyue.icu/gtchsvfqzo.html

Go:   a, b = b, a
来源：http://hz.svipenyu.cn/gtbcssolah.html

Ruby: a, b = b, a
来源：http://hz.dashuyun.cn/gtckyrzhzj.html

C#:   (a, b) = (b, a);
来源：http://hz.zhongyouzk.top/gtpnlgpfop.html

[A20] 读取标准输入
来源：http://hz.yj202588.top/gtxcsoynep.html

Py:   name = input("请输入：")
来源：http://hz.yuxming.cn/gtxqnqgylu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.smart0.xyz/gtqelimkoa.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.9152youxi.cn/gtfifzaair.html

TS:   // Node.js：readline 模块
来源：http://hz.sysykeji.top/gtlaaluhyl.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.tian-w.cn/gtppcwbhdf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yuanzhike.top/gtgceiuuxe.html

Ruby: gets.chomp
来源：http://hz.pycfn.com/gtyggdpqyu.html

C#:   Console.ReadLine();
来源：http://hz.xuetiantiany.cn/gtpxfxsyik.html

[A21] 保留指定小数位输出
来源：http://hz.shuidangran.top/gtpimixtpc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.tanke756.top/gthdwwkbsg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ehwqpu.com/gtbajwctae.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yongpay.top/gtfrkmoysg.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ywan-chungtsiang.top/gthtvnisgx.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.xziqi.cn/gtsdybsgxg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.aibaodan.cn/gtgjlmwypn.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.pengpengdd.cyou/gtvcrawcdb.html

C#:   3.14159.ToString("F2")
来源：http://hz.jinqigfzy.top/gtwxidmscd.html

[A22] 获取字符串长度
来源：http://hz.feifeiyinyue.top/gtclgnubfk.html

Py:   len(s)
来源：http://hz.hnxiangtu.top/gtgasdwfev.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.fengsongda.top/gtymtjbuth.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xuanzx.com/gtpybfamzr.html

TS:   s.length
来源：http://hz.jinghuilouyu.cn/gtvxipqadf.html

Java: s.length()
来源：http://hz.haohaochexian.top/gtpjktjbtl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.ywan-chungtsiang.top/gtfptlzdqv.html

Ruby: s.length
来源：http://hz.jyoumei.cn/gtlhazgpbl.html

C#:   s.Length
来源：http://hz.nanxuanxn.top/gtaxzmmiye.html

[A23] 大小写转换
来源：http://hz.yj20258.top/gtvfzcjgbw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.316326.xyz/gttjpqkjul.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.hywenlv.cn/gtzbzwizum.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hnqzz.top/gthlxfdnff.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.dashuyun.cn/gtmeqkkskw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.iojbl.cn/gtfcxtzydz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.9152youxi.cn/gthrfzobjh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yongpay.top/gtwxnjjrxn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yuanzhike.top/gtswvyrnkt.html

[A24] 去除首尾空白
来源：http://hz.c1oappe.top/gtmvgyjftx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhaomingkeji.xyz/gtbzmaewlr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.quarkkingdee.top/gtvesldpmx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tian-w.cn/gtzmdoevdv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.kuanghao11.cn/gtswvjjtgw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hywenlv.cn/gtymxmibjs.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhijiandao.cn/gtqkvrzfjp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jqgfzy.top/gtvzgjpeae.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.feifeiyinyue.top/gttslzrbxf.html

[A25] 字符串比较
来源：http://hz.daria6918.cn/gtcyjopnrt.html

Py:   s1 == s2; s1 != s2
来源：http://hz.hywenlv.cn/gtfyxwfwpp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yueranfly.top/gtaeiknebv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigfzy.top/gtjrqrtius.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.fzhhl.top/gtcttjmooz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hnqzz.top/gtajxfxagy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jiagoushi.top/gtjrqdamxf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shangyingyoupin.top/gtwktxrkeb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.shangyingyoupin.top/gtixxoljgs.html

[A26] 类型转换总览
来源：http://hz.smart0.xyz/gtwhyczwnz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yj20258888.top/gtddvmwjkx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.svipenyu.cn/gtgbelmmje.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.aizwys.cn/gtngmwavet.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhongyouzk.top/gtfjpfvung.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xuetiantiany.cn/gtamcwwqhs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.dianchejie.cn/gtqnxxurtq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jiagoushi.top/gtjbfpfdjt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhijiandao.cn/gtbecsckni.html

================================================================================
来源：http://hz.yangfankeji.com/gtdusbezvh.html

B. 流程控制
来源：http://hz.ydjk.org.cn/gtofypypfh.html

================================================================================
来源：http://hz.jyoumei.cn/gtrlkpzhlc.html

[B01] 条件判断 if / else
来源：http://hz.snrcjt.cn/gtjsfsxwfr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jianghu66.top/gtdyqvdlet.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yj202588.top/gtwsbxixss.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtmzwjatur.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtdmzxqacz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhoulong.xyz/gtulgvdado.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xylfe.cn/gttlzysoao.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jianghu66.top/gtvioelfgm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gtljbfshjg.html

[B02] 多分支 else if / elif
来源：http://hz.jyoumei.cn/gtayoykikb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhiwuduotai.top/gtlesevuos.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shanyushiyangtech.top/gtmvsewaol.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.havefunace.top/gtoczwsudk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gttghvnagc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gtbvxuyvtu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhongyouzk.top/gtlnwckgyy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.havefunace.top/gtqhsfhosq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.iojbl.cn/gterrdteft.html

[B03] switch / match / case
来源：http://hz.bjfxy.top/gtlfvuxrmt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.guowangkeji.top/gtwvuhsboq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xinyue.icu/gttllrgeuw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jyoumei.cn/gthyruywbu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sxryk.cn/gtsfsxepwo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.svipenyu.cn/gtoiuduhey.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.feifeiyinyue.top/gtkwzclrae.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenlongwang.top/gthkjinemo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.c1oappe.top/gtkmskblut.html

[B04] for 计数循环
来源：http://hz.yongpay.top/gtsmmliwbm.html

Py:   for i in range(10): print(i)
来源：http://hz.yj202588.top/gtjhxuxipc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.xingfuxueyuan.xyz/gtvgkarzbp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.tian-w.cn/gtjjggedjn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.feifeiyinyue.top/gtxhiqwybl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yj20258.top/gtvtroabkc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hysaishi.cn/gtshfzggtq.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yj20258.top/gtlxeoseul.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jyoumei.cn/gtpncmxgwr.html

[B05] 遍历数组 / 列表
来源：http://hz.ivvv.top/gtkwgemlwb.html

Py:   for item in arr: print(item)
来源：http://hz.zhongyouzk.top/gtyoyvybtz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.aibaodan.cn/gtpdsxtkyu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.daria6918.cn/gtkjycmmse.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.gaohongyu789.top/gtubrcionl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xinyue.icu/gtrkzvheyu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.haohaochexian.top/gtnvsvheey.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ivvv.top/gtsdsstpij.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.wangdashe.top/gtyjdilwud.html

[B06] 遍历字典 / 对象
来源：http://hz.quarkkingdee.top/gtchhjheag.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cqqwz.cn/gtazvxzrlh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xziqi.cn/gtivprokgr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shzxlz.cn/gtiwcfpqti.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.daxiang520.top/gtylwxkmkc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtohqvuvkr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.aibaodan.cn/gtagrqmoon.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhaomingkeji.xyz/gtiybosfnk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.9152youxi.cn/gtqhfhsnsy.html

[B07] while 循环
来源：http://hz.gaohongyu789.top/gtjdrcbmoy.html

Py:   while i < 10: i += 1
来源：http://hz.zycfv.cn/gtlehqgioi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuanzhike.top/gtvlrqoxle.html

JS:   while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtlpwvrojk.html

TS:   while (i < 10) { i++; }
来源：http://hz.hammf.cn/gtovwguoyh.html

Java: while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gthkzdkomk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hongshengwenyu.top/gtgauariua.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xziqi.cn/gthnzccpjx.html

C#:   while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtxnvqfemi.html

[B08] do-while（至少执行一次）
来源：http://hz.yj20258888.top/gtzbsqzkhx.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.birdmap.top/gthfqpuzgh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xinyue.icu/gtcflkdydd.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtqjptdeeo.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtkreidppu.html

Java: do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtqeahmfrr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hywenlv.cn/gtrtyeoscq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.sweek.top/gtrfyuwnaw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtiuzrxpjy.html

[B09] break 与 continue
来源：http://hz.cucudq.cn/gtuecxvdes.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.0kj1m.cn/gtgrvzlvqz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sufxvd.cn/gtxvslupus.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gttwuxupww.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtaslfpenk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtmzbuvxls.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hywenlv.cn/gtogziskmc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cheryme.top/gtsxhqwlgj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtommfntxa.html

[B10] 遍历同时拿索引
来源：http://hz.ydzc1.top/gtqfzgfnwu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yuanzhike.top/gtuvbxproq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jinqigufen.top/gtxwgwfisx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yvedp.cn/gtduduqrpr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.snrcjt.cn/gtiapsekdm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.pengpengdd.cyou/gtdieeumvu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zdqjudy.top/gtwstrkddm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jlsjyb.cn/gtorpoewrz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.chenjidiqi.icu/gtzsbtxhrr.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhoulong.xyz/gtvxhvyoot.html

Py:   list(range(0, 10, 2))
来源：http://hz.yanxiufei.cn/gtfapzgyoj.html

PHP:  range(0, 10, 2);
来源：http://hz.zycfv.cn/gtyzabvubx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shanyushiyangtech.top/gtarmaapff.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtfrudgkwm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hnxiangtu.top/gtdawcgkcn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.c1oappe.top/gtgbypkxqc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.c1oappe.top/gtbutusqzv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhiwuduotai.top/gtnkvvhjmb.html

[B12] 跳出多层循环
来源：http://hz.jinqigfzy.top/gtfnvczzpz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hywenlv.cn/gtopmbpids.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zdqjudy.top/gtsrppkgip.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ywan-chungtsiang.top/gtdrhxcclb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtcwjbuzdl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gthsjwzrom.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.wangdashe.top/gtaxeuwoxy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.iojbl.cn/gtlxpatogw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.fzhhl.top/gtlgjllshp.html

[B13] 判断是否为数字
来源：http://hz.tanke756.top/gtswscgpgn.html

Py:   isinstance(x, (int, float))
来源：http://hz.guowangkeji.top/gtydvnimcs.html

PHP:  is_numeric($x)
来源：http://hz.52xcode.cn/gtxhsthisb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtqrmkuduc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhijiandao.cn/gtomlqvesf.html

Java: x instanceof Number
来源：http://hz.ydzc1.top/gtcaclkiqz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cucudq.cn/gtyecymozc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hongshengwenyu.top/gtqakarazt.html

C#:   x is int or double or decimal
来源：http://hz.yonumen.top/gtylgfhqso.html

[B14] 判断值是否在集合内
来源：http://hz.jiagoushi.top/gtllmjkezc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinghuilouyu.cn/gtpelbcsgp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.9152youxi.cn/gtshurixyq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtjralgqma.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gtdddtnedy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gtzywrpvov.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guowangkeji.top/gtijbgweuu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj202588.top/gtklhlgpog.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tianlin.xyz/gtneawppir.html

[B15] 布尔运算与取反
来源：http://hz.tian-w.cn/gtbphqalqo.html

Py:   a and b or not c
来源：http://hz.tian-w.cn/gtrmvzyobm.html

PHP:  $a && $b || !$c
来源：http://hz.hywenlv.cn/gtmtqhraew.html

JS:   a && b || !c
来源：http://hz.xylfe.cn/gtlfhvulxj.html

TS:   a && b || !c
来源：http://hz.vqdsnc.cn/gtkwotujkb.html

Java: a && b || !c
来源：http://hz.xuanzx.com/gtxjntadkg.html

Go:   a && b || !c
来源：http://hz.zhixingplan.top/gtubwgqfmr.html

Ruby: a && b || !c
来源：http://hz.shuidangran.top/gtahkamgfp.html

C#:   a && b || !c
来源：http://hz.mhx1999.top/gtnmcvmecf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.svipenyu.cn/gtydhckout.html

Py:   if not data: return
来源：http://hz.jinyuanbaomall.cn/gtdtvtkzbp.html

PHP:  if (!$data) { return; }
来源：http://hz.sxryk.cn/gtjfjpokcc.html

JS:   if (!data) return;
来源：http://hz.yanxiufei.cn/gtjgphocbt.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtnvslevhm.html

Java: if (data == null) return;
来源：http://hz.pycfn.com/gtkojbndst.html

Go:   if data == nil { return }
来源：http://hz.jiagoushi.top/gtdwupxngs.html

Ruby: return if data.nil?
来源：http://hz.svipenyu.cn/gtvrpmnspj.html

C#:   if (data == null) return;
来源：http://hz.shzxlz.cn/gtkejqhemb.html

================================================================================
来源：http://hz.jiagoushi.top/gtsyhuimge.html

C. 函数与作用域
来源：http://hz.jqgfzy.top/gtfqquzdes.html

================================================================================
来源：http://hz.gotoacloud.top/gtmxqbiqux.html

[C01] 定义函数
来源：http://hz.hammf.cn/gtqvuvtayw.html

Py:   def add(a, b): return a + b
来源：http://hz.shzxlz.cn/gtinlafbpy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.9152youxi.cn/gtyjumuekf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj202588.top/gtqieqkerp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuetiantiany.cn/gthdjnhtoc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtluormjex.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xinyue.icu/gtrxyagvht.html

Ruby: def add(a, b); a + b; end
来源：http://hz.wangdashe.top/gtlmjvqhzu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtuctfjzfr.html

[C02] 默认参数
来源：http://hz.shanyushiyangtech.top/gtnagpbpmb.html

Py:   def greet(name="World"): return name
来源：http://hz.ehwqpu.com/gtdztbikxt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ybcxt.top/gtalqynujv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.c1oappe.top/gtllkxxelx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtoqchpwsp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sweek.top/gtcrmyfust.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gthztatmyl.html

Ruby: def greet(name = "World") = name
来源：http://hz.yueranfly.top/gtisjnwgag.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nwbrower.top/gtdfutnolb.html

[C03] 可变参数
来源：http://hz.daxiang520.top/gtvfjjkkmh.html

Py:   def total(*args): return sum(args)
来源：http://hz.0kj1m.cn/gtifcnoagx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.snrcjt.cn/gtvtdzhyus.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.redwolf501.top/gtgwaqjmda.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.vqdsnc.cn/gthgxykeqq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.havefunace.top/gtrwtfhpnu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.c1oappe.top/gtkzrryknd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tian-w.cn/gtrxerecbp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhiwuduotai.top/gtaqbpknjz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ppjwa.cn/gtmcrjmaih.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhoulong.xyz/gtgwogofqy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jlsjyb.cn/gtgfxxsyjx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gtjvdbbpeg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.guannengcc.top/gtkvsfxcby.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.ybcxt.top/gtdhxhtwdn.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuanzhike.top/gtzyewenin.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hnqzz.top/gtordadezy.html

C#:   f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtdyjjqbez.html

[C05] 返回多个值
来源：http://hz.havefunace.top/gtdydnitmr.html

Py:   return a, b
来源：http://hz.yj20258888.top/gtohzbasnr.html

PHP:  return [$a, $b];
来源：http://hz.0kj1m.cn/gtfnfplvpx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.quarkkingdee.top/gtkfcvehqf.html

TS:   return { a, b };
来源：http://hz.iojbl.cn/gtfrgdcrke.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.xylfe.cn/gtvpvhtjfe.html

Go:   return a, b
来源：http://hz.0kj1m.cn/gtfezxvoah.html

Ruby: return a, b
来源：http://hz.hfpthk.cn/gtgaqmamsb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.mhx1999.top/gtuehmwhxj.html

[C06] 匿名函数 / lambda
来源：http://hz.316326.xyz/gthpsqiqna.html

Py:   square = lambda x: x * x
来源：http://hz.yangfankeji.com/gtgimzqkpn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.haohaochexian.top/gtuwkhilpm.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtwtzjlsvb.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ywan-chungtsiang.top/gtsfwasgwn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.redwolf501.top/gtgqmaepsi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.aibaodan.cn/gtbtpsdjjp.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cdnleiting.top/gtmkjitqhu.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jyoumei.cn/gtklzguugr.html

[C07] 把函数作为参数传入
来源：http://hz.andypj.xyz/gthnwkcapl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.feifeiyinyue.top/gtnbjvdiye.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhijiandao.cn/gtccgssrlf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.c1oappe.top/gtxutensfl.html

TS:   arr.map(String)
来源：http://hz.gaohongyu789.top/gtgqdtprdu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.zhaomingkeji.xyz/gtrpojuqhu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangtech.top/gtcbkyuily.html

Ruby: arr.map(&:upcase)
来源：http://hz.birdmap.top/gtwpvreeub.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhongyouzk.top/gtgccpredo.html

[C08] 闭包
来源：http://hz.vqdsnc.cn/gtebiiqwed.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daxiang520.top/gtkwereqwc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinyuanbaomall.cn/gthooryjgq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtkzbkimkn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.sysykeji.top/gtzhcugosv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgufenzy.top/gtbbgcffgo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtsibynxiv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhijiandao.cn/gtgseuwhdb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtfracaumw.html

[C09] 递归
来源：http://hz.aibaodan.cn/gtpuykvwdl.html


<!-- 参考信息 -->