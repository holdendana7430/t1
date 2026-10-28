代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hz.jlsjyb.cn/gtpblaepuc.html

[A11] 条件表达式（三元）
来源：http://hz.jinqigfzy.top/gtsfwakzjg.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shangyingyoupin.top/gtnxsuaacs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.mhx1999.top/gtrkrzffwq.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.zhijiandao.cn/gtbgfsuubz.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.pengpengdd.cyou/gtvidxixbm.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.hnxiangtu.top/gtinoaypue.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.hnqzz.top/gtsgwnxuyo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtqudndoub.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jinqigfzy.top/gtzmnstcsi.html

[A12] 字符串插值 / 格式化
来源：http://hz.jinqigfzy.top/gtawiijxqw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hongshengwenyu.top/gtmkuerbkh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yj20258.top/gtkdvrovue.html

JS:   `Hello, ${name}!`
来源：http://hz.jinqigfzy.top/gtdfxonviv.html

TS:   `Hello, ${name}!`
来源：http://hz.hfpthk.cn/gtpnuxkpua.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.cucudq.cn/gtkfffmwwg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.iojbl.cn/gtyrkepdam.html

Ruby: "Hello, #{name}!"
来源：http://hz.shanyushiyangtech.top/gtospmvmfk.html

C#:   $"Hello, {name}!"
来源：http://hz.aizwys.cn/gtmjcohawj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.chenlongwang.top/gtyfwwoqvl.html

Py:   "第一行\n第二行"
来源：http://hz.xziqi.cn/gtlsvdpywf.html

PHP:  "第一行\n第二行"
来源：http://hz.ivvv.top/gtrwvmnsbm.html

JS:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtrbpqqxma.html

TS:   "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtrylfiumt.html

Java: "第一行\n第二行"
来源：http://hz.chenlongwang.top/gtorrdlnir.html

Go:   "第一行\n第二行"
来源：http://hz.xziqi.cn/gtqldeysvj.html

Ruby: "第一行\n第二行"
来源：http://hz.smart0.xyz/gtkerszujy.html

C#:   "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtlrczgvyr.html

[A14] 注释写法
来源：http://hz.nanxuanxn.top/gtysxbueay.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.yuxming.cn/gtfuxwbrpv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yj20258.top/gtttpjmaqd.html

JS:   // 单行；/* 多行 */
来源：http://hz.bjfxy.top/gtpgzixevq.html

TS:   // 单行；/* 多行 */
来源：http://hz.redwolf501.top/gtjxizuicn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.daria6918.cn/gtetxeeewf.html

Go:   // 单行；/* 多行 */
来源：http://hz.jyoumei.cn/gtrzqslesg.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yangfankeji.com/gtxjvlgcbn.html

C#:   // 单行；/* 多行 */
来源：http://hz.ivvv.top/gtlepmdohn.html

[A15] 空值判断与默认值
来源：http://hz.yuxming.cn/gtmqywrknx.html

Py:   value = data or "默认值"
来源：http://hz.zhaomingkeji.xyz/gtsirdcwjy.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.jianghu66.top/gtnqvtgjvo.html

JS:   const value = data ?? "默认值";
来源：http://hz.zhengqikj.top/gtbbivxsdo.html

TS:   const value = data ?? "默认值";
来源：http://hz.jqgfzy.top/gtidgfqzqf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yj20258.top/gthxbwfaby.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cucudq.cn/gtprzdtvwj.html

Ruby: value = data || "默认值"
来源：http://hz.ivvv.top/gtphuoxaty.html

C#:   var value = data ?? "默认值";
来源：http://hz.ivvv.top/gtwcekuinb.html

[A16] 真假值判断规则
来源：http://hz.andypj.xyz/gtnsyqeohq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.redwolf501.top/gtjacyydiz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.smart0.xyz/gtasjgfcwn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.sxryk.cn/gtasqzvbxw.html

TS:   if (!x) {}
来源：http://hz.hysaishi.cn/gtzdonpjvs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.tian-w.cn/gtgdzzevga.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jinqigufen.top/gtezhjcrgc.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.hfpthk.cn/gtqupbwtdy.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.havefunace.top/gtsezolyeo.html

[A17] 位运算
来源：http://hz.ppjwa.cn/gtexapmhzr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ehwqpu.com/gtnbxpzuea.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yueranfly.top/gtsazfjygd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.andypj.xyz/gtxvfrtcsr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.tianlin.xyz/gtwbjvqpgv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtajdtvkfe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ivvv.top/gthyeoitxz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigufen.top/gtakwxuemd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhiwuduotai.top/gtapsqkwvk.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jyoumei.cn/gtlfwoetms.html

Py:   ord("A"); chr(65)
来源：http://hz.pycfn.com/gtyftrkuxa.html

PHP:  ord("A"); chr(65)
来源：http://hz.shanyushiyangkeji.top/gtdssbppxm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hywenlv.cn/gtvsmxtryb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xinyue.icu/gtncauhmcs.html

Java: (int) 'A'; (char) 65
来源：http://hz.ywan-chungtsiang.top/gtwqiapqkf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.ppjwa.cn/gttxnjtrrn.html

Ruby: "A".ord; 65.chr
来源：http://hz.ppjwa.cn/gtzurbuhgs.html

C#:   (int)'A'; (char)65
来源：http://hz.shanyushiyangtech.top/gtpuvzbott.html

[A19] 交换两个变量
来源：http://hz.hfpthk.cn/gtykhuccyj.html

Py:   a, b = b, a
来源：http://hz.yj20258888.top/gtiqlduhfx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.ydzc1.top/gtrsfnmfcz.html

JS:   [a, b] = [b, a];
来源：http://hz.xylfe.cn/gtxgeyjwiv.html

TS:   [a, b] = [b, a];
来源：http://hz.shanyushiyangkeji.top/gtultkedlw.html

Java: int t = a; a = b; b = t;
来源：http://hz.cashguo.top/gtmzjjgjww.html

Go:   a, b = b, a
来源：http://hz.hongshengwenyu.top/gtwdjtzabf.html

Ruby: a, b = b, a
来源：http://hz.dashuyun.cn/gtunjfywjt.html

C#:   (a, b) = (b, a);
来源：http://hz.nanxinkj.top/gtukenyewh.html

[A20] 读取标准输入
来源：http://hz.fzhhl.top/gtqnwfuirz.html

Py:   name = input("请输入：")
来源：http://hz.yj20258.top/gtabeptuax.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cqqwz.cn/gtcydhwaik.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.dianchejie.cn/gthpygatmr.html

TS:   // Node.js：readline 模块
来源：http://hz.gotoacloud.top/gtvqctpnnm.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.316326.xyz/gtiznylgyu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.shanyushiyangtech.top/gtzppdioxh.html

Ruby: gets.chomp
来源：http://hz.yangfankeji.com/gtblortrtr.html

C#:   Console.ReadLine();
来源：http://hz.cqqwz.cn/gtctlqozoo.html

[A21] 保留指定小数位输出
来源：http://hz.ydzc1.top/gtbmrgeyqn.html

Py:   f"{3.14159:.2f}"
来源：http://hz.316326.xyz/gtzsovibrr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtmnucojca.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shuidangran.top/gtmjikzdrj.html

TS:   (3.14159).toFixed(2)
来源：http://hz.bjfxy.top/gtpohnbylx.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.havefunace.top/gtthkptogs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtjsjfdnij.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.gogol.net.cn/gtrdywufxh.html

C#:   3.14159.ToString("F2")
来源：http://hz.gogol.net.cn/gtxugwavks.html

[A22] 获取字符串长度
来源：http://hz.birdmap.top/gtmohbndva.html

Py:   len(s)
来源：http://hz.zhongyouzk.top/gtxzmutfjq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.guannengcc.top/gtuvpwduha.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhijiandao.cn/gtvkpqtbln.html

TS:   s.length
来源：http://hz.gotoacloud.top/gtejfzbwat.html

Java: s.length()
来源：http://hz.fengsongda.top/gtgbdyecny.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.shuidangran.top/gtmjtvdwoe.html

Ruby: s.length
来源：http://hz.0kj1m.cn/gtqknhopbd.html

C#:   s.Length
来源：http://hz.sxryk.cn/gthgcsfrog.html

[A23] 大小写转换
来源：http://hz.xuetiantiany.cn/gtngztwmzb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.daxiang520.top/gtnqxrzkdj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.fzhhl.top/gtylmpdsmr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.dianchejie.cn/gtudgvdawt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.chenzaomai.com/gtoikgzpgt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.aizwys.cn/gtlwyyruzy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.feifeiyinyue.top/gtcdgytxuz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhaomingkeji.xyz/gtxgxfocfw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jlsjyb.cn/gtuptpdwlf.html

[A24] 去除首尾空白
来源：http://hz.zhengqikj.top/gtyzfpxvbi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.xziqi.cn/gtrbvkchxx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.andypj.xyz/gtentszfyg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.c1oappe.top/gtyfldndrm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jlsjyb.cn/gtswjhvdzc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.feifeiyinyue.top/gtgozgjoll.html

Go:   strings.TrimSpace(s)
来源：http://hz.fengsongda.top/gtzatnsgjs.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.zdqjudy.top/gtkqosjdec.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.quarkkingdee.top/gtgitmurus.html

[A25] 字符串比较
来源：http://hz.hammf.cn/gtxaqlvxst.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jinyuanbaomall.cn/gtmfbzzuuh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cashguo.top/gtlkowixny.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yueranfly.top/gtyqkbbdqt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.shuidangran.top/gtkwnvgxnh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hongshengwenyu.top/gtqxbdnnrb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.kuanghao11.cn/gtxskpppad.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.iojbl.cn/gtuyyjlbbz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zycfv.cn/gtsvkmdsic.html

[A26] 类型转换总览
来源：http://hz.kuanghao11.cn/gtfmcbsopp.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.redwolf501.top/gtmdezzvmv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yj20258.top/gtvitimwnm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.redwolf501.top/gtpwcgjten.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhoulong.xyz/gtgqfyfogg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.pengpengdd.cyou/gthptlgffz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhijiandao.cn/gtpdcgzwwd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ydjk.org.cn/gtinogizrk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yanxiufei.cn/gtubktmwoe.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvhrhjftq.html

B. 流程控制
来源：http://hz.jianghu66.top/gtqfdftylk.html

================================================================================
来源：http://hz.hnqzz.top/gtdzixfwiu.html

[B01] 条件判断 if / else
来源：http://hz.jiagoushi.top/gthgysemlg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.svipenyu.cn/gtktozdgio.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhixingplan.top/gtnhqyspro.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xziqi.cn/gtbkhcfvnn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtjofsumgs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhiwuduotai.top/gtmshwjbna.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.9152youxi.cn/gtmzklxrvr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jinyuanbaomall.cn/gtkpvbeiff.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtjtuvimwh.html

[B02] 多分支 else if / elif
来源：http://hz.hnxiangtu.top/gtckndhmgt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gzhubu.top/gtokrmtred.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.c1oappe.top/gtkyjvpdqn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtyinxbmlm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xinyue.icu/gtxalnbldi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtdpzzxdoq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.nanxuanxn.top/gtqtraxmbp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.chenjidiqi.icu/gtktbytqlr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangkeji.top/gtxvxdtghn.html

[B03] switch / match / case
来源：http://hz.feifeiyinyue.top/gtwqegxupw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.aizwys.cn/gtdbskldjk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shanyushiyangkeji.top/gtzapwsstl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cdnleiting.top/gtwiuwsnqp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yuanzhike.top/gtxowugwnk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.bjfxy.top/gtappftgrx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.havefunace.top/gtkguginee.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yj202588.top/gtjckdgqsq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.yanxiufei.cn/gtpuffgycy.html

[B04] for 计数循环
来源：http://hz.tanke756.top/gtnxajtzdp.html

Py:   for i in range(10): print(i)
来源：http://hz.feifeiyinyue.top/gtevgapepo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jinqigfzy.top/gtuaydpiww.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xuanzx.com/gthffozsgt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gotoacloud.top/gtrjvpzwqo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.sxryk.cn/gtewfksbpp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.dashuyun.cn/gtbyxyxamd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.iojbl.cn/gtmkciksgg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.redwolf501.top/gtdjqsibni.html

[B05] 遍历数组 / 列表
来源：http://hz.c1oappe.top/gtcjqimpnz.html

Py:   for item in arr: print(item)
来源：http://hz.sufxvd.cn/gtvficygbl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yueranfly.top/gtsozldssf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgfzy.top/gtoelxvlki.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuxming.cn/gtjrahtjxi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sxryk.cn/gtaqayqlgx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.sysykeji.top/gtvgzccebm.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zycfv.cn/gtkvsurjcu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.dashuyun.cn/gtznhufuia.html

[B06] 遍历字典 / 对象
来源：http://hz.yuxming.cn/gtnioncinr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cqqwz.cn/gtewlhrggc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.redwolf501.top/gtuyzfyfqr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jlsjyb.cn/gtzljjosxo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhixingplan.top/gtqtjyhpiv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.xziqi.cn/gtjwnjbpmk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinghuilouyu.cn/gtldztllev.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.316326.xyz/gtbapufnfy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cqqwz.cn/gtbifnteef.html

[B07] while 循环
来源：http://hz.shangyingyoupin.top/gtblxfrolc.html

Py:   while i < 10: i += 1
来源：http://hz.hongshengwenyu.top/gtsbtxcfab.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ivvv.top/gtowigdbto.html

JS:   while (i < 10) { i++; }
来源：http://hz.tianlin.xyz/gtzjotjhry.html

TS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtlidekiji.html

Java: while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtysgzarls.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cdnleiting.top/gteabtjinf.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinyuanbaomall.cn/gtweetyano.html

C#:   while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gthlwijhen.html

[B08] do-while（至少执行一次）
来源：http://hz.wangshuangyany.cn/gtkjlvpvnm.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shanyushiyangkeji.top/gtpzknfxrc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.quarkkingdee.top/gtflzwxrws.html

JS:   do { i++; } while (i < 10);
来源：http://hz.hywenlv.cn/gtrcivwckz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtfcecxtun.html

Java: do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtxlvdlhul.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.tanke756.top/gtdrvgowex.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.birdmap.top/gthsgfftwu.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenlongwang.top/gtgubauecr.html

[B09] break 与 continue
来源：http://hz.meibo888.top/gtrrzthggq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xinyue.icu/gtidlslzpf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.tanke756.top/gtltigqizd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yj202588.top/gtabjtiaxi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtidhtfnwk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gthehqmuoz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yj20258.top/gtaqsufqjb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuanzx.com/gtsvopasnr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhongyouzk.top/gtefvbahyz.html

[B10] 遍历同时拿索引
来源：http://hz.wangshuangyany.cn/gtmkokqdry.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.dianchejie.cn/gtyflsnsxh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tianlin.xyz/gtgjlpmojb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shanyushiyangtech.top/gtyrpsfctu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.iojbl.cn/gtlzcwgsly.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hywenlv.cn/gteyrfpwxr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.bjfxy.top/gtgqizrvka.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.hnqzz.top/gtwewwtvds.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sxryk.cn/gtobztozzb.html

[B11] 生成数字序列 / 区间
来源：http://hz.ivvv.top/gtlpdueufm.html

Py:   list(range(0, 10, 2))
来源：http://hz.yj20258888.top/gteyxhdzvx.html

PHP:  range(0, 10, 2);
来源：http://hz.bjfxy.top/gtfzcsazrj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shangyingyoupin.top/gtbdfkelmf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnxiangtu.top/gtexqtpzih.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xuetiantiany.cn/gtsumjxxae.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.bjfxy.top/gtnpcvonyt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zdqjudy.top/gtoczkvvlb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guowangkeji.top/gtinaknrac.html

[B12] 跳出多层循环
来源：http://hz.ybcxt.top/gtghyffzvf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gaohongyu789.top/gtwhsmljyx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.xingfuxueyuan.xyz/gtyfpqglvf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtsgmjxocw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtftzgfoyj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtuapfgwrz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jianghu66.top/gtznkhgpnw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yonumen.top/gtyspfstax.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenjidiqi.icu/gtbjpypkay.html

[B13] 判断是否为数字
来源：http://hz.ybcxt.top/gtnfvxemnw.html

Py:   isinstance(x, (int, float))
来源：http://hz.ivvv.top/gtlavpxivf.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gttvnuyuco.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hfpthk.cn/gtjkojymiy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.kuanghao11.cn/gteyyglrka.html

Java: x instanceof Number
来源：http://hz.yuanzhike.top/gtcyvmtcry.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinyuanbaomall.cn/gtwqoaalrl.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yonumen.top/gtdnpgqfbp.html

C#:   x is int or double or decimal
来源：http://hz.sweek.top/gtcnsblmtd.html

[B14] 判断值是否在集合内
来源：http://hz.mhx1999.top/gttnhgbojj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zhijiandao.cn/gttwehddds.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.havefunace.top/gtaccyrnoz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.sysykeji.top/gtyokvycte.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.0kj1m.cn/gtzumqrbxu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yuanzhike.top/gtsjsemmbe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.snrcjt.cn/gtfpoxnaky.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xziqi.cn/gttwzezwkk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cqqwz.cn/gthwgmkylt.html

[B15] 布尔运算与取反
来源：http://hz.yueranfly.top/gtlakfbktd.html

Py:   a and b or not c
来源：http://hz.gzhubu.top/gtlukebsbe.html

PHP:  $a && $b || !$c
来源：http://hz.jinqigfzy.top/gttqwxcslp.html

JS:   a && b || !c
来源：http://hz.yuxming.cn/gtzabgzmul.html

TS:   a && b || !c
来源：http://hz.316326.xyz/gtgvhqhyih.html

Java: a && b || !c
来源：http://hz.chenlongwang.top/gtilqvgall.html

Go:   a && b || !c
来源：http://hz.sysykeji.top/gtdcznjylq.html

Ruby: a && b || !c
来源：http://hz.zhoulong.xyz/gtvxxnjarm.html

C#:   a && b || !c
来源：http://hz.yvedp.cn/gtylsqnxpc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sweek.top/gtvevecjnr.html

Py:   if not data: return
来源：http://hz.xylfe.cn/gtihzixusi.html

PHP:  if (!$data) { return; }
来源：http://hz.jlsjyb.cn/gtqxxbrcyh.html

JS:   if (!data) return;
来源：http://hz.yueranfly.top/gtbonknhda.html

TS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtoawtdjtt.html

Java: if (data == null) return;
来源：http://hz.wangdashe.top/gtrybrrwra.html

Go:   if data == nil { return }
来源：http://hz.jinghuilouyu.cn/gterdigkuz.html

Ruby: return if data.nil?
来源：http://hz.zhongyouzk.top/gtevhdvbbz.html

C#:   if (data == null) return;
来源：http://hz.redwolf501.top/gtckqhubzy.html

================================================================================
来源：http://hz.xinyue.icu/gtzopnrudq.html

C. 函数与作用域
来源：http://hz.yongpay.top/gtiozxdoli.html

================================================================================
来源：http://hz.nanxuanxn.top/gtyiehinvz.html

[C01] 定义函数
来源：http://hz.nanxinkj.top/gtukfynulk.html

Py:   def add(a, b): return a + b
来源：http://hz.xuanzx.com/gtvwvmmlnv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtcssdgzpm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gttilafrrq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuetiantiany.cn/gtoefjbcry.html


<!-- 参考信息 -->