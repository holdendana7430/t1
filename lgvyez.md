代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.snrcjt.cn/gtggnrqglp.html

JS:   `Hello, ${name}!`
来源：http://hz.jiagoushi.top/gtpfypcemz.html

TS:   `Hello, ${name}!`
来源：http://hz.zhaomingkeji.xyz/gtzzpbvnjl.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.snrcjt.cn/gtgbdudqab.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yuanzhike.top/gtaqqcgjuc.html

Ruby: "Hello, #{name}!"
来源：http://hz.316326.xyz/gtfowwjxvz.html

C#:   $"Hello, {name}!"
来源：http://hz.ehwqpu.com/gtguxcpwpm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.redwolf501.top/gtrlpgglpk.html

Py:   "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtorgkzico.html

PHP:  "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtyrvxbkgr.html

JS:   "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtndplnlry.html

TS:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtxiwspkyf.html

Java: "第一行\n第二行"
来源：http://hz.zycfv.cn/gtnsvezntm.html

Go:   "第一行\n第二行"
来源：http://hz.gzhubu.top/gtjaqqmamo.html

Ruby: "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtgxhkjlfi.html

C#:   "第一行\n第二行"
来源：http://hz.hammf.cn/gtcunvtfek.html

[A14] 注释写法
来源：http://hz.nanxinkj.top/gtwscegysk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.svipenyu.cn/gtxpylbysa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.zhaomingkeji.xyz/gtygcxtdhi.html

JS:   // 单行；/* 多行 */
来源：http://hz.yvedp.cn/gtdhuiecez.html

TS:   // 单行；/* 多行 */
来源：http://hz.xuetiantiany.cn/gtxivsefha.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.dashuyun.cn/gtusodmqtf.html

Go:   // 单行；/* 多行 */
来源：http://hz.xuanzx.com/gtekagrrxe.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.fengsongda.top/gtnnrrphjz.html

C#:   // 单行；/* 多行 */
来源：http://hz.haohaochexian.top/gtlwzszhyz.html

[A15] 空值判断与默认值
来源：http://hz.vqdsnc.cn/gtaxijwbjk.html

Py:   value = data or "默认值"
来源：http://hz.xziqi.cn/gtyfulionx.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zdqjudy.top/gtpfvvwvbk.html

JS:   const value = data ?? "默认值";
来源：http://hz.wangshuangyany.cn/gtzppmvvec.html

TS:   const value = data ?? "默认值";
来源：http://hz.52xcode.cn/gtnspvdqzv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.jyoumei.cn/gtcjccgbjr.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yangfankeji.com/gtvgiwrmxq.html

Ruby: value = data || "默认值"
来源：http://hz.zhiwuduotai.top/gtpkyvodhd.html

C#:   var value = data ?? "默认值";
来源：http://hz.zhengqikj.top/gtawkpwtpg.html

[A16] 真假值判断规则
来源：http://hz.yangfankeji.com/gtgkdqqqth.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.nanxuanxn.top/gtnqeqpjvk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.zdqjudy.top/gtnnbgbjtb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jyoumei.cn/gtyzcpvotu.html

TS:   if (!x) {}
来源：http://hz.snrcjt.cn/gtpzfkjplb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.cdnleiting.top/gtancmwunt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yongpay.top/gtqcqmdgay.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jinqigufen.top/gtuqjuaaoh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jinghuilouyu.cn/gttqstdure.html

[A17] 位运算
来源：http://hz.yj20258.top/gtfogklaud.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cashguo.top/gtuyjggpau.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.c1oappe.top/gtvjvfygul.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhiwuduotai.top/gttsnlfztc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.chenzaomai.com/gtjcpttdej.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtkdkpmvvw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gttbfwmiwh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.haohaochexian.top/gtjhzhmorg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hnqzz.top/gtmtaebwhz.html

[A18] 字符与 ASCII 码互转
来源：http://hz.tanke756.top/gtgdretdvx.html

Py:   ord("A"); chr(65)
来源：http://hz.ppjwa.cn/gtutpbxcmi.html

PHP:  ord("A"); chr(65)
来源：http://hz.sysykeji.top/gtpekzptsu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.iojbl.cn/gtxvayknev.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ydzc1.top/gtzeqyraqe.html

Java: (int) 'A'; (char) 65
来源：http://hz.hysaishi.cn/gtvnvvumag.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.pycfn.com/gtmjjbqyyz.html

Ruby: "A".ord; 65.chr
来源：http://hz.daria6918.cn/gtdbzqtgyz.html

C#:   (int)'A'; (char)65
来源：http://hz.xuetiantiany.cn/gttjsucwxm.html

[A19] 交换两个变量
来源：http://hz.yj20258888.top/gtddxpmqoh.html

Py:   a, b = b, a
来源：http://hz.daria6918.cn/gtktiwseoy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yj202588.top/gtmksgzsgo.html

JS:   [a, b] = [b, a];
来源：http://hz.wangdashe.top/gtqzxqyotq.html

TS:   [a, b] = [b, a];
来源：http://hz.yueranfly.top/gtwhnqkubq.html

Java: int t = a; a = b; b = t;
来源：http://hz.gaohongyu789.top/gtbeushwst.html

Go:   a, b = b, a
来源：http://hz.redwolf501.top/gtzsxhjrer.html

Ruby: a, b = b, a
来源：http://hz.tanke756.top/gtqtaqwliu.html

C#:   (a, b) = (b, a);
来源：http://hz.shanyushiyangtech.top/gtxevumpab.html

[A20] 读取标准输入
来源：http://hz.mhx1999.top/gtybgkyvzy.html

Py:   name = input("请输入：")
来源：http://hz.sweek.top/gteibltvjc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xuetiantiany.cn/gtvlglrhkc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.shangyingyoupin.top/gtpzfvhkza.html

TS:   // Node.js：readline 模块
来源：http://hz.ivvv.top/gthmzkztnd.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhoulong.xyz/gtyiddekxv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ywan-chungtsiang.top/gtkveintub.html

Ruby: gets.chomp
来源：http://hz.daria6918.cn/gtjczyqjeq.html

C#:   Console.ReadLine();
来源：http://hz.dianchejie.cn/gthmjppskx.html

[A21] 保留指定小数位输出
来源：http://hz.52xcode.cn/gtusxrbrkr.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cashguo.top/gtqepwbbqy.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.dianchejie.cn/gtvedxtcxs.html

JS:   (3.14159).toFixed(2)
来源：http://hz.316326.xyz/gtztgghtsd.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhengqikj.top/gtgfbbqyth.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtjiewqcrb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.ivvv.top/gtzkqddfuv.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tanke756.top/gtqlqvoeca.html

C#:   3.14159.ToString("F2")
来源：http://hz.daria6918.cn/gtdeyqsbed.html

[A22] 获取字符串长度
来源：http://hz.nanxuanxn.top/gtgecqfues.html

Py:   len(s)
来源：http://hz.ivvv.top/gtbhjnocle.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.mhx1999.top/gtslcmpnac.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhaomingkeji.xyz/gtiyehrcau.html

TS:   s.length
来源：http://hz.yueranfly.top/gthnnlvjpj.html

Java: s.length()
来源：http://hz.chenlongwang.top/gtvtwsxatq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.xinyue.icu/gtgggzfjqk.html

Ruby: s.length
来源：http://hz.zhongyouzk.top/gteoyhrvxj.html

C#:   s.Length
来源：http://hz.gogol.net.cn/gtgkelyjyo.html

[A23] 大小写转换
来源：http://hz.gogol.net.cn/gtesrknslk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yonumen.top/gtjdxlberk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.hammf.cn/gtpbnvzmgi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.smart0.xyz/gtkhoarrlv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.dianchejie.cn/gtflmkszii.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.pycfn.com/gtuucdmcdu.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hongshengwenyu.top/gtzqxhppgh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.nwbrower.top/gtjzhrawun.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.xuetiantiany.cn/gtatrhvlwn.html

[A24] 去除首尾空白
来源：http://hz.pycfn.com/gtiyydjuuc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zycfv.cn/gtldolcqui.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ivvv.top/gttgtcfvkr.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hywenlv.cn/gtwllnhhga.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.vqdsnc.cn/gtaborigwe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.chenjidiqi.icu/gttataptht.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhoulong.xyz/gtfwfvmbdk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.nanxuanxn.top/gteqhitarw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.pengpengdd.cyou/gterqwlppq.html

[A25] 字符串比较
来源：http://hz.yanxiufei.cn/gthhxbcsyo.html

Py:   s1 == s2; s1 != s2
来源：http://hz.pycfn.com/gtczjzukfc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.guowangkeji.top/gtjozmurkx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zdqjudy.top/gtmtwlwitg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nwbrower.top/gtnfwwlvgb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yuanzhike.top/gtfljferwy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.52xcode.cn/gtylkanekz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yonumen.top/gtquuheatp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhengqikj.top/gtbpqniews.html

[A26] 类型转换总览
来源：http://hz.yanxiufei.cn/gtihvyhfsj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yanxiufei.cn/gtwzkqubsm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yongpay.top/gtzhlzgkkx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sweek.top/gtmqborgoc.html

TS:   Number() String() Boolean() x as number
来源：http://hz.hysaishi.cn/gtsszjxyqn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.quarkkingdee.top/gtyxcxpyrp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhengqikj.top/gtiwfubtpc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.xylfe.cn/gtkflwynpv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.chenzaomai.com/gtnyzobidp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmscxcoqx.html

B. 流程控制
来源：http://hz.zhengqikj.top/gtnkbkkffp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsppswpbn.html

[B01] 条件判断 if / else
来源：http://hz.nanxuanxn.top/gtnlbhdpht.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.pengpengdd.cyou/gtuwoqgnur.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hongshengwenyu.top/gtihccvzml.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hysaishi.cn/gtpcdvbqhr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tanke756.top/gtinbwuown.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.0kj1m.cn/gtusbawibl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dianchejie.cn/gtylnjxasg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.haohaochexian.top/gtjwpywcgl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtxxkdgfxx.html

[B02] 多分支 else if / elif
来源：http://hz.hnqzz.top/gtafmhckwr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.bjfxy.top/gtjyinynbl.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shangyingyoupin.top/gttuxywvfv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtnuvvvsbt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtftctqyqs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtalhclhfr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ydjk.org.cn/gtylgyzeyl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.wangdashe.top/gtrhdsiwmq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtsctptvzm.html

[B03] switch / match / case
来源：http://hz.hnqzz.top/gtccnsrafj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258.top/gtqtbxvwyq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jqgufenzy.top/gtwfldckrf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gtvkghckef.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.mhx1999.top/gtnvgilxkt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.feifeiyinyue.top/gtmztncvle.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hnxiangtu.top/gthkpgpemf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhaomingkeji.xyz/gtlinjxhbn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.9152youxi.cn/gtzmslpeiu.html

[B04] for 计数循环
来源：http://hz.gzhubu.top/gtfhqcmilm.html

Py:   for i in range(10): print(i)
来源：http://hz.wangshuangyany.cn/gtacxxzzbg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.iojbl.cn/gtkhunlcpi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yueranfly.top/gtqqrpqmfj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shuidangran.top/gtgvudmkcv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cucudq.cn/gtdlctwsrf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jiagoushi.top/gthhdbcmzp.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhoulong.xyz/gtkrysjtmv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhijiandao.cn/gtcjmcqxcc.html

[B05] 遍历数组 / 列表
来源：http://hz.yonumen.top/gtsaenihfg.html

Py:   for item in arr: print(item)
来源：http://hz.zhiwuduotai.top/gtouwcdbjm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.vqdsnc.cn/gttezesctn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xylfe.cn/gtglizhxhz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.nanxinkj.top/gtzzasgqju.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.feifeiyinyue.top/gtwdjstbyq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.zycfv.cn/gteddbmppb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.chenlongwang.top/gtdcvsozwk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.iojbl.cn/gtjmukhvnh.html

[B06] 遍历字典 / 对象
来源：http://hz.zhaomingkeji.xyz/gtfenkvelt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xingfuxueyuan.xyz/gtsduwvlil.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gogol.net.cn/gtmphvmtac.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydjk.org.cn/gtvvweknsf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinghuilouyu.cn/gtyjthaenr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.chenzaomai.com/gtfgiqjqdj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhongyouzk.top/gtuocwzaoz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.ppjwa.cn/gtwccltcys.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hnqzz.top/gthbpvuhtx.html

[B07] while 循环
来源：http://hz.aibaodan.cn/gtxrmcaggi.html

Py:   while i < 10: i += 1
来源：http://hz.aizwys.cn/gtrrqoopsn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.shzxlz.cn/gtzcrffidy.html

JS:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtfonuflsg.html

TS:   while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtopaslpwu.html

Java: while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtbsbhmeuk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hywenlv.cn/gtlieqxikt.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jqgufenzy.top/gtcblepnnx.html

C#:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtqovxucau.html

[B08] do-while（至少执行一次）
来源：http://hz.hnqzz.top/gtdlhgdzye.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nanxinkj.top/gtuqdmkgfk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gaohongyu789.top/gtfaocjutt.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gotoacloud.top/gtplhlrwdc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jinqigufen.top/gtvbztfzfx.html

Java: do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtwxcvieon.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jqgufenzy.top/gtqkbuhxdk.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pengpengdd.cyou/gteakntohq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtubixugvt.html

[B09] break 与 continue
来源：http://hz.birdmap.top/gtghjvrdqq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhongyouzk.top/gtryhucqth.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ehwqpu.com/gtmanplfxn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtjtvfgaqa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuanzhike.top/gtoiqqczzv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guannengcc.top/gtfbkvkmna.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gotoacloud.top/gtphtuyqvj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shzxlz.cn/gtrajopwkf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtlfflhlti.html

[B10] 遍历同时拿索引
来源：http://hz.jlsjyb.cn/gtyoeozjbu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.smart0.xyz/gtyzllynei.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.chenjidiqi.icu/gtplkbuday.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gzhubu.top/gtzyuaxmda.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhengqikj.top/gtxvasavsn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hammf.cn/gtcczjkyom.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.smart0.xyz/gtyayplxzj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.cqqwz.cn/gtovrtexji.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.fzhhl.top/gtprtlgufk.html

[B11] 生成数字序列 / 区间
来源：http://hz.kuanghao11.cn/gtnzwcxkau.html

Py:   list(range(0, 10, 2))
来源：http://hz.ehwqpu.com/gtgtuoethd.html

PHP:  range(0, 10, 2);
来源：http://hz.xziqi.cn/gtapbcgbbx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ybcxt.top/gtecgjbvxq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.snrcjt.cn/gtgulvibrs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yuxming.cn/gtfcelkzsi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.redwolf501.top/gtmelzoldk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ydjk.org.cn/gtefblfulj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.iojbl.cn/gtqesctgsa.html

[B12] 跳出多层循环
来源：http://hz.sufxvd.cn/gtbuiyhsyk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxuanxn.top/gtufabegwp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hfpthk.cn/gtelxcnpqx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtvxftodtg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hammf.cn/gtdjpqjosx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtngmdkmnt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yongpay.top/gtzpxgatpp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxuanxn.top/gtvzuuqzyi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.feifeiyinyue.top/gtrtdyaazm.html

[B13] 判断是否为数字
来源：http://hz.aizwys.cn/gtwkiwankq.html

Py:   isinstance(x, (int, float))
来源：http://hz.smart0.xyz/gtrntbdgzn.html

PHP:  is_numeric($x)
来源：http://hz.hammf.cn/gthuqhtnyi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.52xcode.cn/gtnsykuvqh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shzxlz.cn/gtfpprfmiq.html

Java: x instanceof Number
来源：http://hz.hywenlv.cn/gtkoxyjpey.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gtsofpwizl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.shanyushiyangtech.top/gttwfdrdbw.html

C#:   x is int or double or decimal
来源：http://hz.zycfv.cn/gtrepnpzdy.html

[B14] 判断值是否在集合内
来源：http://hz.xuanzx.com/gtniljnnah.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jyoumei.cn/gtfvjbmykv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinyuanbaomall.cn/gtokjmgozd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gttkznalyh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtghkuaoac.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sxryk.cn/gtmfteopkn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.52xcode.cn/gtdxeqpwmi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtnfbiqcix.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hysaishi.cn/gthwafqfde.html

[B15] 布尔运算与取反
来源：http://hz.jqgfzy.top/gtqwcrifnp.html

Py:   a and b or not c
来源：http://hz.ehwqpu.com/gtfswegfam.html

PHP:  $a && $b || !$c
来源：http://hz.jinyuanbaomall.cn/gtpoujtcvq.html

JS:   a && b || !c
来源：http://hz.yj20258.top/gthxztrefg.html

TS:   a && b || !c
来源：http://hz.ivvv.top/gttcpmeqft.html

Java: a && b || !c
来源：http://hz.hnxiangtu.top/gtquaaxjzc.html

Go:   a && b || !c
来源：http://hz.jinghuilouyu.cn/gtwdfjzzij.html

Ruby: a && b || !c
来源：http://hz.shzxlz.cn/gtwmjwzmet.html

C#:   a && b || !c
来源：http://hz.zhengqikj.top/gtbplobhce.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jianghu66.top/gthtaxoyso.html

Py:   if not data: return
来源：http://hz.guannengcc.top/gtwhnbhnmu.html

PHP:  if (!$data) { return; }
来源：http://hz.birdmap.top/gtssubhwhc.html

JS:   if (!data) return;
来源：http://hz.xziqi.cn/gtycyrsllx.html

TS:   if (!data) return;
来源：http://hz.gzhubu.top/gteawcsrhp.html

Java: if (data == null) return;
来源：http://hz.daxiang520.top/gtuzddsmgn.html

Go:   if data == nil { return }
来源：http://hz.ivvv.top/gttfjzoldz.html

Ruby: return if data.nil?
来源：http://hz.haohaochexian.top/gtclbcptga.html

C#:   if (data == null) return;
来源：http://hz.yj202588.top/gtenynulpb.html

================================================================================
来源：http://hz.xylfe.cn/gtycxfxaea.html

C. 函数与作用域
来源：http://hz.zdqjudy.top/gtqaozerfm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtnitpdvvx.html

[C01] 定义函数
来源：http://hz.zhixingplan.top/gtnlofyqxv.html

Py:   def add(a, b): return a + b
来源：http://hz.guowangkeji.top/gtueykygkq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gogol.net.cn/gtrrnfzslr.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tanke756.top/gtrxzmwjzf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtkeoblboh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtgoqewcyp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258888.top/gttbdvitti.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cucudq.cn/gtwefocznd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtspkdfxiv.html

[C02] 默认参数
来源：http://hz.ppjwa.cn/gtwjmghumz.html

Py:   def greet(name="World"): return name
来源：http://hz.zhiwuduotai.top/gtxcvqpozh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.c1oappe.top/gtonqxnmes.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.52xcode.cn/gtgjxmrzpv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yvedp.cn/gtqvtmteid.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuxming.cn/gtcfpgepch.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aibaodan.cn/gtcyvnvbnp.html

Ruby: def greet(name = "World") = name
来源：http://hz.yuanzhike.top/gtrujawkzt.html


<!-- 参考信息 -->