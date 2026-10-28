代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.iojbl.cn/gtdftffljm.html

[A15] 空值判断与默认值
来源：http://hz.hfpthk.cn/gtudqqqhrd.html

Py:   value = data or "默认值"
来源：http://hz.chenzaomai.com/gtofddkgvx.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.sxryk.cn/gtddgqvvkk.html

JS:   const value = data ?? "默认值";
来源：http://hz.cqqwz.cn/gtmzsmjcph.html

TS:   const value = data ?? "默认值";
来源：http://hz.hnxiangtu.top/gtomvjlowb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.sysykeji.top/gtixblmjvl.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.hysaishi.cn/gtnevqonwt.html

Ruby: value = data || "默认值"
来源：http://hz.daria6918.cn/gtttcumvfe.html

C#:   var value = data ?? "默认值";
来源：http://hz.cdnleiting.top/gtwzfzwhzq.html

[A16] 真假值判断规则
来源：http://hz.sufxvd.cn/gtadezepgt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.shzxlz.cn/gtprlsteby.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sxryk.cn/gtlyxomiwp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhijiandao.cn/gtkgtfsqev.html

TS:   if (!x) {}
来源：http://hz.gotoacloud.top/gtvesgurmp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jqgufenzy.top/gtelywwold.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yuxming.cn/gtsfjcecqw.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.vqdsnc.cn/gtiudyluij.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.ivvv.top/gtynehurfl.html

[A17] 位运算
来源：http://hz.daxiang520.top/gtihinabib.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yvedp.cn/gtxqvlcark.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.quarkkingdee.top/gtjbcvvjrn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtmblcgnzt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.gotoacloud.top/gtklwmpzyw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinyuanbaomall.cn/gtakioaiur.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtxqxabmpd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cqqwz.cn/gtbfbnkecy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangdashe.top/gtdhavlfgo.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zdqjudy.top/gtwnagslcs.html

Py:   ord("A"); chr(65)
来源：http://hz.mhx1999.top/gtrwsdettm.html

PHP:  ord("A"); chr(65)
来源：http://hz.hnqzz.top/gtgnoojref.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxuanxn.top/gtcmvgtwkj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shanyushiyangtech.top/gtcxzzokox.html

Java: (int) 'A'; (char) 65
来源：http://hz.shanyushiyangkeji.top/gtmsxlpflm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yvedp.cn/gtodaqbgkx.html

Ruby: "A".ord; 65.chr
来源：http://hz.jinyuanbaomall.cn/gtvtwgubqy.html

C#:   (int)'A'; (char)65
来源：http://hz.aibaodan.cn/gtseofereg.html

[A19] 交换两个变量
来源：http://hz.jlsjyb.cn/gtfdkuchme.html

Py:   a, b = b, a
来源：http://hz.chenlongwang.top/gtjzwslgdl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.sysykeji.top/gtmmunqash.html

JS:   [a, b] = [b, a];
来源：http://hz.ivvv.top/gtuzwnhgou.html

TS:   [a, b] = [b, a];
来源：http://hz.nwbrower.top/gtyvwegzpr.html

Java: int t = a; a = b; b = t;
来源：http://hz.kuanghao11.cn/gtobeizbii.html

Go:   a, b = b, a
来源：http://hz.ydzc1.top/gtdqzrsxoc.html

Ruby: a, b = b, a
来源：http://hz.shanyushiyangkeji.top/gtawuslzki.html

C#:   (a, b) = (b, a);
来源：http://hz.havefunace.top/gttwwjrunc.html

[A20] 读取标准输入
来源：http://hz.yongpay.top/gtlmfubnty.html

Py:   name = input("请输入：")
来源：http://hz.xuanzx.com/gtfcctthjg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xuanzx.com/gtmjsiejah.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.chenjidiqi.icu/gtlrzpimno.html

TS:   // Node.js：readline 模块
来源：http://hz.9152youxi.cn/gttnhpvwvf.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.cdnleiting.top/gtlrnhirte.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.snrcjt.cn/gtoywtdlzu.html

Ruby: gets.chomp
来源：http://hz.hammf.cn/gtvsozwlkc.html

C#:   Console.ReadLine();
来源：http://hz.316326.xyz/gtsxcwvtnh.html

[A21] 保留指定小数位输出
来源：http://hz.wangshuangyany.cn/gtyiiqcesp.html

Py:   f"{3.14159:.2f}"
来源：http://hz.daria6918.cn/gttyjhdiuu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yangfankeji.com/gtaoujkdmb.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ivvv.top/gtvtpuzcwf.html

TS:   (3.14159).toFixed(2)
来源：http://hz.tianlin.xyz/gtlexrhdcv.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.feifeiyinyue.top/gtscicmytr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.redwolf501.top/gtgyialglo.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.iojbl.cn/gtpzyiistk.html

C#:   3.14159.ToString("F2")
来源：http://hz.hnqzz.top/gtfltjlbmd.html

[A22] 获取字符串长度
来源：http://hz.zhiwuduotai.top/gtdgdnmoie.html

Py:   len(s)
来源：http://hz.shangyingyoupin.top/gtvtxehocn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.snrcjt.cn/gtjswlpbem.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.chenjidiqi.icu/gthpqreiky.html

TS:   s.length
来源：http://hz.sufxvd.cn/gtmiwtrqfz.html

Java: s.length()
来源：http://hz.52xcode.cn/gteqgyxhkf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.shzxlz.cn/gtvaurgppe.html

Ruby: s.length
来源：http://hz.wangshuangyany.cn/gtliyiiigj.html

C#:   s.Length
来源：http://hz.guannengcc.top/gtgrqryvmi.html

[A23] 大小写转换
来源：http://hz.gogol.net.cn/gtkdqpquyi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jlsjyb.cn/gtwyicpapj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.hnqzz.top/gtuhhotitu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yongpay.top/gtvaoebvfl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.mhx1999.top/gtxyfbrhuu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jiagoushi.top/gtmcutssoz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.fengsongda.top/gtrcwxjhoh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.sysykeji.top/gtnxhcnqgd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.gogol.net.cn/gtqrsbngah.html

[A24] 去除首尾空白
来源：http://hz.hongshengwenyu.top/gtxexwcrwz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yj202588.top/gtwpxfygwf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.tianlin.xyz/gtgwynqjxx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yj20258888.top/gtlaujwixk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jlsjyb.cn/gtqmamszsb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.cheryme.top/gtuvbfyfbw.html

Go:   strings.TrimSpace(s)
来源：http://hz.nanxuanxn.top/gtpulfhfzx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ehwqpu.com/gtnqccssjq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cucudq.cn/gtlevoeynx.html

[A25] 字符串比较
来源：http://hz.zhijiandao.cn/gtpahofqjh.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shanyushiyangtech.top/gtfircolqj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yj20258888.top/gtewnnsubf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gogol.net.cn/gtqixpqryj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shzxlz.cn/gtvaoqbute.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xylfe.cn/gtkgojjolo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.dianchejie.cn/gtkddgtqrw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.fzhhl.top/gtbausacjf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jqgufenzy.top/gtpqqfotss.html

[A26] 类型转换总览
来源：http://hz.hnqzz.top/gtdwnrdinn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.iojbl.cn/gtavqobomd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.mhx1999.top/gtipxbqvti.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ehwqpu.com/gthwrkoyce.html

TS:   Number() String() Boolean() x as number
来源：http://hz.daxiang520.top/gtnpinqztr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.nanxinkj.top/gtjkwnrlzo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhongyouzk.top/gtpdzzqhsi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.svipenyu.cn/gthwlnanfi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yj20258.top/gtdhccjrbh.html

================================================================================
来源：http://hz.52xcode.cn/gtempejrkm.html

B. 流程控制
来源：http://hz.bjfxy.top/gtduhlzeht.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbwdcumcw.html

[B01] 条件判断 if / else
来源：http://hz.xuanzx.com/gtwmnieqws.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yongpay.top/gtngtzcees.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.shuidangran.top/gtrakopkse.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gtvjxdyoqk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cucudq.cn/gttyfeubsz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtczgvebbk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.guannengcc.top/gtpvwkgahm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.xuanzx.com/gtsyhbrnct.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yuanzhike.top/gthabtzimf.html

[B02] 多分支 else if / elif
来源：http://hz.dianchejie.cn/gtsbaauhzz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.daxiang520.top/gtgfcxoawv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shangyingyoupin.top/gtctmhtiko.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtrvpznubl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtjzjdhqyj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtwkecmjee.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.zhoulong.xyz/gtnemhsrxr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yj20258.top/gtoyrelghb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gturpawksn.html

[B03] switch / match / case
来源：http://hz.shangyingyoupin.top/gtvxtwvscv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.fzhhl.top/gtvauzjuif.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.dashuyun.cn/gtykvaqcld.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.dashuyun.cn/gtdlheasvx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cucudq.cn/gtlqhhzbfu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.mhx1999.top/gtdatedrai.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.daria6918.cn/gtwuvlyelv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhoulong.xyz/gtkpysznsu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cdnleiting.top/gtuxopsemw.html

[B04] for 计数循环
来源：http://hz.gotoacloud.top/gtvadusice.html

Py:   for i in range(10): print(i)
来源：http://hz.guannengcc.top/gtmsowtdhj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.guannengcc.top/gtepdmmrpi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinqigfzy.top/gtcukavewc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yongpay.top/gtgbfnqkgd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hongshengwenyu.top/gtmhgutygj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yj20258888.top/gtgbhiwchv.html

Ruby: 10.times { |i| puts i }
来源：http://hz.cqqwz.cn/gtsmgxxugb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.gzhubu.top/gtujiibluh.html

[B05] 遍历数组 / 列表
来源：http://hz.nwbrower.top/gtnbzzvrqr.html

Py:   for item in arr: print(item)
来源：http://hz.hnxiangtu.top/gtznevkylf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.nanxuanxn.top/gtzmryszmw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.daria6918.cn/gtahzrminw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuxming.cn/gtxruudshg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj20258888.top/gtkvqvknfi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ywan-chungtsiang.top/gtrihgbppb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.c1oappe.top/gtlwluhafq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jqgfzy.top/gtgoutggxh.html

[B06] 遍历字典 / 对象
来源：http://hz.jlsjyb.cn/gtwunmespx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yj20258.top/gtvckezfiv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hywenlv.cn/gtrsisqavi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shuidangran.top/gtxalgiecy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yongpay.top/gtofvdliqu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.aizwys.cn/gtgigoxlwm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.52xcode.cn/gtjvuokyug.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ivvv.top/gtuqqlhoel.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.haohaochexian.top/gtnbmxnjdw.html

[B07] while 循环
来源：http://hz.wangdashe.top/gtljngzmxh.html

Py:   while i < 10: i += 1
来源：http://hz.xingfuxueyuan.xyz/gtjnihwvdi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yj202588.top/gtobplaoyz.html

JS:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtfvrrxnfj.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gtgrjwdfal.html

Java: while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtotidhhrw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tanke756.top/gtfqgxxcly.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cheryme.top/gtuobxazdg.html

C#:   while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtxexeaxsw.html

[B08] do-while（至少执行一次）
来源：http://hz.gogol.net.cn/gthtqnstjx.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.snrcjt.cn/gtxaanbptt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.snrcjt.cn/gtkctnkgmw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtriazdgub.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtltcsuzmn.html

Java: do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gtzurfcxld.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yongpay.top/gtoztyxdjt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.daria6918.cn/gtqkudywjq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtzauopvja.html

[B09] break 与 continue
来源：http://hz.feifeiyinyue.top/gtfihtlffq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sysykeji.top/gtrsemeeos.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yangfankeji.com/gtiyahmkyq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtrxjcrlam.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtzvcsswpl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258.top/gttspdpyvg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.vqdsnc.cn/gtflslcsiu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shangyingyoupin.top/gtwdiwusyy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtbvtgmmhi.html

[B10] 遍历同时拿索引
来源：http://hz.pengpengdd.cyou/gtgkfijcet.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yuanzhike.top/gtcbtbdzsm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.iojbl.cn/gtgbvticto.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.havefunace.top/gtdanasbhw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gzhubu.top/gttbsxcfop.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hongshengwenyu.top/gttwykmicp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.vqdsnc.cn/gtcuelbobq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.vqdsnc.cn/gtpaawsyrd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ppjwa.cn/gtsrwcygsf.html

[B11] 生成数字序列 / 区间
来源：http://hz.gotoacloud.top/gtxsptudan.html

Py:   list(range(0, 10, 2))
来源：http://hz.ivvv.top/gtrjmnrhtq.html

PHP:  range(0, 10, 2);
来源：http://hz.yj202588.top/gtzyttabvl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenzaomai.com/gttflbhtgh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.havefunace.top/gtvubkquki.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinghuilouyu.cn/gtkbwelnmq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.tianlin.xyz/gtvwkealjg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.daria6918.cn/gtzotfgeax.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigufen.top/gtupxtdstt.html

[B12] 跳出多层循环
来源：http://hz.yuxming.cn/gthqidkvuq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jianghu66.top/gtmiozqozr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.fengsongda.top/gtaigshcla.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtumbiacja.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhoulong.xyz/gtrflisapx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtscjrpybs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hysaishi.cn/gtdajusisz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinghuilouyu.cn/gtsudzmgrb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.sysykeji.top/gtuumngsfv.html

[B13] 判断是否为数字
来源：http://hz.c1oappe.top/gtujhitxak.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhoulong.xyz/gtjtobxgbd.html

PHP:  is_numeric($x)
来源：http://hz.xziqi.cn/gtazvumavg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangtech.top/gtbhhevmbx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangkeji.top/gtmnbgxxgg.html

Java: x instanceof Number
来源：http://hz.sxryk.cn/gtuzzcwort.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shanyushiyangtech.top/gtlvweyrjn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhengqikj.top/gtrfqgxlxz.html

C#:   x is int or double or decimal
来源：http://hz.hnxiangtu.top/gtlpbmpkfr.html

[B14] 判断值是否在集合内
来源：http://hz.sysykeji.top/gtxqyegbhg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yj20258888.top/gtgvuvybyt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.0kj1m.cn/gtbmcwbkxa.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinghuilouyu.cn/gteyaxijfx.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shanyushiyangtech.top/gtozpxitsb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jianghu66.top/gtsnmyxpih.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xylfe.cn/gtrrfeqfbz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.vqdsnc.cn/gtyjfpkfhu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhengqikj.top/gtzfqdfiat.html

[B15] 布尔运算与取反
来源：http://hz.aizwys.cn/gtemkhwomy.html

Py:   a and b or not c
来源：http://hz.wangshuangyany.cn/gtjesawjzo.html

PHP:  $a && $b || !$c
来源：http://hz.sufxvd.cn/gtvynyejju.html

JS:   a && b || !c
来源：http://hz.jqgfzy.top/gtluqxewag.html

TS:   a && b || !c
来源：http://hz.haohaochexian.top/gtddrwalks.html

Java: a && b || !c
来源：http://hz.meibo888.top/gtixwtaepz.html

Go:   a && b || !c
来源：http://hz.tanke756.top/gtltuixpyy.html

Ruby: a && b || !c
来源：http://hz.jqgufenzy.top/gtborputyk.html

C#:   a && b || !c
来源：http://hz.hnxiangtu.top/gtppuixadl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gotoacloud.top/gtofhokpvr.html

Py:   if not data: return
来源：http://hz.hammf.cn/gtlsejywko.html

PHP:  if (!$data) { return; }
来源：http://hz.hywenlv.cn/gtdznjutit.html

JS:   if (!data) return;
来源：http://hz.jiagoushi.top/gtqrokybph.html

TS:   if (!data) return;
来源：http://hz.smart0.xyz/gtizlalbhv.html

Java: if (data == null) return;
来源：http://hz.fengsongda.top/gtdusmyjkh.html

Go:   if data == nil { return }
来源：http://hz.smart0.xyz/gtyutjnelf.html

Ruby: return if data.nil?
来源：http://hz.zhongyouzk.top/gtxyrvyvsa.html

C#:   if (data == null) return;
来源：http://hz.daxiang520.top/gtnqeefvkr.html

================================================================================
来源：http://hz.cucudq.cn/gtuldsjwbw.html

C. 函数与作用域
来源：http://hz.wangshuangyany.cn/gtzkknrnee.html

================================================================================
来源：http://hz.jinqigufen.top/gtwckvrqji.html

[C01] 定义函数
来源：http://hz.daxiang520.top/gtrsuftoyu.html

Py:   def add(a, b): return a + b
来源：http://hz.zhixingplan.top/gtdvpbdecd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtqubygrzq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fengsongda.top/gthpnfiolp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtzonblnjn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.guowangkeji.top/gtmrogqyda.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sufxvd.cn/gtsmthfsda.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnxiangtu.top/gtnscourqh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtaqoualgd.html

[C02] 默认参数
来源：http://hz.jinyuanbaomall.cn/gttnqvzbkq.html

Py:   def greet(name="World"): return name
来源：http://hz.havefunace.top/gtbderpjxn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hnqzz.top/gtopkktjsi.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtitumjozj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuxming.cn/gtxspgjvfd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hammf.cn/gtvsfhczsi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.tanke756.top/gtrabfjpvz.html

Ruby: def greet(name = "World") = name
来源：http://hz.meibo888.top/gtbarylliu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hammf.cn/gtlnoliqbf.html

[C03] 可变参数
来源：http://hz.jinghuilouyu.cn/gtdadfdrjr.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhengqikj.top/gtsntnbimr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangshuangyany.cn/gtqhdjdvmh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hfpthk.cn/gtbdumtjxq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ydjk.org.cn/gttjeqpdgj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hywenlv.cn/gtabnvnsxi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yueranfly.top/gtipvlgtdl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sweek.top/gtgcdsclks.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cashguo.top/gtsabcuvcm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tian-w.cn/gtpmevavez.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangtech.top/gtbbxaqfau.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.quarkkingdee.top/gtkcalfwco.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.0kj1m.cn/gtdygdoezh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhoulong.xyz/gtofzwojnd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.wangshuangyany.cn/gtqsbxcpjo.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuanzhike.top/gtoxffynuq.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shanyushiyangtech.top/gtenyrspsy.html

C#:   f(a: 1, b: 2)
来源：http://hz.hnxiangtu.top/gtveljmgix.html

[C05] 返回多个值
来源：http://hz.yonumen.top/gtmixdblmg.html

Py:   return a, b
来源：http://hz.chenjidiqi.icu/gtkmgkvqgn.html

PHP:  return [$a, $b];
来源：http://hz.smart0.xyz/gtojzjinen.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.guannengcc.top/gtoizgqfio.html

TS:   return { a, b };
来源：http://hz.xuetiantiany.cn/gtcgtlzgsj.html


<!-- 参考信息 -->