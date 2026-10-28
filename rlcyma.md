代发 wailian999

[A14] 注释写法
来源：http://hz.yj20258.top/gtuekvbwul.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.xinyue.icu/gtcnbxhupk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.havefunace.top/gttnqjpgho.html

JS:   // 单行；/* 多行 */
来源：http://hz.pycfn.com/gtrxtricvw.html

TS:   // 单行；/* 多行 */
来源：http://hz.ehwqpu.com/gtgvcbbdvb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.hnxiangtu.top/gtolhdmvka.html

Go:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtfkmuolow.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.dianchejie.cn/gtxfjtlzqx.html

C#:   // 单行；/* 多行 */
来源：http://hz.jlsjyb.cn/gtkxfnknyx.html

[A15] 空值判断与默认值
来源：http://hz.zhaomingkeji.xyz/gtiwhmhwie.html

Py:   value = data or "默认值"
来源：http://hz.nwbrower.top/gthypaipbm.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zhoulong.xyz/gtyonczjlj.html

JS:   const value = data ?? "默认值";
来源：http://hz.pengpengdd.cyou/gtauohxnoj.html

TS:   const value = data ?? "默认值";
来源：http://hz.tanke756.top/gtezoxwjab.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.daria6918.cn/gtpiwectiq.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.aibaodan.cn/gtqahwlhdz.html

Ruby: value = data || "默认值"
来源：http://hz.tian-w.cn/gtfnphyvfq.html

C#:   var value = data ?? "默认值";
来源：http://hz.pengpengdd.cyou/gtaunnookv.html

[A16] 真假值判断规则
来源：http://hz.bjfxy.top/gtctaygqfm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.mhx1999.top/gtmfdivfkb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.andypj.xyz/gtmhltgpde.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.guannengcc.top/gtxubpedce.html

TS:   if (!x) {}
来源：http://hz.xuanzx.com/gtbfqjkyop.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.gogol.net.cn/gtptcugrsz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.sweek.top/gtrasrldrj.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.gotoacloud.top/gtqgbqhfkd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zhixingplan.top/gtbzhjoppe.html

[A17] 位运算
来源：http://hz.yanxiufei.cn/gtnwhpibjd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtujoevbys.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.smart0.xyz/gtkntxhnjn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtxramhpsf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jyoumei.cn/gtphsufgxp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fengsongda.top/gteeskswzg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.xuetiantiany.cn/gtugpmabhd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gtorkoieky.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shanyushiyangkeji.top/gtalpcaytm.html

[A18] 字符与 ASCII 码互转
来源：http://hz.havefunace.top/gtfabfeeib.html

Py:   ord("A"); chr(65)
来源：http://hz.kuanghao11.cn/gtjsvhmhph.html

PHP:  ord("A"); chr(65)
来源：http://hz.tanke756.top/gtquzqkmdy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hnqzz.top/gtsneofcpz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yanxiufei.cn/gtzsguiwwa.html

Java: (int) 'A'; (char) 65
来源：http://hz.quarkkingdee.top/gtvktxfzvi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.daria6918.cn/gthzjhecfa.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhijiandao.cn/gtgvoklypq.html

C#:   (int)'A'; (char)65
来源：http://hz.jinghuilouyu.cn/gtnsbbjgjv.html

[A19] 交换两个变量
来源：http://hz.sufxvd.cn/gtlckojdyq.html

Py:   a, b = b, a
来源：http://hz.yueranfly.top/gtqphvcuoc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.mhx1999.top/gtfcayvmvu.html

JS:   [a, b] = [b, a];
来源：http://hz.dianchejie.cn/gtqticdkro.html

TS:   [a, b] = [b, a];
来源：http://hz.chenzaomai.com/gtfdkzksjo.html

Java: int t = a; a = b; b = t;
来源：http://hz.yueranfly.top/gtqlqmvdeq.html

Go:   a, b = b, a
来源：http://hz.ydjk.org.cn/gtwjshqzxv.html

Ruby: a, b = b, a
来源：http://hz.fzhhl.top/gtwcnuibfd.html

C#:   (a, b) = (b, a);
来源：http://hz.xylfe.cn/gtvizgrdye.html

[A20] 读取标准输入
来源：http://hz.ivvv.top/gtvemsnnyd.html

Py:   name = input("请输入：")
来源：http://hz.smart0.xyz/gtzglupxov.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.shanyushiyangtech.top/gtsxdcilgc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yanxiufei.cn/gtspfwdfgn.html

TS:   // Node.js：readline 模块
来源：http://hz.hnqzz.top/gtovyfyvjg.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.vqdsnc.cn/gtftazbtqd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jinqigufen.top/gtyvxkuohy.html

Ruby: gets.chomp
来源：http://hz.jianghu66.top/gtnrvdsayn.html

C#:   Console.ReadLine();
来源：http://hz.yuxming.cn/gtsyhyrapi.html

[A21] 保留指定小数位输出
来源：http://hz.shzxlz.cn/gtrtehwlyk.html

Py:   f"{3.14159:.2f}"
来源：http://hz.shuidangran.top/gtjqminsmq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.iojbl.cn/gttuegodkg.html

JS:   (3.14159).toFixed(2)
来源：http://hz.haohaochexian.top/gtvkdpobcs.html

TS:   (3.14159).toFixed(2)
来源：http://hz.havefunace.top/gtqzcxgstt.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yongpay.top/gtemipsrwm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.havefunace.top/gtrmjhzoyt.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.quarkkingdee.top/gtxikqtufm.html

C#:   3.14159.ToString("F2")
来源：http://hz.cashguo.top/gtztgmucvk.html

[A22] 获取字符串长度
来源：http://hz.jlsjyb.cn/gteczmauyi.html

Py:   len(s)
来源：http://hz.c1oappe.top/gtfmebxnjz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.fzhhl.top/gtydqdaldx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.sweek.top/gtwyfjnbvq.html

TS:   s.length
来源：http://hz.aizwys.cn/gtpemrurnm.html

Java: s.length()
来源：http://hz.nanxuanxn.top/gtailsdmmr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.zycfv.cn/gtfcqmrwyj.html

Ruby: s.length
来源：http://hz.xinyue.icu/gtzuzvzppc.html

C#:   s.Length
来源：http://hz.zhengqikj.top/gtjrewnpfr.html

[A23] 大小写转换
来源：http://hz.nanxinkj.top/gttyfkbvsj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zhixingplan.top/gtqsnewfgv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.c1oappe.top/gtepfqrkjs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj20258.top/gtaoszrgxz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gaohongyu789.top/gtizprmowc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.guannengcc.top/gtdfqtsero.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.wangdashe.top/gtxlzivobb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinqigfzy.top/gtxnkigupb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.sufxvd.cn/gtrkeuybvv.html

[A24] 去除首尾空白
来源：http://hz.jianghu66.top/gthhfdrcep.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.hnxiangtu.top/gtsylpisix.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yongpay.top/gtuemqnobi.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gotoacloud.top/gttldhfhpd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.chenjidiqi.icu/gtnaeyubth.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jinqigfzy.top/gtbnrnpwix.html

Go:   strings.TrimSpace(s)
来源：http://hz.yonumen.top/gtqydboyxi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.52xcode.cn/gtzacvzknh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.birdmap.top/gtwqbuxgih.html

[A25] 字符串比较
来源：http://hz.bjfxy.top/gtlgezhqti.html

Py:   s1 == s2; s1 != s2
来源：http://hz.nanxuanxn.top/gtehxmjunq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yonumen.top/gtwgyvmafd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aibaodan.cn/gtrorfflfy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.dashuyun.cn/gtmwqqliky.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.andypj.xyz/gtsdubxhjy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.aibaodan.cn/gtaihrenls.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.haohaochexian.top/gtlyyozkms.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xziqi.cn/gtldosznev.html

[A26] 类型转换总览
来源：http://hz.gaohongyu789.top/gtpmwubyun.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.fengsongda.top/gtmmbarher.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.9152youxi.cn/gteyssjmsi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.ybcxt.top/gtscdjkoeq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.shanyushiyangkeji.top/gtleemxdae.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.xziqi.cn/gtrqzoefio.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hysaishi.cn/gtokqzpmdy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.nanxuanxn.top/gtllealgjl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hysaishi.cn/gtmfhybvip.html

================================================================================
来源：http://hz.hfpthk.cn/gtlgbfgvhw.html

B. 流程控制
来源：http://hz.xingfuxueyuan.xyz/gtcqfqwqcb.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpecidlow.html

[B01] 条件判断 if / else
来源：http://hz.jinqigufen.top/gtnyjevcbi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jinqigufen.top/gtpnvlercq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yueranfly.top/gtinboecoy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gtxxutqxxz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tanke756.top/gtmiielwar.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtxtisaeuu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.fzhhl.top/gtvjxihldd.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.hywenlv.cn/gthmvntsss.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gtcqjpdeyo.html

[B02] 多分支 else if / elif
来源：http://hz.yuxming.cn/gtaaohfaak.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.guannengcc.top/gtnkudsqel.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.andypj.xyz/gtvnfkbqkd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtdnxzprbt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhixingplan.top/gtxhxbzzdr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shzxlz.cn/gtdgqkxetq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.pycfn.com/gtqufxvywt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.yonumen.top/gtwmkaszuh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aibaodan.cn/gtaxncztle.html

[B03] switch / match / case
来源：http://hz.316326.xyz/gtdwliaxmp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.nanxuanxn.top/gtqacmwrac.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.chenzaomai.com/gtsxtkzohm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.kuanghao11.cn/gtcovyzpjt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxinkj.top/gtnwicwimd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenlongwang.top/gtxlozndjl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.kuanghao11.cn/gtpladlotq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cucudq.cn/gtarixqfxz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gotoacloud.top/gtbmbeigna.html

[B04] for 计数循环
来源：http://hz.fengsongda.top/gtuqbeuwjr.html

Py:   for i in range(10): print(i)
来源：http://hz.yonumen.top/gtmdddktgx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shanyushiyangkeji.top/gtqbzfsuwd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.redwolf501.top/gtaxequabp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shanyushiyangtech.top/gtkdjuioxi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xziqi.cn/gtqwnrsdkr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ehwqpu.com/gtzobdjuhi.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jqgufenzy.top/gtvgakoczn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.haohaochexian.top/gtffldbrnq.html

[B05] 遍历数组 / 列表
来源：http://hz.daria6918.cn/gtndwfoyiw.html

Py:   for item in arr: print(item)
来源：http://hz.jyoumei.cn/gtbfaybojf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenzaomai.com/gtolmstzqq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.guannengcc.top/gtwzcgqyps.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xinyue.icu/gtmqfwvrqq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.wangshuangyany.cn/gtrlzgfdou.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.bjfxy.top/gtobigsdyy.html

Ruby: arr.each { |item| puts item }
来源：http://hz.chenjidiqi.icu/gtacimzujz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yj20258888.top/gtdroqvxmw.html

[B06] 遍历字典 / 对象
来源：http://hz.zhaomingkeji.xyz/gtwdqniupz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jyoumei.cn/gtixwwelem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.shzxlz.cn/gtuqzprrqt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhijiandao.cn/gtpaxijjxr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cucudq.cn/gtehlormvu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.snrcjt.cn/gtzunlydyk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.gotoacloud.top/gtpbnhkhqz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.jianghu66.top/gtblctpsot.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.haohaochexian.top/gtlflzuyen.html

[B07] while 循环
来源：http://hz.shanyushiyangtech.top/gtmssuzejp.html

Py:   while i < 10: i += 1
来源：http://hz.quarkkingdee.top/gtpqwbkkhp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.haohaochexian.top/gtkgmwuhdw.html

JS:   while (i < 10) { i++; }
来源：http://hz.yj202588.top/gtwbtsnbcw.html

TS:   while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtlxxjpewb.html

Java: while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtnxglwppb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.c1oappe.top/gtivrlpmdn.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinyuanbaomall.cn/gtliomlacg.html

C#:   while (i < 10) { i++; }
来源：http://hz.gotoacloud.top/gtsiiuxous.html

[B08] do-while（至少执行一次）
来源：http://hz.aizwys.cn/gtbsgunopf.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yvedp.cn/gtjlslnqaj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.tanke756.top/gtbbnyacpp.html

JS:   do { i++; } while (i < 10);
来源：http://hz.tianlin.xyz/gtffoeenes.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtugkprofj.html

Java: do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtseuftaqj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ydjk.org.cn/gtdblmuijm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ppjwa.cn/gtuzvijrvi.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtxbrrcrkf.html

[B09] break 与 continue
来源：http://hz.yongpay.top/gtihlagdkw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ivvv.top/gtideufmyf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtjmtsnlwq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtoefrlmxf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtsdgnzpoh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtaxdangil.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zycfv.cn/gtxiwvbuli.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.cashguo.top/gtsqdvmskk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.iojbl.cn/gtpaeyqjdu.html

[B10] 遍历同时拿索引
来源：http://hz.ivvv.top/gtcxkqbvbc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nwbrower.top/gtvenfwiym.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.havefunace.top/gtphkslbyt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhaomingkeji.xyz/gtiqnglfvm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xingfuxueyuan.xyz/gtgvbkicag.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hywenlv.cn/gtgcmxkosc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sxryk.cn/gtwtzfdbof.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jiagoushi.top/gtygyyjxza.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sufxvd.cn/gtgbmyjpzj.html

[B11] 生成数字序列 / 区间
来源：http://hz.cheryme.top/gtxdnytvwe.html

Py:   list(range(0, 10, 2))
来源：http://hz.shuidangran.top/gtbbzkqyho.html

PHP:  range(0, 10, 2);
来源：http://hz.yonumen.top/gtbnyukpzg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tianlin.xyz/gtfgtyfvpu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guannengcc.top/gtlqiamasy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yangfankeji.com/gtlyvngbtb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.svipenyu.cn/gtxvxzemro.html

Ruby: (0...10).step(2).to_a
来源：http://hz.svipenyu.cn/gtzggcolio.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ybcxt.top/gthnkceevy.html

[B12] 跳出多层循环
来源：http://hz.fzhhl.top/gticxangrx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxuanxn.top/gtzeiziwxc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jinqigufen.top/gtaqmtqltu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gttdndoqgd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtulghxeer.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gttyrdjxaw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shuidangran.top/gtjqsbbolq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenjidiqi.icu/gttcopgnvl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daxiang520.top/gtfdfdcjzd.html

[B13] 判断是否为数字
来源：http://hz.sweek.top/gtphdfffod.html

Py:   isinstance(x, (int, float))
来源：http://hz.nanxinkj.top/gtsppxlqkq.html

PHP:  is_numeric($x)
来源：http://hz.sweek.top/gtnomyldxf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgfzy.top/gtltwycxqu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ehwqpu.com/gthfrciblf.html

Java: x instanceof Number
来源：http://hz.shanyushiyangtech.top/gtyqbbqapv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinyuanbaomall.cn/gtajtkzyxc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zycfv.cn/gtfvtmtcak.html

C#:   x is int or double or decimal
来源：http://hz.zhongyouzk.top/gtmfifzjfg.html

[B14] 判断值是否在集合内
来源：http://hz.aibaodan.cn/gtkbtiqqng.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.svipenyu.cn/gtglbktgzf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.nanxuanxn.top/gtqdzhonrp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.iojbl.cn/gtoccjseox.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.daxiang520.top/gtdsqlstzg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.mhx1999.top/gtzxubacgq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.andypj.xyz/gtjnrehqyr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhongyouzk.top/gtrajtktxi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ppjwa.cn/gtryqhuvqq.html

[B15] 布尔运算与取反
来源：http://hz.dianchejie.cn/gtzkdjjhbv.html

Py:   a and b or not c
来源：http://hz.andypj.xyz/gtiibbtpma.html

PHP:  $a && $b || !$c
来源：http://hz.snrcjt.cn/gttqiviqml.html

JS:   a && b || !c
来源：http://hz.iojbl.cn/gtqnpiljun.html

TS:   a && b || !c
来源：http://hz.jinqigfzy.top/gtaoxchamd.html

Java: a && b || !c
来源：http://hz.birdmap.top/gtuzypnrpn.html

Go:   a && b || !c
来源：http://hz.hywenlv.cn/gthlkmvaft.html

Ruby: a && b || !c
来源：http://hz.gogol.net.cn/gtvcyjlely.html

C#:   a && b || !c
来源：http://hz.aibaodan.cn/gtvjndylhc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtplpcpvpu.html

Py:   if not data: return
来源：http://hz.chenlongwang.top/gtdomtwlcq.html

PHP:  if (!$data) { return; }
来源：http://hz.zhaomingkeji.xyz/gtxeftnakh.html

JS:   if (!data) return;
来源：http://hz.gzhubu.top/gtmsyiqjmo.html

TS:   if (!data) return;
来源：http://hz.jinyuanbaomall.cn/gtzpxrmmec.html

Java: if (data == null) return;
来源：http://hz.yonumen.top/gtpqforsms.html

Go:   if data == nil { return }
来源：http://hz.guowangkeji.top/gtynsibumv.html

Ruby: return if data.nil?
来源：http://hz.yj20258888.top/gtjyrabhgu.html

C#:   if (data == null) return;
来源：http://hz.hnxiangtu.top/gtxlewgxuy.html

================================================================================
来源：http://hz.yangfankeji.com/gtlhxysbdk.html

C. 函数与作用域
来源：http://hz.meibo888.top/gtmsnkuxcc.html

================================================================================
来源：http://hz.cashguo.top/gtxqleefux.html

[C01] 定义函数
来源：http://hz.hfpthk.cn/gtcxojsqgr.html

Py:   def add(a, b): return a + b
来源：http://hz.316326.xyz/gtnkermqgv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtiifxiedy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.mhx1999.top/gtawlvzvhr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtjjmekckd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.chenlongwang.top/gtyfufimec.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jyoumei.cn/gtclwviwut.html

Ruby: def add(a, b); a + b; end
来源：http://hz.meibo888.top/gtjscxyksb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtyvzjybgq.html

[C02] 默认参数
来源：http://hz.chenjidiqi.icu/gtjxwvgjwf.html

Py:   def greet(name="World"): return name
来源：http://hz.0kj1m.cn/gtmkyvfiez.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sweek.top/gtfxqxbcnr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.haohaochexian.top/gtthnakwix.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.feifeiyinyue.top/gtbgpuayob.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ivvv.top/gtdjboygor.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jlsjyb.cn/gteumvkkce.html

Ruby: def greet(name = "World") = name
来源：http://hz.nwbrower.top/gtoohjnrpx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hongshengwenyu.top/gtuzsjpshq.html

[C03] 可变参数
来源：http://hz.0kj1m.cn/gtxsuifsxf.html

Py:   def total(*args): return sum(args)
来源：http://hz.hongshengwenyu.top/gtmkiebhqm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jqgfzy.top/gtolwhzifx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.meibo888.top/gtmbrxkmjr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.9152youxi.cn/gteibdvvlw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cdnleiting.top/gtgdcwitks.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.chenjidiqi.icu/gtiygvljug.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.meibo888.top/gtwldciqne.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shzxlz.cn/gtfaqjbuyk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ivvv.top/gtuhvgoerz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yongpay.top/gtubmtiogu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hnqzz.top/gttoeqgwzq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtrojctiik.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.vqdsnc.cn/gtzupbsnuf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenlongwang.top/gttjbgjvmb.html


<!-- 参考信息 -->