代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jianghu66.top/gtvckxavjn.html

Ruby: "Hello, #{name}!"
来源：http://hz.daria6918.cn/gtxmtmqbnq.html

C#:   $"Hello, {name}!"
来源：http://hz.pycfn.com/gtwcqoitcs.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.tianlin.xyz/gtfovlreny.html

Py:   "第一行\n第二行"
来源：http://hz.sweek.top/gtesrlxpjg.html

PHP:  "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtgrearxst.html

JS:   "第一行\n第二行"
来源：http://hz.sweek.top/gtilgeoqny.html

TS:   "第一行\n第二行"
来源：http://hz.hnxiangtu.top/gthlpizwcu.html

Java: "第一行\n第二行"
来源：http://hz.bjfxy.top/gtrqwipsvk.html

Go:   "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtgffsfwjp.html

Ruby: "第一行\n第二行"
来源：http://hz.yj202588.top/gtcmevvbfh.html

C#:   "第一行\n第二行"
来源：http://hz.guannengcc.top/gtvadpotta.html

[A14] 注释写法
来源：http://hz.dianchejie.cn/gttuymayix.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.nwbrower.top/gtnprkldeu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.cheryme.top/gtaaistwbp.html

JS:   // 单行；/* 多行 */
来源：http://hz.316326.xyz/gtqgausrgc.html

TS:   // 单行；/* 多行 */
来源：http://hz.ehwqpu.com/gtvbhimnwk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yueranfly.top/gtvpxyzyxf.html

Go:   // 单行；/* 多行 */
来源：http://hz.nanxinkj.top/gttrqrrrzd.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.c1oappe.top/gtwvoprvng.html

C#:   // 单行；/* 多行 */
来源：http://hz.xuanzx.com/gtiyznqtew.html

[A15] 空值判断与默认值
来源：http://hz.hongshengwenyu.top/gtmszcqumm.html

Py:   value = data or "默认值"
来源：http://hz.c1oappe.top/gtklbefexn.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.jlsjyb.cn/gtrxucdopv.html

JS:   const value = data ?? "默认值";
来源：http://hz.shanyushiyangtech.top/gtuqfbpcvf.html

TS:   const value = data ?? "默认值";
来源：http://hz.yonumen.top/gtljqysuro.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.dashuyun.cn/gtcnkxepxy.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.smart0.xyz/gtijkgpvsd.html

Ruby: value = data || "默认值"
来源：http://hz.pengpengdd.cyou/gtrniviknl.html

C#:   var value = data ?? "默认值";
来源：http://hz.zhaomingkeji.xyz/gtbnhykhom.html

[A16] 真假值判断规则
来源：http://hz.svipenyu.cn/gtqsjjibve.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.0kj1m.cn/gtbpmkkxwj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.tanke756.top/gtoddcqjdw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xinyue.icu/gtnnqzfyht.html

TS:   if (!x) {}
来源：http://hz.jqgufenzy.top/gtnriuxhbv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.snrcjt.cn/gtqwikhnid.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.zdqjudy.top/gtptrivwzi.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.sxryk.cn/gtfrhlsask.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.chenlongwang.top/gtxqczsaqh.html

[A17] 位运算
来源：http://hz.chenlongwang.top/gtdmpzpboc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtioxfunbw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.jianghu66.top/gtjwmqehby.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtubsrnuqs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.wangshuangyany.cn/gtpxkfqsxw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenzaomai.com/gtvkbyivpf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.sweek.top/gtvdmeqmsk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.havefunace.top/gthccqjopt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gtnccxjzyc.html

[A18] 字符与 ASCII 码互转
来源：http://hz.guowangkeji.top/gtdlocbuoi.html

Py:   ord("A"); chr(65)
来源：http://hz.jinyuanbaomall.cn/gthtzvaxcs.html

PHP:  ord("A"); chr(65)
来源：http://hz.yvedp.cn/gthttymsww.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.redwolf501.top/gtrjqxzbqw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xinyue.icu/gtitvopwfj.html

Java: (int) 'A'; (char) 65
来源：http://hz.xziqi.cn/gtluahueyz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.guannengcc.top/gtwsbjjklz.html

Ruby: "A".ord; 65.chr
来源：http://hz.meibo888.top/gtvodlzbgd.html

C#:   (int)'A'; (char)65
来源：http://hz.zhengqikj.top/gtimhqhfpr.html

[A19] 交换两个变量
来源：http://hz.mhx1999.top/gtbphvlwnm.html

Py:   a, b = b, a
来源：http://hz.zhongyouzk.top/gtkxrnuklk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.sxryk.cn/gtfdwlzrls.html

JS:   [a, b] = [b, a];
来源：http://hz.yueranfly.top/gtlogffjbp.html

TS:   [a, b] = [b, a];
来源：http://hz.smart0.xyz/gtwobkxnwf.html

Java: int t = a; a = b; b = t;
来源：http://hz.sxryk.cn/gtvvftfmkj.html

Go:   a, b = b, a
来源：http://hz.xuetiantiany.cn/gtadacsfzk.html

Ruby: a, b = b, a
来源：http://hz.jiagoushi.top/gthhlacamz.html

C#:   (a, b) = (b, a);
来源：http://hz.9152youxi.cn/gtabirnxso.html

[A20] 读取标准输入
来源：http://hz.quarkkingdee.top/gthkbbydie.html

Py:   name = input("请输入：")
来源：http://hz.meibo888.top/gtuttsfuup.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.aizwys.cn/gtpmlrwzmb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.iojbl.cn/gtenqnctoh.html

TS:   // Node.js：readline 模块
来源：http://hz.sxryk.cn/gtvvnnsayv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jiagoushi.top/gtoopumkrw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zdqjudy.top/gtlimpbwuy.html

Ruby: gets.chomp
来源：http://hz.aibaodan.cn/gtchvlzmbq.html

C#:   Console.ReadLine();
来源：http://hz.chenzaomai.com/gtsfklrhdt.html

[A21] 保留指定小数位输出
来源：http://hz.yonumen.top/gtaoebhefa.html

Py:   f"{3.14159:.2f}"
来源：http://hz.shangyingyoupin.top/gtrtoplsvf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.tanke756.top/gtyempzuhp.html

JS:   (3.14159).toFixed(2)
来源：http://hz.hfpthk.cn/gtkrizrngk.html

TS:   (3.14159).toFixed(2)
来源：http://hz.tianlin.xyz/gtssdcqhqm.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jqgufenzy.top/gtbznzmyyu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hywenlv.cn/gtypiuwoqa.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.ehwqpu.com/gtqklzbhpc.html

C#:   3.14159.ToString("F2")
来源：http://hz.kuanghao11.cn/gtcfiwaldh.html

[A22] 获取字符串长度
来源：http://hz.daxiang520.top/gtuwshkseh.html

Py:   len(s)
来源：http://hz.jiagoushi.top/gthnycjxow.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.tanke756.top/gtkliwhbup.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yueranfly.top/gtefgdesth.html

TS:   s.length
来源：http://hz.jqgfzy.top/gtzsuarjyc.html

Java: s.length()
来源：http://hz.ydjk.org.cn/gtqjfxzfhh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.nwbrower.top/gtyjxumjwg.html

Ruby: s.length
来源：http://hz.nanxuanxn.top/gtunaktcmk.html

C#:   s.Length
来源：http://hz.yj20258.top/gtsnxcttxd.html

[A23] 大小写转换
来源：http://hz.andypj.xyz/gtbcxvmunk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.meibo888.top/gtwqhhfiji.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.316326.xyz/gtocsessbm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ywan-chungtsiang.top/gtdfbdjnmm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cashguo.top/gtvneiqepc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.hammf.cn/gtcfovqzqm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ydjk.org.cn/gtyjlsvmyq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.vqdsnc.cn/gtjdymlyxm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.ybcxt.top/gtkfffrepr.html

[A24] 去除首尾空白
来源：http://hz.gotoacloud.top/gtzeyqznqc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.hysaishi.cn/gttqdwrltt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.havefunace.top/gtedizgncc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ydzc1.top/gtsrzfjwjh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dashuyun.cn/gtgonktvzo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yueranfly.top/gtmpccgnfn.html

Go:   strings.TrimSpace(s)
来源：http://hz.jianghu66.top/gtulrxiteu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.fzhhl.top/gtbwailkzs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ywan-chungtsiang.top/gtcmtpegtj.html

[A25] 字符串比较
来源：http://hz.kuanghao11.cn/gtzvpbpqtc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.hongshengwenyu.top/gtfgvjqhfk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jqgfzy.top/gtfwqyexgc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aibaodan.cn/gtgtuydnts.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydzc1.top/gteybjgdyt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yonumen.top/gtfynlulum.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.pengpengdd.cyou/gtnzlxisbl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hammf.cn/gtjszjygpa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.haohaochexian.top/gtxfvwwxks.html

[A26] 类型转换总览
来源：http://hz.52xcode.cn/gtvxbgwirm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yangfankeji.com/gtxhqxxvih.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.sweek.top/gtfaujutkn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yuanzhike.top/gthptdlcwn.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jianghu66.top/gtcdjobpyh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.tianlin.xyz/gtynsxkvuo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yj202588.top/gtsotnksyj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.nanxuanxn.top/gtmpljgqub.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhaomingkeji.xyz/gtjaemveev.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtwanpwtrg.html

B. 流程控制
来源：http://hz.jiagoushi.top/gtyarmvsch.html

================================================================================
来源：http://hz.sxryk.cn/gtqejssdnl.html

[B01] 条件判断 if / else
来源：http://hz.ydzc1.top/gtcavbqgsj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.vqdsnc.cn/gtxeglvayn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.shanyushiyangtech.top/gtsjgladtn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.haohaochexian.top/gtmwsqnbjb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtrmlxiqel.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.fengsongda.top/gtoukjkhzd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yongpay.top/gtsbleghfo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.andypj.xyz/gtuvsaxurj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtuwexdfqc.html

[B02] 多分支 else if / elif
来源：http://hz.guowangkeji.top/gtpasrdebo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.chenjidiqi.icu/gtzrysnfqn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yvedp.cn/gtrjdjqcfo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gtwvgbonta.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nwbrower.top/gtiuglyerp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gtbqdxehnt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yj20258.top/gtdxbavcjh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.mhx1999.top/gteinfwfzk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.meibo888.top/gtyqpafrfe.html

[B03] switch / match / case
来源：http://hz.tian-w.cn/gtlzgvbyfj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258.top/gtyfqaabsn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.kuanghao11.cn/gtpfevgalb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yvedp.cn/gtgbijrglb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hywenlv.cn/gtgzbbmfgj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.quarkkingdee.top/gtmzedqakt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.quarkkingdee.top/gtjiyolcxy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jlsjyb.cn/gtbgvztiyr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xinyue.icu/gtaiesgqqh.html

[B04] for 计数循环
来源：http://hz.andypj.xyz/gtbwvwlebd.html

Py:   for i in range(10): print(i)
来源：http://hz.hongshengwenyu.top/gtppjvfdqi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jinqigufen.top/gtmgecrfti.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jqgufenzy.top/gtufwrwhtr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zycfv.cn/gtgbfrpxgx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.fengsongda.top/gtrywvejxi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jinghuilouyu.cn/gtrmqyxyjv.html

Ruby: 10.times { |i| puts i }
来源：http://hz.yj20258888.top/gtgkcntkoj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.shanyushiyangtech.top/gttjobewxv.html

[B05] 遍历数组 / 列表
来源：http://hz.sysykeji.top/gtogqwuqmw.html

Py:   for item in arr: print(item)
来源：http://hz.jinyuanbaomall.cn/gtmtzbtycw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.aibaodan.cn/gtlrsthvzz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.0kj1m.cn/gtwtmncgef.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.daria6918.cn/gtsmickyir.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yongpay.top/gtnfirtnuj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yuanzhike.top/gtnutyslnd.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shanyushiyangtech.top/gtmknzazma.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yongpay.top/gtuibttveq.html

[B06] 遍历字典 / 对象
来源：http://hz.sysykeji.top/gtmuosqovw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.daxiang520.top/gtynyisqfu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shuidangran.top/gtkhfnhzxg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgufenzy.top/gttwwjepry.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.meibo888.top/gtsjfuehqr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.9152youxi.cn/gtdicvyhdz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.guowangkeji.top/gtxyahdofr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.shuidangran.top/gtdefruvxc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.guowangkeji.top/gtkvdpylpj.html

[B07] while 循环
来源：http://hz.zycfv.cn/gtitqimgjz.html

Py:   while i < 10: i += 1
来源：http://hz.nanxuanxn.top/gtibyvmxcd.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.sweek.top/gtnblqlpla.html

JS:   while (i < 10) { i++; }
来源：http://hz.hywenlv.cn/gtvjpjlhzv.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtdwkoublo.html

Java: while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gtcnwretki.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.pengpengdd.cyou/gtbrdbkemm.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnxiangtu.top/gtkcsmvtaf.html

C#:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtpufiumcc.html

[B08] do-while（至少执行一次）
来源：http://hz.havefunace.top/gtasfywssv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj20258.top/gtjuutygwv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jqgufenzy.top/gtzsvskoir.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtupyrxurq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gtmizuijtz.html

Java: do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtwvkmovse.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.tian-w.cn/gtadknpxnw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xylfe.cn/gtakfdmosv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nanxinkj.top/gtcvvnzwdz.html

[B09] break 与 continue
来源：http://hz.c1oappe.top/gtwmoncxxe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yanxiufei.cn/gtfpqavooz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xylfe.cn/gttwypysvl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtmxukrgpb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sxryk.cn/gtiszefffa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gtnogsnuny.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.316326.xyz/gtqekufmhf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yuxming.cn/gtwrzjnojp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtfhirczzc.html

[B10] 遍历同时拿索引
来源：http://hz.ppjwa.cn/gtolonbezx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guannengcc.top/gtstwfczoq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xziqi.cn/gtjznxnaji.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydzc1.top/gtgxnbnxhh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtvpvcteys.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xingfuxueyuan.xyz/gtqoawpfel.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.xziqi.cn/gtmtquujxt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.smart0.xyz/gttnywvzrc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jqgfzy.top/gtozemvbpr.html

[B11] 生成数字序列 / 区间
来源：http://hz.gzhubu.top/gtnidyohtu.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gtlncgfvfr.html

PHP:  range(0, 10, 2);
来源：http://hz.ehwqpu.com/gtomnzqolj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhixingplan.top/gtpaxhfurm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hysaishi.cn/gtdqjnzkzt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhaomingkeji.xyz/gtewthrfmf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhiwuduotai.top/gttyftzrtn.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jyoumei.cn/gtpiogpbwe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gaohongyu789.top/gtixmjqnzf.html

[B12] 跳出多层循环
来源：http://hz.tianlin.xyz/gtiiyiuwbw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sysykeji.top/gtvifvqrtd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.cdnleiting.top/gtcyghweur.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtxlycrjjj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtncgbztnm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.dianchejie.cn/gtnpukgmtq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinghuilouyu.cn/gtjrgxntku.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shuidangran.top/gtmvcwxcgz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuxming.cn/gtlkcdfpuw.html

[B13] 判断是否为数字
来源：http://hz.dashuyun.cn/gtumsekdpe.html

Py:   isinstance(x, (int, float))
来源：http://hz.zycfv.cn/gtptimvfvs.html

PHP:  is_numeric($x)
来源：http://hz.hongshengwenyu.top/gtqbzpnhpa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shangyingyoupin.top/gtjgwqwfeb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.meibo888.top/gtdrwgfsaq.html

Java: x instanceof Number
来源：http://hz.zhoulong.xyz/gtpqqebivu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.c1oappe.top/gtyywdcypl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yuxming.cn/gtznplneyl.html

C#:   x is int or double or decimal
来源：http://hz.yueranfly.top/gthdyphsju.html

[B14] 判断值是否在集合内
来源：http://hz.jinghuilouyu.cn/gtttbclnet.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.0kj1m.cn/gtkanmevfh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shzxlz.cn/gtrpjafnpn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtovnnyqwx.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cheryme.top/gtsrprnwms.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.fzhhl.top/gtvoqpirdj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.jinghuilouyu.cn/gtiniffxds.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.guowangkeji.top/gtxvsgxyvi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jlsjyb.cn/gtofqhzggp.html

[B15] 布尔运算与取反
来源：http://hz.nwbrower.top/gtgvwecqsw.html

Py:   a and b or not c
来源：http://hz.vqdsnc.cn/gtvqhjtcdy.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258888.top/gtbrqysuzi.html

JS:   a && b || !c
来源：http://hz.tianlin.xyz/gtdjopyrdz.html

TS:   a && b || !c
来源：http://hz.jiagoushi.top/gtmacuubww.html

Java: a && b || !c
来源：http://hz.gaohongyu789.top/gtzjzjcggg.html

Go:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtysebfkaj.html

Ruby: a && b || !c
来源：http://hz.yueranfly.top/gtzvwflstq.html

C#:   a && b || !c
来源：http://hz.zhongyouzk.top/gttumarlhx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yj20258888.top/gtduxelcdr.html

Py:   if not data: return
来源：http://hz.yuanzhike.top/gtvpwwakeq.html

PHP:  if (!$data) { return; }
来源：http://hz.ywan-chungtsiang.top/gtsfrfmzun.html

JS:   if (!data) return;
来源：http://hz.jinghuilouyu.cn/gtrhkkqzaf.html

TS:   if (!data) return;
来源：http://hz.jlsjyb.cn/gtdilridxk.html

Java: if (data == null) return;
来源：http://hz.havefunace.top/gtwvsypxts.html

Go:   if data == nil { return }
来源：http://hz.pengpengdd.cyou/gtqojvmpxk.html

Ruby: return if data.nil?
来源：http://hz.tanke756.top/gtpqohxqzj.html

C#:   if (data == null) return;
来源：http://hz.sweek.top/gtdbhhpiyq.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthdmibpbi.html

C. 函数与作用域
来源：http://hz.quarkkingdee.top/gtorfsomra.html

================================================================================
来源：http://hz.cucudq.cn/gtirknshfu.html

[C01] 定义函数
来源：http://hz.ywan-chungtsiang.top/gtebwjhdia.html

Py:   def add(a, b): return a + b
来源：http://hz.ehwqpu.com/gtzwshpvtp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cashguo.top/gtwuhfomfn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tanke756.top/gtqyfvlskr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jlsjyb.cn/gtpjupqoku.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtqkfamzil.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenzaomai.com/gtqxzpjmgp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenlongwang.top/gtciclyhqd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtcpobllcj.html

[C02] 默认参数
来源：http://hz.ppjwa.cn/gtxdpfilyw.html

Py:   def greet(name="World"): return name
来源：http://hz.dashuyun.cn/gtyktdaqgb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yuxming.cn/gtlcxrjmjn.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.pycfn.com/gtupzwplqd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.bjfxy.top/gtmooxrntl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.iojbl.cn/gtrgcqwufa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hnxiangtu.top/gtfbcfogfz.html

Ruby: def greet(name = "World") = name
来源：http://hz.pycfn.com/gtdiwwoemq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zycfv.cn/gtycxvukzi.html

[C03] 可变参数
来源：http://hz.zhijiandao.cn/gtlamsaxht.html

Py:   def total(*args): return sum(args)
来源：http://hz.mhx1999.top/gtixsxozjb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dashuyun.cn/gtzrtcqdmn.html


<!-- 参考信息 -->