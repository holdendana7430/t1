代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.bjfxy.top/gtjaiejafd.html

Go:   "第一行\n第二行"
来源：http://hz.52xcode.cn/gtitenbfxs.html

Ruby: "第一行\n第二行"
来源：http://hz.hnqzz.top/gtoyufkket.html

C#:   "第一行\n第二行"
来源：http://hz.aibaodan.cn/gtsyebpmmn.html

[A14] 注释写法
来源：http://hz.redwolf501.top/gttiylbnnx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.zhixingplan.top/gtqijexjrl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.ywan-chungtsiang.top/gtbjtvyrdd.html

JS:   // 单行；/* 多行 */
来源：http://hz.xuetiantiany.cn/gtcovwmdio.html

TS:   // 单行；/* 多行 */
来源：http://hz.sufxvd.cn/gtznswntcn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhiwuduotai.top/gtfiayzeph.html

Go:   // 单行；/* 多行 */
来源：http://hz.fengsongda.top/gtzuoqjbkl.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.gotoacloud.top/gtliwbyggf.html

C#:   // 单行；/* 多行 */
来源：http://hz.jqgfzy.top/gtznoucgnr.html

[A15] 空值判断与默认值
来源：http://hz.hnxiangtu.top/gtzwfcaovd.html

Py:   value = data or "默认值"
来源：http://hz.kuanghao11.cn/gtqrfoizcr.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.yj20258888.top/gtvwvxvqxx.html

JS:   const value = data ?? "默认值";
来源：http://hz.havefunace.top/gtawtlyqiy.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhijiandao.cn/gtjzlftdfd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhengqikj.top/gtroaisyyz.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.zycfv.cn/gtlxojvusv.html

Ruby: value = data || "默认值"
来源：http://hz.yanxiufei.cn/gtfnnyxjea.html

C#:   var value = data ?? "默认值";
来源：http://hz.jianghu66.top/gtwwehpftg.html

[A16] 真假值判断规则
来源：http://hz.hywenlv.cn/gtedmzhjac.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.quarkkingdee.top/gtalivqrgb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jinyuanbaomall.cn/gtebjqctlf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.smart0.xyz/gtomjpaafu.html

TS:   if (!x) {}
来源：http://hz.hfpthk.cn/gtrdctskje.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.hysaishi.cn/gtkxowcguh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yvedp.cn/gtdwqzqipc.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.52xcode.cn/gttmbgrlll.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jianghu66.top/gtkoskwzol.html

[A17] 位运算
来源：http://hz.havefunace.top/gtvpeabnjw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cdnleiting.top/gtrfalavht.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.daxiang520.top/gtgonpfnhy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gtldqfhkuv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jlsjyb.cn/gtncezrewk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hnqzz.top/gtvhnukkue.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ydzc1.top/gtvpptpnhs.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hywenlv.cn/gtvotaojcj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gogol.net.cn/gtqplmecjq.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jinqigfzy.top/gtdqtsqawb.html

Py:   ord("A"); chr(65)
来源：http://hz.ppjwa.cn/gthdcrsmpb.html

PHP:  ord("A"); chr(65)
来源：http://hz.shzxlz.cn/gtcrltcckr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jianghu66.top/gtccjpkbft.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.fengsongda.top/gtzxdhrmvo.html

Java: (int) 'A'; (char) 65
来源：http://hz.shuidangran.top/gtmlmfjivg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.birdmap.top/gtwlohtrbw.html

Ruby: "A".ord; 65.chr
来源：http://hz.daxiang520.top/gtwrphtbuk.html

C#:   (int)'A'; (char)65
来源：http://hz.pengpengdd.cyou/gtqnseksvi.html

[A19] 交换两个变量
来源：http://hz.ybcxt.top/gtrmghxogl.html

Py:   a, b = b, a
来源：http://hz.gaohongyu789.top/gtklfgfyea.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.birdmap.top/gtlzlbphou.html

JS:   [a, b] = [b, a];
来源：http://hz.xinyue.icu/gtpiaitbhj.html

TS:   [a, b] = [b, a];
来源：http://hz.jinyuanbaomall.cn/gtzcfqszbh.html

Java: int t = a; a = b; b = t;
来源：http://hz.quarkkingdee.top/gtceewragj.html

Go:   a, b = b, a
来源：http://hz.chenjidiqi.icu/gtmxinctos.html

Ruby: a, b = b, a
来源：http://hz.sxryk.cn/gtifdsoblz.html

C#:   (a, b) = (b, a);
来源：http://hz.jianghu66.top/gtgssphatz.html

[A20] 读取标准输入
来源：http://hz.kuanghao11.cn/gtzsjggwcw.html

Py:   name = input("请输入：")
来源：http://hz.zhoulong.xyz/gtpucpttih.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.jyoumei.cn/gtpmuiuvke.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.jinqigfzy.top/gtndsfotil.html

TS:   // Node.js：readline 模块
来源：http://hz.svipenyu.cn/gtpyrrhdwf.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.aizwys.cn/gtypfmmgzj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zdqjudy.top/gthdbxyjzn.html

Ruby: gets.chomp
来源：http://hz.pycfn.com/gtcyvfchab.html

C#:   Console.ReadLine();
来源：http://hz.hywenlv.cn/gtwpjfrpew.html

[A21] 保留指定小数位输出
来源：http://hz.meibo888.top/gteendkrxg.html

Py:   f"{3.14159:.2f}"
来源：http://hz.52xcode.cn/gtwruyvsel.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gtmbcatvab.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ydzc1.top/gtvdwnqqeh.html

TS:   (3.14159).toFixed(2)
来源：http://hz.cucudq.cn/gthhuxrzbo.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.quarkkingdee.top/gtaeimzopc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.zhongyouzk.top/gtxuuxqjrl.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.gogol.net.cn/gtdjtcuqhf.html

C#:   3.14159.ToString("F2")
来源：http://hz.redwolf501.top/gtqhpvsgry.html

[A22] 获取字符串长度
来源：http://hz.tian-w.cn/gtkmpouxlo.html

Py:   len(s)
来源：http://hz.jiagoushi.top/gtdwaejiyc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.chenlongwang.top/gteddodowb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.kuanghao11.cn/gtestnlczb.html

TS:   s.length
来源：http://hz.yj20258.top/gtxmpnmrkg.html

Java: s.length()
来源：http://hz.daria6918.cn/gtwjqzdkuk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.sysykeji.top/gtrsaprmwd.html

Ruby: s.length
来源：http://hz.yj20258.top/gtitebnvmr.html

C#:   s.Length
来源：http://hz.bjfxy.top/gtvazbrlag.html

[A23] 大小写转换
来源：http://hz.chenzaomai.com/gtylifnahy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.xingfuxueyuan.xyz/gtzcajdnoj.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yuxming.cn/gtqupjqwat.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.316326.xyz/gtgmnnnmzg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jyoumei.cn/gtyxgmsvvu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.wangdashe.top/gtmldxygyb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.c1oappe.top/gtriacwghy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yuxming.cn/gtopjgeyol.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.feifeiyinyue.top/gtcnwcrgoo.html

[A24] 去除首尾空白
来源：http://hz.ydjk.org.cn/gtqpzhbaed.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.gotoacloud.top/gtphkptrhq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ydzc1.top/gtbfjbqgou.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.daxiang520.top/gtdmhgsrjc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tianlin.xyz/gtksvpvnvr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.dianchejie.cn/gtfwpxicsf.html

Go:   strings.TrimSpace(s)
来源：http://hz.yangfankeji.com/gtjqjudmxj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.chenlongwang.top/gtkwytkdef.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.kuanghao11.cn/gtzshwjmsy.html

[A25] 字符串比较
来源：http://hz.sysykeji.top/gtozvkiemw.html

Py:   s1 == s2; s1 != s2
来源：http://hz.aizwys.cn/gtdvvtaohr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.nanxinkj.top/gtequxqwzo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yvedp.cn/gtrolqarpu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xuetiantiany.cn/gtuidjjrdm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.shuidangran.top/gtetnlfabp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cashguo.top/gtbegcucep.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yuanzhike.top/gtfhbbxhyd.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.0kj1m.cn/gtkjojhakv.html

[A26] 类型转换总览
来源：http://hz.smart0.xyz/gtczsykayr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhiwuduotai.top/gthxsurikh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.sysykeji.top/gtburpbtcy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xuanzx.com/gtauhnlidw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.cdnleiting.top/gtemqjoyxi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yongpay.top/gtqtmcctgz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yuanzhike.top/gtnhqrztwv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yuxming.cn/gtwihmyudb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhengqikj.top/gtomxckasa.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtuqnpcvnn.html

B. 流程控制
来源：http://hz.sxryk.cn/gtujpoannd.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvohohmth.html

[B01] 条件判断 if / else
来源：http://hz.mhx1999.top/gtublbwcgn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.c1oappe.top/gtmyqmabxf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.bjfxy.top/gtcgtcanur.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.havefunace.top/gtiejexstv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gtjtyqbjgm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.haohaochexian.top/gtxnxmipyr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yuxming.cn/gtjxpszpxq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gzhubu.top/gtknzcuziu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtirgzcoqm.html

[B02] 多分支 else if / elif
来源：http://hz.yangfankeji.com/gtqgiwjqee.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.xingfuxueyuan.xyz/gtcnggxmns.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.svipenyu.cn/gttxdkeljq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigufen.top/gtwwgftkyo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.52xcode.cn/gtourcprqk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yueranfly.top/gtxseuhqzt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yj20258888.top/gtqigvufnu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ywan-chungtsiang.top/gtoneqpkdm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigfzy.top/gtxhdtpnwz.html

[B03] switch / match / case
来源：http://hz.sweek.top/gtmoghisfz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258888.top/gtsdlcbhzn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.daxiang520.top/gtdvepedjk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtjykilufs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hammf.cn/gtjrzlpgco.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hongshengwenyu.top/gtvsjfldnl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhaomingkeji.xyz/gtssezdonc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnxiangtu.top/gtsmapwiqw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.redwolf501.top/gtkanfnaig.html

[B04] for 计数循环
来源：http://hz.shuidangran.top/gtzercvdln.html

Py:   for i in range(10): print(i)
来源：http://hz.zhijiandao.cn/gtgfyemiym.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.52xcode.cn/gtgiayosts.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shzxlz.cn/gtiktsfxuj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuanzhike.top/gtzlmfuqdu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cheryme.top/gtnuytanwu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.zhoulong.xyz/gtcspxwyut.html

Ruby: 10.times { |i| puts i }
来源：http://hz.ydzc1.top/gtpvdhnkqv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.c1oappe.top/gtrjmfqjvv.html

[B05] 遍历数组 / 列表
来源：http://hz.yanxiufei.cn/gtgtwdwlxg.html

Py:   for item in arr: print(item)
来源：http://hz.ybcxt.top/gtrnhqgvpe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.dashuyun.cn/gtbgwrwsvo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.guowangkeji.top/gtqrlmprtk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinyuanbaomall.cn/gtyxlghqpi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.316326.xyz/gtewnvyszu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.chenzaomai.com/gtjozeuheh.html

Ruby: arr.each { |item| puts item }
来源：http://hz.daria6918.cn/gtukxppaei.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.fzhhl.top/gtpslfzwfj.html

[B06] 遍历字典 / 对象
来源：http://hz.xingfuxueyuan.xyz/gtvtideekr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.svipenyu.cn/gtpectwlwu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.meibo888.top/gtoztuvlih.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.nwbrower.top/gtfnxotpye.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhiwuduotai.top/gtsawcvodn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.daria6918.cn/gtdothagoz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.fengsongda.top/gteitwssaw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yangfankeji.com/gtvwrzqlgx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yj20258888.top/gtqpmssdfz.html

[B07] while 循环
来源：http://hz.gzhubu.top/gtizdzgexz.html

Py:   while i < 10: i += 1
来源：http://hz.ydjk.org.cn/gtpgxckget.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xuanzx.com/gtyhzmwsvz.html

JS:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtegpvwlzg.html

TS:   while (i < 10) { i++; }
来源：http://hz.yangfankeji.com/gtxwaxzlat.html

Java: while (i < 10) { i++; }
来源：http://hz.yonumen.top/gtwtgxssim.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhixingplan.top/gtegpngzot.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gthcynijgu.html

C#:   while (i < 10) { i++; }
来源：http://hz.nwbrower.top/gtuzmydzxl.html

[B08] do-while（至少执行一次）
来源：http://hz.ppjwa.cn/gtckzdllzx.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ivvv.top/gtndomobmu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.daxiang520.top/gtoqeswmle.html

JS:   do { i++; } while (i < 10);
来源：http://hz.andypj.xyz/gtgqppbctu.html

TS:   do { i++; } while (i < 10);
来源：http://hz.daxiang520.top/gtngllyjay.html

Java: do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtyjzzdaxk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hnqzz.top/gtygdjvulv.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenjidiqi.icu/gtfhradltk.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtukizcxmh.html

[B09] break 与 continue
来源：http://hz.ppjwa.cn/gtvulsuukm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.mhx1999.top/gtmndyrcuv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.redwolf501.top/gttlbzlpdn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.quarkkingdee.top/gtlrrauuuo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtxkcptwxv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtgxuslkjw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jinqigfzy.top/gtvifbzleh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.shanyushiyangtech.top/gtpepxediy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuanzx.com/gtgycpclxd.html

[B10] 遍历同时拿索引
来源：http://hz.dashuyun.cn/gtndiibsby.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shzxlz.cn/gtqiuzxmxz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtluxtdnul.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ehwqpu.com/gtnpdlmlrt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ehwqpu.com/gtnmkohjyf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.chenjidiqi.icu/gtekyvdjub.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhaomingkeji.xyz/gtkydchiwh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.fengsongda.top/gtwpufqsvf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhiwuduotai.top/gtclmtajms.html

[B11] 生成数字序列 / 区间
来源：http://hz.zdqjudy.top/gtgmthjefz.html

Py:   list(range(0, 10, 2))
来源：http://hz.haohaochexian.top/gtjkmwnaqw.html

PHP:  range(0, 10, 2);
来源：http://hz.jinqigufen.top/gtibihtdal.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtuaywmfty.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtzyaogzty.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.guowangkeji.top/gtjnrjetbm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.chenjidiqi.icu/gtkmmtppts.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yonumen.top/gtfwakswat.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yanxiufei.cn/gtmclxqueq.html

[B12] 跳出多层循环
来源：http://hz.wangshuangyany.cn/gtyfqhtfks.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.ppjwa.cn/gtzxiwleea.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sweek.top/gtmjyycqks.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ybcxt.top/gtwkrmvpjc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hnxiangtu.top/gtzxmibsnq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.smart0.xyz/gtlgzondia.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.wangshuangyany.cn/gthpzwprhu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gaohongyu789.top/gtbrgjittb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hfpthk.cn/gtcwsulxaj.html

[B13] 判断是否为数字
来源：http://hz.jinghuilouyu.cn/gtelbjnsqv.html

Py:   isinstance(x, (int, float))
来源：http://hz.yongpay.top/gtuxkvwjzi.html

PHP:  is_numeric($x)
来源：http://hz.chenjidiqi.icu/gtpoctwmau.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daria6918.cn/gtsvphkvye.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangshuangyany.cn/gtteolcpni.html

Java: x instanceof Number
来源：http://hz.cucudq.cn/gtduditjyx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.nanxinkj.top/gtcufnpshx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinqigfzy.top/gtiwukbrna.html

C#:   x is int or double or decimal
来源：http://hz.hnqzz.top/gtvjgazuia.html

[B14] 判断值是否在集合内
来源：http://hz.shzxlz.cn/gthzvdbwxo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xuanzx.com/gtvwwtrthm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj202588.top/gtmrmddqfl.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtpyimekzc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gtvebewypr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgfzy.top/gtdtthscde.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.c1oappe.top/gtawiywlwq.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xuetiantiany.cn/gtlgydxisj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.gotoacloud.top/gtairhhdpr.html

[B15] 布尔运算与取反
来源：http://hz.bjfxy.top/gtlcjwadwr.html

Py:   a and b or not c
来源：http://hz.shangyingyoupin.top/gtncasmleq.html

PHP:  $a && $b || !$c
来源：http://hz.sweek.top/gtohsgtyzk.html

JS:   a && b || !c
来源：http://hz.jlsjyb.cn/gtynfrjovs.html

TS:   a && b || !c
来源：http://hz.nanxinkj.top/gtnxaqfatm.html

Java: a && b || !c
来源：http://hz.gogol.net.cn/gtgcahhxlv.html

Go:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtzpadnefv.html

Ruby: a && b || !c
来源：http://hz.zhixingplan.top/gteufdetjp.html

C#:   a && b || !c
来源：http://hz.sysykeji.top/gtteoevres.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xuetiantiany.cn/gtpqsogpaf.html

Py:   if not data: return
来源：http://hz.zdqjudy.top/gtxmkrvshm.html

PHP:  if (!$data) { return; }
来源：http://hz.zhengqikj.top/gthcppswvi.html

JS:   if (!data) return;
来源：http://hz.yj202588.top/gtuutsnufp.html

TS:   if (!data) return;
来源：http://hz.c1oappe.top/gtixnaqfrg.html

Java: if (data == null) return;
来源：http://hz.yueranfly.top/gtzlmbbwuo.html

Go:   if data == nil { return }
来源：http://hz.jinyuanbaomall.cn/gtcgvnsnis.html

Ruby: return if data.nil?
来源：http://hz.ydzc1.top/gtpntrbptk.html

C#:   if (data == null) return;
来源：http://hz.kuanghao11.cn/gtdglvtpmk.html

================================================================================
来源：http://hz.jlsjyb.cn/gtlwmndqhv.html

C. 函数与作用域
来源：http://hz.yuanzhike.top/gtzgqnoeyq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtfgvcgwqg.html

[C01] 定义函数
来源：http://hz.andypj.xyz/gtzpuhfmue.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtktilmqkg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xylfe.cn/gtmqppcwdx.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yueranfly.top/gtppvvtkds.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guannengcc.top/gtbqqtnajd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.nanxinkj.top/gtxbwrjdqc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ywan-chungtsiang.top/gteugdgntn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cdnleiting.top/gtblpjopcl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtfdhpgcdh.html

[C02] 默认参数
来源：http://hz.aibaodan.cn/gtanzxduqa.html

Py:   def greet(name="World"): return name
来源：http://hz.jyoumei.cn/gtldqzmkzr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sweek.top/gtsoqgxdcl.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.andypj.xyz/gttzoidoey.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hnxiangtu.top/gtebhhxrtz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.chenzaomai.com/gtujhvjshq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtnulnatdx.html

Ruby: def greet(name = "World") = name
来源：http://hz.hongshengwenyu.top/gtnmznmrxi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tanke756.top/gtyfqdpzlg.html

[C03] 可变参数
来源：http://hz.aibaodan.cn/gtrxfexmuf.html

Py:   def total(*args): return sum(args)
来源：http://hz.shanyushiyangkeji.top/gtjcoxdcko.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.aibaodan.cn/gtyjkbyesv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtqltvxogs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sweek.top/gthhwqkjsg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.nanxuanxn.top/gtvyafijzv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xuetiantiany.cn/gtnafzcmah.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.svipenyu.cn/gtredwftru.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jiagoushi.top/gtajwlkuwk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ehwqpu.com/gtfgeocsri.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sxryk.cn/gtjhxtqmrj.html


<!-- 参考信息 -->