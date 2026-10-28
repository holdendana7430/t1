代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.shzxlz.cn/gtwpzixshy.html

Ruby: "Hello, #{name}!"
来源：http://hz.yangfankeji.com/gtcdhednfm.html

C#:   $"Hello, {name}!"
来源：http://hz.zhoulong.xyz/gtccfxpcac.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.smart0.xyz/gtukxumask.html

Py:   "第一行\n第二行"
来源：http://hz.jqgfzy.top/gtwcynjavl.html

PHP:  "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtjaoahvff.html

JS:   "第一行\n第二行"
来源：http://hz.zdqjudy.top/gtvjvuhcuz.html

TS:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtbsvegavh.html

Java: "第一行\n第二行"
来源：http://hz.ydjk.org.cn/gtujwmiwvj.html

Go:   "第一行\n第二行"
来源：http://hz.cucudq.cn/gtrhszjqnw.html

Ruby: "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtvxxyimmx.html

C#:   "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtehqrxvqk.html

[A14] 注释写法
来源：http://hz.yuanzhike.top/gtbmuivwjf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.guowangkeji.top/gtmnlbqkhx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.guowangkeji.top/gtboidvcqm.html

JS:   // 单行；/* 多行 */
来源：http://hz.zdqjudy.top/gtrvvaafgv.html

TS:   // 单行；/* 多行 */
来源：http://hz.cdnleiting.top/gttlxcymkw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.quarkkingdee.top/gthamvifum.html

Go:   // 单行；/* 多行 */
来源：http://hz.daria6918.cn/gtolakwmie.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.xziqi.cn/gtqwioupif.html

C#:   // 单行；/* 多行 */
来源：http://hz.yangfankeji.com/gtrgagchfh.html

[A15] 空值判断与默认值
来源：http://hz.chenjidiqi.icu/gtcqzbnolc.html

Py:   value = data or "默认值"
来源：http://hz.nanxinkj.top/gtpaymtgvw.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.ppjwa.cn/gtxtnbwhcr.html

JS:   const value = data ?? "默认值";
来源：http://hz.yuanzhike.top/gtqhwvpbfv.html

TS:   const value = data ?? "默认值";
来源：http://hz.cucudq.cn/gtuojfvchb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.hfpthk.cn/gtwxugmckl.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.iojbl.cn/gtwyhgcamn.html

Ruby: value = data || "默认值"
来源：http://hz.sufxvd.cn/gtdmubseut.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinghuilouyu.cn/gtucajfeww.html

[A16] 真假值判断规则
来源：http://hz.cdnleiting.top/gtqcrgetnd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.52xcode.cn/gtuisisyzl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.chenlongwang.top/gtqrbxqnan.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xuetiantiany.cn/gtjjkikbhx.html

TS:   if (!x) {}
来源：http://hz.gotoacloud.top/gtmgikackt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.sufxvd.cn/gtcqvgtdwy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yangfankeji.com/gtfwafemrg.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zhijiandao.cn/gthwnpvpvv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hfpthk.cn/gtdujqcrhu.html

[A17] 位运算
来源：http://hz.chenjidiqi.icu/gtwgipjido.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ivvv.top/gttcictibg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.bjfxy.top/gtpxsgmvpx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtyhbfvdup.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.aizwys.cn/gtslctzttg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigfzy.top/gtwuymftji.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtmfenelgs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shzxlz.cn/gtckfnmqto.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtzfhjzvzq.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zhixingplan.top/gtjogruubl.html

Py:   ord("A"); chr(65)
来源：http://hz.smart0.xyz/gtzpvwgafm.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhongyouzk.top/gttdzxtkjv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.kuanghao11.cn/gthtuqygeh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhoulong.xyz/gtosyzgolb.html

Java: (int) 'A'; (char) 65
来源：http://hz.nanxinkj.top/gtfnhvsiuc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.sxryk.cn/gtdzifwuyz.html

Ruby: "A".ord; 65.chr
来源：http://hz.daxiang520.top/gtbpjvqrrp.html

C#:   (int)'A'; (char)65
来源：http://hz.aizwys.cn/gtezuleyzd.html

[A19] 交换两个变量
来源：http://hz.yueranfly.top/gtdisjonkk.html

Py:   a, b = b, a
来源：http://hz.sufxvd.cn/gtctorsdot.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hongshengwenyu.top/gtkhbekqek.html

JS:   [a, b] = [b, a];
来源：http://hz.yangfankeji.com/gtkweobzxy.html

TS:   [a, b] = [b, a];
来源：http://hz.hongshengwenyu.top/gtwtroifea.html

Java: int t = a; a = b; b = t;
来源：http://hz.wangdashe.top/gtdjzoogah.html

Go:   a, b = b, a
来源：http://hz.ehwqpu.com/gtnljgotmn.html

Ruby: a, b = b, a
来源：http://hz.hysaishi.cn/gttdrzrfgc.html

C#:   (a, b) = (b, a);
来源：http://hz.cdnleiting.top/gtbetavbre.html

[A20] 读取标准输入
来源：http://hz.jinqigfzy.top/gtnihgrljf.html

Py:   name = input("请输入：")
来源：http://hz.xinyue.icu/gtsfjzcehq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.meibo888.top/gtgwidogjy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xziqi.cn/gtlbmhpmuc.html

TS:   // Node.js：readline 模块
来源：http://hz.cashguo.top/gtbflayjim.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.birdmap.top/gtszgfurdx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yanxiufei.cn/gtxutnnoyu.html

Ruby: gets.chomp
来源：http://hz.zhongyouzk.top/gtcbnmogtk.html

C#:   Console.ReadLine();
来源：http://hz.c1oappe.top/gtbusbqjwy.html

[A21] 保留指定小数位输出
来源：http://hz.xuanzx.com/gtmbcigsgt.html

Py:   f"{3.14159:.2f}"
来源：http://hz.nanxuanxn.top/gtiyiqzosj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.pycfn.com/gtfvfznvky.html

JS:   (3.14159).toFixed(2)
来源：http://hz.chenzaomai.com/gtzvmzpwob.html

TS:   (3.14159).toFixed(2)
来源：http://hz.fengsongda.top/gtqipajspk.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yj20258888.top/gtykpbpvig.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shanyushiyangkeji.top/gtrrcrthnz.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.c1oappe.top/gtjizeexjx.html

C#:   3.14159.ToString("F2")
来源：http://hz.9152youxi.cn/gtpeeaxnvi.html

[A22] 获取字符串长度
来源：http://hz.nanxuanxn.top/gthhjyodhm.html

Py:   len(s)
来源：http://hz.gaohongyu789.top/gtksvhrckn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.smart0.xyz/gtxekucaov.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.sufxvd.cn/gthygvreux.html

TS:   s.length
来源：http://hz.cdnleiting.top/gtilrwcqwx.html

Java: s.length()
来源：http://hz.daxiang520.top/gtedjfexow.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.nanxinkj.top/gtlgrlsuwc.html

Ruby: s.length
来源：http://hz.ybcxt.top/gtnjovfaby.html

C#:   s.Length
来源：http://hz.chenzaomai.com/gtvbtbfqlb.html

[A23] 大小写转换
来源：http://hz.cucudq.cn/gtjlkhxqyk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jqgfzy.top/gtzsxjksyx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.mhx1999.top/gtufqgygfk.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhoulong.xyz/gtolgjsmod.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.andypj.xyz/gtaoozuxeu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.guannengcc.top/gtgryoiifd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hysaishi.cn/gtzxswiysv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.bjfxy.top/gtfqvnbous.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yuanzhike.top/gtuimtdygf.html

[A24] 去除首尾空白
来源：http://hz.snrcjt.cn/gteppvnrnd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.birdmap.top/gtjrsungrp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.316326.xyz/gtgafmnxem.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gogol.net.cn/gtcllcwapl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tianlin.xyz/gtdojxfwfq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yj20258.top/gtdiidgses.html

Go:   strings.TrimSpace(s)
来源：http://hz.hfpthk.cn/gthyuvyqxp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ppjwa.cn/gtuxtuvimx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.52xcode.cn/gteixuuoco.html

[A25] 字符串比较
来源：http://hz.andypj.xyz/gtlpjpfekv.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ywan-chungtsiang.top/gtndgflhpf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cqqwz.cn/gtvkpqbcnx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenzaomai.com/gtlmmbliaz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.chenzaomai.com/gtcdkgmjaf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.andypj.xyz/gturptlpri.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zhijiandao.cn/gtqbmsnnxn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.0kj1m.cn/gtpdapahfb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.shzxlz.cn/gtkxvwjbqu.html

[A26] 类型转换总览
来源：http://hz.zhixingplan.top/gtxojlgjuf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.nanxinkj.top/gtuvyuggqn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhengqikj.top/gtmrbztkmm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.quarkkingdee.top/gttqnwucut.html

TS:   Number() String() Boolean() x as number
来源：http://hz.havefunace.top/gtyborshlp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.52xcode.cn/gtxigufetd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jyoumei.cn/gtdirsfbho.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.fzhhl.top/gtfuozlxer.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.sxryk.cn/gtlwyqqxmd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkwuamypn.html

B. 流程控制
来源：http://hz.ppjwa.cn/gttiljssxf.html

================================================================================
来源：http://hz.andypj.xyz/gtkaxhquun.html

[B01] 条件判断 if / else
来源：http://hz.zhengqikj.top/gttpjoruzj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cdnleiting.top/gtnmdubame.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cheryme.top/gtlzdkfqun.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yangfankeji.com/gtiplveldz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.andypj.xyz/gtzmfltiqj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhaomingkeji.xyz/gtljdvntwk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.dashuyun.cn/gtnpyaqawl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.0kj1m.cn/gtugofjrsh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.pengpengdd.cyou/gtxbrgpjih.html

[B02] 多分支 else if / elif
来源：http://hz.fzhhl.top/gtalqdtvuy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yanxiufei.cn/gtpnqafmpj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj202588.top/gtzubzzkbz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtbdqievvs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtxfclfqfx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hysaishi.cn/gtfhdqlorq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.c1oappe.top/gtkcomynor.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.wangshuangyany.cn/gtxjjeludw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.316326.xyz/gtdwvmgmiy.html

[B03] switch / match / case
来源：http://hz.yonumen.top/gtzmuolzak.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.zhongyouzk.top/gtyxlsykxd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.wangshuangyany.cn/gtocenfsbv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ehwqpu.com/gtouvrckqt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtwthbafdz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.pengpengdd.cyou/gtxhggkslx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.chenlongwang.top/gtmuoisope.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.wangdashe.top/gtsoxzikdk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.sweek.top/gtxwerkeon.html

[B04] for 计数循环
来源：http://hz.zdqjudy.top/gtoywsiflt.html

Py:   for i in range(10): print(i)
来源：http://hz.pycfn.com/gtpyzxvpjo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.hnqzz.top/gtqwybynsr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ywan-chungtsiang.top/gtlqcmkose.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.fengsongda.top/gttiqagtqx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.316326.xyz/gtwijecchd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tianlin.xyz/gtospayfro.html

Ruby: 10.times { |i| puts i }
来源：http://hz.sxryk.cn/gtjdpvampu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jianghu66.top/gtfzjfkncb.html

[B05] 遍历数组 / 列表
来源：http://hz.nanxinkj.top/gtlrcwpqve.html

Py:   for item in arr: print(item)
来源：http://hz.jinyuanbaomall.cn/gtbsrfrvma.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.nwbrower.top/gtipnlqgan.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinyuanbaomall.cn/gtknmoqxge.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shanyushiyangtech.top/gtebobxfbb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shangyingyoupin.top/gtincgtdfv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.smart0.xyz/gtscncecni.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hnqzz.top/gtjdfvngbd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.guannengcc.top/gtggnunqry.html

[B06] 遍历字典 / 对象
来源：http://hz.yueranfly.top/gtrtxpqtud.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xziqi.cn/gtyrkbcfak.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zycfv.cn/gtucrkxbul.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuanzx.com/gtltsbquwd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gotoacloud.top/gtwjfhnyey.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.svipenyu.cn/gtusceofhf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yonumen.top/gtclxecwhq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.snrcjt.cn/gtwzhsropk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.tanke756.top/gtrvvefkkx.html

[B07] while 循环
来源：http://hz.zdqjudy.top/gtpsyzipwn.html

Py:   while i < 10: i += 1
来源：http://hz.hammf.cn/gtfdvcwoac.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.mhx1999.top/gtgbiqmrcv.html

JS:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gttkfnjgxc.html

TS:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtwlpxqucp.html

Java: while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtwbnoarwt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zdqjudy.top/gtvoiyjyte.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhoulong.xyz/gtftrmgoso.html

C#:   while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtrolyfabv.html

[B08] do-while（至少执行一次）
来源：http://hz.ivvv.top/gtxyunmrrf.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cucudq.cn/gtrtpobfho.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.xuetiantiany.cn/gtkwunhspc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gtwtjbqoxf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtxiblwriu.html

Java: do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtrmiizbwv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhongyouzk.top/gtxzjjdkpw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.redwolf501.top/gtpxzidnfy.html

C#:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtmuhvcpzk.html

[B09] break 与 continue
来源：http://hz.xuetiantiany.cn/gtjhohfhrk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xziqi.cn/gtqzxvaqap.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.ybcxt.top/gtxnjxxrmu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jlsjyb.cn/gtuanolifk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gtrsvyfyxa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.aibaodan.cn/gtaiajsfxv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cheryme.top/gtkepznpnj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenlongwang.top/gtfebltyib.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtjfbhqrau.html

[B10] 遍历同时拿索引
来源：http://hz.zhengqikj.top/gtgzsipeeo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.cheryme.top/gtadrebjvk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtvsmqdlcv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtxihpfzae.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jiagoushi.top/gtrfwnbntj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yonumen.top/gthsezyhmw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.0kj1m.cn/gtlbpqtpto.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhiwuduotai.top/gtyxmviloa.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.smart0.xyz/gtookfyatp.html

[B11] 生成数字序列 / 区间
来源：http://hz.yanxiufei.cn/gtopbblbup.html

Py:   list(range(0, 10, 2))
来源：http://hz.iojbl.cn/gtoqmeopht.html

PHP:  range(0, 10, 2);
来源：http://hz.pengpengdd.cyou/gthzjtvjht.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.smart0.xyz/gtehujebcx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ppjwa.cn/gtvqsykjjx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.tian-w.cn/gthrzybcur.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ydjk.org.cn/gtxrealqoa.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xuetiantiany.cn/gtafyluxjj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sufxvd.cn/gtsygmatkg.html

[B12] 跳出多层循环
来源：http://hz.daxiang520.top/gthouywitq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jyoumei.cn/gtorndwliw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xingfuxueyuan.xyz/gtmbzursqo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtuhwwfkte.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtazwjdfgb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtrtcwbuwk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yongpay.top/gtompurkvt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fengsongda.top/gtrwdghacc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.yuanzhike.top/gtfuhhthth.html

[B13] 判断是否为数字
来源：http://hz.guannengcc.top/gtyfqhafll.html

Py:   isinstance(x, (int, float))
来源：http://hz.yueranfly.top/gtuamsxryn.html

PHP:  is_numeric($x)
来源：http://hz.ivvv.top/gtnhphpgri.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhiwuduotai.top/gtnbgflrav.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gaohongyu789.top/gtcanzjiaq.html

Java: x instanceof Number
来源：http://hz.shzxlz.cn/gtqkqfeenh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sufxvd.cn/gtmjlfpolz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangshuangyany.cn/gtkcovcawp.html

C#:   x is int or double or decimal
来源：http://hz.cucudq.cn/gttjzpswrm.html

[B14] 判断值是否在集合内
来源：http://hz.chenzaomai.com/gtavtcdero.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.wangdashe.top/gtnxgpcnrj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.guannengcc.top/gtawbuumwx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtrwmgtjze.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jiagoushi.top/gtrrpzqzwd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhiwuduotai.top/gtonvcskot.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dianchejie.cn/gttavgehey.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yuanzhike.top/gtjaxqkhnv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj202588.top/gtmekvkikj.html

[B15] 布尔运算与取反
来源：http://hz.xinyue.icu/gtggiipsyj.html

Py:   a and b or not c
来源：http://hz.jinyuanbaomall.cn/gtdykuvqnw.html

PHP:  $a && $b || !$c
来源：http://hz.hnxiangtu.top/gtohmowuyv.html

JS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtrcfiwowi.html

TS:   a && b || !c
来源：http://hz.sweek.top/gtsnxqiebt.html

Java: a && b || !c
来源：http://hz.daxiang520.top/gtilkdghfk.html

Go:   a && b || !c
来源：http://hz.zhongyouzk.top/gtabcgitqa.html

Ruby: a && b || !c
来源：http://hz.jlsjyb.cn/gthbdlzfkx.html

C#:   a && b || !c
来源：http://hz.gzhubu.top/gtqmyzsnvy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.snrcjt.cn/gtwcnbsegg.html

Py:   if not data: return
来源：http://hz.ybcxt.top/gtofudrjbs.html

PHP:  if (!$data) { return; }
来源：http://hz.aizwys.cn/gtmsumzlwy.html

JS:   if (!data) return;
来源：http://hz.redwolf501.top/gtdltfpphr.html

TS:   if (!data) return;
来源：http://hz.cqqwz.cn/gtrsjhysbl.html

Java: if (data == null) return;
来源：http://hz.tianlin.xyz/gttpjuuinh.html

Go:   if data == nil { return }
来源：http://hz.nanxuanxn.top/gtlsrclgoa.html

Ruby: return if data.nil?
来源：http://hz.jqgfzy.top/gtfhqnvtbn.html

C#:   if (data == null) return;
来源：http://hz.havefunace.top/gtiubkvete.html

================================================================================
来源：http://hz.yuanzhike.top/gtzqqcbnib.html

C. 函数与作用域
来源：http://hz.shanyushiyangkeji.top/gtcpmcbqbn.html

================================================================================
来源：http://hz.cashguo.top/gtzqiarlwv.html

[C01] 定义函数
来源：http://hz.guannengcc.top/gtejmiwlsh.html

Py:   def add(a, b): return a + b
来源：http://hz.zhoulong.xyz/gtrzfewhyg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nanxinkj.top/gtlzhwunhk.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yonumen.top/gtvkatmklg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yvedp.cn/gtijwoagco.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ydzc1.top/gtzedmpjvi.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shanyushiyangkeji.top/gtdxmoogsr.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gogol.net.cn/gtycrslwjn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtbmsxhesg.html

[C02] 默认参数
来源：http://hz.nanxuanxn.top/gtfsmctaoh.html

Py:   def greet(name="World"): return name
来源：http://hz.jqgfzy.top/gtesfhmrzs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zdqjudy.top/gtbaoiknwz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.andypj.xyz/gtgkhqpqjn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.dashuyun.cn/gtlsdelzjw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yangfankeji.com/gtxuzonlmy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hammf.cn/gtndjcplnk.html

Ruby: def greet(name = "World") = name
来源：http://hz.zycfv.cn/gtiafvfjfg.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yuxming.cn/gtjqzktygx.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gteqtpwmhn.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhiwuduotai.top/gtgspszvav.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dianchejie.cn/gtrjzxrssg.html


<!-- 参考信息 -->