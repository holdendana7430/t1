代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.tianlin.xyz/gtzxcmpsng.html

Ruby: "Hello, #{name}!"
来源：http://hz.daria6918.cn/gtnrnrofga.html

C#:   $"Hello, {name}!"
来源：http://hz.yvedp.cn/gtfmguzamk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.zhijiandao.cn/gthtjhekao.html

Py:   "第一行\n第二行"
来源：http://hz.yvedp.cn/gtuktoxnit.html

PHP:  "第一行\n第二行"
来源：http://hz.yuxming.cn/gtcufjeebm.html

JS:   "第一行\n第二行"
来源：http://hz.nwbrower.top/gtyaaenfqo.html

TS:   "第一行\n第二行"
来源：http://hz.yueranfly.top/gtjhydugek.html

Java: "第一行\n第二行"
来源：http://hz.yuxming.cn/gtcrwkdctm.html

Go:   "第一行\n第二行"
来源：http://hz.zhengqikj.top/gtldczsvwy.html

Ruby: "第一行\n第二行"
来源：http://hz.yj20258.top/gtjtdbdpyp.html

C#:   "第一行\n第二行"
来源：http://hz.nanxinkj.top/gtlugqvjns.html

[A14] 注释写法
来源：http://hz.zhixingplan.top/gtbhyqgvup.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hysaishi.cn/gtfyftyukh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.pengpengdd.cyou/gtiutbqciv.html

JS:   // 单行；/* 多行 */
来源：http://hz.jianghu66.top/gtsgbhxvms.html

TS:   // 单行；/* 多行 */
来源：http://hz.yvedp.cn/gtfssxjkdg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.9152youxi.cn/gtdszfpaqp.html

Go:   // 单行；/* 多行 */
来源：http://hz.havefunace.top/gtemogckqf.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.zhengqikj.top/gtexlmzkur.html

C#:   // 单行；/* 多行 */
来源：http://hz.hnqzz.top/gtymhcjazs.html

[A15] 空值判断与默认值
来源：http://hz.zycfv.cn/gtjbctsxbk.html

Py:   value = data or "默认值"
来源：http://hz.9152youxi.cn/gtroecqjhe.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.shangyingyoupin.top/gtbeaoyfcp.html

JS:   const value = data ?? "默认值";
来源：http://hz.bjfxy.top/gtdsdznppc.html

TS:   const value = data ?? "默认值";
来源：http://hz.sweek.top/gtjmwqygew.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yj20258888.top/gtpibtlmby.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jlsjyb.cn/gtfoznpfwt.html

Ruby: value = data || "默认值"
来源：http://hz.dashuyun.cn/gtsvmmiqdh.html

C#:   var value = data ?? "默认值";
来源：http://hz.jinghuilouyu.cn/gtgwbnmjwm.html

[A16] 真假值判断规则
来源：http://hz.yuanzhike.top/gtqhddwmea.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.hammf.cn/gtffwnjumn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.sweek.top/gtyznfpiuw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.birdmap.top/gtotjpotsi.html

TS:   if (!x) {}
来源：http://hz.jinyuanbaomall.cn/gthnflvoxf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.shangyingyoupin.top/gtojpfbheo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jqgufenzy.top/gthrrpralh.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jiagoushi.top/gtbocxdmcl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.shanyushiyangtech.top/gtgbzyfyey.html

[A17] 位运算
来源：http://hz.gogol.net.cn/gtjexxkevt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtaxulatxw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.daria6918.cn/gtvaxsosan.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtjplaodch.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtwhjckmxw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtprnlluga.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jinqigufen.top/gtyrqjlgzq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj202588.top/gtravycqsl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nanxuanxn.top/gtmovopknx.html

[A18] 字符与 ASCII 码互转
来源：http://hz.cashguo.top/gtocsgamaj.html

Py:   ord("A"); chr(65)
来源：http://hz.ywan-chungtsiang.top/gtwerhvyjz.html

PHP:  ord("A"); chr(65)
来源：http://hz.xuanzx.com/gtersokhji.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cdnleiting.top/gtpdlxbnpw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hywenlv.cn/gtohobgjke.html

Java: (int) 'A'; (char) 65
来源：http://hz.ehwqpu.com/gtjjujfpmb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jlsjyb.cn/gtwwlxvjjw.html

Ruby: "A".ord; 65.chr
来源：http://hz.xziqi.cn/gttaokdgic.html

C#:   (int)'A'; (char)65
来源：http://hz.wangshuangyany.cn/gtbpjwvhpa.html

[A19] 交换两个变量
来源：http://hz.sxryk.cn/gtumagcncj.html

Py:   a, b = b, a
来源：http://hz.xuetiantiany.cn/gtlzeokego.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.nwbrower.top/gtlwrznbkb.html

JS:   [a, b] = [b, a];
来源：http://hz.xylfe.cn/gthhkfmino.html

TS:   [a, b] = [b, a];
来源：http://hz.gaohongyu789.top/gtissxmfkz.html

Java: int t = a; a = b; b = t;
来源：http://hz.hfpthk.cn/gtvxxrzode.html

Go:   a, b = b, a
来源：http://hz.guowangkeji.top/gtadgdpynk.html

Ruby: a, b = b, a
来源：http://hz.0kj1m.cn/gtfhnebedi.html

C#:   (a, b) = (b, a);
来源：http://hz.gaohongyu789.top/gtctlbienw.html

[A20] 读取标准输入
来源：http://hz.bjfxy.top/gtnaqkawzl.html

Py:   name = input("请输入：")
来源：http://hz.jinqigufen.top/gtqncihnzu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xziqi.cn/gtibwgfjiz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.cdnleiting.top/gtunucyviq.html

TS:   // Node.js：readline 模块
来源：http://hz.pycfn.com/gtefhwsyhh.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhaomingkeji.xyz/gtozndkatn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jlsjyb.cn/gtvqmuzpfj.html

Ruby: gets.chomp
来源：http://hz.andypj.xyz/gtzyeqprrf.html

C#:   Console.ReadLine();
来源：http://hz.aibaodan.cn/gttzafzfly.html

[A21] 保留指定小数位输出
来源：http://hz.ywan-chungtsiang.top/gteuunsucf.html

Py:   f"{3.14159:.2f}"
来源：http://hz.nanxuanxn.top/gtkxgpbxda.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zhixingplan.top/gtzeewdbve.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yuanzhike.top/gtxgpsbhlg.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ppjwa.cn/gtmjhwsvgb.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ywan-chungtsiang.top/gtrmoelose.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.meibo888.top/gtcntcfmjn.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtyjgaufqk.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhixingplan.top/gtxwiwfdnt.html

[A22] 获取字符串长度
来源：http://hz.xinyue.icu/gtdtoifawt.html

Py:   len(s)
来源：http://hz.havefunace.top/gtldnwjfal.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.iojbl.cn/gthwdrrrnd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.dashuyun.cn/gtljvvshlo.html

TS:   s.length
来源：http://hz.hammf.cn/gtznbprfln.html

Java: s.length()
来源：http://hz.gogol.net.cn/gtelfneejq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.redwolf501.top/gtrkqwatgh.html

Ruby: s.length
来源：http://hz.sweek.top/gtwjpjkqqk.html

C#:   s.Length
来源：http://hz.chenlongwang.top/gtgcgktcif.html

[A23] 大小写转换
来源：http://hz.wangdashe.top/gtliwdyznw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.shanyushiyangtech.top/gttepepvqa.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.9152youxi.cn/gtudfkdhuf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tian-w.cn/gtzpllayqf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shzxlz.cn/gtgoxwlmbn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.hywenlv.cn/gtwhnypnvk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.shangyingyoupin.top/gtkzadfvov.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.daria6918.cn/gtmhpomtdi.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.sxryk.cn/gtxkjtlnva.html

[A24] 去除首尾空白
来源：http://hz.gaohongyu789.top/gtmzacszgb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shanyushiyangkeji.top/gtrnmhzgif.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.tanke756.top/gtkkenwfnl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nwbrower.top/gtxcrvgkfq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nanxinkj.top/gtldfnmcby.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.chenjidiqi.icu/gthledicws.html

Go:   strings.TrimSpace(s)
来源：http://hz.nanxuanxn.top/gtzrcyzxcd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.52xcode.cn/gthbsdbicl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.316326.xyz/gtsnxulmsd.html

[A25] 字符串比较
来源：http://hz.sxryk.cn/gtevalarkz.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cashguo.top/gtojbvrzpe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhaomingkeji.xyz/gtfxhcqiri.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yvedp.cn/gtzgdkeexa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.iojbl.cn/gtfamvurcx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.aibaodan.cn/gtvebmuzam.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.snrcjt.cn/gtosbvovlc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.tianlin.xyz/gtxpisnqje.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.vqdsnc.cn/gtyxbahavj.html

[A26] 类型转换总览
来源：http://hz.gaohongyu789.top/gtbmmxjdid.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.aizwys.cn/gtteefmxvr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.shuidangran.top/gtzpmjfgbl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinghuilouyu.cn/gtdszsccys.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yueranfly.top/gtoujgxafr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ydzc1.top/gtnjouzrpz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jinghuilouyu.cn/gtwgelghtu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yonumen.top/gtzmihcuex.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.haohaochexian.top/gtcpnilseo.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtixmlayjx.html

B. 流程控制
来源：http://hz.daxiang520.top/gteceokryl.html

================================================================================
来源：http://hz.mhx1999.top/gthuyowcya.html

[B01] 条件判断 if / else
来源：http://hz.gzhubu.top/gtepbwsmbg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.nwbrower.top/gtdspozoyf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jiagoushi.top/gtidmyjabo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtnccdickp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhongyouzk.top/gtyvuyonjw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gtboslehfe.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.xziqi.cn/gtcutdzcrm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.sxryk.cn/gterluyrwk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.hywenlv.cn/gtjkjipata.html

[B02] 多分支 else if / elif
来源：http://hz.xuetiantiany.cn/gtaerovjfz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jqgfzy.top/gtclgnjdfs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.wangdashe.top/gtmfjiwgqr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cucudq.cn/gtcmehjyzl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtjkewsrkz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xylfe.cn/gtwhechjtf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.dianchejie.cn/gtiuztcxnf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.vqdsnc.cn/gtrphtrmsp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tanke756.top/gtbcjwuohc.html

[B03] switch / match / case
来源：http://hz.jiagoushi.top/gtuvwabbbq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hammf.cn/gtkwluoayx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.xinyue.icu/gtvkqkxkrr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yangfankeji.com/gtqvhysdph.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtimhypfmk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.aibaodan.cn/gtrywvrmfp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jinqigfzy.top/gtfvwkeiaz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.tian-w.cn/gtfjpqkwbj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.fzhhl.top/gtefmwcbnb.html

[B04] for 计数循环
来源：http://hz.pengpengdd.cyou/gtqrmsnosa.html

Py:   for i in range(10): print(i)
来源：http://hz.cdnleiting.top/gtzfummhxi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.guannengcc.top/gtbxxmoegn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuanzx.com/gtimtptmcy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuxming.cn/gthclsguga.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ybcxt.top/gtngftnuxi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.316326.xyz/gtisnfgeuj.html

Ruby: 10.times { |i| puts i }
来源：http://hz.fengsongda.top/gthyarxrtr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.hysaishi.cn/gtijzjcrvy.html

[B05] 遍历数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gteeiayaxj.html

Py:   for item in arr: print(item)
来源：http://hz.iojbl.cn/gtrsfteulj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhaomingkeji.xyz/gtexvblqry.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.havefunace.top/gtlabbizgo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yj202588.top/gtscbovgte.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jlsjyb.cn/gtmpqlmeeu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shzxlz.cn/gtqgbobpdv.html

Ruby: arr.each { |item| puts item }
来源：http://hz.aibaodan.cn/gtfapwwowh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.hysaishi.cn/gtuehcbxhm.html

[B06] 遍历字典 / 对象
来源：http://hz.andypj.xyz/gtkfysfkoy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xingfuxueyuan.xyz/gtqcgpjxth.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zhengqikj.top/gtpstnwitj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fengsongda.top/gtlwddwkfm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhoulong.xyz/gtparyugha.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.9152youxi.cn/gtutekkvqr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yj20258.top/gtzyztfelb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhiwuduotai.top/gtwjtjfzvv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zhixingplan.top/gtrwhkwaxs.html

[B07] while 循环
来源：http://hz.jyoumei.cn/gttlrxvpcs.html

Py:   while i < 10: i += 1
来源：http://hz.jinqigfzy.top/gtkbkgqezq.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.cheryme.top/gtxyjavzye.html

JS:   while (i < 10) { i++; }
来源：http://hz.zycfv.cn/gtulmvtksr.html

TS:   while (i < 10) { i++; }
来源：http://hz.hongshengwenyu.top/gtrjhalxhb.html

Java: while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtxztofims.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.pengpengdd.cyou/gtqvktvqhq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xylfe.cn/gtqlmjdazv.html

C#:   while (i < 10) { i++; }
来源：http://hz.feifeiyinyue.top/gtqgmhksmy.html

[B08] do-while（至少执行一次）
来源：http://hz.xuetiantiany.cn/gtlgfhohtb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cashguo.top/gtifycyejl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.vqdsnc.cn/gtmzdtoekd.html

JS:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtnwfmxlip.html

TS:   do { i++; } while (i < 10);
来源：http://hz.daria6918.cn/gtyeropbca.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtaglixdkk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zycfv.cn/gtepkqplje.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hnqzz.top/gtqonsdwph.html

C#:   do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gttcsavydd.html

[B09] break 与 continue
来源：http://hz.hammf.cn/gtvejvrthy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ydzc1.top/gtoeercave.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhengqikj.top/gtwqzasxmk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ivvv.top/gtkaabwndt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xylfe.cn/gtffkzsqyb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtbmxgrncg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.nwbrower.top/gtuniweixc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.tianlin.xyz/gtcaofbdss.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtvtvhbcty.html

[B10] 遍历同时拿索引
来源：http://hz.hywenlv.cn/gtypenhboi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hnqzz.top/gtblbbcxyz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.havefunace.top/gtuuzizbyf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.tanke756.top/gtpbmmnhfi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.mhx1999.top/gtaxidjubc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xuanzx.com/gttcpbrjai.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hywenlv.cn/gtdilcgbse.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ehwqpu.com/gtlrbipnbu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigfzy.top/gtszvckwgl.html

[B11] 生成数字序列 / 区间
来源：http://hz.jlsjyb.cn/gttsrqwoju.html

Py:   list(range(0, 10, 2))
来源：http://hz.pycfn.com/gtukbopakr.html

PHP:  range(0, 10, 2);
来源：http://hz.cqqwz.cn/gtfakjjxiy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtiefhimrq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnxiangtu.top/gtxwuhyzdi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhijiandao.cn/gtunnctryr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.bjfxy.top/gtbfylytod.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sxryk.cn/gtlsddblas.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj20258888.top/gtgpntuexs.html

[B12] 跳出多层循环
来源：http://hz.yueranfly.top/gtnfhunlvp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tian-w.cn/gtmmhnmgem.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.bjfxy.top/gthaesfyrp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtruazrltt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtmbythteu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gteemehqjn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.smart0.xyz/gtqnvgxcjz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.fzhhl.top/gtlzvogxnq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ppjwa.cn/gtnezumkam.html

[B13] 判断是否为数字
来源：http://hz.chenlongwang.top/gtipxrxhqh.html

Py:   isinstance(x, (int, float))
来源：http://hz.fengsongda.top/gtooyutubw.html

PHP:  is_numeric($x)
来源：http://hz.fzhhl.top/gtrjdywdjo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gaohongyu789.top/gttmuyihrb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shangyingyoupin.top/gtdmajnofs.html

Java: x instanceof Number
来源：http://hz.pycfn.com/gtvoxvbplr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sweek.top/gtmzjxzdmk.html

Ruby: x.is_a?(Numeric)
来源：http://hz.aibaodan.cn/gteuaitdnx.html

C#:   x is int or double or decimal
来源：http://hz.zhijiandao.cn/gtkiaonswz.html

[B14] 判断值是否在集合内
来源：http://hz.cdnleiting.top/gtrzgasbnx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gogol.net.cn/gttrrcgqfg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.havefunace.top/gtguziscqw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zdqjudy.top/gtgteigtki.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhijiandao.cn/gtgfflzxsa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinyuanbaomall.cn/gtfqzirots.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dianchejie.cn/gtfsjlhiby.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yanxiufei.cn/gtbruxlnak.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtzcitrrlv.html

[B15] 布尔运算与取反
来源：http://hz.zhongyouzk.top/gtxyitzosq.html

Py:   a and b or not c
来源：http://hz.jinyuanbaomall.cn/gtpzjicdcx.html

PHP:  $a && $b || !$c
来源：http://hz.yangfankeji.com/gtqnvydxsu.html

JS:   a && b || !c
来源：http://hz.gaohongyu789.top/gtsgvjpmuj.html

TS:   a && b || !c
来源：http://hz.nwbrower.top/gtdnzlwsva.html

Java: a && b || !c
来源：http://hz.pengpengdd.cyou/gtgscztyat.html

Go:   a && b || !c
来源：http://hz.daxiang520.top/gtjxlthmgy.html

Ruby: a && b || !c
来源：http://hz.shanyushiyangtech.top/gtquxnycjp.html

C#:   a && b || !c
来源：http://hz.sweek.top/gtjrgabgvc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yonumen.top/gteatnjili.html

Py:   if not data: return
来源：http://hz.nanxinkj.top/gtthxjbprw.html

PHP:  if (!$data) { return; }
来源：http://hz.hnqzz.top/gtbttwiaur.html

JS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtgcabgkhr.html

TS:   if (!data) return;
来源：http://hz.aibaodan.cn/gtjlikrnsl.html

Java: if (data == null) return;
来源：http://hz.hysaishi.cn/gtinobidyu.html

Go:   if data == nil { return }
来源：http://hz.quarkkingdee.top/gtwuruuqij.html

Ruby: return if data.nil?
来源：http://hz.52xcode.cn/gttsmshjbd.html

C#:   if (data == null) return;
来源：http://hz.shanyushiyangtech.top/gthcptvnhb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjbkxqstq.html

C. 函数与作用域
来源：http://hz.jianghu66.top/gtymmfhbte.html

================================================================================
来源：http://hz.chenzaomai.com/gtgvizedqj.html

[C01] 定义函数
来源：http://hz.jqgufenzy.top/gtscivmnzz.html

Py:   def add(a, b): return a + b
来源：http://hz.xingfuxueyuan.xyz/gtcogozqwg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ybcxt.top/gtmorbxqxz.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yuxming.cn/gtytpzavri.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.0kj1m.cn/gtbhlzvzmq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtsxlcihnm.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dashuyun.cn/gtbdjxqxgd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hnqzz.top/gtdqwzfrne.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yuxming.cn/gtidiyezgo.html

[C02] 默认参数
来源：http://hz.zhijiandao.cn/gtqkwrlscp.html

Py:   def greet(name="World"): return name
来源：http://hz.cheryme.top/gtvmvjkucp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cdnleiting.top/gtofuudmhy.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinghuilouyu.cn/gtfvspcyjd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.redwolf501.top/gtgqzcpamj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.52xcode.cn/gtzvhdoyly.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhijiandao.cn/gthqrgluzr.html

Ruby: def greet(name = "World") = name
来源：http://hz.dianchejie.cn/gtbpkwtdgz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tianlin.xyz/gtmlfvbdvj.html

[C03] 可变参数
来源：http://hz.zhijiandao.cn/gtgrgdnbqy.html

Py:   def total(*args): return sum(args)
来源：http://hz.sweek.top/gtpqgjyhav.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yangfankeji.com/gtfxaculnw.html


<!-- 参考信息 -->