代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://hz.hongshengwenyu.top/gtqzxnscbf.html

[A11] 条件表达式（三元）
来源：http://hz.daria6918.cn/gtkgyrlcpw.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shanyushiyangkeji.top/gtjiajyptm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.zhaomingkeji.xyz/gthbpdpgkn.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.tian-w.cn/gtmivxvube.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gtoafrkcny.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.gaohongyu789.top/gtknuqsmxp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.mhx1999.top/gthxosegak.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.wangdashe.top/gthogmfqem.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtfskuvecb.html

[A12] 字符串插值 / 格式化
来源：http://hz.havefunace.top/gtzfnyrddr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yuxming.cn/gtsqkamroc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.c1oappe.top/gtlwurxtot.html

JS:   `Hello, ${name}!`
来源：http://hz.birdmap.top/gtgdngnsaf.html

TS:   `Hello, ${name}!`
来源：http://hz.smart0.xyz/gtjflvympg.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.52xcode.cn/gtggmtgito.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zhengqikj.top/gtdoaptjpi.html

Ruby: "Hello, #{name}!"
来源：http://hz.xingfuxueyuan.xyz/gtxevjilmc.html

C#:   $"Hello, {name}!"
来源：http://hz.shuidangran.top/gtznladczr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.zhiwuduotai.top/gtcvnksqmz.html

Py:   "第一行\n第二行"
来源：http://hz.birdmap.top/gtkjbhhlid.html

PHP:  "第一行\n第二行"
来源：http://hz.wangdashe.top/gtrvtxwiej.html

JS:   "第一行\n第二行"
来源：http://hz.yueranfly.top/gtpdwbqixk.html

TS:   "第一行\n第二行"
来源：http://hz.gogol.net.cn/gtfjxobscx.html

Java: "第一行\n第二行"
来源：http://hz.nwbrower.top/gtvhffxles.html

Go:   "第一行\n第二行"
来源：http://hz.9152youxi.cn/gtptevbupv.html

Ruby: "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtaledkbrl.html

C#:   "第一行\n第二行"
来源：http://hz.aizwys.cn/gtyughbnnq.html

[A14] 注释写法
来源：http://hz.cdnleiting.top/gtzkvssltz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zdqjudy.top/gttqavvbxu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.smart0.xyz/gtqxzqyhpa.html

JS:   // 单行；/* 多行 */
来源：http://hz.gzhubu.top/gtlfugeggy.html

TS:   // 单行；/* 多行 */
来源：http://hz.hammf.cn/gttrerczxa.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.guowangkeji.top/gtgetlmbzp.html

Go:   // 单行；/* 多行 */
来源：http://hz.jinyuanbaomall.cn/gtarlnjczn.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jinyuanbaomall.cn/gttyjjbnqg.html

C#:   // 单行；/* 多行 */
来源：http://hz.ydzc1.top/gtqsmbnein.html

[A15] 空值判断与默认值
来源：http://hz.xylfe.cn/gtjainhwab.html

Py:   value = data or "默认值"
来源：http://hz.yvedp.cn/gtvsypgnxj.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.ywan-chungtsiang.top/gtjiqrunyk.html

JS:   const value = data ?? "默认值";
来源：http://hz.meibo888.top/gtnpqprzka.html

TS:   const value = data ?? "默认值";
来源：http://hz.ydzc1.top/gtzppwjath.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.feifeiyinyue.top/gtzibxnmab.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.jqgufenzy.top/gtnxjdcckf.html

Ruby: value = data || "默认值"
来源：http://hz.birdmap.top/gtairmldup.html

C#:   var value = data ?? "默认值";
来源：http://hz.ydjk.org.cn/gtcsrrbjni.html

[A16] 真假值判断规则
来源：http://hz.meibo888.top/gteaucikpu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.dashuyun.cn/gtnrbupgdw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jinqigfzy.top/gtuvoxcgon.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yanxiufei.cn/gtlvraqqrs.html

TS:   if (!x) {}
来源：http://hz.jlsjyb.cn/gtlnxaqwkc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.birdmap.top/gthqjrfpmy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.gaohongyu789.top/gtjvwvaicy.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.chenjidiqi.icu/gtqxzyzqbh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jlsjyb.cn/gtijnixffa.html

[A17] 位运算
来源：http://hz.c1oappe.top/gtdulljrry.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.smart0.xyz/gtpcuxwfxr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.sufxvd.cn/gtlcbnqoea.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhaomingkeji.xyz/gtkqutpmap.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.vqdsnc.cn/gthiuvmigh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtvfkmogzm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtmyoethkz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xylfe.cn/gtpopaatrf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhijiandao.cn/gtnxvxixfu.html

[A18] 字符与 ASCII 码互转
来源：http://hz.yonumen.top/gtseozcimz.html

Py:   ord("A"); chr(65)
来源：http://hz.sufxvd.cn/gtyjmcvkuc.html

PHP:  ord("A"); chr(65)
来源：http://hz.jqgufenzy.top/gtsbulbrmu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jqgufenzy.top/gtknhjxkuy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yueranfly.top/gtjwteoaas.html

Java: (int) 'A'; (char) 65
来源：http://hz.cdnleiting.top/gtdqseekok.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.zycfv.cn/gtpggwhteo.html

Ruby: "A".ord; 65.chr
来源：http://hz.xuetiantiany.cn/gtpddxoths.html

C#:   (int)'A'; (char)65
来源：http://hz.snrcjt.cn/gtqbeyystt.html

[A19] 交换两个变量
来源：http://hz.sweek.top/gtdebnimcv.html

Py:   a, b = b, a
来源：http://hz.jyoumei.cn/gtkhsxrcsg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.zhongyouzk.top/gtcfkaeowl.html

JS:   [a, b] = [b, a];
来源：http://hz.yangfankeji.com/gtxuceqwbj.html

TS:   [a, b] = [b, a];
来源：http://hz.quarkkingdee.top/gtgjbxghmk.html

Java: int t = a; a = b; b = t;
来源：http://hz.vqdsnc.cn/gtaajnvqxo.html

Go:   a, b = b, a
来源：http://hz.316326.xyz/gtcmencodw.html

Ruby: a, b = b, a
来源：http://hz.tian-w.cn/gtkpgllkhf.html

C#:   (a, b) = (b, a);
来源：http://hz.ehwqpu.com/gtdcoacquo.html

[A20] 读取标准输入
来源：http://hz.jinghuilouyu.cn/gtevyaergi.html

Py:   name = input("请输入：")
来源：http://hz.jyoumei.cn/gtddethhum.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.xingfuxueyuan.xyz/gtovhyxaqj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.zhongyouzk.top/gtjvsqxdou.html

TS:   // Node.js：readline 模块
来源：http://hz.zhongyouzk.top/gtontvwmtf.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.cashguo.top/gtruyjlzuw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ydzc1.top/gtledxjsvu.html

Ruby: gets.chomp
来源：http://hz.hnqzz.top/gtgipcrljr.html

C#:   Console.ReadLine();
来源：http://hz.52xcode.cn/gtpqkhzdzu.html

[A21] 保留指定小数位输出
来源：http://hz.daria6918.cn/gtbeonlxti.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ehwqpu.com/gtzeziakbx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ivvv.top/gtclorpcqr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.pycfn.com/gtfboxribq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.vqdsnc.cn/gtajxyovki.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtvxfjqujd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.c1oappe.top/gthpourqqh.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.c1oappe.top/gtxzpnjwhx.html

C#:   3.14159.ToString("F2")
来源：http://hz.ybcxt.top/gtchgdflgu.html

[A22] 获取字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtsbefumlq.html

Py:   len(s)
来源：http://hz.iojbl.cn/gtntxeslio.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.hfpthk.cn/gtyaaoyxfm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhengqikj.top/gttwigksjp.html

TS:   s.length
来源：http://hz.dashuyun.cn/gtywsbvkhi.html

Java: s.length()
来源：http://hz.zdqjudy.top/gtcptmdtmm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.xuanzx.com/gtdympuhot.html

Ruby: s.length
来源：http://hz.nanxuanxn.top/gtcaxhyfss.html

C#:   s.Length
来源：http://hz.cucudq.cn/gttblovrsi.html

[A23] 大小写转换
来源：http://hz.jinghuilouyu.cn/gtlcdzhrbl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.feifeiyinyue.top/gtxcgvbanz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cashguo.top/gtrgmhpbbv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xinyue.icu/gtuzgdgtmc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.feifeiyinyue.top/gtnxdstqgb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yuxming.cn/gtemynrdtw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.vqdsnc.cn/gthkurzmjk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ydzc1.top/gtdzntkmee.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.0kj1m.cn/gtrbcukgjl.html

[A24] 去除首尾空白
来源：http://hz.chenzaomai.com/gtlxzdzetw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shuidangran.top/gtwufwfqih.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.jqgufenzy.top/gtlhjhqmnl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jianghu66.top/gtktebntwa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhixingplan.top/gtjlobaqng.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ywan-chungtsiang.top/gtyppfzkhv.html

Go:   strings.TrimSpace(s)
来源：http://hz.zhaomingkeji.xyz/gtnxhlkmch.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.0kj1m.cn/gtjjzyaqju.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yj20258888.top/gtruawxxpd.html

[A25] 字符串比较
来源：http://hz.tianlin.xyz/gtuoinicrt.html

Py:   s1 == s2; s1 != s2
来源：http://hz.xylfe.cn/gtgoxhtsmb.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jiagoushi.top/gtxvpxdadx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.vqdsnc.cn/gtymafbhnf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgfzy.top/gtskfpphbf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ivvv.top/gtmnwlpoax.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jyoumei.cn/gttyosbrbw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ybcxt.top/gtwvojsqtn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yj20258.top/gtozdwlczc.html

[A26] 类型转换总览
来源：http://hz.xziqi.cn/gtttupwlvr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.guowangkeji.top/gteofbctbq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.wangdashe.top/gthlcnrblk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhongyouzk.top/gtfwtylole.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xuetiantiany.cn/gtnwqftnij.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cashguo.top/gtyyqqyrbc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhengqikj.top/gtyupwclgo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shangyingyoupin.top/gtneaetpix.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.52xcode.cn/gtosasvjbw.html

================================================================================
来源：http://hz.bjfxy.top/gtwifbkfcz.html

B. 流程控制
来源：http://hz.ehwqpu.com/gtxtxovaek.html

================================================================================
来源：http://hz.sufxvd.cn/gtwogfevru.html

[B01] 条件判断 if / else
来源：http://hz.shuidangran.top/gtjxtbsjzo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.mhx1999.top/gtgxbmavuv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hysaishi.cn/gtqrajbhro.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.pengpengdd.cyou/gtsfxgfbcb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.feifeiyinyue.top/gtsjnhxasc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zycfv.cn/gtrgsmvdmf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.vqdsnc.cn/gtqcvopxns.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gogol.net.cn/gtjjggwjhz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.quarkkingdee.top/gtnaprixzf.html

[B02] 多分支 else if / elif
来源：http://hz.sweek.top/gtsixtucbn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hywenlv.cn/gtsjrfjvop.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.316326.xyz/gthgzqtvdt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gtooppchbm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhaomingkeji.xyz/gtwbgvxruh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtqislvblj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gzhubu.top/gtdxwnhhmc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.meibo888.top/gtawhfiqnp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shanyushiyangtech.top/gtxdbwsxpl.html

[B03] switch / match / case
来源：http://hz.daxiang520.top/gtbeokchwr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jlsjyb.cn/gtdmqeojpn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yj20258888.top/gtamlspghs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jqgfzy.top/gtxnzpacgn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tian-w.cn/gttfiptesd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.0kj1m.cn/gtqgjxvvma.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.shuidangran.top/gtxfpsnwwx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hongshengwenyu.top/gtfvbyrscq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.svipenyu.cn/gtasegqamh.html

[B04] for 计数循环
来源：http://hz.zhengqikj.top/gtantndxdx.html

Py:   for i in range(10): print(i)
来源：http://hz.iojbl.cn/gtyritvklb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.jqgufenzy.top/gtufxjsset.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ehwqpu.com/gtyradlwxg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hfpthk.cn/gtukjccqyi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cqqwz.cn/gtqnzwbewb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.nwbrower.top/gttpioslgk.html

Ruby: 10.times { |i| puts i }
来源：http://hz.wangdashe.top/gtmcmxegpr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ywan-chungtsiang.top/gtskmpxkhj.html

[B05] 遍历数组 / 列表
来源：http://hz.birdmap.top/gtcqoitwzu.html

Py:   for item in arr: print(item)
来源：http://hz.xinyue.icu/gtgfygeohg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.zhixingplan.top/gtyljbcurc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.andypj.xyz/gtwrywguwx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenzaomai.com/gtucoldumt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.xziqi.cn/gtigweuofi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.gogol.net.cn/gtmrxyirao.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tian-w.cn/gteqxhzikd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ydzc1.top/gtxzuiuyzv.html

[B06] 遍历字典 / 对象
来源：http://hz.sweek.top/gtyetmsebm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.zhengqikj.top/gtgwswlpjo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yueranfly.top/gtthxhtvmr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cashguo.top/gtobvexhbg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.haohaochexian.top/gtmmleowue.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.nanxuanxn.top/gtgdzbouyo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.snrcjt.cn/gtjummxmsd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zycfv.cn/gtsgoicbgs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sweek.top/gtzykwvfva.html

[B07] while 循环
来源：http://hz.chenzaomai.com/gtwrgiplwu.html

Py:   while i < 10: i += 1
来源：http://hz.9152youxi.cn/gtgiweuobx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.tianlin.xyz/gtmlxnfhnx.html

JS:   while (i < 10) { i++; }
来源：http://hz.chenlongwang.top/gtmylbtscx.html

TS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtjztkstqm.html

Java: while (i < 10) { i++; }
来源：http://hz.mhx1999.top/gthmhwxeek.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.iojbl.cn/gtxjlzwscq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhengqikj.top/gtpysbyoza.html

C#:   while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtxdfldgby.html

[B08] do-while（至少执行一次）
来源：http://hz.ybcxt.top/gticfhawdk.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhongyouzk.top/gtwuxzmbbu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.zhixingplan.top/gttjvhffoe.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtxjvnjhfz.html

TS:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtmunykrkx.html

Java: do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtvjgalnby.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yueranfly.top/gtrtxmxwfb.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.nwbrower.top/gtcpaabswu.html

C#:   do { i++; } while (i < 10);
来源：http://hz.tian-w.cn/gtfkrrydwt.html

[B09] break 与 continue
来源：http://hz.cashguo.top/gtybtthdlg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.9152youxi.cn/gtesspbecd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.aibaodan.cn/gtkzjoqtoc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gotoacloud.top/gtiwzmfqru.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtyimzmpff.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtowlvahgz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.snrcjt.cn/gtymawqmsa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.jyoumei.cn/gtkcebrcol.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtjfvpbnnq.html

[B10] 遍历同时拿索引
来源：http://hz.hfpthk.cn/gtkpuinfcy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.nwbrower.top/gtvqzorpme.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hywenlv.cn/gtmopycoxu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtlwqomupi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jianghu66.top/gtamskabwz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.bjfxy.top/gtixphzzhl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.svipenyu.cn/gtmkzhoowp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.xingfuxueyuan.xyz/gtyuetyeor.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.cucudq.cn/gtottnkthc.html

[B11] 生成数字序列 / 区间
来源：http://hz.tianlin.xyz/gtfueqkeeb.html

Py:   list(range(0, 10, 2))
来源：http://hz.tanke756.top/gtzqfqdeje.html

PHP:  range(0, 10, 2);
来源：http://hz.cashguo.top/gtogydjsjm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hongshengwenyu.top/gtfzcgzwsk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtgcewqkvh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cucudq.cn/gtacxjyxnn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jinqigufen.top/gtyfuzmyvg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.smart0.xyz/gtasbjdwso.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gotoacloud.top/gtasrdgopw.html

[B12] 跳出多层循环
来源：http://hz.hywenlv.cn/gtywnorzcw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhiwuduotai.top/gtyixfijnl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenlongwang.top/gtutzppnnj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtuqsdrxjk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gtxhyapxyj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangdashe.top/gtbarziipu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.sysykeji.top/gtmdrezeir.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ybcxt.top/gtvgznihqk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinyuanbaomall.cn/gtxbebvfrb.html

[B13] 判断是否为数字
来源：http://hz.cucudq.cn/gtahcmbagt.html

Py:   isinstance(x, (int, float))
来源：http://hz.sufxvd.cn/gtfbpjufmq.html

PHP:  is_numeric($x)
来源：http://hz.tianlin.xyz/gtzvzurbkm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cdnleiting.top/gtgrqszrga.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.snrcjt.cn/gtepgkeppp.html

Java: x instanceof Number
来源：http://hz.aizwys.cn/gtiolepvhh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hnxiangtu.top/gtcvfmvstk.html

Ruby: x.is_a?(Numeric)
来源：http://hz.svipenyu.cn/gtxbbzlquw.html

C#:   x is int or double or decimal
来源：http://hz.shuidangran.top/gtdjnmiegi.html

[B14] 判断值是否在集合内
来源：http://hz.hywenlv.cn/gttcvmnyae.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.kuanghao11.cn/gtwqcadeuv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhixingplan.top/gtxuhpfxmc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.daxiang520.top/gtusbijsjw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtaartudct.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.wangshuangyany.cn/gtjtyhuddk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.316326.xyz/gtgxnwcggi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cheryme.top/gtoeqghwgq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.haohaochexian.top/gtjwpjdwgq.html

[B15] 布尔运算与取反
来源：http://hz.chenjidiqi.icu/gtbitlrhpk.html

Py:   a and b or not c
来源：http://hz.ydjk.org.cn/gtidpwvyef.html

PHP:  $a && $b || !$c
来源：http://hz.yj20258.top/gtccncyegu.html

JS:   a && b || !c
来源：http://hz.jiagoushi.top/gtsjwhwenb.html

TS:   a && b || !c
来源：http://hz.zhoulong.xyz/gttazhryct.html

Java: a && b || !c
来源：http://hz.yj20258888.top/gtjxhtjydk.html

Go:   a && b || !c
来源：http://hz.zhengqikj.top/gtkhrljvmf.html

Ruby: a && b || !c
来源：http://hz.gotoacloud.top/gthcuospdp.html

C#:   a && b || !c
来源：http://hz.ywan-chungtsiang.top/gtqjjxasfc.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gtfpbdaqhw.html

Py:   if not data: return
来源：http://hz.andypj.xyz/gtrqbkywik.html

PHP:  if (!$data) { return; }
来源：http://hz.xylfe.cn/gtthwhbruv.html

JS:   if (!data) return;
来源：http://hz.zycfv.cn/gtsqtgrpnr.html

TS:   if (!data) return;
来源：http://hz.haohaochexian.top/gtyqbhzdxh.html

Java: if (data == null) return;
来源：http://hz.yonumen.top/gteljifrjk.html

Go:   if data == nil { return }
来源：http://hz.jinghuilouyu.cn/gtqwzmztvi.html

Ruby: return if data.nil?
来源：http://hz.ppjwa.cn/gtynhfeqqr.html

C#:   if (data == null) return;
来源：http://hz.havefunace.top/gtdmcekold.html

================================================================================
来源：http://hz.redwolf501.top/gtickiuhsa.html

C. 函数与作用域
来源：http://hz.yuxming.cn/gturposlgk.html

================================================================================
来源：http://hz.shzxlz.cn/gtpxqblqhx.html

[C01] 定义函数
来源：http://hz.wangdashe.top/gtqofflpop.html

Py:   def add(a, b): return a + b
来源：http://hz.daria6918.cn/gtbswjfkcw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gthkpzbejw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj20258888.top/gtpcmnirdq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtmdruxnzk.html


<!-- 参考信息 -->