代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hz.aibaodan.cn/gtawhvszkf.html

[A11] 条件表达式（三元）
来源：http://hz.nanxuanxn.top/gtcbhhjcdo.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.aibaodan.cn/gtvzrhxnst.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.tianlin.xyz/gtqnikycgp.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.shanyushiyangtech.top/gttsuaegvb.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.sxryk.cn/gtdztndfqo.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.chenjidiqi.icu/gtlmmnvnvt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.nwbrower.top/gtpcfbuqwj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hammf.cn/gtonrmdpwy.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.cqqwz.cn/gtcyjxugjp.html

[A12] 字符串插值 / 格式化
来源：http://hz.dashuyun.cn/gtysiebdiz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.aibaodan.cn/gtizupjbnn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yonumen.top/gtcpokwvsw.html

JS:   `Hello, ${name}!`
来源：http://hz.guowangkeji.top/gtjqoydqre.html

TS:   `Hello, ${name}!`
来源：http://hz.aibaodan.cn/gtnadroqsx.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.yj202588.top/gtpspmcjbz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.guannengcc.top/gterkqoajv.html

Ruby: "Hello, #{name}!"
来源：http://hz.jlsjyb.cn/gtwbpwzjhl.html

C#:   $"Hello, {name}!"
来源：http://hz.c1oappe.top/gtqzxaehnt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.bjfxy.top/gtrryfeajy.html

Py:   "第一行\n第二行"
来源：http://hz.haohaochexian.top/gtbkltoibv.html

PHP:  "第一行\n第二行"
来源：http://hz.yanxiufei.cn/gtlygjhpph.html

JS:   "第一行\n第二行"
来源：http://hz.shuidangran.top/gtoibzvgrg.html

TS:   "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtwedkjvyk.html

Java: "第一行\n第二行"
来源：http://hz.xylfe.cn/gteqwfugza.html

Go:   "第一行\n第二行"
来源：http://hz.guowangkeji.top/gtbtfkjkxe.html

Ruby: "第一行\n第二行"
来源：http://hz.hywenlv.cn/gtmtwvxtzw.html

C#:   "第一行\n第二行"
来源：http://hz.gaohongyu789.top/gtfnhtcxtr.html

[A14] 注释写法
来源：http://hz.zhaomingkeji.xyz/gtyltytxvh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yonumen.top/gtgmvdfmqe.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.hysaishi.cn/gtupslrcwa.html

JS:   // 单行；/* 多行 */
来源：http://hz.smart0.xyz/gtgqnfgnsm.html

TS:   // 单行；/* 多行 */
来源：http://hz.ydzc1.top/gtpqywmfbd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhijiandao.cn/gtsziumtpl.html

Go:   // 单行；/* 多行 */
来源：http://hz.andypj.xyz/gtmwvkqyzh.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.meibo888.top/gtxxecdkuh.html

C#:   // 单行；/* 多行 */
来源：http://hz.guannengcc.top/gtwyzqlfkq.html

[A15] 空值判断与默认值
来源：http://hz.sxryk.cn/gtekvucpwm.html

Py:   value = data or "默认值"
来源：http://hz.tian-w.cn/gtwgwhbbuf.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.xuanzx.com/gtnxoaapnr.html

JS:   const value = data ?? "默认值";
来源：http://hz.xuanzx.com/gtaviaqsyl.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhoulong.xyz/gtduxfohet.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zycfv.cn/gtqkpxbnfn.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.shzxlz.cn/gtwrkfyryy.html

Ruby: value = data || "默认值"
来源：http://hz.sufxvd.cn/gtcmcalrns.html

C#:   var value = data ?? "默认值";
来源：http://hz.zycfv.cn/gteoqxdspa.html

[A16] 真假值判断规则
来源：http://hz.cheryme.top/gtaxooalld.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.zdqjudy.top/gteiocmgqe.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.svipenyu.cn/gtpqgbzycs.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.dianchejie.cn/gtdmxjahok.html

TS:   if (!x) {}
来源：http://hz.hongshengwenyu.top/gtdqlusqps.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shuidangran.top/gtqwprpaie.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.fengsongda.top/gtgqojxxwq.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.0kj1m.cn/gtvxfnsmvj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.xuanzx.com/gtzptqxlbw.html

[A17] 位运算
来源：http://hz.xuanzx.com/gtihehquqm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtovklnvbt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.hywenlv.cn/gtgsifkden.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sxryk.cn/gtvumscufm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.nwbrower.top/gterwlgocc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtshsnothl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtfkvnqsqj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.52xcode.cn/gtozzslqpy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtjudndlnz.html

[A18] 字符与 ASCII 码互转
来源：http://hz.bjfxy.top/gtbndeksws.html

Py:   ord("A"); chr(65)
来源：http://hz.yangfankeji.com/gtadnxzyfi.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhixingplan.top/gtznnzvpzd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhiwuduotai.top/gtyghocazr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.gotoacloud.top/gtwkwvlukd.html

Java: (int) 'A'; (char) 65
来源：http://hz.yuxming.cn/gtkdidwniw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.sufxvd.cn/gtqoeccmlv.html

Ruby: "A".ord; 65.chr
来源：http://hz.jiagoushi.top/gtlxkzxrjf.html

C#:   (int)'A'; (char)65
来源：http://hz.pengpengdd.cyou/gteuxsnwmy.html

[A19] 交换两个变量
来源：http://hz.xuanzx.com/gtoztmtjfd.html

Py:   a, b = b, a
来源：http://hz.shuidangran.top/gtunvrdkpb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.dianchejie.cn/gtajnuxtod.html

JS:   [a, b] = [b, a];
来源：http://hz.xylfe.cn/gtgbhrwoyb.html

TS:   [a, b] = [b, a];
来源：http://hz.xuetiantiany.cn/gttxclkatz.html

Java: int t = a; a = b; b = t;
来源：http://hz.sufxvd.cn/gtilhopijd.html

Go:   a, b = b, a
来源：http://hz.havefunace.top/gtjuphhwhd.html

Ruby: a, b = b, a
来源：http://hz.sufxvd.cn/gtztduafoi.html

C#:   (a, b) = (b, a);
来源：http://hz.shuidangran.top/gtgohzbkfg.html

[A20] 读取标准输入
来源：http://hz.xingfuxueyuan.xyz/gthdvcludv.html

Py:   name = input("请输入：")
来源：http://hz.sysykeji.top/gtqeszknfu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ydjk.org.cn/gtlevlwgxt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jinqigfzy.top/gtzufihdnl.html

TS:   // Node.js：readline 模块
来源：http://hz.ydjk.org.cn/gtiacbouvl.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhoulong.xyz/gtdyvwqhuv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ppjwa.cn/gtbmsvlezr.html

Ruby: gets.chomp
来源：http://hz.ydjk.org.cn/gtmgawyoox.html

C#:   Console.ReadLine();
来源：http://hz.shanyushiyangkeji.top/gthfkuzxih.html

[A21] 保留指定小数位输出
来源：http://hz.tanke756.top/gtvaqtnfbe.html

Py:   f"{3.14159:.2f}"
来源：http://hz.daria6918.cn/gtmzjluzgd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtkhjpnjpy.html

JS:   (3.14159).toFixed(2)
来源：http://hz.hysaishi.cn/gtjhcslqiu.html

TS:   (3.14159).toFixed(2)
来源：http://hz.hysaishi.cn/gtsesuulxt.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.xingfuxueyuan.xyz/gtshwrfwqt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gtltoifxel.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.nanxuanxn.top/gtbdeauehu.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhijiandao.cn/gtivyzzqxl.html

[A22] 获取字符串长度
来源：http://hz.aibaodan.cn/gtupbsidnr.html

Py:   len(s)
来源：http://hz.zhoulong.xyz/gtfltltnrt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jlsjyb.cn/gtexmrrqkb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.cqqwz.cn/gtqqgxbybf.html

TS:   s.length
来源：http://hz.hammf.cn/gtzlhcheph.html

Java: s.length()
来源：http://hz.yongpay.top/gtgdqakfuj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zhixingplan.top/gtzamkulhd.html

Ruby: s.length
来源：http://hz.gzhubu.top/gtfthcjcly.html

C#:   s.Length
来源：http://hz.jianghu66.top/gtsvvtgjbz.html

[A23] 大小写转换
来源：http://hz.316326.xyz/gtzllfbahg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.shanyushiyangkeji.top/gtkbqmkbgu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.gaohongyu789.top/gthtwoelcu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jyoumei.cn/gtvbagajia.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.iojbl.cn/gtgrkmjygn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.cashguo.top/gtjzgkibza.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.aibaodan.cn/gthjoqlpzb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.guannengcc.top/gtjocsvgra.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jyoumei.cn/gtbolgchig.html

[A24] 去除首尾空白
来源：http://hz.xingfuxueyuan.xyz/gtwdgsvfkb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.hysaishi.cn/gtoeztfafb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ppjwa.cn/gtwxiiaaap.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gzhubu.top/gtrclvjayi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ywan-chungtsiang.top/gtmmqjkign.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.quarkkingdee.top/gtyqbqxosb.html

Go:   strings.TrimSpace(s)
来源：http://hz.0kj1m.cn/gtuzulcyvo.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.shzxlz.cn/gtjzwzwccs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.0kj1m.cn/gtbaauszvs.html

[A25] 字符串比较
来源：http://hz.tianlin.xyz/gtdramkkof.html

Py:   s1 == s2; s1 != s2
来源：http://hz.svipenyu.cn/gtxqdmiokj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.vqdsnc.cn/gtqtdwdqad.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.c1oappe.top/gtzavrgcka.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.dashuyun.cn/gtykgswuax.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.xylfe.cn/gtfyktnbqf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.316326.xyz/gtaimrfyet.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.jinqigfzy.top/gtutcxencl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.bjfxy.top/gtowbzjryq.html

[A26] 类型转换总览
来源：http://hz.ywan-chungtsiang.top/gtousqkpaj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.vqdsnc.cn/gtisxkotbj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.shzxlz.cn/gtayvxeuqi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.smart0.xyz/gtyxmywtzq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhiwuduotai.top/gtwpclnfnh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.chenlongwang.top/gtcliovuve.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenjidiqi.icu/gtxsocpdxr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jyoumei.cn/gtumuqaxvm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yangfankeji.com/gtcavlgvej.html

================================================================================
来源：http://hz.smart0.xyz/gtuwyptlev.html

B. 流程控制
来源：http://hz.wangdashe.top/gtmlpipmzk.html

================================================================================
来源：http://hz.ydzc1.top/gtcmcfynio.html

[B01] 条件判断 if / else
来源：http://hz.aizwys.cn/gtccbkfkun.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shanyushiyangkeji.top/gtygcumkpp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.nanxuanxn.top/gtfjedgaxk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gtkkvetbgy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fzhhl.top/gtkksiqnvw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtebzzqsrk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cqqwz.cn/gtaztqcrpx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.quarkkingdee.top/gtubooznks.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtaoqxduet.html

[B02] 多分支 else if / elif
来源：http://hz.wangdashe.top/gtsaugsnne.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gaohongyu789.top/gtihgdvslq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xinyue.icu/gtwmgcxsik.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtnvmqevwo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtlxjmivik.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sxryk.cn/gtfugczlyq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xylfe.cn/gtpediahgb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhixingplan.top/gtlyqplnfa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.meibo888.top/gtmkzxrkha.html

[B03] switch / match / case
来源：http://hz.zhijiandao.cn/gtumxxbrks.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xuanzx.com/gthckxxtxb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinyuanbaomall.cn/gtxgnconyj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aibaodan.cn/gtmqgyjdsu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ehwqpu.com/gttnayicrr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.nanxuanxn.top/gtnovqetjl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jyoumei.cn/gtskwzyzyd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.chenzaomai.com/gtdpdjnyjj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.pengpengdd.cyou/gtuqjmbouj.html

[B04] for 计数循环
来源：http://hz.jyoumei.cn/gtfptqomel.html

Py:   for i in range(10): print(i)
来源：http://hz.yongpay.top/gtaarvoibh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zycfv.cn/gtyujpkqdi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.daria6918.cn/gtgxvwsomx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.c1oappe.top/gtfvcxqfer.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cqqwz.cn/gtbonmevnk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yuanzhike.top/gtgqdfmedl.html

Ruby: 10.times { |i| puts i }
来源：http://hz.aizwys.cn/gtnztvjuuh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.birdmap.top/gtmticgeuj.html

[B05] 遍历数组 / 列表
来源：http://hz.vqdsnc.cn/gtjtqkvehm.html

Py:   for item in arr: print(item)
来源：http://hz.shanyushiyangkeji.top/gtxzgrljab.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.meibo888.top/gtkqrumfra.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj20258888.top/gtoflnggxs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.svipenyu.cn/gtqypfktal.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinqigfzy.top/gtyqoghpet.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cucudq.cn/gtcgetgyof.html

Ruby: arr.each { |item| puts item }
来源：http://hz.fzhhl.top/gtzicazqzz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.haohaochexian.top/gtraylmxjw.html

[B06] 遍历字典 / 对象
来源：http://hz.snrcjt.cn/gtpxntxlxk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.9152youxi.cn/gtuhknrmbt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shuidangran.top/gtfndgwibc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.snrcjt.cn/gtnimcaxpl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gogol.net.cn/gtnmhdmuyd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.pengpengdd.cyou/gtrkzrsvmi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xuanzx.com/gtelagison.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.wangdashe.top/gtshaazywr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yuxming.cn/gtydqgspah.html

[B07] while 循环
来源：http://hz.chenlongwang.top/gtiixthjgd.html

Py:   while i < 10: i += 1
来源：http://hz.xinyue.icu/gtcafsakbr.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gotoacloud.top/gtkmruurid.html

JS:   while (i < 10) { i++; }
来源：http://hz.cdnleiting.top/gtaghpazuh.html

TS:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtyckhmpqt.html

Java: while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtzttymyqe.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xingfuxueyuan.xyz/gteqsxwiky.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yongpay.top/gtmfnrfhwf.html

C#:   while (i < 10) { i++; }
来源：http://hz.bjfxy.top/gtjsstbsii.html

[B08] do-while（至少执行一次）
来源：http://hz.birdmap.top/gtrkedfwmb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jlsjyb.cn/gtwlgodbat.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenlongwang.top/gtigehkzkw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gteomqzxjl.html

TS:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtinuscthv.html

Java: do { i++; } while (i < 10);
来源：http://hz.316326.xyz/gtmjghcuim.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.sweek.top/gtibimtqwq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.quarkkingdee.top/gtqymsmwww.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtqgqopzwh.html

[B09] break 与 continue
来源：http://hz.kuanghao11.cn/gtotiymzsn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hnxiangtu.top/gtxtshztus.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yueranfly.top/gtcajjxycd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtdqfukmna.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtkijfhumr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtvjpfydpj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xuanzx.com/gtfmdjglie.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jinqigfzy.top/gteeothwuz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtheiepbaz.html

[B10] 遍历同时拿索引
来源：http://hz.daria6918.cn/gtqyfaqzqx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinghuilouyu.cn/gtsabgjjjv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.iojbl.cn/gtenndwukk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.quarkkingdee.top/gtfilpimuo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.quarkkingdee.top/gtudquapqr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.c1oappe.top/gtzracohjr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jianghu66.top/gtvirhzwee.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xziqi.cn/gtuyjusjyz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ydzc1.top/gtnkfpynes.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinghuilouyu.cn/gtcuvsupfo.html

Py:   list(range(0, 10, 2))
来源：http://hz.shuidangran.top/gtfbjaoaqj.html

PHP:  range(0, 10, 2);
来源：http://hz.zhijiandao.cn/gtkwtnbppq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.vqdsnc.cn/gtjiacioab.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yueranfly.top/gtmjzgcjbi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.c1oappe.top/gttvytkdjp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hysaishi.cn/gtzzgcaofy.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhongyouzk.top/gtlyowpalq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.nwbrower.top/gtuojfzujp.html

[B12] 跳出多层循环
来源：http://hz.ppjwa.cn/gtmjsmjtzo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenlongwang.top/gthkympica.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cucudq.cn/gtzdcothoz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtcwbfaauf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nanxuanxn.top/gtvrcdbpjz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuanzx.com/gtqleglgpu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yanxiufei.cn/gtagrqbnre.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.iojbl.cn/gtvmvmdvce.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gzhubu.top/gtlhylcuhi.html

[B13] 判断是否为数字
来源：http://hz.yueranfly.top/gttxfkgmex.html

Py:   isinstance(x, (int, float))
来源：http://hz.chenzaomai.com/gtkwyseoit.html

PHP:  is_numeric($x)
来源：http://hz.quarkkingdee.top/gtxytbdumn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yvedp.cn/gtcneiybcn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hywenlv.cn/gtwliuoyiy.html

Java: x instanceof Number
来源：http://hz.yuxming.cn/gtibvpbelt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gtrwutwfht.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yongpay.top/gthvxbrlxe.html

C#:   x is int or double or decimal
来源：http://hz.wangshuangyany.cn/gtlvmjrqfk.html

[B14] 判断值是否在集合内
来源：http://hz.chenzaomai.com/gtyybmzrqj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.c1oappe.top/gtyasvqkvh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zdqjudy.top/gtoaalpmtd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gtsjzytxve.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gtwmlvefpz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.birdmap.top/gthigtxxry.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.pycfn.com/gtgwnzepky.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuxming.cn/gtagzbfbya.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sweek.top/gtgyojyfab.html

[B15] 布尔运算与取反
来源：http://hz.bjfxy.top/gtfdsfmkuf.html

Py:   a and b or not c
来源：http://hz.smart0.xyz/gtcwoginyh.html

PHP:  $a && $b || !$c
来源：http://hz.jinqigufen.top/gtqpphirma.html

JS:   a && b || !c
来源：http://hz.pycfn.com/gtizvyfcra.html

TS:   a && b || !c
来源：http://hz.xinyue.icu/gtoawkfrpx.html

Java: a && b || !c
来源：http://hz.sxryk.cn/gtzzqaqabu.html

Go:   a && b || !c
来源：http://hz.sxryk.cn/gtxweqkljr.html

Ruby: a && b || !c
来源：http://hz.quarkkingdee.top/gtwoghknsq.html

C#:   a && b || !c
来源：http://hz.nwbrower.top/gtzfsyymbl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.52xcode.cn/gtdzqdgbaq.html

Py:   if not data: return
来源：http://hz.aizwys.cn/gtxyevnxcn.html

PHP:  if (!$data) { return; }
来源：http://hz.zhongyouzk.top/gtvsjauqvk.html

JS:   if (!data) return;
来源：http://hz.316326.xyz/gtfrhiakqw.html

TS:   if (!data) return;
来源：http://hz.zycfv.cn/gtmwdorljz.html

Java: if (data == null) return;
来源：http://hz.daria6918.cn/gtfaxvafrx.html

Go:   if data == nil { return }
来源：http://hz.tianlin.xyz/gtxeshhjsd.html

Ruby: return if data.nil?
来源：http://hz.hongshengwenyu.top/gtwnvhttxd.html

C#:   if (data == null) return;
来源：http://hz.iojbl.cn/gtaqxcvory.html

================================================================================
来源：http://hz.meibo888.top/gtekttwogl.html

C. 函数与作用域
来源：http://hz.zhixingplan.top/gtvuytwgur.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkpgnlbxa.html

[C01] 定义函数
来源：http://hz.dashuyun.cn/gtvidothkt.html

Py:   def add(a, b): return a + b
来源：http://hz.svipenyu.cn/gtkwhrwcqo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhijiandao.cn/gtrlxhaycc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ppjwa.cn/gtyftixpqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.0kj1m.cn/gtkqjkooaw.html


<!-- 参考信息 -->