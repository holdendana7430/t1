代发 wailian999

[A14] 注释写法
来源：http://hz.hywenlv.cn/gtahutfrac.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.aizwys.cn/gtryclcbgj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.kuanghao11.cn/gtwhsmvruv.html

JS:   // 单行；/* 多行 */
来源：http://hz.hysaishi.cn/gtejpmqtek.html

TS:   // 单行；/* 多行 */
来源：http://hz.ydjk.org.cn/gtajitkukf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.ppjwa.cn/gtjemphves.html

Go:   // 单行；/* 多行 */
来源：http://hz.zhijiandao.cn/gtwimlzzod.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.wangdashe.top/gttccvmqqf.html

C#:   // 单行；/* 多行 */
来源：http://hz.ydzc1.top/gtdwvhlyqh.html

[A15] 空值判断与默认值
来源：http://hz.xziqi.cn/gtupwlcstz.html

Py:   value = data or "默认值"
来源：http://hz.chenlongwang.top/gtzxyzdyel.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.guannengcc.top/gtbiaqgrcd.html

JS:   const value = data ?? "默认值";
来源：http://hz.cheryme.top/gtznewagvh.html

TS:   const value = data ?? "默认值";
来源：http://hz.zycfv.cn/gtlcehtdbf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.0kj1m.cn/gtijynjdci.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.daxiang520.top/gtwsczmash.html

Ruby: value = data || "默认值"
来源：http://hz.xinyue.icu/gtkqxyfdkg.html

C#:   var value = data ?? "默认值";
来源：http://hz.hfpthk.cn/gtcaiwdhde.html

[A16] 真假值判断规则
来源：http://hz.xinyue.icu/gtbfofnbob.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yangfankeji.com/gtahzuinbq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.nwbrower.top/gtsogqjcri.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.cashguo.top/gtegpgvbne.html

TS:   if (!x) {}
来源：http://hz.jqgufenzy.top/gtbeunecli.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.tianlin.xyz/gtamgxyyxp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.birdmap.top/gtygpoxsud.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.9152youxi.cn/gtizmkjdju.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.vqdsnc.cn/gttlkdjtzt.html

[A17] 位运算
来源：http://hz.jqgufenzy.top/gtzucmhmdf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nanxinkj.top/gtzzuezzwj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.gzhubu.top/gtmojjxkut.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtqjecloia.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtegdngdyg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtswhfiocf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtggjfpyiz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtelizkasp.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gaohongyu789.top/gtqanqsbbb.html

[A18] 字符与 ASCII 码互转
来源：http://hz.nanxinkj.top/gtldrrdqpb.html

Py:   ord("A"); chr(65)
来源：http://hz.dashuyun.cn/gtkwxxcjve.html

PHP:  ord("A"); chr(65)
来源：http://hz.jinyuanbaomall.cn/gttgfpkjjk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhengqikj.top/gtrwkkhvfh.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.redwolf501.top/gthzrlchgw.html

Java: (int) 'A'; (char) 65
来源：http://hz.316326.xyz/gtmaarkkos.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.hammf.cn/gtdkuwseph.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhoulong.xyz/gturrrwugb.html

C#:   (int)'A'; (char)65
来源：http://hz.daria6918.cn/gtgakibmqn.html

[A19] 交换两个变量
来源：http://hz.gzhubu.top/gtidjevfki.html

Py:   a, b = b, a
来源：http://hz.xuanzx.com/gtbdtecplt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yj20258.top/gtxehtysft.html

JS:   [a, b] = [b, a];
来源：http://hz.yongpay.top/gtyrmkjbsy.html

TS:   [a, b] = [b, a];
来源：http://hz.yuanzhike.top/gtjaagkkzv.html

Java: int t = a; a = b; b = t;
来源：http://hz.hywenlv.cn/gtyaotdivy.html

Go:   a, b = b, a
来源：http://hz.cucudq.cn/gtnqhnfael.html

Ruby: a, b = b, a
来源：http://hz.dianchejie.cn/gtkwmbdrlu.html

C#:   (a, b) = (b, a);
来源：http://hz.vqdsnc.cn/gtmyeryrxa.html

[A20] 读取标准输入
来源：http://hz.gzhubu.top/gtvwmlwvzn.html

Py:   name = input("请输入：")
来源：http://hz.andypj.xyz/gtrbqwirat.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.zhixingplan.top/gthlbdbjag.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.guowangkeji.top/gthhftccbw.html

TS:   // Node.js：readline 模块
来源：http://hz.xziqi.cn/gtadgtzfsw.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.shzxlz.cn/gtvdlxskta.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.dashuyun.cn/gtmmpokiue.html

Ruby: gets.chomp
来源：http://hz.cheryme.top/gtopkprpzp.html

C#:   Console.ReadLine();
来源：http://hz.yangfankeji.com/gtksevthod.html

[A21] 保留指定小数位输出
来源：http://hz.nanxinkj.top/gtkwsuqgzv.html

Py:   f"{3.14159:.2f}"
来源：http://hz.chenjidiqi.icu/gtadfgpshv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.meibo888.top/gtfpflrbou.html

JS:   (3.14159).toFixed(2)
来源：http://hz.wangdashe.top/gtzaolvera.html

TS:   (3.14159).toFixed(2)
来源：http://hz.ppjwa.cn/gtcjrqvyqp.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.sweek.top/gtixmeuifo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.kuanghao11.cn/gtvgmaynsd.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.ivvv.top/gtbpsdshpu.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhijiandao.cn/gtyknenmkn.html

[A22] 获取字符串长度
来源：http://hz.andypj.xyz/gtespfmebc.html

Py:   len(s)
来源：http://hz.chenjidiqi.icu/gtjjbivggq.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jqgufenzy.top/gtujdbhgwv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xingfuxueyuan.xyz/gttgyhgkuy.html

TS:   s.length
来源：http://hz.zycfv.cn/gtqmoddaty.html

Java: s.length()
来源：http://hz.cheryme.top/gtjhcelnrt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.dianchejie.cn/gtzvxvdyly.html

Ruby: s.length
来源：http://hz.chenzaomai.com/gtrdsxmzhh.html

C#:   s.Length
来源：http://hz.tianlin.xyz/gtcvydufjx.html

[A23] 大小写转换
来源：http://hz.chenjidiqi.icu/gtxxaaoqfk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.shzxlz.cn/gtkepenzef.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zhixingplan.top/gtiybnvhal.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhijiandao.cn/gtlbbuoaza.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gtsxvxmawa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.ehwqpu.com/gtzeswhrtb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jqgfzy.top/gtozzgshmj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ydjk.org.cn/gtqqospxfb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.dianchejie.cn/gtfvgyfbcl.html

[A24] 去除首尾空白
来源：http://hz.yj20258888.top/gtwgeivlno.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jinqigfzy.top/gtjrgixidt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.shanyushiyangkeji.top/gtggnwykab.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jlsjyb.cn/gtucrjlxfi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.mhx1999.top/gtlvcmyqxw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.sysykeji.top/gtlnkywehm.html

Go:   strings.TrimSpace(s)
来源：http://hz.shuidangran.top/gtizinhcsh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xinyue.icu/gtmkmcdosj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.guannengcc.top/gtybxpkmhv.html

[A25] 字符串比较
来源：http://hz.fzhhl.top/gtfnvyufkq.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhoulong.xyz/gtsysuypeg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.fengsongda.top/gtyprntovb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.redwolf501.top/gtzdwcsnxo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydjk.org.cn/gtygrgqjxb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.guowangkeji.top/gtgffwfchv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yuxming.cn/gtbdbxtnth.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhixingplan.top/gtarcscjnw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.kuanghao11.cn/gtvemwixte.html

[A26] 类型转换总览
来源：http://hz.ybcxt.top/gtfzziwffs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zycfv.cn/gtncrbdriw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ybcxt.top/gtyhjtymeo.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhijiandao.cn/gtkflwzuuq.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhoulong.xyz/gtbptcrflb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.tianlin.xyz/gtflcanhvp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.chenzaomai.com/gtcscuiuhz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.sxryk.cn/gtnfdmabgn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.vqdsnc.cn/gtndmatnya.html

================================================================================
来源：http://hz.52xcode.cn/gtzumeedeb.html

B. 流程控制
来源：http://hz.316326.xyz/gtlyzqtipa.html

================================================================================
来源：http://hz.gaohongyu789.top/gttsizmfyu.html

[B01] 条件判断 if / else
来源：http://hz.tianlin.xyz/gtvhnpuvke.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.quarkkingdee.top/gtpqrpyjkw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhoulong.xyz/gtaljssrqp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hammf.cn/gtoezzgaau.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gthvsgumej.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yongpay.top/gtymrifzhg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.tianlin.xyz/gtwabicjgu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.shanyushiyangkeji.top/gtsqohccwd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gtqxcbddst.html

[B02] 多分支 else if / elif
来源：http://hz.zhixingplan.top/gtwcwyhjnz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.smart0.xyz/gttlatfurh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.svipenyu.cn/gtifaisjfd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtcczobfav.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtedaebwzr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.c1oappe.top/gtcdewjofd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.wangdashe.top/gtalkbegnz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinyuanbaomall.cn/gtingjamyx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jiagoushi.top/gtibulbfux.html

[B03] switch / match / case
来源：http://hz.daria6918.cn/gtlogyyxms.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.ybcxt.top/gtthsbpqhi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.chenlongwang.top/gtjrdhdaig.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yonumen.top/gtjerdlltw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.birdmap.top/gtxcwbacyk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.feifeiyinyue.top/gtxywehiop.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cqqwz.cn/gtipwbvcue.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cheryme.top/gtlroacaxv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.guowangkeji.top/gtcrwsycqq.html

[B04] for 计数循环
来源：http://hz.cucudq.cn/gtrpzdvywt.html

Py:   for i in range(10): print(i)
来源：http://hz.zhaomingkeji.xyz/gthnwswabr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.mhx1999.top/gtafsavwsk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shanyushiyangkeji.top/gtuoflllxl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shuidangran.top/gtqvdzkqkp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xuetiantiany.cn/gtjrokfayt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.gogol.net.cn/gtwuruvfit.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zycfv.cn/gtbpovpezu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.quarkkingdee.top/gtpecqllch.html

[B05] 遍历数组 / 列表
来源：http://hz.jinqigfzy.top/gtwbbkoesz.html

Py:   for item in arr: print(item)
来源：http://hz.tianlin.xyz/gtjmcxdcpk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yuanzhike.top/gtikhrrjqw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgufenzy.top/gtvhhhvibg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtofnpmlip.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ywan-chungtsiang.top/gthwkkgphh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yonumen.top/gtfakdanhm.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ydzc1.top/gtzkzgrmkz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.0kj1m.cn/gtyidpyrae.html

[B06] 遍历字典 / 对象
来源：http://hz.ydjk.org.cn/gtgxvupaxc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hywenlv.cn/gtyfvhkjnf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.316326.xyz/gtbmiqfyby.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.svipenyu.cn/gtesapufyq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shangyingyoupin.top/gtfwofwuxf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shanyushiyangtech.top/gtacimyxta.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.haohaochexian.top/gtunmbqjbd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xziqi.cn/gtktszdeih.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.pycfn.com/gtpxpjqgdq.html

[B07] while 循环
来源：http://hz.aizwys.cn/gtsctpnmom.html

Py:   while i < 10: i += 1
来源：http://hz.gogol.net.cn/gtxgjojydo.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.smart0.xyz/gtokthyfmb.html

JS:   while (i < 10) { i++; }
来源：http://hz.nanxuanxn.top/gtofhuahmg.html

TS:   while (i < 10) { i++; }
来源：http://hz.birdmap.top/gtasyoaqdz.html

Java: while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtjazqfkyd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cheryme.top/gtjicjpnwf.html

Ruby: while i < 10; i += 1; end
来源：http://hz.xuanzx.com/gtrycndnud.html

C#:   while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gttatdwbfu.html

[B08] do-while（至少执行一次）
来源：http://hz.tanke756.top/gttxohcbmp.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xuanzx.com/gtwrjtjnar.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.svipenyu.cn/gtdvlzugji.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhengqikj.top/gtkrpvntoj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ybcxt.top/gteumlucds.html

Java: do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtefithgvu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.haohaochexian.top/gtcikpzbzt.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.svipenyu.cn/gtgmtepngc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.fzhhl.top/gtsszwfrer.html

[B09] break 与 continue
来源：http://hz.zhaomingkeji.xyz/gtqxuryogt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.wangshuangyany.cn/gtzxkpztlb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hnxiangtu.top/gtuplwgkde.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtdercfrkh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhixingplan.top/gtidyldyft.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtfujxlvzx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jlsjyb.cn/gttngpvjec.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hammf.cn/gtitcxincw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtgrkjcslg.html

[B10] 遍历同时拿索引
来源：http://hz.jyoumei.cn/gtmlzfsgwn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.iojbl.cn/gtfmgvcdta.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zdqjudy.top/gtkkggpwon.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gtemcxpqva.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.zhijiandao.cn/gtzusopwwm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jianghu66.top/gtetddfxeb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.dianchejie.cn/gtlkbgsxgr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shzxlz.cn/gtuugrmeyk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ywan-chungtsiang.top/gtwyazlozi.html

[B11] 生成数字序列 / 区间
来源：http://hz.svipenyu.cn/gtouytoeod.html

Py:   list(range(0, 10, 2))
来源：http://hz.guannengcc.top/gtqinuiqys.html

PHP:  range(0, 10, 2);
来源：http://hz.yongpay.top/gtauvydcrx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shuidangran.top/gtxxumbwuv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj202588.top/gtaauhonrl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yj202588.top/gttqffkwbn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.ehwqpu.com/gtzwrbtwxc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenlongwang.top/gtldmzpeuz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigfzy.top/gtuxrmzjlj.html

[B12] 跳出多层循环
来源：http://hz.yonumen.top/gtbpelcvnr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.c1oappe.top/gteybiazrf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhijiandao.cn/gtdgqqafqd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigfzy.top/gtleliptsg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yongpay.top/gtbbkhojxc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtmjnoiidq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hnxiangtu.top/gtuxyagubf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.mhx1999.top/gtpxwoefgp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hywenlv.cn/gtywyogvus.html

[B13] 判断是否为数字
来源：http://hz.kuanghao11.cn/gtldihwrfk.html

Py:   isinstance(x, (int, float))
来源：http://hz.xinyue.icu/gtliaqiowr.html

PHP:  is_numeric($x)
来源：http://hz.chenlongwang.top/gtgarkrtub.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.tanke756.top/gttydesfgp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gtudybhzju.html

Java: x instanceof Number
来源：http://hz.9152youxi.cn/gtwsaluxvb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jiagoushi.top/gtwokoqzyp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nanxinkj.top/gtezvwiyqj.html

C#:   x is int or double or decimal
来源：http://hz.xylfe.cn/gtepozmbuj.html

[B14] 判断值是否在集合内
来源：http://hz.yongpay.top/gtohfdngdq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.daria6918.cn/gtextkrrhv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenzaomai.com/gtawiityke.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhengqikj.top/gthpijxwmi.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtynmipnhy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.wangshuangyany.cn/gtknsuqocq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.316326.xyz/gtggyacwdu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yongpay.top/gtauxqrlsa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.9152youxi.cn/gtbxintyxx.html

[B15] 布尔运算与取反
来源：http://hz.gzhubu.top/gthgdlprku.html

Py:   a and b or not c
来源：http://hz.tian-w.cn/gtfhdfaiuy.html

PHP:  $a && $b || !$c
来源：http://hz.fengsongda.top/gtmolmhdvx.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtpgfhahkz.html

TS:   a && b || !c
来源：http://hz.zhixingplan.top/gtymufvepx.html

Java: a && b || !c
来源：http://hz.yuxming.cn/gtnbqtrzsv.html

Go:   a && b || !c
来源：http://hz.smart0.xyz/gtuougflhd.html

Ruby: a && b || !c
来源：http://hz.yueranfly.top/gtgcapyilh.html

C#:   a && b || !c
来源：http://hz.zhengqikj.top/gtjnwxdznh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jqgufenzy.top/gtmsjwssnh.html

Py:   if not data: return
来源：http://hz.daria6918.cn/gthmfmkrct.html

PHP:  if (!$data) { return; }
来源：http://hz.andypj.xyz/gtseuhlwzp.html

JS:   if (!data) return;
来源：http://hz.sysykeji.top/gtkkkshony.html

TS:   if (!data) return;
来源：http://hz.smart0.xyz/gtwazuadwn.html

Java: if (data == null) return;
来源：http://hz.hysaishi.cn/gtahmpwhzf.html

Go:   if data == nil { return }
来源：http://hz.dashuyun.cn/gtolqilxls.html

Ruby: return if data.nil?
来源：http://hz.hnqzz.top/gtetfaszpj.html

C#:   if (data == null) return;
来源：http://hz.mhx1999.top/gtofrzihxi.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtoyhaxqkt.html

C. 函数与作用域
来源：http://hz.snrcjt.cn/gtvdwhajka.html

================================================================================
来源：http://hz.sysykeji.top/gtkuzyujjf.html

[C01] 定义函数
来源：http://hz.smart0.xyz/gtvnwmipui.html

Py:   def add(a, b): return a + b
来源：http://hz.c1oappe.top/gtklxvsmxx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtorttulwm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtwueqjjms.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtpxihhavi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtxmqiwujz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.feifeiyinyue.top/gtevgpkgwh.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hfpthk.cn/gtsmsziavx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gtfzsnsrlw.html

[C02] 默认参数
来源：http://hz.chenlongwang.top/gtzvflqthn.html

Py:   def greet(name="World"): return name
来源：http://hz.cucudq.cn/gtaohxqlfy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.guowangkeji.top/gtoqarxghd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hnqzz.top/gtgeiqdutj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.hywenlv.cn/gtafgxqaem.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jqgufenzy.top/gthltlatdk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jyoumei.cn/gtpryddkfu.html

Ruby: def greet(name = "World") = name
来源：http://hz.sweek.top/gtrzttqzks.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hammf.cn/gtbuflacpw.html

[C03] 可变参数
来源：http://hz.zhaomingkeji.xyz/gtnpeqaxfd.html

Py:   def total(*args): return sum(args)
来源：http://hz.quarkkingdee.top/gtispkexes.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xuanzx.com/gtiauuzlxy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtcyeycxeo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinqigfzy.top/gtofcamcib.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hywenlv.cn/gtavcakkha.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxuanxn.top/gtenhicnaa.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.aibaodan.cn/gthgqllizv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.guannengcc.top/gtranixdlr.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xinyue.icu/gtmmxmauzk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sysykeji.top/gtydfkjniu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.vqdsnc.cn/gtjfwydlmg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hongshengwenyu.top/gtlfulcaou.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhoulong.xyz/gtohvrwnfy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.shanyushiyangkeji.top/gtpliezgdl.html


<!-- 参考信息 -->