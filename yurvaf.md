代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.xuetiantiany.cn/gticbfjhoj.html

Ruby: "Hello, #{name}!"
来源：http://hz.gotoacloud.top/gtavbiacil.html

C#:   $"Hello, {name}!"
来源：http://hz.zdqjudy.top/gtlkmwfnbw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.zhijiandao.cn/gtmkbjtzsw.html

Py:   "第一行\n第二行"
来源：http://hz.xylfe.cn/gtjdjyvfhu.html

PHP:  "第一行\n第二行"
来源：http://hz.hammf.cn/gtiaokefxy.html

JS:   "第一行\n第二行"
来源：http://hz.52xcode.cn/gtfnnssnku.html

TS:   "第一行\n第二行"
来源：http://hz.zhoulong.xyz/gtbuyxyhro.html

Java: "第一行\n第二行"
来源：http://hz.52xcode.cn/gtqdcdhicv.html

Go:   "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtznjsgdtt.html

Ruby: "第一行\n第二行"
来源：http://hz.guowangkeji.top/gtzqmsizmi.html

C#:   "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtjwisnmwo.html

[A14] 注释写法
来源：http://hz.sxryk.cn/gtywmucwuk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.ivvv.top/gtmagdsgtr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.chenlongwang.top/gtonofxxzj.html

JS:   // 单行；/* 多行 */
来源：http://hz.snrcjt.cn/gtnyjayoua.html

TS:   // 单行；/* 多行 */
来源：http://hz.316326.xyz/gtcaghjsyv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.andypj.xyz/gtnkwiaazf.html

Go:   // 单行；/* 多行 */
来源：http://hz.xuanzx.com/gtbdcylcup.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhoulong.xyz/gtrqliweyp.html

C#:   // 单行；/* 多行 */
来源：http://hz.pengpengdd.cyou/gttjtamkxt.html

[A15] 空值判断与默认值
来源：http://hz.shanyushiyangkeji.top/gtprolczvh.html

Py:   value = data or "默认值"
来源：http://hz.guannengcc.top/gtaclovegn.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.dianchejie.cn/gtylqdhyep.html

JS:   const value = data ?? "默认值";
来源：http://hz.c1oappe.top/gtegserind.html

TS:   const value = data ?? "默认值";
来源：http://hz.9152youxi.cn/gteraxhbhs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhaomingkeji.xyz/gtifazfrey.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.guowangkeji.top/gtfzviqtvy.html

Ruby: value = data || "默认值"
来源：http://hz.ivvv.top/gtuczqvgap.html

C#:   var value = data ?? "默认值";
来源：http://hz.ydjk.org.cn/gthljjfsfl.html

[A16] 真假值判断规则
来源：http://hz.zhiwuduotai.top/gttclivscc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.cdnleiting.top/gthwmpdlof.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.zhijiandao.cn/gtfxdoypmu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xylfe.cn/gtdyfxkbjz.html

TS:   if (!x) {}
来源：http://hz.chenlongwang.top/gthdmrpghi.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jinyuanbaomall.cn/gtjkopksfp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.daxiang520.top/gtuohvmcwv.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.yvedp.cn/gtiwmungki.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jyoumei.cn/gtkuanlojt.html

[A17] 位运算
来源：http://hz.zhongyouzk.top/gtxedxsbjo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sufxvd.cn/gtmhuvaqrr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.guowangkeji.top/gtqepxlfrw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yvedp.cn/gtwueimapw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.nanxuanxn.top/gtexmqkxjj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtywwtetzd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtnwqpzgwn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.meibo888.top/gtmhimpzlb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinyuanbaomall.cn/gthdcnsfvv.html

[A18] 字符与 ASCII 码互转
来源：http://hz.tian-w.cn/gtkzbecvjz.html

Py:   ord("A"); chr(65)
来源：http://hz.c1oappe.top/gttixmiqvj.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhongyouzk.top/gtbugtknaj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhixingplan.top/gtijdblktx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhengqikj.top/gtpflctzdv.html

Java: (int) 'A'; (char) 65
来源：http://hz.tanke756.top/gtpmpeocda.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jinqigfzy.top/gthmdirgal.html

Ruby: "A".ord; 65.chr
来源：http://hz.zycfv.cn/gtnatgspts.html

C#:   (int)'A'; (char)65
来源：http://hz.xziqi.cn/gtebcicmxv.html

[A19] 交换两个变量
来源：http://hz.tanke756.top/gtoltnqdpp.html

Py:   a, b = b, a
来源：http://hz.hammf.cn/gtxwhruavo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ehwqpu.com/gtoneilhch.html

JS:   [a, b] = [b, a];
来源：http://hz.0kj1m.cn/gtysqfcvzy.html

TS:   [a, b] = [b, a];
来源：http://hz.feifeiyinyue.top/gthvtcpezl.html

Java: int t = a; a = b; b = t;
来源：http://hz.mhx1999.top/gtrvanvnmc.html

Go:   a, b = b, a
来源：http://hz.snrcjt.cn/gtxxtmezrt.html

Ruby: a, b = b, a
来源：http://hz.quarkkingdee.top/gttkcwswkn.html

C#:   (a, b) = (b, a);
来源：http://hz.sxryk.cn/gtsyivkzyk.html

[A20] 读取标准输入
来源：http://hz.hongshengwenyu.top/gtjloutsat.html

Py:   name = input("请输入：")
来源：http://hz.hongshengwenyu.top/gtlzaefhvg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hnxiangtu.top/gtjhabkaji.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.quarkkingdee.top/gtjrlevxwl.html

TS:   // Node.js：readline 模块
来源：http://hz.jinghuilouyu.cn/gtcxejxhqv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.hnqzz.top/gtyrujycgf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.smart0.xyz/gtldkixqex.html

Ruby: gets.chomp
来源：http://hz.gogol.net.cn/gthqggadld.html

C#:   Console.ReadLine();
来源：http://hz.zhengqikj.top/gttrklxvox.html

[A21] 保留指定小数位输出
来源：http://hz.ydzc1.top/gtidehyses.html

Py:   f"{3.14159:.2f}"
来源：http://hz.pycfn.com/gtpqbherny.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cheryme.top/gthtgwezon.html

JS:   (3.14159).toFixed(2)
来源：http://hz.daxiang520.top/gtdckpaymy.html

TS:   (3.14159).toFixed(2)
来源：http://hz.chenlongwang.top/gtejkrqocz.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.hongshengwenyu.top/gtstgsakdi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.sysykeji.top/gtjeusalmr.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yuanzhike.top/gtrtevgjds.html

C#:   3.14159.ToString("F2")
来源：http://hz.nanxinkj.top/gtznbgassf.html

[A22] 获取字符串长度
来源：http://hz.tian-w.cn/gtpryotyop.html

Py:   len(s)
来源：http://hz.xuetiantiany.cn/gtlqahziye.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.ybcxt.top/gtnoqpkdkl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yonumen.top/gtcuagspiz.html

TS:   s.length
来源：http://hz.yvedp.cn/gtvqpwtxmm.html

Java: s.length()
来源：http://hz.xziqi.cn/gthjnsadmp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.pycfn.com/gtfcwdzode.html

Ruby: s.length
来源：http://hz.yanxiufei.cn/gtbhkcwxjn.html

C#:   s.Length
来源：http://hz.redwolf501.top/gtncrttcqz.html

[A23] 大小写转换
来源：http://hz.birdmap.top/gtrjuyfgvb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.cashguo.top/gtuigzojsw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ivvv.top/gtcunmsjgy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinghuilouyu.cn/gthilctgax.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shzxlz.cn/gtvkrsiutd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zdqjudy.top/gtzuabilrr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.iojbl.cn/gtylfvnyxd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zdqjudy.top/gttposbwtk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yj20258.top/gtrhbsspzj.html

[A24] 去除首尾空白
来源：http://hz.bjfxy.top/gtmeysvhqr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.aizwys.cn/gtelosuwzx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.sweek.top/gtpcxmivsq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tanke756.top/gtdhzraeoi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shuidangran.top/gtapjdzcfw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gzhubu.top/gtzjsvffui.html

Go:   strings.TrimSpace(s)
来源：http://hz.nwbrower.top/gtzpnetzvs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cheryme.top/gtrkotorqk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.gaohongyu789.top/gtfehsmqao.html

[A25] 字符串比较
来源：http://hz.fzhhl.top/gtqvrejqgh.html

Py:   s1 == s2; s1 != s2
来源：http://hz.havefunace.top/gtmagdmubi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ppjwa.cn/gtczfdzoom.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ywan-chungtsiang.top/gtxtstpzth.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cheryme.top/gtjafoamkf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jinqigufen.top/gtztwiuexz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jqgufenzy.top/gtqdnlpksn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.sxryk.cn/gtxjmxylho.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.vqdsnc.cn/gthdgubvyi.html

[A26] 类型转换总览
来源：http://hz.iojbl.cn/gtcwnqrcke.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenlongwang.top/gtbtggbiky.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.fzhhl.top/gtgrpnpfyt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jqgufenzy.top/gtfizhhunz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.tian-w.cn/gthfaujhti.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.birdmap.top/gtxahrizbw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.redwolf501.top/gtnsllvbzu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.sufxvd.cn/gtmmdhutvn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shzxlz.cn/gtzscdmcnb.html

================================================================================
来源：http://hz.ehwqpu.com/gtstsfctcs.html

B. 流程控制
来源：http://hz.ydzc1.top/gtblaqprhj.html

================================================================================
来源：http://hz.hywenlv.cn/gthwoepqbb.html

[B01] 条件判断 if / else
来源：http://hz.hnqzz.top/gtdynkrvqq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yangfankeji.com/gtcxcejllp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yvedp.cn/gtvzjbooef.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gttcmxgwsm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangtech.top/gtsndedakb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jinyuanbaomall.cn/gtrtbxgnwx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jlsjyb.cn/gtowunblhr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yj202588.top/gtduwyvhsz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.guannengcc.top/gtwqxgoffz.html

[B02] 多分支 else if / elif
来源：http://hz.tianlin.xyz/gtdrvuegsf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.316326.xyz/gtvuygagnf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hnqzz.top/gtdpganwxn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtjyzvfhkg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtqeoipqlq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtfmradptm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jiagoushi.top/gtasypitqm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ywan-chungtsiang.top/gtnlrnbfdj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zdqjudy.top/gtrhqyvwxy.html

[B03] switch / match / case
来源：http://hz.cashguo.top/gtqibiwuke.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hnxiangtu.top/gtjsgxfulr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xuetiantiany.cn/gtlaygcamf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xziqi.cn/gtiatcvxze.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tian-w.cn/gteauqblte.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.bjfxy.top/gtwjfeqchg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.xinyue.icu/gtigdfgfov.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.xuetiantiany.cn/gtjqetuqhw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.mhx1999.top/gtovblpsgz.html

[B04] for 计数循环
来源：http://hz.bjfxy.top/gtgkueamcb.html

Py:   for i in range(10): print(i)
来源：http://hz.zhijiandao.cn/gtkcdvectm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.wangshuangyany.cn/gthvrlbdjx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.mhx1999.top/gtcuyxtark.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.c1oappe.top/gtzprprhxw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.dashuyun.cn/gtbiwfdehz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.aibaodan.cn/gtdwpfbbwz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shangyingyoupin.top/gtsjcyepbe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.vqdsnc.cn/gtpjvoujut.html

[B05] 遍历数组 / 列表
来源：http://hz.aibaodan.cn/gtyoamefqh.html

Py:   for item in arr: print(item)
来源：http://hz.shzxlz.cn/gthijbmxhk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xziqi.cn/gtmmpjqomo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xingfuxueyuan.xyz/gtrdfdgfrh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.cucudq.cn/gtnbleesho.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xuetiantiany.cn/gtmnwfasmm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jinghuilouyu.cn/gtqctumcym.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yonumen.top/gthpxbdixw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj20258888.top/gtialjnmwe.html

[B06] 遍历字典 / 对象
来源：http://hz.yueranfly.top/gtqqagnvbd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zdqjudy.top/gtemwttdem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xylfe.cn/gtblwgrorv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hnxiangtu.top/gtvbyvajhp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hfpthk.cn/gtcgljfcmi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ybcxt.top/gtlrhnieke.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shanyushiyangtech.top/gtlgotlnez.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.wangshuangyany.cn/gtluobhwsk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yueranfly.top/gtmfyeqiaq.html

[B07] while 循环
来源：http://hz.jyoumei.cn/gtsffpjhmo.html

Py:   while i < 10: i += 1
来源：http://hz.sufxvd.cn/gtxqhyxtpm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jyoumei.cn/gtwhwmhigv.html

JS:   while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtlqsacvgq.html

TS:   while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtiphpmbml.html

Java: while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtecbtrbfb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.daria6918.cn/gtzugmwapd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.havefunace.top/gtdtvrjivc.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtvodvvkze.html

[B08] do-while（至少执行一次）
来源：http://hz.wangdashe.top/gtilutfwhv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jlsjyb.cn/gtzjfyudnw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.cqqwz.cn/gtcgnxeacw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtdxutkpxh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258.top/gtvnpuyyvu.html

Java: do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtzmvlwtpb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ehwqpu.com/gtklwnmxfg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.sweek.top/gtiqzobryc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtvjluckjw.html

[B09] break 与 continue
来源：http://hz.jinqigfzy.top/gtzplqknlr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gzhubu.top/gtiajlighl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ehwqpu.com/gtanbqhvoy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtbhpvusye.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gtpgdmxyrw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gttjzbxmqr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gotoacloud.top/gtkgomcbcp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenzaomai.com/gtwspspcjs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtvbndpuel.html

[B10] 遍历同时拿索引
来源：http://hz.yongpay.top/gtieytfswr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhengqikj.top/gtqtvgidbp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yueranfly.top/gthwvvjcen.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.andypj.xyz/gtuwgjbhht.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hnqzz.top/gtfioozule.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.cheryme.top/gtivnsfcwk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.haohaochexian.top/gtxsaighev.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ybcxt.top/gtheevmweu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.dashuyun.cn/gtuvnykhns.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenjidiqi.icu/gtugoyzgxi.html

Py:   list(range(0, 10, 2))
来源：http://hz.xylfe.cn/gtlebnngzy.html

PHP:  range(0, 10, 2);
来源：http://hz.daria6918.cn/gtibptghwh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tanke756.top/gtncddjfzx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shuidangran.top/gtxwweifba.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.fengsongda.top/gtthxfcryb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.daria6918.cn/gtaomrnmul.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hnxiangtu.top/gtiatnppzj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ydzc1.top/gttkanrouz.html

[B12] 跳出多层循环
来源：http://hz.nanxinkj.top/gttofffnxl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.andypj.xyz/gtvkgpbkks.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guannengcc.top/gtjiwnsbqx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.feifeiyinyue.top/gtjmoqegdn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tanke756.top/gtbehtojst.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yangfankeji.com/gtkvkmczgn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shanyushiyangkeji.top/gtsraxoqcx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258888.top/gtfjlxqwtc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tian-w.cn/gtxndgjgjs.html

[B13] 判断是否为数字
来源：http://hz.jinghuilouyu.cn/gtdgjyfpxm.html

Py:   isinstance(x, (int, float))
来源：http://hz.fengsongda.top/gtrwwtbfmk.html

PHP:  is_numeric($x)
来源：http://hz.cucudq.cn/gtyqvjkzra.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtsmgunojk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhoulong.xyz/gtihdlqqhs.html

Java: x instanceof Number
来源：http://hz.yongpay.top/gtbqfyecow.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.aibaodan.cn/gtkywqgoyr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.birdmap.top/gtjsvspfxh.html

C#:   x is int or double or decimal
来源：http://hz.xingfuxueyuan.xyz/gtrkyirswy.html

[B14] 判断值是否在集合内
来源：http://hz.bjfxy.top/gtmpxpyvlh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tanke756.top/gtpvrrlgck.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yvedp.cn/gtdmxkbgro.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ehwqpu.com/gtszachizq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhengqikj.top/gtszjsvwlo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jiagoushi.top/gtqvbwlvlo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.bjfxy.top/gtppvviebx.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuanzhike.top/gtlvinarux.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gzhubu.top/gtedwdlxeb.html

[B15] 布尔运算与取反
来源：http://hz.chenzaomai.com/gtkriyjeqt.html

Py:   a and b or not c
来源：http://hz.xylfe.cn/gttfzqduer.html

PHP:  $a && $b || !$c
来源：http://hz.tanke756.top/gtozlpjczc.html

JS:   a && b || !c
来源：http://hz.hysaishi.cn/gtxcqjoygx.html

TS:   a && b || !c
来源：http://hz.chenlongwang.top/gtlhabarvp.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtplfnbnfj.html

Go:   a && b || !c
来源：http://hz.shzxlz.cn/gtviqwwhxd.html

Ruby: a && b || !c
来源：http://hz.pengpengdd.cyou/gttijzzloj.html

C#:   a && b || !c
来源：http://hz.guowangkeji.top/gtbhdmocac.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtsruwtoet.html

Py:   if not data: return
来源：http://hz.316326.xyz/gtkmaodand.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gtifdueatk.html

JS:   if (!data) return;
来源：http://hz.hnqzz.top/gtqwrldslm.html

TS:   if (!data) return;
来源：http://hz.0kj1m.cn/gtmgdmqovh.html

Java: if (data == null) return;
来源：http://hz.gzhubu.top/gtmhidgtct.html

Go:   if data == nil { return }
来源：http://hz.jinqigfzy.top/gtphfvfzuz.html

Ruby: return if data.nil?
来源：http://hz.shzxlz.cn/gtplwsmpaa.html

C#:   if (data == null) return;
来源：http://hz.jlsjyb.cn/gtgxmzgmsy.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrtsvotjt.html

C. 函数与作用域
来源：http://hz.zhoulong.xyz/gtwnqrtcew.html

================================================================================
来源：http://hz.fengsongda.top/gtfszitnuh.html

[C01] 定义函数
来源：http://hz.fzhhl.top/gtbclygzpv.html

Py:   def add(a, b): return a + b
来源：http://hz.guannengcc.top/gtwvtbthgt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gtxxwwysdp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.c1oappe.top/gtaenmqumc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtqwhefcgr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtjsfzjkjc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.sysykeji.top/gtuovnqwsl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xuanzx.com/gtqhvuoxfs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtseptuxpi.html

[C02] 默认参数
来源：http://hz.chenjidiqi.icu/gtqwcsurqb.html

Py:   def greet(name="World"): return name
来源：http://hz.fzhhl.top/gtytlxxnvg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cqqwz.cn/gtuwhirdjw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gogol.net.cn/gtzzbkuitz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.redwolf501.top/gtkqqwrykd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangtech.top/gtjfgcjbcg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guowangkeji.top/gtskxzfjnc.html

Ruby: def greet(name = "World") = name
来源：http://hz.zycfv.cn/gtatbrivtd.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.wangdashe.top/gtbmdtcsoy.html

[C03] 可变参数
来源：http://hz.pengpengdd.cyou/gtjtrillxq.html

Py:   def total(*args): return sum(args)
来源：http://hz.nanxinkj.top/gtpwqpctbh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.tianlin.xyz/gtfrdzkxvw.html


<!-- 参考信息 -->