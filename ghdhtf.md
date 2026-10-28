代发 wailian999

[A14] 注释写法
来源：http://hz.cdnleiting.top/gtyexmtfgq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.cheryme.top/gtjvrixmiw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yongpay.top/gthedljwyy.html

JS:   // 单行；/* 多行 */
来源：http://hz.ywan-chungtsiang.top/gtynvtqpxd.html

TS:   // 单行；/* 多行 */
来源：http://hz.jinqigfzy.top/gtdzllynhy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.wangdashe.top/gtnhycqjxz.html

Go:   // 单行；/* 多行 */
来源：http://hz.kuanghao11.cn/gtsqqiwsec.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.xuetiantiany.cn/gticzvfjzg.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhoulong.xyz/gtrlsasbph.html

[A15] 空值判断与默认值
来源：http://hz.tanke756.top/gtuqznhftm.html

Py:   value = data or "默认值"
来源：http://hz.bjfxy.top/gtovhputfg.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.tian-w.cn/gtufsigghb.html

JS:   const value = data ?? "默认值";
来源：http://hz.sxryk.cn/gtsfpxtapi.html

TS:   const value = data ?? "默认值";
来源：http://hz.cucudq.cn/gtzadwnpxx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hfpthk.cn/gtyhghsqic.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cdnleiting.top/gtmxuqgwqa.html

Ruby: value = data || "默认值"
来源：http://hz.gaohongyu789.top/gtpxpmsteg.html

C#:   var value = data ?? "默认值";
来源：http://hz.gogol.net.cn/gtykzwfkql.html

[A16] 真假值判断规则
来源：http://hz.tianlin.xyz/gtmtphwkyr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.aizwys.cn/gtnixzqhbq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.0kj1m.cn/gtbbtylecz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.gogol.net.cn/gtfegzizqc.html

TS:   if (!x) {}
来源：http://hz.jqgufenzy.top/gtbeuturwq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.aizwys.cn/gtwpzcqqhs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.c1oappe.top/gtvubcdemb.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.shuidangran.top/gthyevmtjp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yangfankeji.com/gtxuadzgdc.html

[A17] 位运算
来源：http://hz.cheryme.top/gtkmjsedzz.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.quarkkingdee.top/gtgtuygbhg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.ivvv.top/gtcpujnkcd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.redwolf501.top/gtyfdrivii.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jinqigfzy.top/gtwpdcfunj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gtrtsrcqps.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ivvv.top/gtjdplohzh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtaeffwepz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhongyouzk.top/gtokkrecrf.html

[A18] 字符与 ASCII 码互转
来源：http://hz.0kj1m.cn/gtnfuuhspy.html

Py:   ord("A"); chr(65)
来源：http://hz.bjfxy.top/gttsgexejp.html

PHP:  ord("A"); chr(65)
来源：http://hz.chenjidiqi.icu/gtyotgijdx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xylfe.cn/gtfdixxlex.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinqigfzy.top/gtiirlmikd.html

Java: (int) 'A'; (char) 65
来源：http://hz.shzxlz.cn/gtewuxkzht.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.daria6918.cn/gtaexjhyhf.html

Ruby: "A".ord; 65.chr
来源：http://hz.xylfe.cn/gtdeuzgpsg.html

C#:   (int)'A'; (char)65
来源：http://hz.hysaishi.cn/gtcszlvlim.html

[A19] 交换两个变量
来源：http://hz.guannengcc.top/gtkqlmjfzj.html

Py:   a, b = b, a
来源：http://hz.shanyushiyangkeji.top/gtvebpttlr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.aizwys.cn/gtuqdommvu.html

JS:   [a, b] = [b, a];
来源：http://hz.0kj1m.cn/gtxlclpzzm.html

TS:   [a, b] = [b, a];
来源：http://hz.nanxinkj.top/gtjqtkgsjl.html

Java: int t = a; a = b; b = t;
来源：http://hz.cdnleiting.top/gthowcxzam.html

Go:   a, b = b, a
来源：http://hz.hammf.cn/gterpwiwwn.html

Ruby: a, b = b, a
来源：http://hz.zhixingplan.top/gtwaqqygcv.html

C#:   (a, b) = (b, a);
来源：http://hz.aizwys.cn/gtbcgfuimw.html

[A20] 读取标准输入
来源：http://hz.fzhhl.top/gtlnsxmvnk.html

Py:   name = input("请输入：")
来源：http://hz.ivvv.top/gtdrtvtkfz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.shangyingyoupin.top/gtekqasbjl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.sxryk.cn/gtxjyzrffv.html

TS:   // Node.js：readline 模块
来源：http://hz.havefunace.top/gtyyhikasb.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xylfe.cn/gtjhtotvjg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jianghu66.top/gttjzjjkfi.html

Ruby: gets.chomp
来源：http://hz.xuanzx.com/gtuxmviztq.html

C#:   Console.ReadLine();
来源：http://hz.zdqjudy.top/gtouljpjjj.html

[A21] 保留指定小数位输出
来源：http://hz.cashguo.top/gtkanmocxd.html

Py:   f"{3.14159:.2f}"
来源：http://hz.gogol.net.cn/gtodfridyi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yueranfly.top/gtdyaurjjz.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yuxming.cn/gtybtgaqak.html

TS:   (3.14159).toFixed(2)
来源：http://hz.cqqwz.cn/gtyvpdideu.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ydzc1.top/gttuersbot.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.fengsongda.top/gtrsztmcho.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yuanzhike.top/gtohhcksee.html

C#:   3.14159.ToString("F2")
来源：http://hz.cheryme.top/gtzbqwxlvp.html

[A22] 获取字符串长度
来源：http://hz.guannengcc.top/gtgurqoxhs.html

Py:   len(s)
来源：http://hz.daria6918.cn/gtohiprwxn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xziqi.cn/gtfreuoaip.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xinyue.icu/gtmyvxifid.html

TS:   s.length
来源：http://hz.yonumen.top/gtftcjhtxx.html

Java: s.length()
来源：http://hz.jyoumei.cn/gtnjgatjvw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.haohaochexian.top/gtlkjshfsc.html

Ruby: s.length
来源：http://hz.zhiwuduotai.top/gtreyjiwve.html

C#:   s.Length
来源：http://hz.hnxiangtu.top/gtamikkibi.html

[A23] 大小写转换
来源：http://hz.guannengcc.top/gtrswpixom.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yanxiufei.cn/gtaleamgmh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yuanzhike.top/gticodmvav.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cashguo.top/gthqkdbldc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.bjfxy.top/gtzaukkjfw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.meibo888.top/gtgshvwlmk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinyuanbaomall.cn/gtcpzzqlkt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xuanzx.com/gtdaletbaz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.shuidangran.top/gtebcidccq.html

[A24] 去除首尾空白
来源：http://hz.0kj1m.cn/gtxtbglfcw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yueranfly.top/gttpivlyxl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yangfankeji.com/gtjxdkuzzm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ywan-chungtsiang.top/gtukewqrjk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.haohaochexian.top/gtxnuhmgkr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.shanyushiyangtech.top/gtqhykxfqv.html

Go:   strings.TrimSpace(s)
来源：http://hz.aibaodan.cn/gtayzpvxhi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.c1oappe.top/gtqfowszhg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.pengpengdd.cyou/gtuguzflsb.html

[A25] 字符串比较
来源：http://hz.cdnleiting.top/gtopoeqynf.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shangyingyoupin.top/gtogyacbeq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ydzc1.top/gtfrirwamt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xuetiantiany.cn/gtkokmfzfb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gzhubu.top/gtbpcmueau.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.smart0.xyz/gtpifufrsm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sxryk.cn/gtpvazxvfl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shangyingyoupin.top/gtjprwbven.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.quarkkingdee.top/gtxifbluck.html

[A26] 类型转换总览
来源：http://hz.nanxuanxn.top/gtzqqjdkbk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ybcxt.top/gtnrszawhy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.tianlin.xyz/gtdxwaojkn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.wangdashe.top/gtfmxaxyyl.html

TS:   Number() String() Boolean() x as number
来源：http://hz.chenjidiqi.icu/gtqiyxnqgk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.feifeiyinyue.top/gtsshzmiig.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yangfankeji.com/gtvktgzcxx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yuxming.cn/gtlbrbjbic.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jyoumei.cn/gtfmpiztlb.html

================================================================================
来源：http://hz.birdmap.top/gtxtcmyshp.html

B. 流程控制
来源：http://hz.gaohongyu789.top/gtaxgxljhb.html

================================================================================
来源：http://hz.316326.xyz/gtaagwrnxd.html

[B01] 条件判断 if / else
来源：http://hz.hnxiangtu.top/gtlbsscjdu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.tianlin.xyz/gtoktrxpwc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.nanxinkj.top/gtmbgzajoo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cqqwz.cn/gtavdoombh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinyuanbaomall.cn/gtamnnbwfv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.cashguo.top/gtwfpynvdm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.mhx1999.top/gtsedbaxwl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zhengqikj.top/gtiiaomoyw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.cucudq.cn/gteklbhgdz.html

[B02] 多分支 else if / elif
来源：http://hz.zhoulong.xyz/gtzzdcwxzr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhijiandao.cn/gtfntfeilw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.fengsongda.top/gtuuleafvt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtoskspvua.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.andypj.xyz/gtciqhmtqg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuanzhike.top/gtkxqqavqj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yueranfly.top/gtotzqlskt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhengqikj.top/gtyuxjggkd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gttmdzehqu.html

[B03] switch / match / case
来源：http://hz.0kj1m.cn/gtmylyqquw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yuanzhike.top/gtsfvcsrpp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.aizwys.cn/gttbsmhdbi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ivvv.top/gtdpuhpujl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.fengsongda.top/gtocrnbams.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.nanxuanxn.top/gtogdwmefg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.havefunace.top/gttjyrsdgb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.sufxvd.cn/gtjgbdnxjp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.daria6918.cn/gtruedymau.html

[B04] for 计数循环
来源：http://hz.kuanghao11.cn/gtsdymwylo.html

Py:   for i in range(10): print(i)
来源：http://hz.xingfuxueyuan.xyz/gtvxysvwxy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.ywan-chungtsiang.top/gtvshtsdfg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zycfv.cn/gtqaeiqvgx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nanxinkj.top/gtmlewkmic.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.wangshuangyany.cn/gtjyspfdbp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cucudq.cn/gtdwsxghyw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.pycfn.com/gtqarvvrej.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.c1oappe.top/gtjqfjudxa.html

[B05] 遍历数组 / 列表
来源：http://hz.redwolf501.top/gtuigxxqwz.html

Py:   for item in arr: print(item)
来源：http://hz.redwolf501.top/gtnlxkrdcc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sweek.top/gtyjynldrw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.316326.xyz/gtqszbgurr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shuidangran.top/gtrcabixiq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sysykeji.top/gtyuipvfcw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnqzz.top/gtffwiiqjt.html

Ruby: arr.each { |item| puts item }
来源：http://hz.xuanzx.com/gtomedxlaj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhaomingkeji.xyz/gtmyofvsna.html

[B06] 遍历字典 / 对象
来源：http://hz.tanke756.top/gthrvtlxyu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.316326.xyz/gtvsfdanmy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.smart0.xyz/gtdneiuwwz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.redwolf501.top/gtlfznzhez.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zdqjudy.top/gthiteuctn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hywenlv.cn/gtkacuasjd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yonumen.top/gtqdipysfw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xingfuxueyuan.xyz/gtvmwxaino.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.dianchejie.cn/gtuxjdqlzj.html

[B07] while 循环
来源：http://hz.ydjk.org.cn/gtwpfzwulo.html

Py:   while i < 10: i += 1
来源：http://hz.jinghuilouyu.cn/gtlrxlfczt.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.gogol.net.cn/gtnxfnlbve.html

JS:   while (i < 10) { i++; }
来源：http://hz.havefunace.top/gtwpgxvgek.html

TS:   while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtfinrbrot.html

Java: while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtleonrmsd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.pengpengdd.cyou/gtjeznosyh.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shangyingyoupin.top/gtathtbpjk.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtizzilzvu.html

[B08] do-while（至少执行一次）
来源：http://hz.cheryme.top/gtyjyreldp.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxinkj.top/gtlxnworco.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.jyoumei.cn/gtoiwymlbi.html

JS:   do { i++; } while (i < 10);
来源：http://hz.smart0.xyz/gtwdhlnamd.html

TS:   do { i++; } while (i < 10);
来源：http://hz.wangshuangyany.cn/gtwitsqvec.html

Java: do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtebjalmij.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hnqzz.top/gtudajuvwg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hnqzz.top/gtpbbnmeos.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gttjmcptvm.html

[B09] break 与 continue
来源：http://hz.yanxiufei.cn/gtjbbeqana.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jiagoushi.top/gtasycwjct.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ivvv.top/gtkordaspx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtzsvdtmbr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtxytdemyi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtztimczss.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhijiandao.cn/gttrrlirxy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhiwuduotai.top/gtdpenbfev.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtlruztvrv.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtxydncvil.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.0kj1m.cn/gtbvhuqbmf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.guowangkeji.top/gtbjaismtp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.fengsongda.top/gterlmcurn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.redwolf501.top/gtspevvavm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.dianchejie.cn/gtawibowrp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sufxvd.cn/gtmetyeigu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.pycfn.com/gtugmnehez.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.meibo888.top/gtflhifbxg.html

[B11] 生成数字序列 / 区间
来源：http://hz.sufxvd.cn/gtlsujjobs.html

Py:   list(range(0, 10, 2))
来源：http://hz.gaohongyu789.top/gtzgnsvhar.html

PHP:  range(0, 10, 2);
来源：http://hz.xylfe.cn/gtvpvksbou.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.andypj.xyz/gtsifwrurz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jianghu66.top/gtujdhqacy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinghuilouyu.cn/gtngopovih.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gogol.net.cn/gtikwavzti.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xylfe.cn/gtflmlcltr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.316326.xyz/gteavlynsa.html

[B12] 跳出多层循环
来源：http://hz.sufxvd.cn/gtiziwywqt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.wangshuangyany.cn/gtyksprzjz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.shanyushiyangtech.top/gtukiuzfpo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.c1oappe.top/gtqfpikdwk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gturcwzsea.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.aibaodan.cn/gtptmfxuqy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.havefunace.top/gtzzqdptge.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.feifeiyinyue.top/gtvjejdgbu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yueranfly.top/gtpwpobdql.html

[B13] 判断是否为数字
来源：http://hz.cqqwz.cn/gtodlijcih.html

Py:   isinstance(x, (int, float))
来源：http://hz.yvedp.cn/gtwsggutuq.html

PHP:  is_numeric($x)
来源：http://hz.zhijiandao.cn/gtmkkqogni.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hnxiangtu.top/gtcipscjfs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhengqikj.top/gthpucruww.html

Java: x instanceof Number
来源：http://hz.svipenyu.cn/gtnhwnozku.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tianlin.xyz/gteqjjtuvh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenzaomai.com/gtwictpkab.html

C#:   x is int or double or decimal
来源：http://hz.jianghu66.top/gtwjmgjorj.html

[B14] 判断值是否在集合内
来源：http://hz.nwbrower.top/gtyiiidmdu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.9152youxi.cn/gtbelgpcyr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daria6918.cn/gtpaowaxku.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xylfe.cn/gtljdpzzdo.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ywan-chungtsiang.top/gtmohtfqvh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hywenlv.cn/gtstxsbelh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yvedp.cn/gtpuhzwwyi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuxming.cn/gtfzlvoblz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jiagoushi.top/gtmtjumfwg.html

[B15] 布尔运算与取反
来源：http://hz.xingfuxueyuan.xyz/gtseotzduf.html

Py:   a and b or not c
来源：http://hz.fengsongda.top/gtyitbvfrr.html

PHP:  $a && $b || !$c
来源：http://hz.guowangkeji.top/gtwqogfpxy.html

JS:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtcyebrzte.html

TS:   a && b || !c
来源：http://hz.xuanzx.com/gtoiftmfyy.html

Java: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtyctmnaqi.html

Go:   a && b || !c
来源：http://hz.ydjk.org.cn/gtsentobpn.html

Ruby: a && b || !c
来源：http://hz.zhengqikj.top/gtzuezgdqf.html

C#:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtvicaxbyk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.pengpengdd.cyou/gttpxteimp.html

Py:   if not data: return
来源：http://hz.xuetiantiany.cn/gtjeirlwtu.html

PHP:  if (!$data) { return; }
来源：http://hz.hnxiangtu.top/gtkiofjfhs.html

JS:   if (!data) return;
来源：http://hz.chenlongwang.top/gtyesctief.html

TS:   if (!data) return;
来源：http://hz.cashguo.top/gtvvzdetis.html

Java: if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtjukbwwus.html

Go:   if data == nil { return }
来源：http://hz.nanxinkj.top/gtbojwdual.html

Ruby: return if data.nil?
来源：http://hz.cqqwz.cn/gtvayyzqfc.html

C#:   if (data == null) return;
来源：http://hz.guannengcc.top/gtwancbgte.html

================================================================================
来源：http://hz.gzhubu.top/gtruiibwyz.html

C. 函数与作用域
来源：http://hz.zhaomingkeji.xyz/gtychssmlx.html

================================================================================
来源：http://hz.yj202588.top/gtktwakxnf.html

[C01] 定义函数
来源：http://hz.aibaodan.cn/gtgkrcefdp.html

Py:   def add(a, b): return a + b
来源：http://hz.jqgfzy.top/gtbkpzifvg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.feifeiyinyue.top/gtjvxgcigc.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtxhrceear.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinqigfzy.top/gtlohnsrvo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ppjwa.cn/gtzvjfdrxy.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigfzy.top/gtnrwfkhsm.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yongpay.top/gtsinyaxmn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtzfikbxac.html

[C02] 默认参数
来源：http://hz.9152youxi.cn/gtikgodbng.html

Py:   def greet(name="World"): return name
来源：http://hz.52xcode.cn/gtypliimlm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.daxiang520.top/gtspsjxhba.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.tian-w.cn/gthgkyguvd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gtjaxhjzdk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.andypj.xyz/gtolqyibhe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yangfankeji.com/gtowlahzoa.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigfzy.top/gtjaodeurx.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jinyuanbaomall.cn/gtfnpewpjy.html

[C03] 可变参数
来源：http://hz.havefunace.top/gtbzrszkft.html

Py:   def total(*args): return sum(args)
来源：http://hz.guannengcc.top/gtbzpyudjv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yj20258888.top/gtrdgsbnhp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gtzqhrfnvp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hfpthk.cn/gtftlszcaq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sweek.top/gtfyawmwdd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtrviukrqf.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hongshengwenyu.top/gtcphjbbjd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.316326.xyz/gtogtrnhlp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhengqikj.top/gtgnroxvue.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.pycfn.com/gtlvowhpni.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hnqzz.top/gticslbqve.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gogol.net.cn/gtzgpqbpfa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.c1oappe.top/gtlpocvvny.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.daria6918.cn/gtlmlhxrhf.html


<!-- 参考信息 -->