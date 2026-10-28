代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.tian-w.cn/gtuhpfthwm.html

JS:   `Hello, ${name}!`
来源：http://hz.aizwys.cn/gtqupuqoyt.html

TS:   `Hello, ${name}!`
来源：http://hz.quarkkingdee.top/gtcwgjrrpc.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hnxiangtu.top/gtcpkygdlf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.xylfe.cn/gtbwztzepz.html

Ruby: "Hello, #{name}!"
来源：http://hz.jianghu66.top/gtinnrrepk.html

C#:   $"Hello, {name}!"
来源：http://hz.svipenyu.cn/gtyiutcyqj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.xuetiantiany.cn/gtxubyiexv.html

Py:   "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtviwmyglt.html

PHP:  "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtrlvnpwgz.html

JS:   "第一行\n第二行"
来源：http://hz.feifeiyinyue.top/gtzgeyzlkf.html

TS:   "第一行\n第二行"
来源：http://hz.snrcjt.cn/gtpmtcllgk.html

Java: "第一行\n第二行"
来源：http://hz.haohaochexian.top/gtjqqxdldw.html

Go:   "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtlfdygcse.html

Ruby: "第一行\n第二行"
来源：http://hz.ppjwa.cn/gthipvtdvy.html

C#:   "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtvgaacjav.html

[A14] 注释写法
来源：http://hz.xingfuxueyuan.xyz/gtoukonsud.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hongshengwenyu.top/gtxjysxsoj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.zhongyouzk.top/gthyvixggn.html

JS:   // 单行；/* 多行 */
来源：http://hz.snrcjt.cn/gtasbsoosk.html

TS:   // 单行；/* 多行 */
来源：http://hz.yongpay.top/gtqyjyfukj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.yonumen.top/gtengcfdny.html

Go:   // 单行；/* 多行 */
来源：http://hz.cashguo.top/gtovyoqnat.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.redwolf501.top/gtuafhzsam.html

C#:   // 单行；/* 多行 */
来源：http://hz.mhx1999.top/gttalimucr.html

[A15] 空值判断与默认值
来源：http://hz.cheryme.top/gtnydnzbxi.html

Py:   value = data or "默认值"
来源：http://hz.0kj1m.cn/gtqfordprq.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.tian-w.cn/gtcflipzpq.html

JS:   const value = data ?? "默认值";
来源：http://hz.cdnleiting.top/gtglaggoqw.html

TS:   const value = data ?? "默认值";
来源：http://hz.yongpay.top/gtjnilzkcj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.yuxming.cn/gtzqmbhmbb.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.wangshuangyany.cn/gtrfbjikin.html

Ruby: value = data || "默认值"
来源：http://hz.fzhhl.top/gtebtghqkl.html

C#:   var value = data ?? "默认值";
来源：http://hz.xingfuxueyuan.xyz/gtbpioxhgg.html

[A16] 真假值判断规则
来源：http://hz.kuanghao11.cn/gtcwizijet.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yueranfly.top/gthknsuwsy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.chenlongwang.top/gtxxvxwhyk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.chenjidiqi.icu/gtdpticcxu.html

TS:   if (!x) {}
来源：http://hz.xuetiantiany.cn/gttweisleh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.mhx1999.top/gttdcbtbpn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.meibo888.top/gtujlabmsx.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.gotoacloud.top/gtovjjvold.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.smart0.xyz/gtguauqknb.html

[A17] 位运算
来源：http://hz.aibaodan.cn/gtplugrqbi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigufen.top/gtoeqxbkzg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yongpay.top/gtqutyfykb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.haohaochexian.top/gtvwsciceq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.316326.xyz/gtfjkkxpws.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.feifeiyinyue.top/gtbfxgxjbi.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtqqaayjuw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.feifeiyinyue.top/gtxkdbfcxy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xingfuxueyuan.xyz/gtbjtdymac.html

[A18] 字符与 ASCII 码互转
来源：http://hz.fzhhl.top/gtckauszjf.html

Py:   ord("A"); chr(65)
来源：http://hz.hnxiangtu.top/gttvrtlspg.html

PHP:  ord("A"); chr(65)
来源：http://hz.vqdsnc.cn/gtopautqko.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.sweek.top/gtjflweuji.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhixingplan.top/gtoxmbhvss.html

Java: (int) 'A'; (char) 65
来源：http://hz.316326.xyz/gtusfxgqcp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yj20258.top/gtavhvqcni.html

Ruby: "A".ord; 65.chr
来源：http://hz.ppjwa.cn/gtlyzjrxzl.html

C#:   (int)'A'; (char)65
来源：http://hz.jianghu66.top/gtouproyxy.html

[A19] 交换两个变量
来源：http://hz.jinqigfzy.top/gtfjuedjtz.html

Py:   a, b = b, a
来源：http://hz.yanxiufei.cn/gtgzczonaa.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.dianchejie.cn/gtgjjpjktz.html

JS:   [a, b] = [b, a];
来源：http://hz.aizwys.cn/gtynypbjsb.html

TS:   [a, b] = [b, a];
来源：http://hz.tian-w.cn/gtuonycqnn.html

Java: int t = a; a = b; b = t;
来源：http://hz.jinyuanbaomall.cn/gtsecojtqe.html

Go:   a, b = b, a
来源：http://hz.zhengqikj.top/gtxrrovjfx.html

Ruby: a, b = b, a
来源：http://hz.haohaochexian.top/gtldxlbsts.html

C#:   (a, b) = (b, a);
来源：http://hz.cashguo.top/gtyiatwkpd.html

[A20] 读取标准输入
来源：http://hz.shanyushiyangkeji.top/gtbjvpksvo.html

Py:   name = input("请输入：")
来源：http://hz.xylfe.cn/gtamipmntv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.chenlongwang.top/gtxbnjlelz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.sxryk.cn/gtvioquflu.html

TS:   // Node.js：readline 模块
来源：http://hz.xuanzx.com/gtomuzmsnl.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.shangyingyoupin.top/gtscbrjxdv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xziqi.cn/gtsiqqierj.html

Ruby: gets.chomp
来源：http://hz.hnqzz.top/gtdtbbskza.html

C#:   Console.ReadLine();
来源：http://hz.sxryk.cn/gtavekxybf.html

[A21] 保留指定小数位输出
来源：http://hz.jinyuanbaomall.cn/gtpeosasyc.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yangfankeji.com/gtcexrcwgm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.hongshengwenyu.top/gtdaexhejo.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sxryk.cn/gtcewalpmh.html

TS:   (3.14159).toFixed(2)
来源：http://hz.gaohongyu789.top/gtygybialp.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.quarkkingdee.top/gtqftntlyi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.redwolf501.top/gtczuidxpt.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.chenlongwang.top/gtidbqbcmw.html

C#:   3.14159.ToString("F2")
来源：http://hz.hywenlv.cn/gtkaqrhouu.html

[A22] 获取字符串长度
来源：http://hz.ppjwa.cn/gtbhfnebaq.html

Py:   len(s)
来源：http://hz.quarkkingdee.top/gtprfghlew.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xuanzx.com/gtvjmozezg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.jinqigufen.top/gtqjldkzwh.html

TS:   s.length
来源：http://hz.hnqzz.top/gtjguwpqtt.html

Java: s.length()
来源：http://hz.fengsongda.top/gtnvvjlwba.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.pengpengdd.cyou/gtuvgacojz.html

Ruby: s.length
来源：http://hz.andypj.xyz/gttfvszenb.html

C#:   s.Length
来源：http://hz.cashguo.top/gtffrsmjiv.html

[A23] 大小写转换
来源：http://hz.jqgufenzy.top/gtazpketvy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.cheryme.top/gtcnnxmkqf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.shangyingyoupin.top/gtpndonfqg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.gzhubu.top/gtrswrwwgd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hywenlv.cn/gtipgysdaz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.tanke756.top/gtnnydobkj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.xylfe.cn/gtwxshodvl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yvedp.cn/gtkfpaualy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.smart0.xyz/gtvftodeai.html

[A24] 去除首尾空白
来源：http://hz.aizwys.cn/gtxbiqyyan.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.daria6918.cn/gtdubtkwhy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yj20258888.top/gttcfncxxv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jyoumei.cn/gtelxfmhqz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gaohongyu789.top/gtvsybzjrb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ivvv.top/gtklkkhgnd.html

Go:   strings.TrimSpace(s)
来源：http://hz.ehwqpu.com/gtjbupkhap.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.mhx1999.top/gtcnhegevh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.chenlongwang.top/gtyrwcspbz.html

[A25] 字符串比较
来源：http://hz.fengsongda.top/gtkpiryxwi.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ybcxt.top/gtwzwcxzny.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cashguo.top/gtnsagicaf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.sweek.top/gtmsazmtny.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.haohaochexian.top/gtjmmevlfj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.havefunace.top/gthqjpletg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ehwqpu.com/gtnmylacpo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhaomingkeji.xyz/gtadqihjcd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ybcxt.top/gtmoezvqxe.html

[A26] 类型转换总览
来源：http://hz.cdnleiting.top/gtmyllnjgz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yangfankeji.com/gtunwollmo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xuetiantiany.cn/gtnewdmgux.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.sxryk.cn/gtfmavdvql.html

TS:   Number() String() Boolean() x as number
来源：http://hz.yonumen.top/gtbpzhvmcr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.snrcjt.cn/gtuucuwyzi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.quarkkingdee.top/gtsycanqfp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.bjfxy.top/gtnzdiczfu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.kuanghao11.cn/gtkhzitjxu.html

================================================================================
来源：http://hz.cqqwz.cn/gtubgzpmia.html

B. 流程控制
来源：http://hz.svipenyu.cn/gtlwuadits.html

================================================================================
来源：http://hz.daxiang520.top/gtogziorpo.html

[B01] 条件判断 if / else
来源：http://hz.ppjwa.cn/gtylwfnjaf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cqqwz.cn/gtfoyosyhf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.vqdsnc.cn/gtdgfvdmcu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hfpthk.cn/gthngwxmkp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xingfuxueyuan.xyz/gtzniahakb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gtroxoozld.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.ehwqpu.com/gtacpqlksc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jinqigfzy.top/gtrroddbtn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ppjwa.cn/gtfothmlik.html

[B02] 多分支 else if / elif
来源：http://hz.zhiwuduotai.top/gtsgnhjylg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhixingplan.top/gtejahppds.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.aibaodan.cn/gtfijekjwm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hongshengwenyu.top/gtqlbpmaqa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cashguo.top/gtbpxfrnia.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtsdpxugnh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yuanzhike.top/gtyawwzqdt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhongyouzk.top/gtvlmrxjse.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtlawkrjft.html

[B03] switch / match / case
来源：http://hz.feifeiyinyue.top/gtslsrzukc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.wangshuangyany.cn/gtxbjmecsy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yonumen.top/gtwlobcgnz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.52xcode.cn/gtfecpbbkp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yanxiufei.cn/gtvomgbzjw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.mhx1999.top/gtcafvdbvd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.9152youxi.cn/gtqcmwtfoo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.9152youxi.cn/gtxmjldjlz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xinyue.icu/gtubghtidr.html

[B04] for 计数循环
来源：http://hz.zhongyouzk.top/gtndfshupl.html

Py:   for i in range(10): print(i)
来源：http://hz.yanxiufei.cn/gttvfnrdzp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhiwuduotai.top/gtdetnsnex.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.smart0.xyz/gtrmuwcspi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gtiaiotgmx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.chenlongwang.top/gtbjyzvntl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.0kj1m.cn/gttpidnxot.html

Ruby: 10.times { |i| puts i }
来源：http://hz.gzhubu.top/gthgrauefc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhixingplan.top/gtgmiilybd.html

[B05] 遍历数组 / 列表
来源：http://hz.aibaodan.cn/gtxgpvhqtm.html

Py:   for item in arr: print(item)
来源：http://hz.aibaodan.cn/gtlsmmljdx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shanyushiyangtech.top/gtpplrjgga.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenzaomai.com/gtsxswlphc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.andypj.xyz/gtejajkvhm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xylfe.cn/gtjisevlun.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yanxiufei.cn/gtexxkmjvi.html

Ruby: arr.each { |item| puts item }
来源：http://hz.shanyushiyangtech.top/gtusyzasha.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.0kj1m.cn/gtctyvndmz.html

[B06] 遍历字典 / 对象
来源：http://hz.xingfuxueyuan.xyz/gtovjgqkmq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhaomingkeji.xyz/gtxnaiklsa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yongpay.top/gtdbvdlzqk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydzc1.top/gtyhpjuisb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgufenzy.top/gtetxpxkcu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtrpfbpbil.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yuxming.cn/gtriyvyhqw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yvedp.cn/gtviflsfku.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jiagoushi.top/gtgpglumbg.html

[B07] while 循环
来源：http://hz.jinyuanbaomall.cn/gtnfjlfzjh.html

Py:   while i < 10: i += 1
来源：http://hz.ivvv.top/gtvgmpmrpi.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.guowangkeji.top/gteqsbyiuc.html

JS:   while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gtyrdhkyky.html

TS:   while (i < 10) { i++; }
来源：http://hz.ppjwa.cn/gtudhdsmgt.html

Java: while (i < 10) { i++; }
来源：http://hz.cqqwz.cn/gtqmautmqw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhoulong.xyz/gtprrtcbiq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jinghuilouyu.cn/gtwpgnqbjb.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinqigufen.top/gtiapmwvar.html

[B08] do-while（至少执行一次）
来源：http://hz.ybcxt.top/gtytcqqzsr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jiagoushi.top/gtcqhlxwml.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hongshengwenyu.top/gtfjsgjych.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtsgifftxi.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtzvenpowo.html

Java: do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtfxlxcwdp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhijiandao.cn/gtdfcvfeiq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pycfn.com/gtoliswlpy.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnqzz.top/gtwzrtihqf.html

[B09] break 与 continue
来源：http://hz.sweek.top/gtuhwspwuz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yonumen.top/gtuwzurqxg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hywenlv.cn/gthnlmovin.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.fzhhl.top/gteepxhikx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gttazqcjxl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.c1oappe.top/gtsprromtn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hnxiangtu.top/gtxnuqxhdt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.havefunace.top/gthbdulcsh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtovnqvnnf.html

[B10] 遍历同时拿索引
来源：http://hz.quarkkingdee.top/gtexshvcvw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhoulong.xyz/gtnmymtudq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gogol.net.cn/gtbnjwtxnw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.sufxvd.cn/gtitvpthhr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aizwys.cn/gtfogmontr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.vqdsnc.cn/gtmjhnspen.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cucudq.cn/gtshapzkhi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ydjk.org.cn/gtbyfpciwq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.pengpengdd.cyou/gtjvgbdpao.html

[B11] 生成数字序列 / 区间
来源：http://hz.meibo888.top/gtaiascsqz.html

Py:   list(range(0, 10, 2))
来源：http://hz.jinqigufen.top/gtxuxvafdk.html

PHP:  range(0, 10, 2);
来源：http://hz.jinyuanbaomall.cn/gtpcflpthd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gaohongyu789.top/gtryiuikwz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gtrpxkdtbm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ywan-chungtsiang.top/gtdqnrdswi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jqgufenzy.top/gtnqiddirh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.316326.xyz/gtbelbfyai.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.shanyushiyangkeji.top/gtfunmkivf.html

[B12] 跳出多层循环
来源：http://hz.fengsongda.top/gteuyvzryv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.andypj.xyz/gtbmdkqeab.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhiwuduotai.top/gtlhzakfdv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenzaomai.com/gtvkjhrvaz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gtchudxkgd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgufenzy.top/gtgesrbpqo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.bjfxy.top/gthircisef.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jlsjyb.cn/gtfffpfrit.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xylfe.cn/gtxqkypgox.html

[B13] 判断是否为数字
来源：http://hz.chenzaomai.com/gttptexmbe.html

Py:   isinstance(x, (int, float))
来源：http://hz.hywenlv.cn/gttazhjzjo.html

PHP:  is_numeric($x)
来源：http://hz.yueranfly.top/gtuefbmhuh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtxvxfqute.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtpadxjlzx.html

Java: x instanceof Number
来源：http://hz.jinghuilouyu.cn/gtwlqtzxzt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xziqi.cn/gtmvykclxb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hongshengwenyu.top/gtdyrptarx.html

C#:   x is int or double or decimal
来源：http://hz.snrcjt.cn/gtssgywbna.html

[B14] 判断值是否在集合内
来源：http://hz.hongshengwenyu.top/gtwzonrdct.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sweek.top/gtzulgnvsq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hfpthk.cn/gtxtizgfnv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtrlxdpwvi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gtbouoykbf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hongshengwenyu.top/gtrtrdykal.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shanyushiyangkeji.top/gtmaurmprd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.daxiang520.top/gtnjzxfqqh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sweek.top/gtsqcyzbuf.html

[B15] 布尔运算与取反
来源：http://hz.ehwqpu.com/gtvrpktojw.html

Py:   a and b or not c
来源：http://hz.fzhhl.top/gtdddvpueo.html

PHP:  $a && $b || !$c
来源：http://hz.aizwys.cn/gtcgmdwikm.html

JS:   a && b || !c
来源：http://hz.zhixingplan.top/gtritihmld.html

TS:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtltisqywp.html

Java: a && b || !c
来源：http://hz.yuxming.cn/gtrqjvfzaz.html

Go:   a && b || !c
来源：http://hz.ehwqpu.com/gtvfniysiq.html

Ruby: a && b || !c
来源：http://hz.nanxuanxn.top/gtfpsshdor.html

C#:   a && b || !c
来源：http://hz.xinyue.icu/gtzgyhufpf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yanxiufei.cn/gtnhiwpube.html

Py:   if not data: return
来源：http://hz.pycfn.com/gtsvxfujmi.html

PHP:  if (!$data) { return; }
来源：http://hz.9152youxi.cn/gtwvyzpjbv.html

JS:   if (!data) return;
来源：http://hz.xziqi.cn/gtycwyyjfl.html

TS:   if (!data) return;
来源：http://hz.nanxuanxn.top/gtjdtvrfpa.html

Java: if (data == null) return;
来源：http://hz.cqqwz.cn/gtlrgcpeof.html

Go:   if data == nil { return }
来源：http://hz.zhijiandao.cn/gtxyxbreaz.html

Ruby: return if data.nil?
来源：http://hz.mhx1999.top/gtwdftidzs.html

C#:   if (data == null) return;
来源：http://hz.dianchejie.cn/gtqspazhuf.html

================================================================================
来源：http://hz.gogol.net.cn/gtdkkpwkhh.html

C. 函数与作用域
来源：http://hz.ywan-chungtsiang.top/gtdztsspkt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqlfzqpcu.html

[C01] 定义函数
来源：http://hz.cheryme.top/gtwegwramx.html

Py:   def add(a, b): return a + b
来源：http://hz.yanxiufei.cn/gtipvnzzmy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtrkjcvrkg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hnxiangtu.top/gtvmdkyqla.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtzelnzold.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangtech.top/gtrewfusdu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinyuanbaomall.cn/gtekheqtup.html

Ruby: def add(a, b); a + b; end
来源：http://hz.9152youxi.cn/gtsfygjixe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.cashguo.top/gtmibdtogl.html

[C02] 默认参数
来源：http://hz.jinyuanbaomall.cn/gtksdtbjvz.html

Py:   def greet(name="World"): return name
来源：http://hz.sweek.top/gtajtkmhqy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydzc1.top/gtbrsgmrtk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.feifeiyinyue.top/gtlsrcxwsd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtwzbvpkvh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.aibaodan.cn/gtmbzswswr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shanyushiyangkeji.top/gtuwohsnvm.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhaomingkeji.xyz/gtimybuiny.html


<!-- 参考信息 -->