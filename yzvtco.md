代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.andypj.xyz/gtwcrltkmv.html

C#:   var value = data ?? "默认值";
来源：http://hz.shanyushiyangtech.top/gthafwbjce.html

[A16] 真假值判断规则
来源：http://hz.c1oappe.top/gtbxtvdblz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yuxming.cn/gtvlzfaniv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sysykeji.top/gtckazgage.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hnqzz.top/gtysapcvmo.html

TS:   if (!x) {}
来源：http://hz.hfpthk.cn/gtiojtrhje.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.sxryk.cn/gtlinzwmjm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.0kj1m.cn/gttrkwgcvx.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.yj20258.top/gtrrtmlpps.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yj20258888.top/gtumyotukj.html

[A17] 位运算
来源：http://hz.kuanghao11.cn/gtctvkaxhc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gaohongyu789.top/gtghskepbd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.shzxlz.cn/gtsqrpvfgf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xylfe.cn/gtyqnabwfm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.mhx1999.top/gtrlsisclc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jqgufenzy.top/gtdxoogluo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtsdjuxqnq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sxryk.cn/gtyoyqmfqx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenlongwang.top/gtaxxvejaw.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ehwqpu.com/gtcknwsveb.html

Py:   ord("A"); chr(65)
来源：http://hz.zhiwuduotai.top/gtuzjbvqpa.html

PHP:  ord("A"); chr(65)
来源：http://hz.hongshengwenyu.top/gtktdkxfam.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hammf.cn/gtoazqkppy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.smart0.xyz/gtdbyidojw.html

Java: (int) 'A'; (char) 65
来源：http://hz.cqqwz.cn/gtsvmmrzdc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.0kj1m.cn/gtuzkdmxxr.html

Ruby: "A".ord; 65.chr
来源：http://hz.yongpay.top/gtqzbpsisf.html

C#:   (int)'A'; (char)65
来源：http://hz.jianghu66.top/gtzknxtvsc.html

[A19] 交换两个变量
来源：http://hz.nanxuanxn.top/gtapvuglgh.html

Py:   a, b = b, a
来源：http://hz.gaohongyu789.top/gtjpkvfmmk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.cdnleiting.top/gtadqpgetu.html

JS:   [a, b] = [b, a];
来源：http://hz.fzhhl.top/gtkptkkzay.html

TS:   [a, b] = [b, a];
来源：http://hz.shanyushiyangkeji.top/gtlvopgfxv.html

Java: int t = a; a = b; b = t;
来源：http://hz.cdnleiting.top/gttfqwwfsj.html

Go:   a, b = b, a
来源：http://hz.yj202588.top/gttctgtumb.html

Ruby: a, b = b, a
来源：http://hz.yongpay.top/gtimezjsur.html

C#:   (a, b) = (b, a);
来源：http://hz.zycfv.cn/gtbkhyzecj.html

[A20] 读取标准输入
来源：http://hz.yangfankeji.com/gtexhdugwj.html

Py:   name = input("请输入：")
来源：http://hz.xuetiantiany.cn/gtljhyaedo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ybcxt.top/gthijnmluq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xinyue.icu/gtblfhjfhh.html

TS:   // Node.js：readline 模块
来源：http://hz.mhx1999.top/gtrdrstwud.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.sysykeji.top/gtmxlziwmy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.dianchejie.cn/gtihlzaahf.html

Ruby: gets.chomp
来源：http://hz.yj202588.top/gtxhygyszn.html

C#:   Console.ReadLine();
来源：http://hz.quarkkingdee.top/gtelcgwetg.html

[A21] 保留指定小数位输出
来源：http://hz.xuetiantiany.cn/gtztqdmtay.html

Py:   f"{3.14159:.2f}"
来源：http://hz.tianlin.xyz/gtijvvgoqo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cheryme.top/gtsogmtxpy.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yanxiufei.cn/gtopjxhzbe.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jqgfzy.top/gtmlovnwlv.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shanyushiyangtech.top/gthuevuxmp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gtnhafadzo.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.havefunace.top/gtopnovvwh.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhoulong.xyz/gttymrmupz.html

[A22] 获取字符串长度
来源：http://hz.wangdashe.top/gtpmklzyvf.html

Py:   len(s)
来源：http://hz.yj20258888.top/gtnwczogyc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jyoumei.cn/gtrxcnqgwi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.cheryme.top/gtzoghmuyg.html

TS:   s.length
来源：http://hz.daxiang520.top/gtodotmgrm.html

Java: s.length()
来源：http://hz.gotoacloud.top/gtdllseocn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.chenzaomai.com/gtfzxyqrge.html

Ruby: s.length
来源：http://hz.shanyushiyangkeji.top/gttkfzbmmx.html

C#:   s.Length
来源：http://hz.quarkkingdee.top/gtoytfweme.html

[A23] 大小写转换
来源：http://hz.hywenlv.cn/gtugjbaxgy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ehwqpu.com/gtanhklmwz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.redwolf501.top/gtlzgmydau.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zdqjudy.top/gtgmnezpsy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.nanxinkj.top/gtrgeckslb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.c1oappe.top/gtmlmtimww.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.wangshuangyany.cn/gtcypkskhd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yuxming.cn/gtazpqmqjg.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.sxryk.cn/gtqnuyihck.html

[A24] 去除首尾空白
来源：http://hz.shanyushiyangtech.top/gtbjiwvmyj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.hysaishi.cn/gtaksmjufd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yj20258.top/gtqfqwqxpy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenzaomai.com/gtblpdzysb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.quarkkingdee.top/gtsidzqyrt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xinyue.icu/gtyfyjpqiz.html

Go:   strings.TrimSpace(s)
来源：http://hz.sufxvd.cn/gtykdivfsx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.snrcjt.cn/gtrfxwyeoy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.mhx1999.top/gtbtqhrgbu.html

[A25] 字符串比较
来源：http://hz.zdqjudy.top/gtqwuqxppm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yonumen.top/gtarheakqq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.tian-w.cn/gtytkiauwl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhixingplan.top/gtwgfahdlp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gotoacloud.top/gtsbjrgdwo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.birdmap.top/gtivluimcw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhixingplan.top/gtfsaoorlz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.wangshuangyany.cn/gtzjbysdcn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yuxming.cn/gtsoljsfdp.html

[A26] 类型转换总览
来源：http://hz.hywenlv.cn/gtdgywcbzu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhoulong.xyz/gtmqpxaozu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xylfe.cn/gtefmhawme.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhaomingkeji.xyz/gtclljvyem.html

TS:   Number() String() Boolean() x as number
来源：http://hz.nanxinkj.top/gtcmslokmn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jlsjyb.cn/gtliflssyx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenjidiqi.icu/gtdrwgcsvb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.gotoacloud.top/gtcrfqvuuv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.snrcjt.cn/gtzjdsyafc.html

================================================================================
来源：http://hz.gotoacloud.top/gtujowcura.html

B. 流程控制
来源：http://hz.sufxvd.cn/gtqaycwtum.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtgklbowdq.html

[B01] 条件判断 if / else
来源：http://hz.yuxming.cn/gtusmvkssz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.nanxuanxn.top/gtvzueopzn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jqgufenzy.top/gtadzdrmko.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.pengpengdd.cyou/gtdwwegdgu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangtech.top/gtiusizawp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtxanbbisg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xziqi.cn/gtmkmdpumq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yvedp.cn/gtmvvjsfce.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.haohaochexian.top/gtsucmpafv.html

[B02] 多分支 else if / elif
来源：http://hz.guowangkeji.top/gtvkxyjnyy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yueranfly.top/gtqdhrpnaj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jyoumei.cn/gtkmypauso.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtytrceydb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cheryme.top/gtvijeocco.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtchkefogk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.pycfn.com/gtrvrpufpc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.fzhhl.top/gtjjvtllyf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gzhubu.top/gtuqbprens.html

[B03] switch / match / case
来源：http://hz.cucudq.cn/gtrzruzoxn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.zycfv.cn/gtmhnzcxxx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.guannengcc.top/gtrxycuggc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xinyue.icu/gtxhvvjtpj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxinkj.top/gtonwhxygn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.iojbl.cn/gtgdimspwc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yj20258.top/gtydrfquvw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cdnleiting.top/gtfozssjrr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.fzhhl.top/gtgaethmbb.html

[B04] for 计数循环
来源：http://hz.svipenyu.cn/gtrsgjcadx.html

Py:   for i in range(10): print(i)
来源：http://hz.cqqwz.cn/gtubofgfsi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jiagoushi.top/gtuutuexed.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.havefunace.top/gtavvlkzmb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangshuangyany.cn/gtdkwzkohd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhongyouzk.top/gtuamdvjgw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xinyue.icu/gtkjpyyxfq.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shuidangran.top/gtgcsskjoj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.cashguo.top/gtgscsvoyi.html

[B05] 遍历数组 / 列表
来源：http://hz.tian-w.cn/gtmgszatdy.html

Py:   for item in arr: print(item)
来源：http://hz.pycfn.com/gtviwtkogt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yueranfly.top/gtszppcsqi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenzaomai.com/gtbpdzjchg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.meibo888.top/gtjkgdxppp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.52xcode.cn/gtuuybxjfp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.pycfn.com/gtlaxamwrw.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yangfankeji.com/gtmfeddceq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.nanxinkj.top/gtmbcgwukl.html

[B06] 遍历字典 / 对象
来源：http://hz.tanke756.top/gtqpolbnse.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuxming.cn/gtxmhflbqm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yj20258.top/gtkaulnpwm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shuidangran.top/gtptlbojzp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.9152youxi.cn/gtwxzdfytx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.nanxuanxn.top/gtoaxbsode.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinyuanbaomall.cn/gtoxlfwxyv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jiagoushi.top/gtjziybyuj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.tianlin.xyz/gtspcsxhmf.html

[B07] while 循环
来源：http://hz.yvedp.cn/gtnvjgywau.html

Py:   while i < 10: i += 1
来源：http://hz.shanyushiyangtech.top/gtnbtnnnxn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gzhubu.top/gtngpoodpy.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhijiandao.cn/gtjwciikhl.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gthbgnjdgw.html

Java: while (i < 10) { i++; }
来源：http://hz.andypj.xyz/gtxybgwgid.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.sweek.top/gtuigaqqnl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.dianchejie.cn/gtskrtntcg.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtwsqzpskn.html

[B08] do-while（至少执行一次）
来源：http://hz.guowangkeji.top/gtcgitrpvj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuanzx.com/gtxofjrjdz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sxryk.cn/gtzmaxtwis.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hysaishi.cn/gtidknpuzw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtyiketadj.html

Java: do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtbqvtdsrd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.smart0.xyz/gtrxkomnka.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pycfn.com/gtflzlupvp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtriplskwg.html

[B09] break 与 continue
来源：http://hz.yj20258.top/gtaybqtbwi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.cucudq.cn/gtgmctmlea.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.c1oappe.top/gtnrjtatra.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtshoycuei.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtkjdfxyqw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtrwrihrtc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yongpay.top/gtyvmbyule.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinghuilouyu.cn/gtwccoeoan.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtwknsanmm.html

[B10] 遍历同时拿索引
来源：http://hz.wangdashe.top/gtmivswtjw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.tianlin.xyz/gtceptfday.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.mhx1999.top/gtcbupirxf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.cashguo.top/gtzhwgccul.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtmpabqjjh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.gogol.net.cn/gtmtvsoasn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hammf.cn/gtiwurnevx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.chenlongwang.top/gtnadppuzt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yueranfly.top/gtkjctsvrr.html

[B11] 生成数字序列 / 区间
来源：http://hz.jlsjyb.cn/gtgtmlkeps.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhiwuduotai.top/gtzxzszbqm.html

PHP:  range(0, 10, 2);
来源：http://hz.jianghu66.top/gtbjyaczjm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtkenkklor.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jqgfzy.top/gtjgmfpxih.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.birdmap.top/gtdzjinwvj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yvedp.cn/gtbbwgjejh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenlongwang.top/gtsocthvee.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigfzy.top/gtxkmszxpp.html

[B12] 跳出多层循环
来源：http://hz.gotoacloud.top/gtvmzpvgbx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.birdmap.top/gtrymswkhl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guannengcc.top/gtasvjvmox.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtwxvvrurd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hfpthk.cn/gtpzdnenlq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtoxgtbflk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yuanzhike.top/gthkvbnymq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.sxryk.cn/gtfzkhauxh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zdqjudy.top/gtmbcxynnw.html

[B13] 判断是否为数字
来源：http://hz.yonumen.top/gtmgrjtkgo.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnqzz.top/gtmgvnvurs.html

PHP:  is_numeric($x)
来源：http://hz.xuanzx.com/gtsepavizc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ehwqpu.com/gtbvfjsuzf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydzc1.top/gtzlcjrsod.html

Java: x instanceof Number
来源：http://hz.hnxiangtu.top/gtoeodezwt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gzhubu.top/gtlqbngbio.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sufxvd.cn/gtgfbpzpyo.html

C#:   x is int or double or decimal
来源：http://hz.dashuyun.cn/gtilinxlbp.html

[B14] 判断值是否在集合内
来源：http://hz.xuetiantiany.cn/gtqghpatcw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yonumen.top/gtezuzmwbd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yueranfly.top/gtprahswls.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.meibo888.top/gtgojyquyj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.mhx1999.top/gtcrezzxpo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jiagoushi.top/gtczoljxkr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zdqjudy.top/gtcbzxdedn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gzhubu.top/gtwcxotfxy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuxming.cn/gtvibafjts.html

[B15] 布尔运算与取反
来源：http://hz.cqqwz.cn/gtnznlanwn.html

Py:   a and b or not c
来源：http://hz.ehwqpu.com/gtptcepjxu.html

PHP:  $a && $b || !$c
来源：http://hz.zycfv.cn/gtqcnqevwo.html

JS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtkywlfqhn.html

TS:   a && b || !c
来源：http://hz.ydzc1.top/gtlzgkdool.html

Java: a && b || !c
来源：http://hz.shangyingyoupin.top/gtpfsixgyx.html

Go:   a && b || !c
来源：http://hz.yangfankeji.com/gtnujvfcyz.html

Ruby: a && b || !c
来源：http://hz.feifeiyinyue.top/gttyghyjgc.html

C#:   a && b || !c
来源：http://hz.sweek.top/gtyyjlwcjj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ehwqpu.com/gtbgurjgzf.html

Py:   if not data: return
来源：http://hz.zhiwuduotai.top/gtvuufjbjn.html

PHP:  if (!$data) { return; }
来源：http://hz.jqgfzy.top/gtuurfmgio.html

JS:   if (!data) return;
来源：http://hz.ydjk.org.cn/gtyvsdutva.html

TS:   if (!data) return;
来源：http://hz.jinqigfzy.top/gtdtnnggot.html

Java: if (data == null) return;
来源：http://hz.guannengcc.top/gtfaembqze.html

Go:   if data == nil { return }
来源：http://hz.svipenyu.cn/gtvjahlmbm.html

Ruby: return if data.nil?
来源：http://hz.dashuyun.cn/gtyazdlktr.html

C#:   if (data == null) return;
来源：http://hz.nanxinkj.top/gtfcbwfink.html

================================================================================
来源：http://hz.sufxvd.cn/gthdtvacsp.html

C. 函数与作用域
来源：http://hz.guowangkeji.top/gthuqpemnw.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtdectxsml.html

[C01] 定义函数
来源：http://hz.yvedp.cn/gtiygzbxaw.html

Py:   def add(a, b): return a + b
来源：http://hz.dianchejie.cn/gtzfeuzbdp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtoxqqepzd.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtzianfurm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtfryqgrun.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtrzahqqmr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.hongshengwenyu.top/gtljtkerda.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jyoumei.cn/gtvebsndsy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gthqhxulwp.html

[C02] 默认参数
来源：http://hz.zhoulong.xyz/gtctxjmjuy.html

Py:   def greet(name="World"): return name
来源：http://hz.sufxvd.cn/gtklsxrvei.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.haohaochexian.top/gtfytntdvk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtltfyqajg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.andypj.xyz/gtegukqiry.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgufenzy.top/gtybczqioa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hywenlv.cn/gtnitlpczg.html

Ruby: def greet(name = "World") = name
来源：http://hz.c1oappe.top/gtmogznruj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenlongwang.top/gtqvaumauy.html

[C03] 可变参数
来源：http://hz.yuxming.cn/gttqznhqxb.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydjk.org.cn/gtoeqqlwms.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gtssifgcal.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtdorsaiic.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xinyue.icu/gtikcqtyna.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.c1oappe.top/gtnaovxcho.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgufenzy.top/gtzlmrfdmv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hnqzz.top/gtmbnpzqrz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.dashuyun.cn/gthuqjuacq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sxryk.cn/gtbnvdsvld.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cqqwz.cn/gtrmclzmyb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.0kj1m.cn/gtprpjhohz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhongyouzk.top/gtmehxnpim.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenlongwang.top/gtpgxuszjz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jlsjyb.cn/gtehtanbib.html

Go:   // 无：用配置结构体参数
来源：http://hz.vqdsnc.cn/gtgbkyqrsh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtqdkxlfqw.html

C#:   f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtckocycgp.html

[C05] 返回多个值
来源：http://hz.cheryme.top/gtzpaqczzx.html

Py:   return a, b
来源：http://hz.haohaochexian.top/gtqvlbctls.html

PHP:  return [$a, $b];
来源：http://hz.gzhubu.top/gtsngcvxwr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pengpengdd.cyou/gthvaerjuz.html

TS:   return { a, b };
来源：http://hz.shanyushiyangkeji.top/gtctnibtaw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gotoacloud.top/gtdojqnwuw.html

Go:   return a, b
来源：http://hz.nanxuanxn.top/gtcshoxetm.html

Ruby: return a, b
来源：http://hz.fengsongda.top/gthwjpuwij.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinghuilouyu.cn/gthjlxmtwe.html

[C06] 匿名函数 / lambda
来源：http://hz.zdqjudy.top/gtungevlqp.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtylzjtgic.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangkeji.top/gtdcfflvla.html

JS:   const square = x => x * x;
来源：http://hz.xuetiantiany.cn/gtrkfbhxal.html


<!-- 参考信息 -->