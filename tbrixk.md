代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.svipenyu.cn/gtrghyhzzm.html

Py:   ord("A"); chr(65)
来源：http://hz.gotoacloud.top/gtaiptfwpa.html

PHP:  ord("A"); chr(65)
来源：http://hz.ydjk.org.cn/gtheaoapel.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.iojbl.cn/gtgcdzjtik.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yj20258888.top/gtseqlshkj.html

Java: (int) 'A'; (char) 65
来源：http://hz.guowangkeji.top/gtlqeulutk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.bjfxy.top/gthqjvbpez.html

Ruby: "A".ord; 65.chr
来源：http://hz.sysykeji.top/gtbhlypjow.html

C#:   (int)'A'; (char)65
来源：http://hz.ybcxt.top/gthfflbbsa.html

[A19] 交换两个变量
来源：http://hz.shanyushiyangtech.top/gtnggvfjtk.html

Py:   a, b = b, a
来源：http://hz.nanxuanxn.top/gtevrwfvky.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.xziqi.cn/gtyoudlfoj.html

JS:   [a, b] = [b, a];
来源：http://hz.yj202588.top/gtpqgkidfs.html

TS:   [a, b] = [b, a];
来源：http://hz.sxryk.cn/gtveoamgzb.html

Java: int t = a; a = b; b = t;
来源：http://hz.redwolf501.top/gtarsnplqu.html

Go:   a, b = b, a
来源：http://hz.yj20258.top/gtprvmwves.html

Ruby: a, b = b, a
来源：http://hz.fzhhl.top/gtflhszizn.html

C#:   (a, b) = (b, a);
来源：http://hz.daxiang520.top/gtskpljjwu.html

[A20] 读取标准输入
来源：http://hz.hnqzz.top/gtlhyvonfy.html

Py:   name = input("请输入：")
来源：http://hz.ybcxt.top/gtueltkmda.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ppjwa.cn/gtlmdcbzme.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.shanyushiyangtech.top/gtaveklclg.html

TS:   // Node.js：readline 模块
来源：http://hz.cheryme.top/gttfsqitdg.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.52xcode.cn/gtvwqjtdwi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yj202588.top/gtbkhxqwam.html

Ruby: gets.chomp
来源：http://hz.ppjwa.cn/gtklymvvtw.html

C#:   Console.ReadLine();
来源：http://hz.yuxming.cn/gtgvvbrmnx.html

[A21] 保留指定小数位输出
来源：http://hz.yj202588.top/gtfnqismgh.html

Py:   f"{3.14159:.2f}"
来源：http://hz.nanxinkj.top/gtuccbymmf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.hammf.cn/gtduwcxqkj.html

JS:   (3.14159).toFixed(2)
来源：http://hz.pengpengdd.cyou/gtmriawypb.html

TS:   (3.14159).toFixed(2)
来源：http://hz.fzhhl.top/gtivhxwotb.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtgbtirwos.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.redwolf501.top/gtvyoixmqt.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.shzxlz.cn/gtvfufqolv.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj202588.top/gtcmsrximi.html

[A22] 获取字符串长度
来源：http://hz.cucudq.cn/gtajbuvxxd.html

Py:   len(s)
来源：http://hz.zhijiandao.cn/gthloidijb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.c1oappe.top/gtzybmjvso.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.ivvv.top/gtfunwlarl.html

TS:   s.length
来源：http://hz.chenlongwang.top/gtbawwpkcb.html

Java: s.length()
来源：http://hz.52xcode.cn/gtprssesfk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.0kj1m.cn/gtyarrejvj.html

Ruby: s.length
来源：http://hz.xylfe.cn/gtqvamomij.html

C#:   s.Length
来源：http://hz.snrcjt.cn/gtblbqgifp.html

[A23] 大小写转换
来源：http://hz.xinyue.icu/gtervmjffj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.tanke756.top/gttiytfqtm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.feifeiyinyue.top/gtigeycxmp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.meibo888.top/gtzdlutawe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.dashuyun.cn/gtqcgjults.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.quarkkingdee.top/gtqeldymfk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yangfankeji.com/gtjfdjvqxq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.feifeiyinyue.top/gtokdpbcuu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.zhiwuduotai.top/gtklekaneg.html

[A24] 去除首尾空白
来源：http://hz.gotoacloud.top/gtpfgxsycz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.havefunace.top/gtdffoohof.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.nwbrower.top/gtpacabczo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dianchejie.cn/gtcppyjbwu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cucudq.cn/gtssazyaid.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ppjwa.cn/gtgvvernbz.html

Go:   strings.TrimSpace(s)
来源：http://hz.nanxinkj.top/gtzipdvyrr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jqgufenzy.top/gthhndsnmd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.0kj1m.cn/gtikmgplfh.html

[A25] 字符串比较
来源：http://hz.tianlin.xyz/gthqojmidz.html

Py:   s1 == s2; s1 != s2
来源：http://hz.quarkkingdee.top/gtmqjwmeyy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.quarkkingdee.top/gtvghzooij.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.fzhhl.top/gtnnumdhol.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinqigfzy.top/gtntlwjwsb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zdqjudy.top/gtuhqprlla.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.iojbl.cn/gthqifyjgv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ehwqpu.com/gtpwcmpqqz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ppjwa.cn/gtvsktjplw.html

[A26] 类型转换总览
来源：http://hz.sysykeji.top/gtuybniwzf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xuetiantiany.cn/gtaavvksfp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yuxming.cn/gtshsucqws.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.bjfxy.top/gtwhwdhace.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ybcxt.top/gtdpectvsj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.sweek.top/gttlggmxzv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yongpay.top/gtspijbbei.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.zhixingplan.top/gttdzilnkf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.daria6918.cn/gtxgbxqvwr.html

================================================================================
来源：http://hz.zdqjudy.top/gtpemjawer.html

B. 流程控制
来源：http://hz.jianghu66.top/gtihjbtyui.html

================================================================================
来源：http://hz.zdqjudy.top/gtvongwjtz.html

[B01] 条件判断 if / else
来源：http://hz.zhixingplan.top/gtlbeglwim.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.quarkkingdee.top/gtywvdvdwi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.meibo888.top/gtnnbedvze.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fzhhl.top/gtwuxcsywz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.iojbl.cn/gtupdokjos.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.daria6918.cn/gtpybssvgx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.sysykeji.top/gtugztjhbo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jiagoushi.top/gtcahduwba.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gttpxiplxs.html

[B02] 多分支 else if / elif
来源：http://hz.zhongyouzk.top/gteawepuyf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.redwolf501.top/gtnxmiyfvl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tian-w.cn/gthbfdnnhq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtjnenprzn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtijcmtlgo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtlgtdaful.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sysykeji.top/gtaxtoqyku.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinghuilouyu.cn/gtydgnkxod.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtmolhmobd.html

[B03] switch / match / case
来源：http://hz.shuidangran.top/gtyloybfdn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.guannengcc.top/gtbmfqhxmz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hfpthk.cn/gtwmveorrx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cheryme.top/gtwccmmbbp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.havefunace.top/gtqhvrusgt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.pycfn.com/gtvtrodpzl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.aibaodan.cn/gtvauvhtss.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.aibaodan.cn/gtnmikqupp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hywenlv.cn/gtmdmywfii.html

[B04] for 计数循环
来源：http://hz.fengsongda.top/gtwurppliu.html

Py:   for i in range(10): print(i)
来源：http://hz.zdqjudy.top/gtmovhfgmk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zdqjudy.top/gtofjglloy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.quarkkingdee.top/gtkxgqxusd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangshuangyany.cn/gtjtuoxarh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yueranfly.top/gtmxnesrrh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.chenlongwang.top/gtlesfipfu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhijiandao.cn/gtxvbkwnea.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.wangdashe.top/gtehyajqti.html

[B05] 遍历数组 / 列表
来源：http://hz.9152youxi.cn/gtmbtvjboq.html

Py:   for item in arr: print(item)
来源：http://hz.ybcxt.top/gtvmtrrqpc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.cdnleiting.top/gtekgtjgti.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.nanxinkj.top/gtxxhgdhra.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtvztkleot.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhengqikj.top/gtukbfqtji.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.tanke756.top/gtsfteomnx.html

Ruby: arr.each { |item| puts item }
来源：http://hz.xuetiantiany.cn/gtvyoyivcm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.tanke756.top/gtcablqbkw.html

[B06] 遍历字典 / 对象
来源：http://hz.mhx1999.top/gtvnrolsdh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj20258.top/gtufgjhgdk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.fzhhl.top/gtyyadwmhc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yonumen.top/gthglbftxh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.meibo888.top/gtcrufvpxb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shuidangran.top/gtouunyjvb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xuetiantiany.cn/gtdbgvlcyy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xingfuxueyuan.xyz/gtbzewcrow.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.pycfn.com/gtbzlmtrdc.html

[B07] while 循环
来源：http://hz.dashuyun.cn/gtdlijbhmp.html

Py:   while i < 10: i += 1
来源：http://hz.guowangkeji.top/gtgjlwfnra.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.tianlin.xyz/gtaqgxovxw.html

JS:   while (i < 10) { i++; }
来源：http://hz.feifeiyinyue.top/gttgoksklk.html

TS:   while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gttnrsasax.html

Java: while (i < 10) { i++; }
来源：http://hz.yangfankeji.com/gtsykxvjnj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.ppjwa.cn/gtqiycvswv.html

Ruby: while i < 10; i += 1; end
来源：http://hz.redwolf501.top/gtggpegpup.html

C#:   while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtlkjfryde.html

[B08] do-while（至少执行一次）
来源：http://hz.xuanzx.com/gtlqnhhrfn.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxinkj.top/gtpkwroull.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.fzhhl.top/gtvkgaghzb.html

JS:   do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gtyeulyaje.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtqgsxvtfq.html

Java: do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtofsjmkbk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.smart0.xyz/gtnstfmggb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tian-w.cn/gtdwqlvmle.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtblrsdqyk.html

[B09] break 与 continue
来源：http://hz.vqdsnc.cn/gtyfrszndr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydjk.org.cn/gtcxcivckn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtmvwnbykz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gtuogicmvh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtoxjkbkqt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtrwrpfuyh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jiagoushi.top/gtbmfxvdnn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgfzy.top/gtjelqxfgj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ppjwa.cn/gtoblxmjmq.html

[B10] 遍历同时拿索引
来源：http://hz.daxiang520.top/gtyymhagzj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guannengcc.top/gtbyukfynk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shangyingyoupin.top/gtlytfeibc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.snrcjt.cn/gtsomubudh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtldfukgyd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xuanzx.com/gtaizkzgfz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.pycfn.com/gtnrdctvam.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hfpthk.cn/gtmxzvrpop.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hysaishi.cn/gtkfqedmzp.html

[B11] 生成数字序列 / 区间
来源：http://hz.shangyingyoupin.top/gtkkknowxv.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj202588.top/gtywyzcofc.html

PHP:  range(0, 10, 2);
来源：http://hz.gaohongyu789.top/gtvrwnmosm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yongpay.top/gtgpxjrqtj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtrumhqblc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hammf.cn/gtezlfizwg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.haohaochexian.top/gtjtydxvbb.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ybcxt.top/gtlaqqbznq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dianchejie.cn/gtqsxafqht.html

[B12] 跳出多层循环
来源：http://hz.zycfv.cn/gtxowngsdq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gzhubu.top/gtwmrgupox.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cucudq.cn/gtutpehdwh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.bjfxy.top/gtboiviqee.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtbrsdaitw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtvnfboxsm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xylfe.cn/gtbbwjobkl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhongyouzk.top/gtqbqzdoqo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sweek.top/gtjhxhgokn.html

[B13] 判断是否为数字
来源：http://hz.zhixingplan.top/gtlimasbzr.html

Py:   isinstance(x, (int, float))
来源：http://hz.ydjk.org.cn/gtyorhbddd.html

PHP:  is_numeric($x)
来源：http://hz.hfpthk.cn/gtbocccihc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnxiangtu.top/gtujkbxgqu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtieyxfrle.html

Java: x instanceof Number
来源：http://hz.gogol.net.cn/gtjarkvgmz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xinyue.icu/gtokqifevu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yvedp.cn/gtlzvtigtl.html

C#:   x is int or double or decimal
来源：http://hz.haohaochexian.top/gtwljckuik.html

[B14] 判断值是否在集合内
来源：http://hz.zhijiandao.cn/gtlqbosoyp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ydjk.org.cn/gttdyjivwh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.tanke756.top/gtiynnxlbf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.andypj.xyz/gtalnhszur.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shangyingyoupin.top/gtsxvfswao.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gaohongyu789.top/gtvqlrfiqx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xuanzx.com/gtbpkhczoa.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hongshengwenyu.top/gtezllxlal.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zycfv.cn/gtethaltfh.html

[B15] 布尔运算与取反
来源：http://hz.jinghuilouyu.cn/gtfbwhwgua.html

Py:   a and b or not c
来源：http://hz.nanxuanxn.top/gtseqpkhlu.html

PHP:  $a && $b || !$c
来源：http://hz.meibo888.top/gtnbxuzdbl.html

JS:   a && b || !c
来源：http://hz.nanxuanxn.top/gtuiyrfdnc.html

TS:   a && b || !c
来源：http://hz.gzhubu.top/gtechqnyfa.html

Java: a && b || !c
来源：http://hz.316326.xyz/gtvdaxhcgh.html

Go:   a && b || !c
来源：http://hz.cqqwz.cn/gtqckuasml.html

Ruby: a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtbtghxisc.html

C#:   a && b || !c
来源：http://hz.yj20258.top/gtlbcvkqfb.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zycfv.cn/gtxuxneviu.html

Py:   if not data: return
来源：http://hz.gaohongyu789.top/gtpirktxnt.html

PHP:  if (!$data) { return; }
来源：http://hz.yueranfly.top/gtiyqsvuww.html

JS:   if (!data) return;
来源：http://hz.xylfe.cn/gtsyejhbob.html

TS:   if (!data) return;
来源：http://hz.hammf.cn/gtypgpcxip.html

Java: if (data == null) return;
来源：http://hz.hammf.cn/gticffldgo.html

Go:   if data == nil { return }
来源：http://hz.jiagoushi.top/gtfcnymqot.html

Ruby: return if data.nil?
来源：http://hz.svipenyu.cn/gtanlusial.html

C#:   if (data == null) return;
来源：http://hz.jqgfzy.top/gtfyszkyph.html

================================================================================
来源：http://hz.guowangkeji.top/gtvkbmwauf.html

C. 函数与作用域
来源：http://hz.dianchejie.cn/gtszzegzdf.html

================================================================================
来源：http://hz.ybcxt.top/gthbkcvikb.html

[C01] 定义函数
来源：http://hz.nanxuanxn.top/gtbhrbvpus.html

Py:   def add(a, b): return a + b
来源：http://hz.ywan-chungtsiang.top/gtewsbrgak.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtbktwgpjk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cucudq.cn/gtloenuxvw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinghuilouyu.cn/gtigopxsiv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtyetdvcwv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ehwqpu.com/gtdbymhgvg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gaohongyu789.top/gtdfzqbnni.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtsrmcmuib.html

[C02] 默认参数
来源：http://hz.sufxvd.cn/gtiufiecfk.html

Py:   def greet(name="World"): return name
来源：http://hz.haohaochexian.top/gtezvwutat.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.nanxuanxn.top/gtwnudmuia.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pengpengdd.cyou/gtogfvgcre.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.redwolf501.top/gtpmgcrgja.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxuanxn.top/gteufvjtgo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.wangdashe.top/gtcsysesnj.html

Ruby: def greet(name = "World") = name
来源：http://hz.tian-w.cn/gtsygakhei.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zdqjudy.top/gthpapwoqa.html

[C03] 可变参数
来源：http://hz.jinqigufen.top/gtvrirbgvq.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydzc1.top/gtzpvzsnhp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxuanxn.top/gtftonfjnh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aibaodan.cn/gtzsyqakvr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtodxbiydw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtdtyxjdvx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daxiang520.top/gtuwbqgsus.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zdqjudy.top/gtfbjxxrep.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shzxlz.cn/gtkrbsyfhm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yongpay.top/gththpuxwd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daria6918.cn/gtqnomqjnt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtpxjdfcgn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.xylfe.cn/gtpzryamae.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.ywan-chungtsiang.top/gtyiuvedym.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.feifeiyinyue.top/gtfjfbqxxv.html

Go:   // 无：用配置结构体参数
来源：http://hz.yonumen.top/gtavguugos.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shzxlz.cn/gtvsyfnmqq.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtrzxknecp.html

[C05] 返回多个值
来源：http://hz.yongpay.top/gtzgprhzvh.html

Py:   return a, b
来源：http://hz.xuetiantiany.cn/gtlmkjhpmp.html

PHP:  return [$a, $b];
来源：http://hz.sufxvd.cn/gtdbtmlyni.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jianghu66.top/gtrhofcrgg.html

TS:   return { a, b };
来源：http://hz.dashuyun.cn/gtlmlfwecz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yangfankeji.com/gtdzwmpazw.html

Go:   return a, b
来源：http://hz.yanxiufei.cn/gthtxbumpz.html

Ruby: return a, b
来源：http://hz.sysykeji.top/gtlsozmfbz.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xziqi.cn/gthfwafvir.html

[C06] 匿名函数 / lambda
来源：http://hz.zdqjudy.top/gtnitzuyow.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangkeji.top/gtzfiouupk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hywenlv.cn/gtupedfywu.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gtxhhcbwhl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zycfv.cn/gtldzuqzes.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.hnxiangtu.top/gtegtunbja.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhoulong.xyz/gtxfspcndf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sufxvd.cn/gtbbmpmyhh.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.guannengcc.top/gtsxbwxssj.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtboxodkaq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.aizwys.cn/gtydadfolb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenjidiqi.icu/gtrnuqbenc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shanyushiyangkeji.top/gturhdcfhl.html

TS:   arr.map(String)
来源：http://hz.yuxming.cn/gtdebxgrii.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shangyingyoupin.top/gtfktjdbcx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zdqjudy.top/gthinehsvp.html

Ruby: arr.map(&:upcase)
来源：http://hz.vqdsnc.cn/gtbphlaooz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jlsjyb.cn/gtmyxpjber.html

[C08] 闭包
来源：http://hz.zdqjudy.top/gtuuzjvsjd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinghuilouyu.cn/gtqwifpqpt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuanzx.com/gtrirueibz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gthmyccioo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.nanxuanxn.top/gteovbddnp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aibaodan.cn/gtnjqdekzq.html


<!-- 参考信息 -->