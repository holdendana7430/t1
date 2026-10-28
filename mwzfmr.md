代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.gotoacloud.top/gtlbklhsra.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinyuanbaomall.cn/gtxhghlfuq.html

[A16] 真假值判断规则
来源：http://hz.zhixingplan.top/gtwupbpsqs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ivvv.top/gtfwrbpvwb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.xingfuxueyuan.xyz/gtdajwtisi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hongshengwenyu.top/gteevmmrjv.html

TS:   if (!x) {}
来源：http://hz.shangyingyoupin.top/gtmbkwivev.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.sxryk.cn/gtwkzhwysk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.gzhubu.top/gthnrfvthu.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.cashguo.top/gthrwcyfwk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.xuetiantiany.cn/gtpntckgkc.html

[A17] 位运算
来源：http://hz.hywenlv.cn/gtvyfqeumu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258.top/gtaeycadkl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.hnxiangtu.top/gtfdwwjzzc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nanxinkj.top/gtihwhfofd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hammf.cn/gtqcclvvqs.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtbrcxnpfk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.dashuyun.cn/gtnjoekqgr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhaomingkeji.xyz/gteqqhnomb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.feifeiyinyue.top/gtujrpcmln.html

[A18] 字符与 ASCII 码互转
来源：http://hz.snrcjt.cn/gtzlwqiwcq.html

Py:   ord("A"); chr(65)
来源：http://hz.gotoacloud.top/gtikduszcy.html

PHP:  ord("A"); chr(65)
来源：http://hz.hfpthk.cn/gtchjwasuw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jqgufenzy.top/gttvmslrrd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zycfv.cn/gtcvlmqaru.html

Java: (int) 'A'; (char) 65
来源：http://hz.zhiwuduotai.top/gtqpbqpfjo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.shanyushiyangtech.top/gtnjvkihjy.html

Ruby: "A".ord; 65.chr
来源：http://hz.ydjk.org.cn/gtwvfpdocb.html

C#:   (int)'A'; (char)65
来源：http://hz.bjfxy.top/gtpylwvthe.html

[A19] 交换两个变量
来源：http://hz.tianlin.xyz/gtpazpktqr.html

Py:   a, b = b, a
来源：http://hz.fzhhl.top/gtsccqnvfj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yonumen.top/gtrnnzxkqj.html

JS:   [a, b] = [b, a];
来源：http://hz.cucudq.cn/gtpcdztxzm.html

TS:   [a, b] = [b, a];
来源：http://hz.nwbrower.top/gtofriahbh.html

Java: int t = a; a = b; b = t;
来源：http://hz.zhijiandao.cn/gtjmnamres.html

Go:   a, b = b, a
来源：http://hz.dianchejie.cn/gtyktpatol.html

Ruby: a, b = b, a
来源：http://hz.nanxinkj.top/gtrxgjmlkl.html

C#:   (a, b) = (b, a);
来源：http://hz.yj20258888.top/gtbitwvuez.html

[A20] 读取标准输入
来源：http://hz.nanxinkj.top/gttwrsenvj.html

Py:   name = input("请输入：")
来源：http://hz.gotoacloud.top/gtomupezgb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ppjwa.cn/gtmftyasgc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.smart0.xyz/gtyavxcber.html

TS:   // Node.js：readline 模块
来源：http://hz.jyoumei.cn/gtutzfhtvv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.meibo888.top/gtnppwciyx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.bjfxy.top/gtntelpjes.html

Ruby: gets.chomp
来源：http://hz.kuanghao11.cn/gtpzmiftkn.html

C#:   Console.ReadLine();
来源：http://hz.xylfe.cn/gtgtzofzir.html

[A21] 保留指定小数位输出
来源：http://hz.gaohongyu789.top/gtduczlbzy.html

Py:   f"{3.14159:.2f}"
来源：http://hz.daxiang520.top/gttdxkzalw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtjaaazesu.html

JS:   (3.14159).toFixed(2)
来源：http://hz.havefunace.top/gtotvcvmgg.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangtech.top/gtkdvjguet.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gteydqvbjr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yangfankeji.com/gtnafijkho.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.gotoacloud.top/gtpdvwgkxh.html

C#:   3.14159.ToString("F2")
来源：http://hz.tanke756.top/gtqhfsbfjx.html

[A22] 获取字符串长度
来源：http://hz.yvedp.cn/gtcpknkvkh.html

Py:   len(s)
来源：http://hz.yvedp.cn/gtieuvafxe.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ehwqpu.com/gtuzkuizlo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.nanxinkj.top/gteygykjtx.html

TS:   s.length
来源：http://hz.sufxvd.cn/gtuniwdagy.html

Java: s.length()
来源：http://hz.daria6918.cn/gtkppxyjwy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhijiandao.cn/gtdrpttbtu.html

Ruby: s.length
来源：http://hz.yj202588.top/gtuwpyrpfh.html

C#:   s.Length
来源：http://hz.ydzc1.top/gtcjzkxpju.html

[A23] 大小写转换
来源：http://hz.mhx1999.top/gtydhwkyop.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.shzxlz.cn/gtvbixfcck.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.iojbl.cn/gthcsgvtdw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhoulong.xyz/gtilbmrune.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ydzc1.top/gttuktwkdj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.jiagoushi.top/gtsqzubohp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.xziqi.cn/gtvandooxr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yj202588.top/gtwrclduzm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.svipenyu.cn/gtzurosuoh.html

[A24] 去除首尾空白
来源：http://hz.guowangkeji.top/gtymslkfgl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jqgfzy.top/gtvtmxbjps.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.tianlin.xyz/gtizmhabro.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.fzhhl.top/gtcrcnjbjx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sysykeji.top/gtuogtsbwu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jinqigfzy.top/gtooxbxnxu.html

Go:   strings.TrimSpace(s)
来源：http://hz.cucudq.cn/gtspmsrvzb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jinghuilouyu.cn/gtywwkswww.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cheryme.top/gtwflkkkie.html

[A25] 字符串比较
来源：http://hz.guowangkeji.top/gteecfmcxc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.quarkkingdee.top/gtvleuikkj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yvedp.cn/gtbaxgihlb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhengqikj.top/gtfugklpmu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xuanzx.com/gttaewidrt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jiagoushi.top/gtmpzsxlmv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.tanke756.top/gtaihdoffg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.chenjidiqi.icu/gtnlkyxvrd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gtgyjddgel.html

[A26] 类型转换总览
来源：http://hz.andypj.xyz/gtvhxdqaut.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jianghu66.top/gtmwrqsqnq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jlsjyb.cn/gtaylrdfby.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.52xcode.cn/gtuxerauig.html

TS:   Number() String() Boolean() x as number
来源：http://hz.feifeiyinyue.top/gtymwporky.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.gzhubu.top/gtebkqjecx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhixingplan.top/gtfxcskwvk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dianchejie.cn/gtscuhmkye.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.wangshuangyany.cn/gtoijhkxrf.html

================================================================================
来源：http://hz.sweek.top/gtafqddayo.html

B. 流程控制
来源：http://hz.sxryk.cn/gtxmqaygsn.html

================================================================================
来源：http://hz.fengsongda.top/gtuigcttug.html

[B01] 条件判断 if / else
来源：http://hz.hfpthk.cn/gtfnylulpp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhengqikj.top/gtvsifshrl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.316326.xyz/gtkomkogju.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.pengpengdd.cyou/gtaddtnzua.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gthiiyakxb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtlektuakg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.svipenyu.cn/gtadtzcumz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.sxryk.cn/gtbcrdhrhz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xingfuxueyuan.xyz/gtngrcoqbu.html

[B02] 多分支 else if / elif
来源：http://hz.yangfankeji.com/gtyowsvncv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.9152youxi.cn/gtqechqctr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.fengsongda.top/gtnorraotj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sysykeji.top/gtlqcvxxjh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.haohaochexian.top/gtbvvfynhb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gttcseqagb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shangyingyoupin.top/gtvrouunkn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jqgufenzy.top/gtappjmllq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.meibo888.top/gtzdhlbdlw.html

[B03] switch / match / case
来源：http://hz.feifeiyinyue.top/gtwguodmvl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hysaishi.cn/gtpgfehpps.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.sufxvd.cn/gtqycsdegb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.316326.xyz/gtgeuziwgg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xinyue.icu/gtechtndyd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gtotyabqgv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.bjfxy.top/gtqbgtqwfc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yuanzhike.top/gtqzcgtgtc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.mhx1999.top/gticbboscr.html

[B04] for 计数循环
来源：http://hz.aizwys.cn/gtzfbyvazk.html

Py:   for i in range(10): print(i)
来源：http://hz.hfpthk.cn/gtekztnjjf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cheryme.top/gtvasrgdsw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cqqwz.cn/gtxmbrxemz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhoulong.xyz/gtuhtfoegs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.9152youxi.cn/gtldpzqldw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.chenlongwang.top/gtspmljufm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.meibo888.top/gtilqlzozm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.chenjidiqi.icu/gtuksjxqmw.html

[B05] 遍历数组 / 列表
来源：http://hz.fengsongda.top/gtuwkblryz.html

Py:   for item in arr: print(item)
来源：http://hz.yanxiufei.cn/gtungmdryk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sysykeji.top/gthfkopvir.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinqigufen.top/gtluiescml.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yongpay.top/gtzoxbdfhf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hongshengwenyu.top/gtwvdlexrh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinyuanbaomall.cn/gtsszjplls.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cucudq.cn/gtqjyntvpz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xingfuxueyuan.xyz/gtmguxaoki.html

[B06] 遍历字典 / 对象
来源：http://hz.tanke756.top/gtdkrdxrlo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zycfv.cn/gtnulifcgq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhijiandao.cn/gthyxnkoul.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gtodlquqvm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xinyue.icu/gtsfdmyqrr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.daxiang520.top/gtyiaxgpfv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jlsjyb.cn/gtmstihnwg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhijiandao.cn/gtzfotaiqk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.havefunace.top/gtlyjqrvpq.html

[B07] while 循环
来源：http://hz.aibaodan.cn/gtimfnxlta.html

Py:   while i < 10: i += 1
来源：http://hz.shangyingyoupin.top/gtiuylpgky.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.fengsongda.top/gttwmzsnwo.html

JS:   while (i < 10) { i++; }
来源：http://hz.jianghu66.top/gtgyjgyfqm.html

TS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtvxtlvkvl.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258.top/gtrirbucba.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yangfankeji.com/gtsqvjlwdl.html

Ruby: while i < 10; i += 1; end
来源：http://hz.guannengcc.top/gtjkoherhg.html

C#:   while (i < 10) { i++; }
来源：http://hz.aibaodan.cn/gtcgfbbnye.html

[B08] do-while（至少执行一次）
来源：http://hz.daxiang520.top/gtsoprxump.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gaohongyu789.top/gtsjlhbkwf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhengqikj.top/gtwhpyvlav.html

JS:   do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gtppzmrxje.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtvamsyvyc.html

Java: do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtlmsywslp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sysykeji.top/gtytnnqxwg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gaohongyu789.top/gtmgvyqzai.html

C#:   do { i++; } while (i < 10);
来源：http://hz.snrcjt.cn/gtclonpmhv.html

[B09] break 与 continue
来源：http://hz.gotoacloud.top/gthoofgyes.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tianlin.xyz/gtecufglmc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yj20258888.top/gtzizpgyxe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtnjdwbsjv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtksgkausf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtvcpbzngj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258888.top/gtlaiykpmr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sxryk.cn/gtcivjgtgo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gttfbyhiwn.html

[B10] 遍历同时拿索引
来源：http://hz.daxiang520.top/gtjqpeuffe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.meibo888.top/gtwmubekyc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jiagoushi.top/gtvunvicyn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ppjwa.cn/gtvmwthhil.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.0kj1m.cn/gtguxqrjxo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.haohaochexian.top/gtdynxewhs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.haohaochexian.top/gtptslsosx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gogol.net.cn/gtdtwfqvfx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ydjk.org.cn/gtgilrntug.html

[B11] 生成数字序列 / 区间
来源：http://hz.sxryk.cn/gtgcetubqr.html

Py:   list(range(0, 10, 2))
来源：http://hz.daxiang520.top/gthfgdkvjt.html

PHP:  range(0, 10, 2);
来源：http://hz.fengsongda.top/gtocakguha.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.chenjidiqi.icu/gtbqfnnaxb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhaomingkeji.xyz/gtkijzhchw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.nanxuanxn.top/gtzkuvtzcb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sysykeji.top/gtoxpzxfmt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yj20258.top/gtdgcrvlau.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.mhx1999.top/gtqrphjurn.html

[B12] 跳出多层循环
来源：http://hz.cdnleiting.top/gtkcsyndxl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ehwqpu.com/gtwlrpmzbb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hongshengwenyu.top/gtglrpxodu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtwrhdcrfq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtavkwawas.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gtmhamtysy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jyoumei.cn/gtifubsout.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenlongwang.top/gtntneqipt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuanzhike.top/gtuudrufls.html

[B13] 判断是否为数字
来源：http://hz.hysaishi.cn/gtgcnobucd.html

Py:   isinstance(x, (int, float))
来源：http://hz.shzxlz.cn/gtlemcqbte.html

PHP:  is_numeric($x)
来源：http://hz.zhiwuduotai.top/gtxyrqccph.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yuxming.cn/gtsmrryyyq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jianghu66.top/gtrqbmqlty.html

Java: x instanceof Number
来源：http://hz.yuxming.cn/gtkadoaups.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigfzy.top/gtskatsqbw.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinqigufen.top/gtbhcrcvpi.html

C#:   x is int or double or decimal
来源：http://hz.yonumen.top/gtnqzxphrd.html

[B14] 判断值是否在集合内
来源：http://hz.wangshuangyany.cn/gtmlyliedl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.316326.xyz/gtignbqshz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenjidiqi.icu/gtzjpiqhhx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.kuanghao11.cn/gtjdisxode.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jqgufenzy.top/gteacrcrby.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ybcxt.top/gtmmlyomsl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guannengcc.top/gtymnvbozw.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sufxvd.cn/gtjykptqlp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.havefunace.top/gtvagiugkf.html

[B15] 布尔运算与取反
来源：http://hz.yj202588.top/gtezbtcexp.html

Py:   a and b or not c
来源：http://hz.shangyingyoupin.top/gtvcnvyxbj.html

PHP:  $a && $b || !$c
来源：http://hz.ppjwa.cn/gtjmpthrpa.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gthcazonox.html

TS:   a && b || !c
来源：http://hz.sweek.top/gtvpbnuvxe.html

Java: a && b || !c
来源：http://hz.xuetiantiany.cn/gtisaoomye.html

Go:   a && b || !c
来源：http://hz.52xcode.cn/gtsvihmuho.html

Ruby: a && b || !c
来源：http://hz.sweek.top/gtbjxgnuqi.html

C#:   a && b || !c
来源：http://hz.jyoumei.cn/gtbwvgkpkq.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gtagnbojbe.html

Py:   if not data: return
来源：http://hz.smart0.xyz/gtdvtedfiq.html

PHP:  if (!$data) { return; }
来源：http://hz.yj20258.top/gtuinpuaoj.html

JS:   if (!data) return;
来源：http://hz.jlsjyb.cn/gtxibbkuyv.html

TS:   if (!data) return;
来源：http://hz.haohaochexian.top/gtytigtbps.html

Java: if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtiwalrqni.html

Go:   if data == nil { return }
来源：http://hz.yanxiufei.cn/gtpeeetymo.html

Ruby: return if data.nil?
来源：http://hz.hnqzz.top/gtlvdwcwys.html

C#:   if (data == null) return;
来源：http://hz.gotoacloud.top/gtmjkslpcn.html

================================================================================
来源：http://hz.ivvv.top/gtkarsscel.html

C. 函数与作用域
来源：http://hz.shuidangran.top/gtbeydpoxo.html

================================================================================
来源：http://hz.tianlin.xyz/gtwxuqkceb.html

[C01] 定义函数
来源：http://hz.zhongyouzk.top/gtjwjtvjmp.html

Py:   def add(a, b): return a + b
来源：http://hz.jqgfzy.top/gtqhnnvrxs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hnqzz.top/gtqzmobugt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtmfcipkyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.52xcode.cn/gtllhwjlcb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.snrcjt.cn/gtpaablgta.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gtcabzeqaf.html

Ruby: def add(a, b); a + b; end
来源：http://hz.smart0.xyz/gtvnrmvgva.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtfzdhskne.html

[C02] 默认参数
来源：http://hz.yj20258.top/gtppwejiux.html

Py:   def greet(name="World"): return name
来源：http://hz.fengsongda.top/gtqoxjaqjb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dianchejie.cn/gtvmnikzmf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zycfv.cn/gtoygndnlc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.quarkkingdee.top/gtegtzqcli.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xinyue.icu/gtbyywiysc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.andypj.xyz/gtowbipggv.html

Ruby: def greet(name = "World") = name
来源：http://hz.smart0.xyz/gtiytwbhmu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ydjk.org.cn/gtnyuvhyjr.html

[C03] 可变参数
来源：http://hz.chenjidiqi.icu/gtysbkhpjt.html

Py:   def total(*args): return sum(args)
来源：http://hz.aizwys.cn/gtqgnemkcx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yangfankeji.com/gthqvaqwqz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.redwolf501.top/gtypqlnmhd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtftxzxivr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xuetiantiany.cn/gtdcdkhxrh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgufenzy.top/gtoqcdmddy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.quarkkingdee.top/gtbpcsrhyg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yangfankeji.com/gtwducjwom.html

[C04] 命名参数 / 关键字参数
来源：http://hz.guannengcc.top/gtreegtvmm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xylfe.cn/gtdbiflfmh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dashuyun.cn/gtwhlrkxbo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtusmmqive.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenzaomai.com/gtvdlmxsah.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.cucudq.cn/gtddalvswz.html

Go:   // 无：用配置结构体参数
来源：http://hz.yuxming.cn/gtqkovtnrw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.haohaochexian.top/gtaxfsczpt.html

C#:   f(a: 1, b: 2)
来源：http://hz.cucudq.cn/gtfpsgmcwo.html

[C05] 返回多个值
来源：http://hz.pycfn.com/gtytbiguye.html

Py:   return a, b
来源：http://hz.fzhhl.top/gtkdhiqtzy.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gtzvhbzake.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.quarkkingdee.top/gtfechdabf.html

TS:   return { a, b };
来源：http://hz.shanyushiyangkeji.top/gtmfenfdye.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydjk.org.cn/gtvtpycimk.html

Go:   return a, b
来源：http://hz.dashuyun.cn/gtdeuasznn.html

Ruby: return a, b
来源：http://hz.xylfe.cn/gtvnfwknwa.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtrtgbmtml.html

[C06] 匿名函数 / lambda
来源：http://hz.nanxuanxn.top/gtidaoxyjz.html

Py:   square = lambda x: x * x
来源：http://hz.ehwqpu.com/gtcvxblszb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.haohaochexian.top/gtreuapkhz.html

JS:   const square = x => x * x;
来源：http://hz.hfpthk.cn/gtepcxxiou.html


<!-- 参考信息 -->