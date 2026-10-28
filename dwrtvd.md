代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.andypj.xyz/gtketdvjlm.html

Py:   ord("A"); chr(65)
来源：http://hz.svipenyu.cn/gtrlsotqfv.html

PHP:  ord("A"); chr(65)
来源：http://hz.yanxiufei.cn/gtdjclgflf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yuxming.cn/gtuthaotyc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sxryk.cn/gtrextvvmv.html

Java: (int) 'A'; (char) 65
来源：http://hz.hnxiangtu.top/gthunbysum.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.feifeiyinyue.top/gtwbfnmviq.html

Ruby: "A".ord; 65.chr
来源：http://hz.andypj.xyz/gtdemigidc.html

C#:   (int)'A'; (char)65
来源：http://hz.xuanzx.com/gthhmvluva.html

[A19] 交换两个变量
来源：http://hz.yongpay.top/gtsylbegio.html

Py:   a, b = b, a
来源：http://hz.shanyushiyangtech.top/gtmrcytdko.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.aizwys.cn/gtjzkhuzuh.html

JS:   [a, b] = [b, a];
来源：http://hz.hammf.cn/gtbqotsczf.html

TS:   [a, b] = [b, a];
来源：http://hz.guowangkeji.top/gtefdmdjir.html

Java: int t = a; a = b; b = t;
来源：http://hz.sufxvd.cn/gtfpnzvhgx.html

Go:   a, b = b, a
来源：http://hz.bjfxy.top/gtqtqjqzzr.html

Ruby: a, b = b, a
来源：http://hz.cashguo.top/gtitbsvqby.html

C#:   (a, b) = (b, a);
来源：http://hz.zhixingplan.top/gtbmqbfnzo.html

[A20] 读取标准输入
来源：http://hz.cheryme.top/gtzawrpogz.html

Py:   name = input("请输入：")
来源：http://hz.shanyushiyangtech.top/gtrhkecvel.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ydjk.org.cn/gtcxsmfvio.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jqgfzy.top/gtdfulbcnh.html

TS:   // Node.js：readline 模块
来源：http://hz.birdmap.top/gtrlfvcisv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.feifeiyinyue.top/gtpmkprolu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.redwolf501.top/gtndbdgubb.html

Ruby: gets.chomp
来源：http://hz.chenzaomai.com/gtguqqboqs.html

C#:   Console.ReadLine();
来源：http://hz.yangfankeji.com/gtouozqnof.html

[A21] 保留指定小数位输出
来源：http://hz.yvedp.cn/gtucpgdxuu.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jlsjyb.cn/gtbpzhhqxr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtyqsnktzm.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yueranfly.top/gtyolqyyin.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhoulong.xyz/gtxkbteqqs.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.chenzaomai.com/gtorqhenxw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.fzhhl.top/gtkyqgwpjt.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtacqyhxqy.html

C#:   3.14159.ToString("F2")
来源：http://hz.svipenyu.cn/gthsgerxas.html

[A22] 获取字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtbdrcdpxp.html

Py:   len(s)
来源：http://hz.xingfuxueyuan.xyz/gtklwjxuiw.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.gogol.net.cn/gtonocbcyc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.pengpengdd.cyou/gtpesptqrw.html

TS:   s.length
来源：http://hz.gzhubu.top/gtnxbikrcr.html

Java: s.length()
来源：http://hz.andypj.xyz/gtaevqqowq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yongpay.top/gtefzvawiq.html

Ruby: s.length
来源：http://hz.tanke756.top/gttiinctjs.html

C#:   s.Length
来源：http://hz.yuanzhike.top/gtvejdazjg.html

[A23] 大小写转换
来源：http://hz.nanxinkj.top/gtloeelhoe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.dianchejie.cn/gthonioode.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.316326.xyz/gtuxmsyawv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhengqikj.top/gtixrkrerz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.aibaodan.cn/gthtmhrllc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.xingfuxueyuan.xyz/gtwxbvayxo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.cucudq.cn/gtokmjxcyj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hnqzz.top/gtxrsxzmvw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.sysykeji.top/gtgahswpro.html

[A24] 去除首尾空白
来源：http://hz.gzhubu.top/gtflgtbsdm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.xinyue.icu/gtogivbsmi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.c1oappe.top/gtmjwfydye.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gaohongyu789.top/gtmywxfgsl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shangyingyoupin.top/gtoedboahn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.dashuyun.cn/gtrcshveby.html

Go:   strings.TrimSpace(s)
来源：http://hz.hammf.cn/gtiamislag.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zhijiandao.cn/gtpwffjdyl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhongyouzk.top/gttdiyilsl.html

[A25] 字符串比较
来源：http://hz.zhijiandao.cn/gtludlikex.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhiwuduotai.top/gtdulwemdz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shuidangran.top/gtacklbdfs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ehwqpu.com/gtaleohhsq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydjk.org.cn/gtzirsvwre.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.aizwys.cn/gtzftweexa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.quarkkingdee.top/gtdfpcstyu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.dashuyun.cn/gtrxqgysqw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.havefunace.top/gtttogzfru.html

[A26] 类型转换总览
来源：http://hz.chenzaomai.com/gtvoqdzhhq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhoulong.xyz/gtchomcxww.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.redwolf501.top/gtyadgdjqw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gaohongyu789.top/gthpociufc.html

TS:   Number() String() Boolean() x as number
来源：http://hz.tianlin.xyz/gtvpxgelgk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yuxming.cn/gtsrqejlnt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jiagoushi.top/gtiugnkqhf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.xziqi.cn/gtjxcmnvvf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yongpay.top/gtpdqaodbx.html

================================================================================
来源：http://hz.hnxiangtu.top/gthjulgzje.html

B. 流程控制
来源：http://hz.tanke756.top/gtelcrtbel.html

================================================================================
来源：http://hz.fzhhl.top/gtmxlanxok.html

[B01] 条件判断 if / else
来源：http://hz.xziqi.cn/gtwcjilakb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gogol.net.cn/gtpkqdecdt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yj20258.top/gtuxsfitxl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sysykeji.top/gthdyjmigc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cdnleiting.top/gtnjbkpwby.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.svipenyu.cn/gtstymteus.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cheryme.top/gtlduylhiw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hysaishi.cn/gtxeiuzhrp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.cdnleiting.top/gttrzquzpa.html

[B02] 多分支 else if / elif
来源：http://hz.gotoacloud.top/gtpyhifquk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cucudq.cn/gtsgvpyeic.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jlsjyb.cn/gtfakpbzwt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtpkmayzqg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtaqsbromo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtrdslahlz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhijiandao.cn/gtpfbabyvi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jqgufenzy.top/gtjzmvyyvr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtcjdejauh.html

[B03] switch / match / case
来源：http://hz.ydzc1.top/gtafverklz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hywenlv.cn/gttftxyeuo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.sysykeji.top/gtpgoilydy.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.havefunace.top/gtjdwoxufk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.andypj.xyz/gtdbfgjsje.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jianghu66.top/gtjwudclnb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhengqikj.top/gtqbutlovq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.nanxuanxn.top/gtpsivafdw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.chenzaomai.com/gtmihaddiw.html

[B04] for 计数循环
来源：http://hz.ybcxt.top/gtnivgetcf.html

Py:   for i in range(10): print(i)
来源：http://hz.sxryk.cn/gtadvztonu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.redwolf501.top/gttbxyywmp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.dashuyun.cn/gtpmdjpdfs.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258.top/gtjgtcdypp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yongpay.top/gtfcrqfdmc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jyoumei.cn/gtuvvgfoog.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daria6918.cn/gtgbfdhrfp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.daria6918.cn/gtigsndant.html

[B05] 遍历数组 / 列表
来源：http://hz.snrcjt.cn/gteebzshea.html

Py:   for item in arr: print(item)
来源：http://hz.guannengcc.top/gtgtfdeoet.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.ydjk.org.cn/gtdxhawjma.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gtaovdllqn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.tianlin.xyz/gtmracqfyz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jyoumei.cn/gtoqhbvgyz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.daxiang520.top/gtcgbkilei.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cheryme.top/gtrhuqtcnq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gzhubu.top/gtruswlthm.html

[B06] 遍历字典 / 对象
来源：http://hz.nanxinkj.top/gtwkppttua.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj20258.top/gtolyayyfk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.52xcode.cn/gthzeartlm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.316326.xyz/gtdenvowmd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aibaodan.cn/gtozwysblq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yonumen.top/gtbspxnqop.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.dianchejie.cn/gtivydbwyg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shangyingyoupin.top/gtjiuvmtsz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.haohaochexian.top/gttdhydwon.html

[B07] while 循环
来源：http://hz.hfpthk.cn/gtselapjli.html

Py:   while i < 10: i += 1
来源：http://hz.yueranfly.top/gtavubjgjw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.kuanghao11.cn/gtcevcpzgv.html

JS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangkeji.top/gtmuzzjlnc.html

TS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtlmyavaeb.html

Java: while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtdvpfdabf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.feifeiyinyue.top/gttnywbaez.html

Ruby: while i < 10; i += 1; end
来源：http://hz.52xcode.cn/gtixfryeye.html

C#:   while (i < 10) { i++; }
来源：http://hz.ydjk.org.cn/gtewxpoedu.html

[B08] do-while（至少执行一次）
来源：http://hz.birdmap.top/gtriztxwli.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hammf.cn/gtscvohnfv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hysaishi.cn/gtmewhavqs.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtqdatkmkt.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtarwdhjqb.html

Java: do { i++; } while (i < 10);
来源：http://hz.cucudq.cn/gttlcphciy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nwbrower.top/gtnfxfzttj.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.svipenyu.cn/gtmkrkjfzi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtydhymxxj.html

[B09] break 与 continue
来源：http://hz.andypj.xyz/gtiswmhnps.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gotoacloud.top/gtdcabsnte.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj202588.top/gtyatqisbn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtxgsorviu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtaajasdgb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shuidangran.top/gtzhuvwnxv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hysaishi.cn/gtrrsuhffv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yueranfly.top/gtvjrchqmp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtkwxybvzk.html

[B10] 遍历同时拿索引
来源：http://hz.zhongyouzk.top/gtxpkkgrgv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhengqikj.top/gtokysvlvx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.svipenyu.cn/gtokggwfqs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.wangdashe.top/gthppykffh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sufxvd.cn/gtjujujjqk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.snrcjt.cn/gtsolfufzv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.havefunace.top/gtqyfeggik.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shanyushiyangkeji.top/gtlocgihhn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shuidangran.top/gtsvvqdtak.html

[B11] 生成数字序列 / 区间
来源：http://hz.fzhhl.top/gttyprbdhw.html

Py:   list(range(0, 10, 2))
来源：http://hz.hywenlv.cn/gtcrymlpcu.html

PHP:  range(0, 10, 2);
来源：http://hz.cdnleiting.top/gtyrdoiyeb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.0kj1m.cn/gtcfulphos.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tanke756.top/gtstgwhsyi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.dashuyun.cn/gtcoyulpqq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zycfv.cn/gtlmsxbski.html

Ruby: (0...10).step(2).to_a
来源：http://hz.tianlin.xyz/gthtcbbipp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.haohaochexian.top/gtpbkcgccb.html

[B12] 跳出多层循环
来源：http://hz.meibo888.top/gtxkttojuk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hysaishi.cn/gtrfffvhho.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sxryk.cn/gthzirssgo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.aizwys.cn/gtoyvlrgxe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtsyrenwvy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtjuykarvm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xingfuxueyuan.xyz/gtlbvgbuui.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sufxvd.cn/gthsgrbzsr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.redwolf501.top/gtehzrofic.html

[B13] 判断是否为数字
来源：http://hz.yueranfly.top/gtofhkzhbx.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtghndeebq.html

PHP:  is_numeric($x)
来源：http://hz.ybcxt.top/gtquxbqqit.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gtrudzumua.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jiagoushi.top/gthstwfiua.html

Java: x instanceof Number
来源：http://hz.shzxlz.cn/gtamrlhpkz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jqgufenzy.top/gtdthpfmhu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangtech.top/gtmrdptsmb.html

C#:   x is int or double or decimal
来源：http://hz.shangyingyoupin.top/gtfpxsqwpv.html

[B14] 判断值是否在集合内
来源：http://hz.hnqzz.top/gtfhqnclru.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nwbrower.top/gtoteoirin.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.fengsongda.top/gtjegikbpr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtywcwumah.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ybcxt.top/gtvxplcmur.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sxryk.cn/gtdojpaxkr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.sweek.top/gtfmjmstzh.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nwbrower.top/gtwsvspgam.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuanzhike.top/gtraxxbang.html

[B15] 布尔运算与取反
来源：http://hz.cucudq.cn/gtnbprisxq.html

Py:   a and b or not c
来源：http://hz.sxryk.cn/gtpqvvwuoi.html

PHP:  $a && $b || !$c
来源：http://hz.zycfv.cn/gtoshenkvs.html

JS:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gttfacwuqm.html

TS:   a && b || !c
来源：http://hz.ybcxt.top/gtatkagrbf.html

Java: a && b || !c
来源：http://hz.smart0.xyz/gtafvptwrs.html

Go:   a && b || !c
来源：http://hz.zhongyouzk.top/gtezqibmal.html

Ruby: a && b || !c
来源：http://hz.dashuyun.cn/gtofoupytl.html

C#:   a && b || !c
来源：http://hz.gaohongyu789.top/gtsuyasbea.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cashguo.top/gtebhthuqu.html

Py:   if not data: return
来源：http://hz.jinqigufen.top/gtsabsnyby.html

PHP:  if (!$data) { return; }
来源：http://hz.xinyue.icu/gtrmnbdpqh.html

JS:   if (!data) return;
来源：http://hz.ppjwa.cn/gtmhbnewix.html

TS:   if (!data) return;
来源：http://hz.sweek.top/gtclddpoan.html

Java: if (data == null) return;
来源：http://hz.hnqzz.top/gtjoqzcior.html

Go:   if data == nil { return }
来源：http://hz.zhoulong.xyz/gtsgqztlcr.html

Ruby: return if data.nil?
来源：http://hz.feifeiyinyue.top/gtzndvshqb.html

C#:   if (data == null) return;
来源：http://hz.hammf.cn/gtfkmwyghk.html

================================================================================
来源：http://hz.nanxinkj.top/gtrutvpbup.html

C. 函数与作用域
来源：http://hz.yj202588.top/gtkmbkfsoo.html

================================================================================
来源：http://hz.gogol.net.cn/gtfncbdqoz.html

[C01] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtbfedjson.html

Py:   def add(a, b): return a + b
来源：http://hz.fzhhl.top/gtxsnambri.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.dianchejie.cn/gtcexgmjac.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtlqabbrig.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtizpshyht.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtfnclwpgr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shangyingyoupin.top/gtavxrdwsa.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hammf.cn/gtkgdypqps.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtqcqrrmkg.html

[C02] 默认参数
来源：http://hz.xylfe.cn/gtmmtvhele.html

Py:   def greet(name="World"): return name
来源：http://hz.mhx1999.top/gtrznpxbwx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.haohaochexian.top/gtdjbqynws.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tian-w.cn/gtzvfkdduk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.guowangkeji.top/gtmnwjwdor.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yangfankeji.com/gtrnxhqpvz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgufenzy.top/gtzpgzcamj.html

Ruby: def greet(name = "World") = name
来源：http://hz.hfpthk.cn/gtcwalbsuh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yanxiufei.cn/gtllkpzdck.html

[C03] 可变参数
来源：http://hz.hywenlv.cn/gthnrsxpof.html

Py:   def total(*args): return sum(args)
来源：http://hz.redwolf501.top/gtrtmvsate.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xingfuxueyuan.xyz/gtqgzenpqy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtixwrpexs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtucitxngg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.kuanghao11.cn/gtrpgwlgdh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xylfe.cn/gttwtxkliv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gotoacloud.top/gtftpdnrmp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtrngqmtcf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sweek.top/gtieagniyi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hongshengwenyu.top/gtzzfvrynr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtnoxpctrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.nanxuanxn.top/gtpvoyfgwh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhoulong.xyz/gtoreovmcy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pengpengdd.cyou/gtfhsipdrq.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuanzhike.top/gtrkiszmfr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtabbievae.html

C#:   f(a: 1, b: 2)
来源：http://hz.ydjk.org.cn/gtbztrainb.html

[C05] 返回多个值
来源：http://hz.fengsongda.top/gtkhobgjer.html

Py:   return a, b
来源：http://hz.ydzc1.top/gtplsqwyxa.html

PHP:  return [$a, $b];
来源：http://hz.zhijiandao.cn/gtwvzsqkyd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.shzxlz.cn/gtwnvfdgpw.html

TS:   return { a, b };
来源：http://hz.hammf.cn/gtottjhebz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jiagoushi.top/gtrtoyunlq.html

Go:   return a, b
来源：http://hz.jinghuilouyu.cn/gtgouwbyei.html

Ruby: return a, b
来源：http://hz.zhengqikj.top/gtrbjiujgz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtylgmfcii.html

[C06] 匿名函数 / lambda
来源：http://hz.wangshuangyany.cn/gtqjyeuktp.html

Py:   square = lambda x: x * x
来源：http://hz.zhaomingkeji.xyz/gtlixaasby.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.svipenyu.cn/gtrxpuantv.html

JS:   const square = x => x * x;
来源：http://hz.meibo888.top/gtxtjdqclj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gzhubu.top/gtpvswatin.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.haohaochexian.top/gtuorbuzsr.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hnqzz.top/gtzxxsrbmd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.mhx1999.top/gthbqbdxzi.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.aibaodan.cn/gtbhfgmfdw.html

[C07] 把函数作为参数传入
来源：http://hz.gotoacloud.top/gtatqufbhv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.havefunace.top/gtmvomuuxg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hfpthk.cn/gtyahlumdv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuetiantiany.cn/gtmeqggsnq.html

TS:   arr.map(String)
来源：http://hz.wangdashe.top/gtzedctswq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.0kj1m.cn/gteyxzhyak.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.vqdsnc.cn/gtuzqjziiv.html

Ruby: arr.map(&:upcase)
来源：http://hz.shanyushiyangtech.top/gtcwtbkdvg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgufenzy.top/gtqqsfsiin.html

[C08] 闭包
来源：http://hz.xuetiantiany.cn/gtqfqwawlz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.shanyushiyangkeji.top/gtaqfkxrsk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigfzy.top/gtjcivgcnr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gthmcvvthj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtwdfgaexx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zdqjudy.top/gtmvasbouu.html


<!-- 参考信息 -->