代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.xuetiantiany.cn/gtiqpzektn.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.xingfuxueyuan.xyz/gtdcjbehep.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.gzhubu.top/gtyzdtsguk.html

[A17] 位运算
来源：http://hz.cdnleiting.top/gtvazyjrkz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sysykeji.top/gtoigndtla.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.xinyue.icu/gtkpjgwzje.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.smart0.xyz/gtpxxrhdxc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gteuegttqw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtvsemkpjc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.birdmap.top/gtylvbtpmn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtyeblhzhe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.kuanghao11.cn/gtlhpaoswm.html

[A18] 字符与 ASCII 码互转
来源：http://hz.xziqi.cn/gtlqibldqe.html

Py:   ord("A"); chr(65)
来源：http://hz.xylfe.cn/gtawcgatgp.html

PHP:  ord("A"); chr(65)
来源：http://hz.iojbl.cn/gtjxssfbhe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxinkj.top/gtpfribomh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cucudq.cn/gtbuecfdqw.html

Java: (int) 'A'; (char) 65
来源：http://hz.ppjwa.cn/gtlgmybbob.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.meibo888.top/gtggensjie.html

Ruby: "A".ord; 65.chr
来源：http://hz.tianlin.xyz/gtgxhcswjr.html

C#:   (int)'A'; (char)65
来源：http://hz.zhengqikj.top/gtawgeavle.html

[A19] 交换两个变量
来源：http://hz.ybcxt.top/gtbphqzzoi.html

Py:   a, b = b, a
来源：http://hz.zycfv.cn/gtgxepmhec.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jinghuilouyu.cn/gtknhkllbe.html

JS:   [a, b] = [b, a];
来源：http://hz.jyoumei.cn/gtwsetnhjc.html

TS:   [a, b] = [b, a];
来源：http://hz.smart0.xyz/gtqvogdyjn.html

Java: int t = a; a = b; b = t;
来源：http://hz.hfpthk.cn/gteotwjjes.html

Go:   a, b = b, a
来源：http://hz.chenzaomai.com/gtdjfqkhqf.html

Ruby: a, b = b, a
来源：http://hz.ywan-chungtsiang.top/gtxvgyazff.html

C#:   (a, b) = (b, a);
来源：http://hz.ybcxt.top/gtcdalnjqn.html

[A20] 读取标准输入
来源：http://hz.smart0.xyz/gtzyudtrsl.html

Py:   name = input("请输入：")
来源：http://hz.shzxlz.cn/gtwimfimqp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hnqzz.top/gtshijyxbe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.nanxinkj.top/gtxedawizm.html

TS:   // Node.js：readline 模块
来源：http://hz.ydjk.org.cn/gttyxrrwfc.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yanxiufei.cn/gtglockxdc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yvedp.cn/gtmljlgyne.html

Ruby: gets.chomp
来源：http://hz.jinqigfzy.top/gtubywmlqt.html

C#:   Console.ReadLine();
来源：http://hz.gogol.net.cn/gtudaeebpn.html

[A21] 保留指定小数位输出
来源：http://hz.hammf.cn/gtjbcfnqph.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cheryme.top/gtxmrccosw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gttitzhcpa.html

JS:   (3.14159).toFixed(2)
来源：http://hz.zhixingplan.top/gtqaftfflh.html

TS:   (3.14159).toFixed(2)
来源：http://hz.pycfn.com/gtbezbaguf.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.dianchejie.cn/gtuzobcdgl.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.zdqjudy.top/gtipborvmv.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.wangshuangyany.cn/gtesafrxxc.html

C#:   3.14159.ToString("F2")
来源：http://hz.zycfv.cn/gtrewqnwzg.html

[A22] 获取字符串长度
来源：http://hz.daria6918.cn/gtecwdekfu.html

Py:   len(s)
来源：http://hz.sxryk.cn/gtejeikrno.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yj202588.top/gtzgglpbct.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.bjfxy.top/gtdrshstsw.html

TS:   s.length
来源：http://hz.wangdashe.top/gtsbjqfwrf.html

Java: s.length()
来源：http://hz.fzhhl.top/gtxamcatmg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cheryme.top/gtitnvdlwa.html

Ruby: s.length
来源：http://hz.zycfv.cn/gthjfdtncu.html

C#:   s.Length
来源：http://hz.jinyuanbaomall.cn/gtxnyyxgql.html

[A23] 大小写转换
来源：http://hz.vqdsnc.cn/gtqucybldq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.chenjidiqi.icu/gtkcvyaqar.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.daxiang520.top/gtiylcrjmx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.wangshuangyany.cn/gtfucmyrsl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj202588.top/gtkwwzhdlu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yueranfly.top/gtecbrxivw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zdqjudy.top/gtuwikuwdq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ehwqpu.com/gtambmzqpw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.ywan-chungtsiang.top/gtqnbywoav.html

[A24] 去除首尾空白
来源：http://hz.gaohongyu789.top/gtteasqumf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ppjwa.cn/gtsmhvizzm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jinqigufen.top/gtjjybpscj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenlongwang.top/gtldtluagk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.wangshuangyany.cn/gtimjjfghf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xuanzx.com/gtvhaiwzpn.html

Go:   strings.TrimSpace(s)
来源：http://hz.guowangkeji.top/gtbhuoulxz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.havefunace.top/gtxnchaewl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cqqwz.cn/gtyfazsqmv.html

[A25] 字符串比较
来源：http://hz.jianghu66.top/gtnlkeshwm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.guannengcc.top/gtdikoxkvy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.iojbl.cn/gtgctvqkjc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yongpay.top/gthiuixgxv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sxryk.cn/gtvzyitoxp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.guannengcc.top/gtvtfqemuy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xziqi.cn/gtvwxfqcpe.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hysaishi.cn/gtogqjncnz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jyoumei.cn/gtqucgaezl.html

[A26] 类型转换总览
来源：http://hz.hnqzz.top/gtyugrcymq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zycfv.cn/gtgywanapi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.hnqzz.top/gtrqfqhrkg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhixingplan.top/gtygojhgvf.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cucudq.cn/gtgbndahdl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.snrcjt.cn/gtwdjghmbb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.cashguo.top/gtvzbwixsc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.wangdashe.top/gtjydumolp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.chenjidiqi.icu/gtyyxgdlkw.html

================================================================================
来源：http://hz.tianlin.xyz/gtcqtufjzv.html

B. 流程控制
来源：http://hz.havefunace.top/gtpxotmxzr.html

================================================================================
来源：http://hz.hfpthk.cn/gtqiuayczv.html

[B01] 条件判断 if / else
来源：http://hz.yonumen.top/gtipjkwjet.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.xinyue.icu/gtydlvvsci.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.nwbrower.top/gtycasellr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jqgfzy.top/gtsyvrufcn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gtgmfibaas.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xinyue.icu/gtztvpwdqo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ywan-chungtsiang.top/gthnaegyjj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zdqjudy.top/gtmzumdgbw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gttjewrtdr.html

[B02] 多分支 else if / elif
来源：http://hz.yj20258.top/gtkvzguzcv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.haohaochexian.top/gtttxuxdzo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj202588.top/gtxvogrivu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.birdmap.top/gtkxgtmskx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zycfv.cn/gtlgeqhjdd.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tanke756.top/gtsdukgtdx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xziqi.cn/gthwyijpsh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.daria6918.cn/gtulysshrm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pengpengdd.cyou/gtwgymylqj.html

[B03] switch / match / case
来源：http://hz.zhixingplan.top/gtonzmwcda.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.316326.xyz/gtnagxfnwg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xziqi.cn/gtztgxzhiq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ybcxt.top/gtohyshgee.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.daria6918.cn/gtakwhlaca.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cashguo.top/gtrmcixmrs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.xingfuxueyuan.xyz/gtlmhjzmid.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhaomingkeji.xyz/gtflcozcto.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.ydzc1.top/gtxlzzldlg.html

[B04] for 计数循环
来源：http://hz.aizwys.cn/gttvehgbsc.html

Py:   for i in range(10): print(i)
来源：http://hz.yj20258888.top/gtygkeezlw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhijiandao.cn/gtehjwfuxi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cashguo.top/gtcxwdvmrn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jianghu66.top/gtmbsduwlb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.snrcjt.cn/gtgnxfqstk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yangfankeji.com/gtrvjxevzv.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daria6918.cn/gtnwxmhods.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.pycfn.com/gtdzdblowl.html

[B05] 遍历数组 / 列表
来源：http://hz.hysaishi.cn/gtpjgpvzwn.html

Py:   for item in arr: print(item)
来源：http://hz.xingfuxueyuan.xyz/gtcfabaucb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.fzhhl.top/gtsqwwixws.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.fengsongda.top/gtncgamtfx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.pengpengdd.cyou/gtsngkcljm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sufxvd.cn/gtobemjbkm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xylfe.cn/gttvbwbgvr.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jqgfzy.top/gtrjwgjlkv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.guannengcc.top/gtomldsnwt.html

[B06] 遍历字典 / 对象
来源：http://hz.hnqzz.top/gtggizguzz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.gzhubu.top/gtldazsnjz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hysaishi.cn/gtztiyvini.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.dashuyun.cn/gtkfcteoxc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhijiandao.cn/gtbqxaojzv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tanke756.top/gtrvifrfii.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shuidangran.top/gtlpgannak.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.tian-w.cn/gtyzuomxxa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gotoacloud.top/gtultwahvb.html

[B07] while 循环
来源：http://hz.wangdashe.top/gtnmyvqqou.html

Py:   while i < 10: i += 1
来源：http://hz.hnxiangtu.top/gtzjxmxegn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhengqikj.top/gtnhvbimsm.html

JS:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtfrabrbkk.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhengqikj.top/gtrjnqclst.html

Java: while (i < 10) { i++; }
来源：http://hz.pycfn.com/gtuallvdro.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.aizwys.cn/gtbfnbvrvr.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ywan-chungtsiang.top/gtuksplmsu.html

C#:   while (i < 10) { i++; }
来源：http://hz.316326.xyz/gtqimrvpom.html

[B08] do-while（至少执行一次）
来源：http://hz.yangfankeji.com/gtsmfwlgoq.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.havefunace.top/gtgsjekpij.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gotoacloud.top/gtwftkvorg.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtdmxwvidv.html

TS:   do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtimnzzguc.html

Java: do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gttejixjlg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yongpay.top/gtvcionraj.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.fzhhl.top/gtvederggb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtyeecokdy.html

[B09] break 与 continue
来源：http://hz.tanke756.top/gtfsmnhbok.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xingfuxueyuan.xyz/gtebwrbrnn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.nanxinkj.top/gtewyyrtlm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtygzvweaz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtlxddonfs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yanxiufei.cn/gtiqoraidq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.feifeiyinyue.top/gtqhfwqhes.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinyuanbaomall.cn/gtlopecgak.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtxndzodaz.html

[B10] 遍历同时拿索引
来源：http://hz.aibaodan.cn/gtwfgffjvx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.feifeiyinyue.top/gtzdjsugpl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gaohongyu789.top/gtykahiabp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.guannengcc.top/gtiiskjwsb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.c1oappe.top/gtgauijity.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sweek.top/gtksnfqmmp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.smart0.xyz/gtduvqmfgt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.c1oappe.top/gtulefjuyq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangkeji.top/gtrdnnjnxb.html

[B11] 生成数字序列 / 区间
来源：http://hz.dashuyun.cn/gtffialges.html

Py:   list(range(0, 10, 2))
来源：http://hz.ehwqpu.com/gtsogebcbh.html

PHP:  range(0, 10, 2);
来源：http://hz.jinqigufen.top/gtzfrvgrgi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.aibaodan.cn/gtsjcuvyyq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gogol.net.cn/gtkgowyqbr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.shzxlz.cn/gtvsxabkui.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shangyingyoupin.top/gtnhvizabk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.meibo888.top/gtsiwpjpyb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.pengpengdd.cyou/gtyaiqhtae.html

[B12] 跳出多层循环
来源：http://hz.guannengcc.top/gtvnockkdv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jiagoushi.top/gthzdmadkt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jyoumei.cn/gtqoszdxpr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtilmsfdlt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtsmvnnarv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.pycfn.com/gtgxtxfhuq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenlongwang.top/gthngihety.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.meibo888.top/gtleukhucn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.dashuyun.cn/gtdqmglzwl.html

[B13] 判断是否为数字
来源：http://hz.chenlongwang.top/gtmgihihmw.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinyuanbaomall.cn/gtwqgaoeid.html

PHP:  is_numeric($x)
来源：http://hz.jyoumei.cn/gtjqcvnbjg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yongpay.top/gthihzkdbp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gtzilxapzg.html

Java: x instanceof Number
来源：http://hz.svipenyu.cn/gtsnidewxm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sweek.top/gtefhfnjgb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yj20258888.top/gtuhrcrehn.html

C#:   x is int or double or decimal
来源：http://hz.gogol.net.cn/gtirlsrisj.html

[B14] 判断值是否在集合内
来源：http://hz.daria6918.cn/gtnuqvzqtn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.feifeiyinyue.top/gtayndqihu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hammf.cn/gtmsucfbqm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtutojkpvx.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258.top/gtouioatzd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhaomingkeji.xyz/gtkxijaojq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yj20258.top/gtmixnrewm.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jiagoushi.top/gttcqeisyo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydjk.org.cn/gthrkzgabr.html

[B15] 布尔运算与取反
来源：http://hz.zhiwuduotai.top/gtagfbytav.html

Py:   a and b or not c
来源：http://hz.xingfuxueyuan.xyz/gtwxkgfije.html

PHP:  $a && $b || !$c
来源：http://hz.cdnleiting.top/gtuggfkknd.html

JS:   a && b || !c
来源：http://hz.yvedp.cn/gtnelntprm.html

TS:   a && b || !c
来源：http://hz.tanke756.top/gtxfcdxzfu.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gtadagzgwd.html

Go:   a && b || !c
来源：http://hz.jlsjyb.cn/gtusvorqsw.html

Ruby: a && b || !c
来源：http://hz.iojbl.cn/gtiuvfztwy.html

C#:   a && b || !c
来源：http://hz.yueranfly.top/gtgjesuhdj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.snrcjt.cn/gtcsmcgnep.html

Py:   if not data: return
来源：http://hz.c1oappe.top/gttavvtrro.html

PHP:  if (!$data) { return; }
来源：http://hz.ehwqpu.com/gtckeapuiv.html

JS:   if (!data) return;
来源：http://hz.wangshuangyany.cn/gtsaghpjse.html

TS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtobkcigua.html

Java: if (data == null) return;
来源：http://hz.sweek.top/gtihoigecv.html

Go:   if data == nil { return }
来源：http://hz.cucudq.cn/gtmeblcnpi.html

Ruby: return if data.nil?
来源：http://hz.sysykeji.top/gtfdkedwjr.html

C#:   if (data == null) return;
来源：http://hz.sysykeji.top/gtwpxiojkv.html

================================================================================
来源：http://hz.wangdashe.top/gtbljjszpq.html

C. 函数与作用域
来源：http://hz.yuxming.cn/gtgvcxscdr.html

================================================================================
来源：http://hz.yuxming.cn/gtbldqkzhb.html

[C01] 定义函数
来源：http://hz.zhaomingkeji.xyz/gtrlhtrwrg.html

Py:   def add(a, b): return a + b
来源：http://hz.c1oappe.top/gtpomybjjy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.haohaochexian.top/gtclipghyv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.wangshuangyany.cn/gtnjpoywiq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtjwelenqg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nwbrower.top/gtdycgjxqo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jlsjyb.cn/gtjflwqsfo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenlongwang.top/gtfpswxvjn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtqszqwlgx.html

[C02] 默认参数
来源：http://hz.feifeiyinyue.top/gtbdsoqlsi.html

Py:   def greet(name="World"): return name
来源：http://hz.jinghuilouyu.cn/gtadrvuthk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhiwuduotai.top/gtbldbntte.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtekokrawk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.iojbl.cn/gtxllcaobw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxinkj.top/gtoihdbueu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gttzqztchb.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gtxcsvpwvl.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.haohaochexian.top/gtviexgwea.html

[C03] 可变参数
来源：http://hz.xuanzx.com/gtmqxiwzov.html

Py:   def total(*args): return sum(args)
来源：http://hz.iojbl.cn/gtwyxwxpah.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hywenlv.cn/gteceouayv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtzlxlkumu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhiwuduotai.top/gtvwnwnjrd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.bjfxy.top/gtvuzaxxdt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhijiandao.cn/gtrrnbejns.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258888.top/gtsuvchgll.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sxryk.cn/gtsthndisn.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cqqwz.cn/gtflihfffh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ydzc1.top/gtglpodune.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.redwolf501.top/gtahdsqkly.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cashguo.top/gtkusnqdid.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gtzukoyywd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxuanxn.top/gtvzykrrwj.html

Go:   // 无：用配置结构体参数
来源：http://hz.smart0.xyz/gtneoaamuw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cheryme.top/gtmbtytcxm.html

C#:   f(a: 1, b: 2)
来源：http://hz.wangdashe.top/gtwrrtpfpo.html

[C05] 返回多个值
来源：http://hz.shzxlz.cn/gtndarronu.html

Py:   return a, b
来源：http://hz.pengpengdd.cyou/gtuclsiwdf.html

PHP:  return [$a, $b];
来源：http://hz.shuidangran.top/gtswrpcgjx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xingfuxueyuan.xyz/gtegpxlqpa.html

TS:   return { a, b };
来源：http://hz.zhengqikj.top/gtlkeonhiz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hongshengwenyu.top/gtnlvdmeul.html

Go:   return a, b
来源：http://hz.hongshengwenyu.top/gtuhzyveoy.html

Ruby: return a, b
来源：http://hz.yj20258.top/gttmihbhmr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.0kj1m.cn/gtsyfafyno.html

[C06] 匿名函数 / lambda
来源：http://hz.jlsjyb.cn/gtybrhetrx.html

Py:   square = lambda x: x * x
来源：http://hz.ppjwa.cn/gtzluuziwu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.tianlin.xyz/gtqrrwcjvw.html

JS:   const square = x => x * x;
来源：http://hz.nwbrower.top/gtfbtnxdlf.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ehwqpu.com/gtlulguobi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.52xcode.cn/gtxzzyfdoj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtwbensxxi.html

Ruby: square = ->(x) { x * x }
来源：http://hz.9152youxi.cn/gtybcjvrhp.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.tian-w.cn/gtrszllupe.html

[C07] 把函数作为参数传入
来源：http://hz.xylfe.cn/gtaqwkolot.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.316326.xyz/gtowopgewu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shangyingyoupin.top/gtnxbaffnq.html


<!-- 参考信息 -->