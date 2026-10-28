代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.gotoacloud.top/gtjmwwuzrw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xinyue.icu/gtclotxzph.html

TS:   if (!x) {}
来源：http://hz.shanyushiyangtech.top/gtfedaqwwa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.bjfxy.top/gtosbhxfxp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.birdmap.top/gtzhnmalmh.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zdqjudy.top/gtgzjrhpdw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.shanyushiyangkeji.top/gtrworhlec.html

[A17] 位运算
来源：http://hz.dianchejie.cn/gtdyijyydb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gthdwvticz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.zdqjudy.top/gttuenwtlt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jqgfzy.top/gtkvqwnqhs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gtxutbnaiw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ybcxt.top/gtcgsnkifi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtdhurukjx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtaetryfeq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtdjwvlnks.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jianghu66.top/gtwbsspuzh.html

Py:   ord("A"); chr(65)
来源：http://hz.sweek.top/gtnlptdeqt.html

PHP:  ord("A"); chr(65)
来源：http://hz.hongshengwenyu.top/gtjvdevxxi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xuetiantiany.cn/gtfonlfusr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinqigufen.top/gtxupbfurc.html

Java: (int) 'A'; (char) 65
来源：http://hz.cashguo.top/gtijruhrxf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.chenzaomai.com/gtqbrhkbgx.html

Ruby: "A".ord; 65.chr
来源：http://hz.52xcode.cn/gtknwlsglx.html

C#:   (int)'A'; (char)65
来源：http://hz.zycfv.cn/gtuxoynxoy.html

[A19] 交换两个变量
来源：http://hz.jyoumei.cn/gtnvnuxwkw.html

Py:   a, b = b, a
来源：http://hz.jyoumei.cn/gtdskngpir.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.gzhubu.top/gtvepdravw.html

JS:   [a, b] = [b, a];
来源：http://hz.gotoacloud.top/gtezlutrzd.html

TS:   [a, b] = [b, a];
来源：http://hz.chenzaomai.com/gttevsirok.html

Java: int t = a; a = b; b = t;
来源：http://hz.yvedp.cn/gtnxfvgkxr.html

Go:   a, b = b, a
来源：http://hz.xuanzx.com/gtiqguptow.html

Ruby: a, b = b, a
来源：http://hz.yuxming.cn/gtekykstif.html

C#:   (a, b) = (b, a);
来源：http://hz.nanxinkj.top/gtisjrwdmi.html

[A20] 读取标准输入
来源：http://hz.9152youxi.cn/gtfgbofpsa.html

Py:   name = input("请输入：")
来源：http://hz.52xcode.cn/gtcdmjjznr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hammf.cn/gthpktaiau.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.smart0.xyz/gtmpnsnsyx.html

TS:   // Node.js：readline 模块
来源：http://hz.yueranfly.top/gtaosutvtr.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.tian-w.cn/gteaofpgak.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ehwqpu.com/gtcblbwzco.html

Ruby: gets.chomp
来源：http://hz.yonumen.top/gtwxeqpurs.html

C#:   Console.ReadLine();
来源：http://hz.xinyue.icu/gtngexxhcj.html

[A21] 保留指定小数位输出
来源：http://hz.wangdashe.top/gtywjxmxvi.html

Py:   f"{3.14159:.2f}"
来源：http://hz.wangshuangyany.cn/gthbmkhvmr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.xingfuxueyuan.xyz/gtwdkchpqi.html

JS:   (3.14159).toFixed(2)
来源：http://hz.cashguo.top/gtdsenxgvw.html

TS:   (3.14159).toFixed(2)
来源：http://hz.feifeiyinyue.top/gtwraptjsb.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.redwolf501.top/gtazckteat.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.gzhubu.top/gtgbysvsnh.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yj202588.top/gtaxnmyrts.html

C#:   3.14159.ToString("F2")
来源：http://hz.guowangkeji.top/gtnjkoldpy.html

[A22] 获取字符串长度
来源：http://hz.sufxvd.cn/gtgccvxfiz.html

Py:   len(s)
来源：http://hz.zhongyouzk.top/gthrvkhwjd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.meibo888.top/gtkeneoakr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.cdnleiting.top/gtjhtdaxas.html

TS:   s.length
来源：http://hz.aizwys.cn/gtiyeuktoi.html

Java: s.length()
来源：http://hz.dianchejie.cn/gtbxanrrfc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.daria6918.cn/gtmjkuebhz.html

Ruby: s.length
来源：http://hz.jlsjyb.cn/gtoofivzkf.html

C#:   s.Length
来源：http://hz.jyoumei.cn/gtkfjjprfq.html

[A23] 大小写转换
来源：http://hz.yvedp.cn/gtmwavdhiv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.shanyushiyangtech.top/gtzplrwxcp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xylfe.cn/gtplnnaeal.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cqqwz.cn/gtumcexvsi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shuidangran.top/gtdkzchmuj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.feifeiyinyue.top/gtvqkvubab.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.cheryme.top/gtzxwedxpy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.feifeiyinyue.top/gttvwdbtml.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.sysykeji.top/gtdwffwuvz.html

[A24] 去除首尾空白
来源：http://hz.fzhhl.top/gtmibyhegi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.hammf.cn/gtdkuikyyx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ivvv.top/gtlinydugz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhaomingkeji.xyz/gtlmtodptz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cdnleiting.top/gtlbdntiez.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.chenjidiqi.icu/gtgxogwcbn.html

Go:   strings.TrimSpace(s)
来源：http://hz.jiagoushi.top/gtrfjffmim.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinqigufen.top/gtwvzdysvv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.hnqzz.top/gtkhdbvczi.html

[A25] 字符串比较
来源：http://hz.shanyushiyangkeji.top/gteqroopka.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jinghuilouyu.cn/gtpqeamsln.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.quarkkingdee.top/gtrrhgmsze.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shanyushiyangkeji.top/gtrrddpnpw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhixingplan.top/gtuhsunrnt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.pengpengdd.cyou/gtmjrnfuen.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yangfankeji.com/gttvcdsvxp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shanyushiyangtech.top/gtdvrabalf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhaomingkeji.xyz/gtexuhlsgl.html

[A26] 类型转换总览
来源：http://hz.havefunace.top/gtknfeufsu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhoulong.xyz/gtatdbxydg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hnxiangtu.top/gtbpspvbhj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.wangdashe.top/gtnfolvzyq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xuanzx.com/gtjajiejxc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.wangshuangyany.cn/gtwtyypthd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.mhx1999.top/gtqbchkpvy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.guannengcc.top/gtqkfvhffi.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xziqi.cn/gtsnknljhc.html

================================================================================
来源：http://hz.daxiang520.top/gtitcafbah.html

B. 流程控制
来源：http://hz.daria6918.cn/gtzmqxpvby.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjappbran.html

[B01] 条件判断 if / else
来源：http://hz.xziqi.cn/gtzliycktl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.snrcjt.cn/gtliteypeb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.fengsongda.top/gtbuzyylml.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.chenzaomai.com/gtenjkxjqa.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangtech.top/gtchjmwifh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gticvrirbu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.0kj1m.cn/gtlbqystcc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yonumen.top/gtnlvpdyqi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xingfuxueyuan.xyz/gtoonqiujx.html

[B02] 多分支 else if / elif
来源：http://hz.ivvv.top/gtrgindlli.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yj20258.top/gthpefyntd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zdqjudy.top/gtmnldekhy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtsqneogjm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhongyouzk.top/gtpqrqnhhr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.vqdsnc.cn/gtfmqcxgaw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.cheryme.top/gtypgbibei.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yj20258888.top/gtvwgfmsbu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtlvugrblm.html

[B03] switch / match / case
来源：http://hz.ppjwa.cn/gttlmzwagv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.zhengqikj.top/gtjzsuyaku.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhaomingkeji.xyz/gtbbzztxas.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj202588.top/gtgxjrswmu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gaohongyu789.top/gtqndoyofu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.dianchejie.cn/gtdvnjjzrv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.birdmap.top/gttabwxxmf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hongshengwenyu.top/gtqllzpbbz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.sweek.top/gtguortuzm.html

[B04] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtdwwvndcy.html

Py:   for i in range(10): print(i)
来源：http://hz.daria6918.cn/gtohyrffhl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yanxiufei.cn/gtgqdyuqpw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jyoumei.cn/gtacucyvck.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.9152youxi.cn/gtbdgjgoul.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhoulong.xyz/gtiqoteezn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.hywenlv.cn/gtoolchdxl.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ivvv.top/gtiapvhxpq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhengqikj.top/gtmwlnhqva.html

[B05] 遍历数组 / 列表
来源：http://hz.andypj.xyz/gtbhuczofz.html

Py:   for item in arr: print(item)
来源：http://hz.yongpay.top/gtdprzgtlg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jqgufenzy.top/gtwoudctnx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ybcxt.top/gtttjyjtkc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hammf.cn/gtrkjbwwbw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shanyushiyangkeji.top/gtjcdgshbp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cqqwz.cn/gtwaogpjqr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sysykeji.top/gtyhjmqatg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.9152youxi.cn/gtdhbaffxy.html

[B06] 遍历字典 / 对象
来源：http://hz.tanke756.top/gttxfgupbq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhiwuduotai.top/gtzazmfkfp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hywenlv.cn/gtlphbofuz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yonumen.top/gtilpmzpkm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ivvv.top/gtdktvivri.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.52xcode.cn/gtdodygwsq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ydzc1.top/gtaonummsx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jiagoushi.top/gtpsxfeuod.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cashguo.top/gthjpwhnuu.html

[B07] while 循环
来源：http://hz.xuetiantiany.cn/gtqfocrxqg.html

Py:   while i < 10: i += 1
来源：http://hz.chenlongwang.top/gtqtmvgrjr.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.shanyushiyangkeji.top/gtlyvpauns.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtlgzuxxoh.html

TS:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtmvdnrskl.html

Java: while (i < 10) { i++; }
来源：http://hz.hnxiangtu.top/gtovhgbvdh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jqgfzy.top/gtosolqrka.html

Ruby: while i < 10; i += 1; end
来源：http://hz.aibaodan.cn/gttxenanis.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtozfgtssx.html

[B08] do-while（至少执行一次）
来源：http://hz.shanyushiyangkeji.top/gtlmubdpkn.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jyoumei.cn/gtkdgcglaz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.wangdashe.top/gtepkbkkps.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ydzc1.top/gtggvmnqug.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtixwgqxts.html

Java: do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtmybvtvhs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cashguo.top/gtseckcdsv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.52xcode.cn/gtubekjoyo.html

C#:   do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtuhipmrkr.html

[B09] break 与 continue
来源：http://hz.zhiwuduotai.top/gtnjnqesxd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.nwbrower.top/gtbdfcstoh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.nanxuanxn.top/gthjidwpdt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gttrafkxcj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.svipenyu.cn/gtmibaapbo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtbxzcmzct.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhengqikj.top/gtuavmtfgx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cdnleiting.top/gtfkwucaqb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhaomingkeji.xyz/gtdwlcgjnn.html

[B10] 遍历同时拿索引
来源：http://hz.svipenyu.cn/gtpfhldwdw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenjidiqi.icu/gtczfhhshd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gotoacloud.top/gtfpdsxqma.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hysaishi.cn/gtbxaahckl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhoulong.xyz/gtxhceazhb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.vqdsnc.cn/gtuzrhcqki.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258.top/gtercjwtxs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zdqjudy.top/gtcxmivbnt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yuanzhike.top/gtbiktfnak.html

[B11] 生成数字序列 / 区间
来源：http://hz.sufxvd.cn/gtxhuceiop.html

Py:   list(range(0, 10, 2))
来源：http://hz.chenjidiqi.icu/gtbduhziym.html

PHP:  range(0, 10, 2);
来源：http://hz.yonumen.top/gtomyjidmk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenlongwang.top/gtdvlqsnwu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gtosokpbfb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cashguo.top/gtznttodvb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.meibo888.top/gtmarwwawo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pycfn.com/gtqljmqrul.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.daria6918.cn/gtmghksoze.html

[B12] 跳出多层循环
来源：http://hz.hfpthk.cn/gtmdmsawpi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ydjk.org.cn/gtyafuxklr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tian-w.cn/gtxarmwjnw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gthgsuxvmj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtxdfelvzs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.havefunace.top/gtfxirywel.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jyoumei.cn/gtexxjzysu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtrpjhtxdp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhixingplan.top/gtttjabrpc.html

[B13] 判断是否为数字
来源：http://hz.quarkkingdee.top/gtbpqcfekp.html

Py:   isinstance(x, (int, float))
来源：http://hz.ivvv.top/gtrnumbhka.html

PHP:  is_numeric($x)
来源：http://hz.gogol.net.cn/gtvtkmttcq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.iojbl.cn/gtvileogdo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pycfn.com/gtdudnyopq.html

Java: x instanceof Number
来源：http://hz.tanke756.top/gtxzecnsop.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hywenlv.cn/gtdbhkkeqz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jlsjyb.cn/gtgqvzkngg.html

C#:   x is int or double or decimal
来源：http://hz.cdnleiting.top/gtpqpmsglm.html

[B14] 判断值是否在集合内
来源：http://hz.zhongyouzk.top/gtynkfcrye.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ppjwa.cn/gtpgzeqbps.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yonumen.top/gtjpmexgvq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hnxiangtu.top/gtreqwwhza.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yj202588.top/gttllbzldu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.wangdashe.top/gtplktbtlk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ywan-chungtsiang.top/gtpvikddoj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hongshengwenyu.top/gttpjlrrsg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydzc1.top/gttcetgbcw.html

[B15] 布尔运算与取反
来源：http://hz.ydzc1.top/gtzhwjmadq.html

Py:   a and b or not c
来源：http://hz.redwolf501.top/gtkzvheycj.html

PHP:  $a && $b || !$c
来源：http://hz.yuxming.cn/gtibltnjmq.html

JS:   a && b || !c
来源：http://hz.ydjk.org.cn/gtrwukmflb.html

TS:   a && b || !c
来源：http://hz.ehwqpu.com/gthheawoha.html

Java: a && b || !c
来源：http://hz.dianchejie.cn/gtwexztatl.html

Go:   a && b || !c
来源：http://hz.yuanzhike.top/gtgqgtgwkg.html

Ruby: a && b || !c
来源：http://hz.chenjidiqi.icu/gtkbnuqufi.html

C#:   a && b || !c
来源：http://hz.sweek.top/gtzwhmympd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ppjwa.cn/gtauqhpjed.html

Py:   if not data: return
来源：http://hz.zycfv.cn/gtddzpqsqk.html

PHP:  if (!$data) { return; }
来源：http://hz.nanxuanxn.top/gtducnwpsc.html

JS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gtfnqoawck.html

TS:   if (!data) return;
来源：http://hz.fzhhl.top/gttdkqexll.html

Java: if (data == null) return;
来源：http://hz.tanke756.top/gtgzjtcwlp.html

Go:   if data == nil { return }
来源：http://hz.zhengqikj.top/gteovkzgwc.html

Ruby: return if data.nil?
来源：http://hz.cheryme.top/gtidrkcutn.html

C#:   if (data == null) return;
来源：http://hz.cheryme.top/gtctkrhhvw.html

================================================================================
来源：http://hz.smart0.xyz/gtwblsryqd.html

C. 函数与作用域
来源：http://hz.aibaodan.cn/gtrrasnmtk.html

================================================================================
来源：http://hz.chenlongwang.top/gtedmtlwnd.html

[C01] 定义函数
来源：http://hz.gogol.net.cn/gtppiqnrwl.html

Py:   def add(a, b): return a + b
来源：http://hz.sufxvd.cn/gtwqmotqmz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zdqjudy.top/gtqjflfwmm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.nanxinkj.top/gtgdiuvvdl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xinyue.icu/gtjdcnirye.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtqxxrhxfk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pycfn.com/gtgrhknkgu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.pycfn.com/gtzqzjgdor.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtajnynnby.html

[C02] 默认参数
来源：http://hz.jiagoushi.top/gtpqtarrju.html

Py:   def greet(name="World"): return name
来源：http://hz.sysykeji.top/gtuqmgtorl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jinqigfzy.top/gtxywrtrpp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtatntjjzl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.xinyue.icu/gtoudzkavm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtogcjfnum.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yj202588.top/gtfbbghqgq.html

Ruby: def greet(name = "World") = name
来源：http://hz.9152youxi.cn/gthktcrffb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.snrcjt.cn/gtgjfpsewh.html

[C03] 可变参数
来源：http://hz.shzxlz.cn/gtwxtjdpwu.html

Py:   def total(*args): return sum(args)
来源：http://hz.gogol.net.cn/gtywrdaoxj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.0kj1m.cn/gtuheuzgtz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.shanyushiyangkeji.top/gtylwkupsa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhoulong.xyz/gtbmapkinc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gtfismrtgn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.snrcjt.cn/gtounmzwyj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenzaomai.com/gtnrlmdzcm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shanyushiyangtech.top/gtdoofndmz.html

[C04] 命名参数 / 关键字参数
来源：http://hz.sweek.top/gtcwkiahbg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guowangkeji.top/gtukamcejj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gzhubu.top/gtgtcldkqs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hammf.cn/gtecqqwaqi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhoulong.xyz/gtebxkynwy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.smart0.xyz/gtuyibnyjl.html

Go:   // 无：用配置结构体参数
来源：http://hz.yonumen.top/gtnskqstco.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtymsbftxa.html

C#:   f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtckdcaltg.html

[C05] 返回多个值
来源：http://hz.yj20258888.top/gtodskhinb.html

Py:   return a, b
来源：http://hz.zhiwuduotai.top/gtprzjnfqq.html

PHP:  return [$a, $b];
来源：http://hz.gotoacloud.top/gtznlcpvev.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.0kj1m.cn/gtscdqbkgf.html

TS:   return { a, b };
来源：http://hz.zhaomingkeji.xyz/gtlqshkynm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shzxlz.cn/gtuzugeefp.html

Go:   return a, b
来源：http://hz.yangfankeji.com/gtpfvfpkrz.html

Ruby: return a, b
来源：http://hz.yj202588.top/gtprtqkzld.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hnxiangtu.top/gtopeetbyt.html

[C06] 匿名函数 / lambda
来源：http://hz.gogol.net.cn/gtzomzgmqt.html

Py:   square = lambda x: x * x
来源：http://hz.jqgufenzy.top/gtpfqenqoq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gzhubu.top/gtltkqcazr.html

JS:   const square = x => x * x;
来源：http://hz.jqgfzy.top/gtlwixoxhy.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ydzc1.top/gtubnnxedv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ydzc1.top/gtjwsetwqe.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhiwuduotai.top/gtiqotvcfj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ppjwa.cn/gtkxdfiidg.html


<!-- 参考信息 -->