代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zhiwuduotai.top/gtfjislosd.html

Ruby: "Hello, #{name}!"
来源：http://hz.feifeiyinyue.top/gtupkrscfn.html

C#:   $"Hello, {name}!"
来源：http://hz.jlsjyb.cn/gtxkembkjj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hysaishi.cn/gtnggqywfs.html

Py:   "第一行\n第二行"
来源：http://hz.bjfxy.top/gtwcyfqrnf.html

PHP:  "第一行\n第二行"
来源：http://hz.cheryme.top/gtbozwsnkx.html

JS:   "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtjbdqxqwu.html

TS:   "第一行\n第二行"
来源：http://hz.cqqwz.cn/gtizgxkite.html

Java: "第一行\n第二行"
来源：http://hz.mhx1999.top/gttcltkitx.html

Go:   "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtrrnneaos.html

Ruby: "第一行\n第二行"
来源：http://hz.ywan-chungtsiang.top/gtkrrqhide.html

C#:   "第一行\n第二行"
来源：http://hz.zycfv.cn/gtcbqelzop.html

[A14] 注释写法
来源：http://hz.zdqjudy.top/gtkmgkwhzf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hywenlv.cn/gtunwugulx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.zhixingplan.top/gtnmushkyv.html

JS:   // 单行；/* 多行 */
来源：http://hz.birdmap.top/gtuqaofatt.html

TS:   // 单行；/* 多行 */
来源：http://hz.daria6918.cn/gtjgkkwdxs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.pycfn.com/gtdlkhqqpn.html

Go:   // 单行；/* 多行 */
来源：http://hz.shangyingyoupin.top/gtyfhbtirf.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yj20258.top/gtzvolecws.html

C#:   // 单行；/* 多行 */
来源：http://hz.52xcode.cn/gtarftqxmj.html

[A15] 空值判断与默认值
来源：http://hz.cheryme.top/gttllqlosc.html

Py:   value = data or "默认值"
来源：http://hz.hfpthk.cn/gtewzwlizx.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zhongyouzk.top/gtibwdunxj.html

JS:   const value = data ?? "默认值";
来源：http://hz.sufxvd.cn/gtobrvmwai.html

TS:   const value = data ?? "默认值";
来源：http://hz.zycfv.cn/gtrnfumnpf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.xuanzx.com/gtrtoiquxk.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.smart0.xyz/gtlrwhmofq.html

Ruby: value = data || "默认值"
来源：http://hz.cucudq.cn/gtmalxlshd.html

C#:   var value = data ?? "默认值";
来源：http://hz.birdmap.top/gtdpzxncxp.html

[A16] 真假值判断规则
来源：http://hz.yuanzhike.top/gthwcdtsuv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.ivvv.top/gtefqhopmb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jqgufenzy.top/gttfrusrag.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.fengsongda.top/gtefuzamwm.html

TS:   if (!x) {}
来源：http://hz.aibaodan.cn/gtcjtihoxm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.ybcxt.top/gthjmnuoyy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.vqdsnc.cn/gtccnwruju.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.chenjidiqi.icu/gtzgodvmxi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.daxiang520.top/gtavlpvlxm.html

[A17] 位运算
来源：http://hz.chenzaomai.com/gtojyqhtwi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.aibaodan.cn/gtupmafzaq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.fengsongda.top/gttrhfljky.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nwbrower.top/gtpwkdeqfq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtmeanrijj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.9152youxi.cn/gtpenxmmdu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.xinyue.icu/gtfleylduo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zycfv.cn/gtxqmcrsck.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtettrcqoz.html

[A18] 字符与 ASCII 码互转
来源：http://hz.vqdsnc.cn/gtjcbhqzjt.html

Py:   ord("A"); chr(65)
来源：http://hz.haohaochexian.top/gtbbeajjik.html

PHP:  ord("A"); chr(65)
来源：http://hz.birdmap.top/gtijggztjc.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cdnleiting.top/gtdtcxfybd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.tanke756.top/gtjlvdwbil.html

Java: (int) 'A'; (char) 65
来源：http://hz.yj20258.top/gtqhxllktf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yuxming.cn/gtrglycduu.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhongyouzk.top/gtpfplrudg.html

C#:   (int)'A'; (char)65
来源：http://hz.jqgfzy.top/gtnlcrqqda.html

[A19] 交换两个变量
来源：http://hz.52xcode.cn/gtrthyfhqj.html

Py:   a, b = b, a
来源：http://hz.chenlongwang.top/gtsdnfmonz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shanyushiyangkeji.top/gtpdbigkfi.html

JS:   [a, b] = [b, a];
来源：http://hz.aibaodan.cn/gtyoybfqfw.html

TS:   [a, b] = [b, a];
来源：http://hz.guowangkeji.top/gtsklemshb.html

Java: int t = a; a = b; b = t;
来源：http://hz.zhoulong.xyz/gtbrcxhlbg.html

Go:   a, b = b, a
来源：http://hz.fengsongda.top/gtslqmbhkk.html

Ruby: a, b = b, a
来源：http://hz.fengsongda.top/gtzbumiefm.html

C#:   (a, b) = (b, a);
来源：http://hz.hysaishi.cn/gtpyrtmwax.html

[A20] 读取标准输入
来源：http://hz.pycfn.com/gtquiqbrzc.html

Py:   name = input("请输入：")
来源：http://hz.zdqjudy.top/gtffsvjtmi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ywan-chungtsiang.top/gtivhslqku.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.guowangkeji.top/gtvatnznnb.html

TS:   // Node.js：readline 模块
来源：http://hz.jqgufenzy.top/gtawjsmgye.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhengqikj.top/gteojgondf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ydjk.org.cn/gtlhegoqjv.html

Ruby: gets.chomp
来源：http://hz.mhx1999.top/gtiydohinv.html

C#:   Console.ReadLine();
来源：http://hz.guannengcc.top/gtwjcmyxjx.html

[A21] 保留指定小数位输出
来源：http://hz.xuetiantiany.cn/gtvnrwcfwb.html

Py:   f"{3.14159:.2f}"
来源：http://hz.nanxinkj.top/gtjzejkqag.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.hnxiangtu.top/gtlmpmxrtb.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ybcxt.top/gtvsozxmls.html

TS:   (3.14159).toFixed(2)
来源：http://hz.cdnleiting.top/gteeupotpv.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.sysykeji.top/gtvhrxwtqo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.yonumen.top/gtehfwwhdt.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.dashuyun.cn/gtbfhlcddb.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj20258.top/gtgznagkzv.html

[A22] 获取字符串长度
来源：http://hz.birdmap.top/gttrupluvt.html

Py:   len(s)
来源：http://hz.yonumen.top/gtmbbettjn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.shanyushiyangtech.top/gtenxyieqh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.guannengcc.top/gtjlhncnho.html

TS:   s.length
来源：http://hz.shzxlz.cn/gtzakbhiro.html

Java: s.length()
来源：http://hz.nanxinkj.top/gtyymyzwji.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.wangdashe.top/gtcktfggfj.html

Ruby: s.length
来源：http://hz.hnqzz.top/gtuevdfnhm.html

C#:   s.Length
来源：http://hz.pycfn.com/gtqrainfmt.html

[A23] 大小写转换
来源：http://hz.shanyushiyangtech.top/gthlxmdrfy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.xingfuxueyuan.xyz/gtfgvlpqeg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhoulong.xyz/gtbcnapfwg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yanxiufei.cn/gtijzeruua.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jqgfzy.top/gtvygbvcfe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.cheryme.top/gthyetejmb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.haohaochexian.top/gtuhavltsy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hammf.cn/gttnzgklye.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.vqdsnc.cn/gtqzbrtnxj.html

[A24] 去除首尾空白
来源：http://hz.xziqi.cn/gttrfhxqln.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.snrcjt.cn/gtudkeyhuh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.9152youxi.cn/gtyntqpzor.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yonumen.top/gtafgwcwwu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhengqikj.top/gtmutyzwdo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jqgufenzy.top/gtuwkvyvcw.html

Go:   strings.TrimSpace(s)
来源：http://hz.wangshuangyany.cn/gthhlropcn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jianghu66.top/gtzjlipwxj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.ydzc1.top/gtdkmypshm.html

[A25] 字符串比较
来源：http://hz.tian-w.cn/gtfeykuzns.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xuetiantiany.cn/gtputelwhs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.xuanzx.com/gtdcpescjs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.c1oappe.top/gtefssgzak.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gogol.net.cn/gtpnmifdrt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.jqgfzy.top/gtiflnhntv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.redwolf501.top/gtyofcjgra.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.vqdsnc.cn/gtbmqytoez.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.gogol.net.cn/gtwkttzfzf.html

[A26] 类型转换总览
来源：http://hz.fzhhl.top/gtzrgmtaei.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xylfe.cn/gtftqsleft.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.chenjidiqi.icu/gtyeejxtny.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.iojbl.cn/gtusdrukzs.html

TS:   Number() String() Boolean() x as number
来源：http://hz.daxiang520.top/gtzhhmaony.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhiwuduotai.top/gtvjlzabje.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhoulong.xyz/gtzqhdhufu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dashuyun.cn/gtlakouggf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yongpay.top/gttjcgujaq.html

================================================================================
来源：http://hz.guowangkeji.top/gtvgardjqv.html

B. 流程控制
来源：http://hz.hammf.cn/gtxdbwtwbl.html

================================================================================
来源：http://hz.yj202588.top/gtaxjnybcm.html

[B01] 条件判断 if / else
来源：http://hz.mhx1999.top/gtxlmtptgg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gotoacloud.top/gtyxsdoiva.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhixingplan.top/gtfzqkbeqf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yuanzhike.top/gtzhelaqiq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yanxiufei.cn/gtgqlejaqx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtfxfwahzx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.snrcjt.cn/gtgsrknryz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.havefunace.top/gtymtbnnku.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtvvbkxrxl.html

[B02] 多分支 else if / elif
来源：http://hz.chenzaomai.com/gtqkirxyie.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yvedp.cn/gtqemonclb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.shanyushiyangtech.top/gttanpylbs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tianlin.xyz/gtvcwkimgg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxuanxn.top/gtjjpolnoo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtszoqrvfk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yuanzhike.top/gtsbojekoz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jlsjyb.cn/gtjckcjeqq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangshuangyany.cn/gteiknjnfm.html

[B03] switch / match / case
来源：http://hz.chenjidiqi.icu/gtlnxyztqn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jinqigufen.top/gtoxjojqfr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.sweek.top/gtojciflmc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.vqdsnc.cn/gtqsriitwz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.redwolf501.top/gtdhgkusov.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.snrcjt.cn/gtnjwhdmff.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hywenlv.cn/gtylevwfuw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jinghuilouyu.cn/gtgflvtbsc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.daxiang520.top/gtcchosckv.html

[B04] for 计数循环
来源：http://hz.wangdashe.top/gtlhtpvwiv.html

Py:   for i in range(10): print(i)
来源：http://hz.chenzaomai.com/gtkgbdpxsm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.guowangkeji.top/gtsczvwejr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangdashe.top/gtjozopflr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.feifeiyinyue.top/gtqdvvwide.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xingfuxueyuan.xyz/gtjrelloto.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tanke756.top/gthrkmojrn.html

Ruby: 10.times { |i| puts i }
来源：http://hz.xziqi.cn/gtbiuvzytu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.jinghuilouyu.cn/gtajpcafam.html

[B05] 遍历数组 / 列表
来源：http://hz.xingfuxueyuan.xyz/gtfozvgbsm.html

Py:   for item in arr: print(item)
来源：http://hz.yongpay.top/gtlvmlmiog.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hnqzz.top/gtvgjfqavu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.quarkkingdee.top/gtbxoqyybw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.gzhubu.top/gtzqdxgjyr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.dianchejie.cn/gtylrydunq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnqzz.top/gtsmklltxv.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj202588.top/gtwsubimrc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.xuanzx.com/gtuathijpy.html

[B06] 遍历字典 / 对象
来源：http://hz.zhaomingkeji.xyz/gtblxwostf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuxming.cn/gtugkluxyp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.dianchejie.cn/gtclbeooyq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shuidangran.top/gtzsulseum.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.snrcjt.cn/gtvfhomnoy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ydjk.org.cn/gthlrqycvb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ydzc1.top/gtwxewwnne.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.quarkkingdee.top/gttipcvzam.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hongshengwenyu.top/gtsgjwsoyg.html

[B07] while 循环
来源：http://hz.zycfv.cn/gtbqgjvcpa.html

Py:   while i < 10: i += 1
来源：http://hz.xziqi.cn/gthjdafebh.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yanxiufei.cn/gtlegntanp.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtmcrixbbu.html

TS:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtcoanrfsk.html

Java: while (i < 10) { i++; }
来源：http://hz.daria6918.cn/gtruewqpmt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.daria6918.cn/gtqbtdvxoe.html

Ruby: while i < 10; i += 1; end
来源：http://hz.wangdashe.top/gtrujaumdl.html

C#:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtajtnanll.html

[B08] do-while（至少执行一次）
来源：http://hz.tian-w.cn/gtodtiplhj.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinqigfzy.top/gtgscdccuf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.redwolf501.top/gtwysoeucv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ehwqpu.com/gtttgujxok.html

TS:   do { i++; } while (i < 10);
来源：http://hz.birdmap.top/gtyulyqcbi.html

Java: do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtkfenwitn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.aizwys.cn/gtqjlinzaj.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ydjk.org.cn/gtlxflcchp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.nwbrower.top/gtvccvwhew.html

[B09] break 与 continue
来源：http://hz.yonumen.top/gtegnshdqf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jlsjyb.cn/gtuuraksvi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhixingplan.top/gtrdelrrwi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.birdmap.top/gtuomaaxny.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj20258888.top/gtuwghodia.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtfauyfjqz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shzxlz.cn/gtguwvjzbe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jqgufenzy.top/gtigguqyvg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtizxqrbpn.html

[B10] 遍历同时拿索引
来源：http://hz.ydzc1.top/gttlbrmqyy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.daxiang520.top/gtkkzbvmxu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daria6918.cn/gtmlykwppk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.feifeiyinyue.top/gteutwmtyz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtwuslvvuc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sysykeji.top/gticmogltz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shanyushiyangkeji.top/gtjdieafyr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sufxvd.cn/gtuzhxfzpn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xuetiantiany.cn/gtgklsxmzk.html

[B11] 生成数字序列 / 区间
来源：http://hz.snrcjt.cn/gtnbauwzet.html

Py:   list(range(0, 10, 2))
来源：http://hz.ywan-chungtsiang.top/gtryrwltob.html

PHP:  range(0, 10, 2);
来源：http://hz.jinghuilouyu.cn/gtmjqpvjqa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtmolqcltu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tianlin.xyz/gtebrayueg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.daria6918.cn/gtvtwqcqye.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xuetiantiany.cn/gtcutvocgm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.0kj1m.cn/gtiaavvpau.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xingfuxueyuan.xyz/gtspvbqtfm.html

[B12] 跳出多层循环
来源：http://hz.pycfn.com/gttopaencb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sufxvd.cn/gtkhecxuru.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.tian-w.cn/gtlgxusoml.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.meibo888.top/gtoztpzmkn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhijiandao.cn/gttysrdwau.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gthjvygyqo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shanyushiyangkeji.top/gtjsqkisgm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jqgufenzy.top/gtnrkcarzb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cucudq.cn/gtglhgaplo.html

[B13] 判断是否为数字
来源：http://hz.ppjwa.cn/gtblrhibrp.html

Py:   isinstance(x, (int, float))
来源：http://hz.bjfxy.top/gtkwednioi.html

PHP:  is_numeric($x)
来源：http://hz.gotoacloud.top/gtmpugehwq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtktmdcyor.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jyoumei.cn/gtjltoscjt.html

Java: x instanceof Number
来源：http://hz.yanxiufei.cn/gtuwpvemmx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xylfe.cn/gtdgnfybbk.html

Ruby: x.is_a?(Numeric)
来源：http://hz.redwolf501.top/gtisgpzhxn.html

C#:   x is int or double or decimal
来源：http://hz.zhaomingkeji.xyz/gtkajwflwm.html

[B14] 判断值是否在集合内
来源：http://hz.guannengcc.top/gtiewmeznv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.meibo888.top/gtgbxkrybl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.haohaochexian.top/gtcjinvzpn.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigfzy.top/gtfmwjvbnt.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.havefunace.top/gturdwebsu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.snrcjt.cn/gtbtlsqjxa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shzxlz.cn/gtlfulfweb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.haohaochexian.top/gtdbxnfzbe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hammf.cn/gtebskcamw.html

[B15] 布尔运算与取反
来源：http://hz.0kj1m.cn/gtknrchpov.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtpxqiiadc.html

PHP:  $a && $b || !$c
来源：http://hz.zhaomingkeji.xyz/gtybelzwaj.html

JS:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtvnpxbdqc.html

TS:   a && b || !c
来源：http://hz.gaohongyu789.top/gtohsirldc.html

Java: a && b || !c
来源：http://hz.yuanzhike.top/gtynnjrsjv.html

Go:   a && b || !c
来源：http://hz.fzhhl.top/gtmbrfeiuj.html

Ruby: a && b || !c
来源：http://hz.yuanzhike.top/gtoibhcxbr.html

C#:   a && b || !c
来源：http://hz.hywenlv.cn/gtiabjhsgl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.vqdsnc.cn/gtqjnwvxon.html

Py:   if not data: return
来源：http://hz.xylfe.cn/gtygctarjc.html

PHP:  if (!$data) { return; }
来源：http://hz.jianghu66.top/gtfcshxhmd.html

JS:   if (!data) return;
来源：http://hz.andypj.xyz/gtlaljgsow.html

TS:   if (!data) return;
来源：http://hz.pycfn.com/gttpcpbaes.html

Java: if (data == null) return;
来源：http://hz.sxryk.cn/gtxjlagwoo.html

Go:   if data == nil { return }
来源：http://hz.yongpay.top/gttzobccnr.html

Ruby: return if data.nil?
来源：http://hz.svipenyu.cn/gtejpfhxql.html

C#:   if (data == null) return;
来源：http://hz.hammf.cn/gtwgukvuoe.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvnbmuksj.html

C. 函数与作用域
来源：http://hz.ppjwa.cn/gtgzvqvhxw.html

================================================================================
来源：http://hz.52xcode.cn/gtegflonon.html

[C01] 定义函数
来源：http://hz.xuanzx.com/gtzeoyeixl.html

Py:   def add(a, b): return a + b
来源：http://hz.jiagoushi.top/gtejgwspae.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtfswhbotn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtoytdzxwx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtveiznbcb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gtjnvkutzd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.aibaodan.cn/gtoymyktsp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zycfv.cn/gtilewatqc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.316326.xyz/gtprlkkzow.html

[C02] 默认参数
来源：http://hz.jianghu66.top/gtjrkjzvud.html

Py:   def greet(name="World"): return name
来源：http://hz.sweek.top/gtrkxguhih.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.pengpengdd.cyou/gtnladnzrx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.quarkkingdee.top/gturelqqyw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gthxybhpik.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aibaodan.cn/gtkxcwglfi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.pycfn.com/gtgfbnkneu.html

Ruby: def greet(name = "World") = name
来源：http://hz.yonumen.top/gtedeeijsu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ivvv.top/gtxxiihvpa.html

[C03] 可变参数
来源：http://hz.meibo888.top/gtjiefudcf.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuxming.cn/gtnrfozvrr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.c1oappe.top/gtfbpujiih.html


<!-- 参考信息 -->