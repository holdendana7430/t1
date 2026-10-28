代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.wangshuangyany.cn/gtjarrlpii.html

JS:   `Hello, ${name}!`
来源：http://hz.fengsongda.top/gtbbelcaev.html

TS:   `Hello, ${name}!`
来源：http://hz.aizwys.cn/gtihdgqcje.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.tanke756.top/gtldwrfilw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zycfv.cn/gtvqwliaob.html

Ruby: "Hello, #{name}!"
来源：http://hz.hywenlv.cn/gtnxxvvlwz.html

C#:   $"Hello, {name}!"
来源：http://hz.chenlongwang.top/gtpwkzwrqa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.shzxlz.cn/gtwyjbkezg.html

Py:   "第一行\n第二行"
来源：http://hz.ivvv.top/gtidnitjvv.html

PHP:  "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtnalozahx.html

JS:   "第一行\n第二行"
来源：http://hz.daria6918.cn/gtizjllkod.html

TS:   "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtevdyylzg.html

Java: "第一行\n第二行"
来源：http://hz.bjfxy.top/gtuzjvnxnq.html

Go:   "第一行\n第二行"
来源：http://hz.birdmap.top/gtyghmsqbv.html

Ruby: "第一行\n第二行"
来源：http://hz.hysaishi.cn/gteevuoegr.html

C#:   "第一行\n第二行"
来源：http://hz.cheryme.top/gtretgqdjv.html

[A14] 注释写法
来源：http://hz.xinyue.icu/gtwsoyunbw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.ydjk.org.cn/gtrepbxjmn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yueranfly.top/gtbwijymds.html

JS:   // 单行；/* 多行 */
来源：http://hz.hammf.cn/gtsmhubdfr.html

TS:   // 单行；/* 多行 */
来源：http://hz.daria6918.cn/gtfpcfgfww.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.tanke756.top/gtkkpaexpp.html

Go:   // 单行；/* 多行 */
来源：http://hz.dashuyun.cn/gtkztfnfkj.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jlsjyb.cn/gtygakjgso.html

C#:   // 单行；/* 多行 */
来源：http://hz.quarkkingdee.top/gtvuhthnfh.html

[A15] 空值判断与默认值
来源：http://hz.shuidangran.top/gttqyzpuau.html

Py:   value = data or "默认值"
来源：http://hz.yj20258.top/gtxskhrqso.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.dashuyun.cn/gtapdamwfv.html

JS:   const value = data ?? "默认值";
来源：http://hz.jinyuanbaomall.cn/gtqridknpx.html

TS:   const value = data ?? "默认值";
来源：http://hz.yvedp.cn/gtyayvzbbk.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.cashguo.top/gtbbheusmf.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.quarkkingdee.top/gtwkctrobz.html

Ruby: value = data || "默认值"
来源：http://hz.daxiang520.top/gtbekffrmx.html

C#:   var value = data ?? "默认值";
来源：http://hz.zdqjudy.top/gtrjuejvrw.html

[A16] 真假值判断规则
来源：http://hz.yueranfly.top/gtduvnfcpz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.gzhubu.top/gtuiwbmvnn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.nwbrower.top/gthbkypzti.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.zhengqikj.top/gtxuytwqvb.html

TS:   if (!x) {}
来源：http://hz.hnqzz.top/gtdycnkpzd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.52xcode.cn/gtozftjroh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.shanyushiyangtech.top/gtpkhzmptv.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.hywenlv.cn/gtzlcyzlhd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yongpay.top/gtsfmbevsf.html

[A17] 位运算
来源：http://hz.zycfv.cn/gtuiwzcvag.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtgbsnsmhu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.gotoacloud.top/gtbjfegtis.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtebyncgin.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtvzkeducv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ivvv.top/gtrnsakcnt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.daxiang520.top/gtuspljoux.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhengqikj.top/gtvvfpsslj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtjnjfvtwu.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jinghuilouyu.cn/gtobrjzfpq.html

Py:   ord("A"); chr(65)
来源：http://hz.zhoulong.xyz/gtjlidqkdc.html

PHP:  ord("A"); chr(65)
来源：http://hz.jinghuilouyu.cn/gtvjrqgeua.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxinkj.top/gtlzneictx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xylfe.cn/gtjktptfso.html

Java: (int) 'A'; (char) 65
来源：http://hz.jiagoushi.top/gtyiejatxh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.ybcxt.top/gtmejhrbxq.html

Ruby: "A".ord; 65.chr
来源：http://hz.nanxuanxn.top/gtsrcrnrcf.html

C#:   (int)'A'; (char)65
来源：http://hz.sxryk.cn/gtwuywsebf.html

[A19] 交换两个变量
来源：http://hz.xuetiantiany.cn/gttournagk.html

Py:   a, b = b, a
来源：http://hz.hammf.cn/gtgvduzbxp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.nanxinkj.top/gtlnmytnvm.html

JS:   [a, b] = [b, a];
来源：http://hz.hfpthk.cn/gtotsctkvz.html

TS:   [a, b] = [b, a];
来源：http://hz.jlsjyb.cn/gtkofmcmkl.html

Java: int t = a; a = b; b = t;
来源：http://hz.hammf.cn/gtzlztgubm.html

Go:   a, b = b, a
来源：http://hz.sweek.top/gtglomwdcg.html

Ruby: a, b = b, a
来源：http://hz.nwbrower.top/gtuomunirb.html

C#:   (a, b) = (b, a);
来源：http://hz.cheryme.top/gthjfzrynu.html

[A20] 读取标准输入
来源：http://hz.zhiwuduotai.top/gtkoxqoxpo.html

Py:   name = input("请输入：")
来源：http://hz.cqqwz.cn/gtxmbwqfwz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xingfuxueyuan.xyz/gtvazufkvf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.xinyue.icu/gtscjeivse.html

TS:   // Node.js：readline 模块
来源：http://hz.yj20258.top/gtyapjetso.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.chenlongwang.top/gttqzetebg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.tianlin.xyz/gthpaugctu.html

Ruby: gets.chomp
来源：http://hz.cashguo.top/gtjfrytqcr.html

C#:   Console.ReadLine();
来源：http://hz.9152youxi.cn/gtivdhzkao.html

[A21] 保留指定小数位输出
来源：http://hz.jinqigfzy.top/gtmndzjilc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.sufxvd.cn/gtoabkshbe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.aizwys.cn/gtuttfvojo.html

JS:   (3.14159).toFixed(2)
来源：http://hz.pycfn.com/gtmjcoriyd.html

TS:   (3.14159).toFixed(2)
来源：http://hz.daria6918.cn/gtgrodcphl.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.fzhhl.top/gtasrkuanw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.daria6918.cn/gtjewsszlq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gthaknkkyb.html

C#:   3.14159.ToString("F2")
来源：http://hz.yvedp.cn/gtyagrnhev.html

[A22] 获取字符串长度
来源：http://hz.9152youxi.cn/gtgwlqjrkf.html

Py:   len(s)
来源：http://hz.gogol.net.cn/gtocakhdtt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.316326.xyz/gtpmjasdjj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.wangdashe.top/gtyngsesgs.html

TS:   s.length
来源：http://hz.havefunace.top/gtwmnmcdlf.html

Java: s.length()
来源：http://hz.tian-w.cn/gtssmezmky.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cdnleiting.top/gttbujycco.html

Ruby: s.length
来源：http://hz.xinyue.icu/gtkyrbsilp.html

C#:   s.Length
来源：http://hz.yanxiufei.cn/gtakbnzzyv.html

[A23] 大小写转换
来源：http://hz.aizwys.cn/gturkwltrb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.meibo888.top/gtsaxjoaib.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.jinyuanbaomall.cn/gtssjwldxb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yonumen.top/gthxlerkyt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenjidiqi.icu/gtejbyrcjw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.daxiang520.top/gtnugijldb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zhixingplan.top/gteblhqwrr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ivvv.top/gtvfeshhvk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.ydjk.org.cn/gtpigrgmjk.html

[A24] 去除首尾空白
来源：http://hz.xziqi.cn/gtzxmmbnvg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yangfankeji.com/gtkjwqjdol.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yonumen.top/gtfqutkhoz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jyoumei.cn/gtazfhayrs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gotoacloud.top/gtjegecbxt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.tianlin.xyz/gtofamzmdf.html

Go:   strings.TrimSpace(s)
来源：http://hz.shanyushiyangkeji.top/gtjivysdcj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.cheryme.top/gtlhendrkm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.sysykeji.top/gtwetdgjrd.html

[A25] 字符串比较
来源：http://hz.ydjk.org.cn/gtzlrmmvnq.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ppjwa.cn/gtyjjlmmjp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.andypj.xyz/gtttcvtqxy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yangfankeji.com/gtvtacjqlh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hywenlv.cn/gtgvtahhre.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yueranfly.top/gtmjywcrsr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shanyushiyangtech.top/gtcjpteswl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.shangyingyoupin.top/gtrulbmspq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhixingplan.top/gtwsmhvhio.html

[A26] 类型转换总览
来源：http://hz.guannengcc.top/gtfwxzngxk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.iojbl.cn/gtmzitpema.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.pycfn.com/gtkbojfzac.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.kuanghao11.cn/gtyzcnicli.html

TS:   Number() String() Boolean() x as number
来源：http://hz.andypj.xyz/gtkcyjklmg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.svipenyu.cn/gtygwdtfbv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.gogol.net.cn/gtfrfmgzpi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yj20258.top/gtjzsqdyvn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.feifeiyinyue.top/gtlvcikojq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtssnmmilg.html

B. 流程控制
来源：http://hz.smart0.xyz/gtmekavxah.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttmetfvty.html

[B01] 条件判断 if / else
来源：http://hz.sxryk.cn/gtuxnmxysr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.mhx1999.top/gtqqapdtyb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.snrcjt.cn/gtnjggvxji.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhiwuduotai.top/gtwezazzdb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yuanzhike.top/gtlgxgwyer.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yongpay.top/gtyvutcelh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.shanyushiyangkeji.top/gtzmtbgfqf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.nanxinkj.top/gtshtrhpiy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yanxiufei.cn/gtxyzgwwdl.html

[B02] 多分支 else if / elif
来源：http://hz.fengsongda.top/gtjayrcmcg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.daria6918.cn/gtnrozprhm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jinyuanbaomall.cn/gtayyugmaa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cqqwz.cn/gtzkzvenkc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydjk.org.cn/gtuyglwpqg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gtjwrdzjqy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.shanyushiyangkeji.top/gtlfpwwatf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhiwuduotai.top/gtvqgbhbpe.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.9152youxi.cn/gtvmmvdwhc.html

[B03] switch / match / case
来源：http://hz.tian-w.cn/gtljwiwxyo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.tanke756.top/gtdvgwpsrd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.pengpengdd.cyou/gtyxgvkzzk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.0kj1m.cn/gtrhachhya.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.feifeiyinyue.top/gteqjbrbfj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.nanxinkj.top/gtazzbuhov.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.fengsongda.top/gtsmhgazyj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.svipenyu.cn/gtedvxwjbe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xinyue.icu/gtctagirsk.html

[B04] for 计数循环
来源：http://hz.zhoulong.xyz/gtskrxqipr.html

Py:   for i in range(10): print(i)
来源：http://hz.hnxiangtu.top/gtgckhodne.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.316326.xyz/gtbdcrpvte.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ybcxt.top/gthrzuajjf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.c1oappe.top/gtmqljpomb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.sufxvd.cn/gtjlvqmqbx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.chenzaomai.com/gtycpljibz.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hfpthk.cn/gtuvijdoyw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.kuanghao11.cn/gtpypvkcmp.html

[B05] 遍历数组 / 列表
来源：http://hz.316326.xyz/gtntbqfrkr.html

Py:   for item in arr: print(item)
来源：http://hz.shangyingyoupin.top/gtyuegyfgk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hammf.cn/gtarzpttcd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.gaohongyu789.top/gtvqjhzsth.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtmavedwrm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hysaishi.cn/gtvktebomk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yj20258.top/gtpsaqayaj.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tianlin.xyz/gtramuhors.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ehwqpu.com/gtwmflkhyg.html

[B06] 遍历字典 / 对象
来源：http://hz.yuxming.cn/gthnittjkm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hnxiangtu.top/gtrwzdziba.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.dianchejie.cn/gtewaixkmu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shuidangran.top/gtnmpsbmzd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuetiantiany.cn/gtzypfrugp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhaomingkeji.xyz/gtvexsfjqa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangshuangyany.cn/gtajbhjatj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.gotoacloud.top/gtcbexygtx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.chenzaomai.com/gtzcsqwzzq.html

[B07] while 循环
来源：http://hz.jinqigufen.top/gtguhzupvo.html

Py:   while i < 10: i += 1
来源：http://hz.zhijiandao.cn/gttdvjhxef.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.nwbrower.top/gtwxolmicb.html

JS:   while (i < 10) { i++; }
来源：http://hz.xziqi.cn/gtrogdezzu.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhiwuduotai.top/gtjmqmpolo.html

Java: while (i < 10) { i++; }
来源：http://hz.xylfe.cn/gtbneqgcvn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jqgfzy.top/gtmvgbqbvi.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jianghu66.top/gtuinqpqng.html

C#:   while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gtragsozfa.html

[B08] do-while（至少执行一次）
来源：http://hz.cqqwz.cn/gtevjaiaaa.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.daria6918.cn/gtkvrejfol.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhengqikj.top/gtpqdazgvk.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtsbgaflry.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jiagoushi.top/gtqbdigxen.html

Java: do { i++; } while (i < 10);
来源：http://hz.cheryme.top/gtydnijljy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.quarkkingdee.top/gteatiyrwd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yongpay.top/gtkalkrrsk.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtcdujfdnn.html

[B09] break 与 continue
来源：http://hz.jianghu66.top/gtdqynkxbb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pengpengdd.cyou/gtofkuuhtc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.mhx1999.top/gtspcpibzk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtpevrqdxd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtqirytcvk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yueranfly.top/gtlxwgkclq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zycfv.cn/gtstscdkou.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.sufxvd.cn/gtxrixwncx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtmrhidmns.html

[B10] 遍历同时拿索引
来源：http://hz.9152youxi.cn/gtlcwqipde.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinyuanbaomall.cn/gtyjasfhxw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhiwuduotai.top/gtxprpvslz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.redwolf501.top/gtszvoxdru.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.guannengcc.top/gtektmwqun.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.haohaochexian.top/gtyptvfigj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hfpthk.cn/gtchryuuxu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hongshengwenyu.top/gtgddiblow.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.c1oappe.top/gtsoayzpoj.html

[B11] 生成数字序列 / 区间
来源：http://hz.hammf.cn/gtrnxjheyp.html

Py:   list(range(0, 10, 2))
来源：http://hz.hnxiangtu.top/gtcrsmubcy.html

PHP:  range(0, 10, 2);
来源：http://hz.dianchejie.cn/gtihmvrirh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.birdmap.top/gtlkxwtqwl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtbvejzukp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.9152youxi.cn/gtcvuekgtt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ywan-chungtsiang.top/gtkupsvvqo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangkeji.top/gtrubbfvez.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.mhx1999.top/gtxqgeunov.html

[B12] 跳出多层循环
来源：http://hz.jinqigufen.top/gtbdneaygn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cashguo.top/gtxsavsggp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jiagoushi.top/gtzycerqzl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gtxsbxanck.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtbhslfhdu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cheryme.top/gtyrnkwuwb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhijiandao.cn/gtvgovnpez.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.bjfxy.top/gtklcgrhcu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shanyushiyangkeji.top/gtjfxlqvhl.html

[B13] 判断是否为数字
来源：http://hz.shzxlz.cn/gtdaquanan.html

Py:   isinstance(x, (int, float))
来源：http://hz.zycfv.cn/gtcadvjpua.html

PHP:  is_numeric($x)
来源：http://hz.nanxuanxn.top/gtdfbuoano.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jqgufenzy.top/gtwdvpivbg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.316326.xyz/gtqeggdawu.html

Java: x instanceof Number
来源：http://hz.tanke756.top/gtdjtxbovh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.haohaochexian.top/gtfexflhgu.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nwbrower.top/gtqjoqjtbi.html

C#:   x is int or double or decimal
来源：http://hz.svipenyu.cn/gtuillxqlg.html

[B14] 判断值是否在集合内
来源：http://hz.zdqjudy.top/gtnfikoplo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuetiantiany.cn/gtnqfdbrqf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj20258.top/gtsuqltbva.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shuidangran.top/gtowuuphhy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtxbmchewe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.meibo888.top/gtqlmsvxud.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ppjwa.cn/gtfwebvasu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj202588.top/gtiynvovyv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenlongwang.top/gtwcxlosjb.html

[B15] 布尔运算与取反
来源：http://hz.gaohongyu789.top/gtukcrjquh.html

Py:   a and b or not c
来源：http://hz.quarkkingdee.top/gtkclwbuqy.html

PHP:  $a && $b || !$c
来源：http://hz.gotoacloud.top/gteawcccuw.html

JS:   a && b || !c
来源：http://hz.jyoumei.cn/gtwjdtvctg.html

TS:   a && b || !c
来源：http://hz.daria6918.cn/gtiytrmurb.html

Java: a && b || !c
来源：http://hz.cheryme.top/gtefijecgz.html

Go:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtzlonutjt.html

Ruby: a && b || !c
来源：http://hz.zhengqikj.top/gttdpiario.html

C#:   a && b || !c
来源：http://hz.shuidangran.top/gtszmglbyd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.daxiang520.top/gtumbgcivg.html

Py:   if not data: return
来源：http://hz.jinghuilouyu.cn/gtqauabiuf.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gtsyckqqga.html

JS:   if (!data) return;
来源：http://hz.jqgfzy.top/gtyulayfnn.html

TS:   if (!data) return;
来源：http://hz.havefunace.top/gtnhnmijmx.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gtrtsyjbim.html

Go:   if data == nil { return }
来源：http://hz.redwolf501.top/gtwfcyafba.html

Ruby: return if data.nil?
来源：http://hz.jinqigufen.top/gtzxfoswpd.html

C#:   if (data == null) return;
来源：http://hz.quarkkingdee.top/gttoogyhyt.html

================================================================================
来源：http://hz.hywenlv.cn/gtpqhalxcy.html

C. 函数与作用域
来源：http://hz.yuanzhike.top/gteunooshn.html

================================================================================
来源：http://hz.chenzaomai.com/gtgdrzbzjt.html

[C01] 定义函数
来源：http://hz.gotoacloud.top/gtvvsicrwl.html

Py:   def add(a, b): return a + b
来源：http://hz.snrcjt.cn/gtkogxfdjh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtmuxnrxql.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.iojbl.cn/gtuvrquuwq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fzhhl.top/gtnpmgfudo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gthgktidfc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.haohaochexian.top/gtzlapwwco.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nanxuanxn.top/gtnpvzkapr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtcqjlnovu.html

[C02] 默认参数
来源：http://hz.nanxinkj.top/gtujztbdyi.html

Py:   def greet(name="World"): return name
来源：http://hz.wangdashe.top/gtloarvaah.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydjk.org.cn/gtnbktpynf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtrymytdql.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gtpjnbxmjx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xingfuxueyuan.xyz/gtchvfwvan.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.guowangkeji.top/gteszramji.html

Ruby: def greet(name = "World") = name
来源：http://hz.redwolf501.top/gtsdbwfhqo.html


<!-- 参考信息 -->