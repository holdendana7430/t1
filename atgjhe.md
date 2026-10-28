代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yvedp.cn/gtaptfainn.html

JS:   `Hello, ${name}!`
来源：http://hz.tianlin.xyz/gtvlxpukuw.html

TS:   `Hello, ${name}!`
来源：http://hz.zhoulong.xyz/gtkdhhkpwg.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.xziqi.cn/gtuxthranb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.sysykeji.top/gtfzcznfym.html

Ruby: "Hello, #{name}!"
来源：http://hz.sufxvd.cn/gtqmfckzbe.html

C#:   $"Hello, {name}!"
来源：http://hz.tian-w.cn/gtctiophoo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.fengsongda.top/gtdsjlocwu.html

Py:   "第一行\n第二行"
来源：http://hz.zhijiandao.cn/gtskrcipvy.html

PHP:  "第一行\n第二行"
来源：http://hz.aizwys.cn/gtrgoaqrfg.html

JS:   "第一行\n第二行"
来源：http://hz.smart0.xyz/gtnufnzsnl.html

TS:   "第一行\n第二行"
来源：http://hz.316326.xyz/gtnnexitvd.html

Java: "第一行\n第二行"
来源：http://hz.tanke756.top/gtmvhkeeir.html

Go:   "第一行\n第二行"
来源：http://hz.gzhubu.top/gtnxvdslll.html

Ruby: "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtkfhrkybj.html

C#:   "第一行\n第二行"
来源：http://hz.havefunace.top/gtvipwtvfq.html

[A14] 注释写法
来源：http://hz.yj202588.top/gtwdqadiiv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.nanxinkj.top/gtftunkmvm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.yueranfly.top/gtpwulgreg.html

JS:   // 单行；/* 多行 */
来源：http://hz.aibaodan.cn/gtccmzuprv.html

TS:   // 单行；/* 多行 */
来源：http://hz.sxryk.cn/gtnbxbmfhc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.sufxvd.cn/gtoazxlkxa.html

Go:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtdlgzadwr.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hammf.cn/gttrhkkmsm.html

C#:   // 单行；/* 多行 */
来源：http://hz.gogol.net.cn/gtapgnvffe.html

[A15] 空值判断与默认值
来源：http://hz.ivvv.top/gtnwgbqrps.html

Py:   value = data or "默认值"
来源：http://hz.zycfv.cn/gtmolaqgji.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.snrcjt.cn/gtkptplfuz.html

JS:   const value = data ?? "默认值";
来源：http://hz.wangdashe.top/gtgaaqrrig.html

TS:   const value = data ?? "默认值";
来源：http://hz.cucudq.cn/gtjbvjjeaf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.tianlin.xyz/gtwfyyypst.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.chenjidiqi.icu/gtmcrmlrja.html

Ruby: value = data || "默认值"
来源：http://hz.jqgfzy.top/gtiujvthii.html

C#:   var value = data ?? "默认值";
来源：http://hz.hnxiangtu.top/gtpkvvjuxw.html

[A16] 真假值判断规则
来源：http://hz.smart0.xyz/gtcsuckzsk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.jqgfzy.top/gthpohwnzg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.quarkkingdee.top/gtzoylncdn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jqgufenzy.top/gtjnjquysy.html

TS:   if (!x) {}
来源：http://hz.jyoumei.cn/gthtoffjab.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.tian-w.cn/gthnyuzkzo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.kuanghao11.cn/gtffflanqa.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.hongshengwenyu.top/gtvedgberh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.aizwys.cn/gtiokxfron.html

[A17] 位运算
来源：http://hz.aibaodan.cn/gteeimrkmh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xylfe.cn/gtfazziwku.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.shuidangran.top/gtaxnenvjt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yanxiufei.cn/gttuqkrvub.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtrwsqbtay.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtwcghdizm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.haohaochexian.top/gtvuuwswtn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.havefunace.top/gteowvpxsm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gtxjwqfwzq.html

[A18] 字符与 ASCII 码互转
来源：http://hz.cucudq.cn/gtbbyjswzc.html

Py:   ord("A"); chr(65)
来源：http://hz.pycfn.com/gtydrljucd.html

PHP:  ord("A"); chr(65)
来源：http://hz.mhx1999.top/gtfzrjnvcv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.chenzaomai.com/gtyplhyovl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yvedp.cn/gtcdgphswp.html

Java: (int) 'A'; (char) 65
来源：http://hz.haohaochexian.top/gtuypcttaz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.shzxlz.cn/gtardaklnb.html

Ruby: "A".ord; 65.chr
来源：http://hz.jqgfzy.top/gthadwahjf.html

C#:   (int)'A'; (char)65
来源：http://hz.zhongyouzk.top/gttwytxqra.html

[A19] 交换两个变量
来源：http://hz.gzhubu.top/gtriddfafn.html

Py:   a, b = b, a
来源：http://hz.jinghuilouyu.cn/gtpdwjvsnv.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shangyingyoupin.top/gtzmaxdicu.html

JS:   [a, b] = [b, a];
来源：http://hz.hysaishi.cn/gtvocmctdt.html

TS:   [a, b] = [b, a];
来源：http://hz.zhijiandao.cn/gtemrqdpvw.html

Java: int t = a; a = b; b = t;
来源：http://hz.cqqwz.cn/gtdpraezjg.html

Go:   a, b = b, a
来源：http://hz.xuanzx.com/gtxwqdveng.html

Ruby: a, b = b, a
来源：http://hz.ybcxt.top/gtoxutzokl.html

C#:   (a, b) = (b, a);
来源：http://hz.nwbrower.top/gtmhxxovxp.html

[A20] 读取标准输入
来源：http://hz.kuanghao11.cn/gtkefdrnth.html

Py:   name = input("请输入：")
来源：http://hz.dashuyun.cn/gtgjhrspqu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.quarkkingdee.top/gthzzlxjiw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.nanxinkj.top/gtgjmrrztv.html

TS:   // Node.js：readline 模块
来源：http://hz.yuxming.cn/gtngdhyrgu.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.feifeiyinyue.top/gtjfuibvlz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.guannengcc.top/gtuxjetesv.html

Ruby: gets.chomp
来源：http://hz.bjfxy.top/gtfxjlxvit.html

C#:   Console.ReadLine();
来源：http://hz.yangfankeji.com/gtaeaduvmz.html

[A21] 保留指定小数位输出
来源：http://hz.chenzaomai.com/gtxhumoyju.html

Py:   f"{3.14159:.2f}"
来源：http://hz.c1oappe.top/gtvlcfjdpr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.cqqwz.cn/gtufbeghyr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sysykeji.top/gtyexalrxy.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yangfankeji.com/gtvgsasspi.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jinghuilouyu.cn/gtsgcyczqk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtjnxbaqea.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtdksmqidr.html

C#:   3.14159.ToString("F2")
来源：http://hz.xingfuxueyuan.xyz/gtsmbusvqn.html

[A22] 获取字符串长度
来源：http://hz.gzhubu.top/gtjufzlcjk.html

Py:   len(s)
来源：http://hz.chenjidiqi.icu/gtrxtunrko.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.tanke756.top/gttkxovoqz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.iojbl.cn/gtwafnlrsy.html

TS:   s.length
来源：http://hz.ivvv.top/gtkztuorgx.html

Java: s.length()
来源：http://hz.dashuyun.cn/gteatakayj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.ywan-chungtsiang.top/gtvpcufiqb.html

Ruby: s.length
来源：http://hz.nwbrower.top/gtamzjjzzk.html

C#:   s.Length
来源：http://hz.gotoacloud.top/gtxolyzyzu.html

[A23] 大小写转换
来源：http://hz.zhiwuduotai.top/gtycnxnzpi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ppjwa.cn/gtknzyerdv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.hywenlv.cn/gtrmupqjtc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.iojbl.cn/gtccuhfcqr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.nanxuanxn.top/gtrguxpglt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhoulong.xyz/gtiicmovzp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.zdqjudy.top/gtshhrolqs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinghuilouyu.cn/gtjchlppoo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jinqigufen.top/gtguzmdcea.html

[A24] 去除首尾空白
来源：http://hz.sweek.top/gtxrkccqtd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.52xcode.cn/gtfuaduamo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.shanyushiyangtech.top/gtfmrajhdl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhixingplan.top/gtkwmvkpic.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.haohaochexian.top/gtisxpacvk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ywan-chungtsiang.top/gtgtnjqpyp.html

Go:   strings.TrimSpace(s)
来源：http://hz.gogol.net.cn/gtnvdhhxrb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.9152youxi.cn/gtxocfuqtp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.guowangkeji.top/gtbeslggis.html

[A25] 字符串比较
来源：http://hz.shuidangran.top/gtjnvekxfy.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jyoumei.cn/gtmzwbnaka.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.wangdashe.top/gtvehmahoo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.cheryme.top/gteubksyzg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jianghu66.top/gtrrfchxyj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.havefunace.top/gtbjvdjhah.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.gzhubu.top/gtfbosjbtm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ywan-chungtsiang.top/gtelpxkdvb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.hammf.cn/gtyzerqlnu.html

[A26] 类型转换总览
来源：http://hz.zycfv.cn/gtgmxbolld.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.9152youxi.cn/gtswqcsjwl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.sxryk.cn/gtmgxqgnwe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhiwuduotai.top/gtifsmliga.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cdnleiting.top/gtcxgphbyb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhiwuduotai.top/gtclopdwup.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenzaomai.com/gtublmzsod.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shangyingyoupin.top/gttwqcurdr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.aizwys.cn/gtccaaksks.html

================================================================================
来源：http://hz.hnxiangtu.top/gtirquvjta.html

B. 流程控制
来源：http://hz.zhengqikj.top/gtjkoqxpiv.html

================================================================================
来源：http://hz.havefunace.top/gttgfpuuru.html

[B01] 条件判断 if / else
来源：http://hz.pycfn.com/gtxbwnhvvi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.aibaodan.cn/gthwkeegph.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yj20258.top/gtjuksewyw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.cashguo.top/gtgkammhip.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtqhlwtutg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtgpbeqbll.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhongyouzk.top/gtlmhodyiw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yuanzhike.top/gtynggezzw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtpnwtujys.html

[B02] 多分支 else if / elif
来源：http://hz.hfpthk.cn/gtepecbkcv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.fengsongda.top/gtepiowvwu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.hammf.cn/gtqzhgoawm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gtzhxzsybg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aibaodan.cn/gtyxtbohxc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtyfdjedhw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jinyuanbaomall.cn/gtptlewtqj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhongyouzk.top/gteggtnnid.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yuxming.cn/gtqlkeswyb.html

[B03] switch / match / case
来源：http://hz.feifeiyinyue.top/gthszrsfku.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yangfankeji.com/gtvazxtkri.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.hywenlv.cn/gtyiieplgg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cdnleiting.top/gtoipqtusi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtholmnake.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yj202588.top/gtspewpwiy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jinyuanbaomall.cn/gtaaoqsxiw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.0kj1m.cn/gtivypjnbz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhoulong.xyz/gtciclvyhs.html

[B04] for 计数循环
来源：http://hz.hywenlv.cn/gtdhxksdka.html

Py:   for i in range(10): print(i)
来源：http://hz.pengpengdd.cyou/gthlciqwwa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cheryme.top/gtexckarbz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ivvv.top/gtazmbdjvp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yangfankeji.com/gtywokecpe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hfpthk.cn/gtgtftvbgb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jlsjyb.cn/gtpuvlofzu.html

Ruby: 10.times { |i| puts i }
来源：http://hz.chenzaomai.com/gtenzgcjwb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.daxiang520.top/gtzxxbqeew.html

[B05] 遍历数组 / 列表
来源：http://hz.guannengcc.top/gtqjpwdeoc.html

Py:   for item in arr: print(item)
来源：http://hz.52xcode.cn/gtlqnzsddj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shanyushiyangkeji.top/gtedycgusi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhengqikj.top/gtrqxfnuap.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhixingplan.top/gtrnljgsrf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.dianchejie.cn/gthnmlizfo.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cashguo.top/gtsubjkmzu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.feifeiyinyue.top/gtfqvqipcn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shuidangran.top/gtyuxpjkkn.html

[B06] 遍历字典 / 对象
来源：http://hz.gotoacloud.top/gtufpcvktj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.kuanghao11.cn/gtrstihdib.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinghuilouyu.cn/gtkigqzkpv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.quarkkingdee.top/gtlpxnqpvy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ppjwa.cn/gtulyjdbno.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.tianlin.xyz/gtjtajubku.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.haohaochexian.top/gtebulgoel.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.gotoacloud.top/gtgxmfdnjt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.tanke756.top/gtblzbhjif.html

[B07] while 循环
来源：http://hz.meibo888.top/gtgxxgnndm.html

Py:   while i < 10: i += 1
来源：http://hz.c1oappe.top/gtzfifjkfx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhijiandao.cn/gttbzzzmub.html

JS:   while (i < 10) { i++; }
来源：http://hz.gzhubu.top/gtotnrfmfc.html

TS:   while (i < 10) { i++; }
来源：http://hz.smart0.xyz/gtbpkdanyt.html

Java: while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtqgpygzvr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.andypj.xyz/gtrznfmddm.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jqgufenzy.top/gtmwjvjtsv.html

C#:   while (i < 10) { i++; }
来源：http://hz.xylfe.cn/gtgrkneglq.html

[B08] do-while（至少执行一次）
来源：http://hz.xinyue.icu/gtvpnipadr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinghuilouyu.cn/gtnnaiwzjt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hysaishi.cn/gtvsdasqgj.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gttbzhcaqv.html

TS:   do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtxvocecll.html

Java: do { i++; } while (i < 10);
来源：http://hz.wangshuangyany.cn/gtmwxktuax.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.tanke756.top/gtvhfcpbnq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.yanxiufei.cn/gtyqhvthcs.html

C#:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtflrsmbcy.html

[B09] break 与 continue
来源：http://hz.hfpthk.cn/gtdamwxcwo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhijiandao.cn/gtigpzxakn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtveicwinr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtqclwfquh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shuidangran.top/gtwhmhojsx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtmvvweucw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hysaishi.cn/gtxohnsgzg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shanyushiyangkeji.top/gtpneuwfnn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.9152youxi.cn/gtqfqxzqug.html

[B10] 遍历同时拿索引
来源：http://hz.hfpthk.cn/gttcsxlxob.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.haohaochexian.top/gtxztljznc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xylfe.cn/gthoaklzzc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ydzc1.top/gthkdeccdn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.yuanzhike.top/gtrxtsphrf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigufen.top/gtsckybuzx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.52xcode.cn/gtnprtxdby.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.guowangkeji.top/gthplyyxlg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.nanxuanxn.top/gtilojhuhb.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhongyouzk.top/gtbliliqqw.html

Py:   list(range(0, 10, 2))
来源：http://hz.kuanghao11.cn/gtwvbnbbnc.html

PHP:  range(0, 10, 2);
来源：http://hz.aibaodan.cn/gtgahwixzw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tian-w.cn/gtjjkiztjw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtoggfdptv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.fengsongda.top/gtiqkxnqmn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigfzy.top/gtfwxkbksx.html

Ruby: (0...10).step(2).to_a
来源：http://hz.0kj1m.cn/gtmxdjubpo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hammf.cn/gtrseyahjj.html

[B12] 跳出多层循环
来源：http://hz.jianghu66.top/gtwjfwhjgs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yj202588.top/gtqayaenyt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.guowangkeji.top/gtjrghgmnu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnqzz.top/gttbbnhuir.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuanzx.com/gtpgtwiiwr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtwnmubrjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.haohaochexian.top/gtcyjmxmui.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shuidangran.top/gtkabvmjsi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.quarkkingdee.top/gtbmbfclca.html

[B13] 判断是否为数字
来源：http://hz.svipenyu.cn/gtjwrrlgqq.html

Py:   isinstance(x, (int, float))
来源：http://hz.pengpengdd.cyou/gtypxafdhg.html

PHP:  is_numeric($x)
来源：http://hz.52xcode.cn/gtjflbicwt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yangfankeji.com/gtmpvdiudr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yanxiufei.cn/gtakdugfwu.html

Java: x instanceof Number
来源：http://hz.zhongyouzk.top/gtpcrrxokr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ybcxt.top/gtdukhujco.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hnqzz.top/gtlxxlttpl.html

C#:   x is int or double or decimal
来源：http://hz.dashuyun.cn/gttubzqnuk.html

[B14] 判断值是否在集合内
来源：http://hz.tianlin.xyz/gtpuvuiksf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tian-w.cn/gtvqgkexqa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ybcxt.top/gtnshznlmd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtvkfxtfnj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.sufxvd.cn/gtccgrfhqk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jyoumei.cn/gtvptoudms.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.chenjidiqi.icu/gttlzxplxk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.iojbl.cn/gtmtmyvclm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tian-w.cn/gtirfpbwlv.html

[B15] 布尔运算与取反
来源：http://hz.hysaishi.cn/gtbybeuoyn.html

Py:   a and b or not c
来源：http://hz.sweek.top/gtmfjkxuia.html

PHP:  $a && $b || !$c
来源：http://hz.zhongyouzk.top/gtoovwlpwq.html

JS:   a && b || !c
来源：http://hz.pycfn.com/gtvmfidrmv.html

TS:   a && b || !c
来源：http://hz.hywenlv.cn/gtnklwador.html

Java: a && b || !c
来源：http://hz.hongshengwenyu.top/gtkzfgqtfh.html

Go:   a && b || !c
来源：http://hz.xziqi.cn/gtvwszeacy.html

Ruby: a && b || !c
来源：http://hz.mhx1999.top/gtiqsvmsah.html

C#:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtmrhukato.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yueranfly.top/gtqlcouyfe.html

Py:   if not data: return
来源：http://hz.xziqi.cn/gtvyslydzh.html

PHP:  if (!$data) { return; }
来源：http://hz.jqgfzy.top/gtmsqijtjh.html

JS:   if (!data) return;
来源：http://hz.kuanghao11.cn/gtppgqtlxu.html

TS:   if (!data) return;
来源：http://hz.xingfuxueyuan.xyz/gtmdjreqdb.html

Java: if (data == null) return;
来源：http://hz.chenjidiqi.icu/gtvpouhkqy.html

Go:   if data == nil { return }
来源：http://hz.haohaochexian.top/gtccbkdxik.html

Ruby: return if data.nil?
来源：http://hz.aibaodan.cn/gtkbdvftrp.html

C#:   if (data == null) return;
来源：http://hz.pycfn.com/gthypmisop.html

================================================================================
来源：http://hz.yonumen.top/gtghgdikiu.html

C. 函数与作用域
来源：http://hz.jqgufenzy.top/gtszsnwsxw.html

================================================================================
来源：http://hz.smart0.xyz/gtcmuwbtup.html

[C01] 定义函数
来源：http://hz.zhijiandao.cn/gtauynpljp.html

Py:   def add(a, b): return a + b
来源：http://hz.redwolf501.top/gtgkdulzeq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gtectyujai.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtgrfbmonn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtynkyqgro.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtoiojixuf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenjidiqi.icu/gtfaakvivc.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sysykeji.top/gtxojuldns.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtzpfrdzdl.html

[C02] 默认参数
来源：http://hz.xuetiantiany.cn/gtaohudmtw.html

Py:   def greet(name="World"): return name
来源：http://hz.jqgufenzy.top/gtzlxnqqui.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.0kj1m.cn/gtuhpsenlr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.gogol.net.cn/gtnpbsgwod.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.andypj.xyz/gtusiushuo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuxming.cn/gtwxojorrd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cdnleiting.top/gtohzdiput.html

Ruby: def greet(name = "World") = name
来源：http://hz.zhengqikj.top/gteulynafb.html


<!-- 参考信息 -->