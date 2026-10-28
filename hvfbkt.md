代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.jinghuilouyu.cn/gtwcaxaglh.html

Go:   "第一行\n第二行"
来源：http://hz.yj20258.top/gtfarqlzej.html

Ruby: "第一行\n第二行"
来源：http://hz.fzhhl.top/gtodttyufl.html

C#:   "第一行\n第二行"
来源：http://hz.mhx1999.top/gtwxpkkhkl.html

[A14] 注释写法
来源：http://hz.gzhubu.top/gtrpiulong.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.xuanzx.com/gtzeggxifa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.xuanzx.com/gtcdzssahr.html

JS:   // 单行；/* 多行 */
来源：http://hz.daxiang520.top/gtchvufxjx.html

TS:   // 单行；/* 多行 */
来源：http://hz.gzhubu.top/gtpawpzarp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.nanxuanxn.top/gtwwiewgzs.html

Go:   // 单行；/* 多行 */
来源：http://hz.nwbrower.top/gtaaagkcws.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.ivvv.top/gtwddyiuuo.html

C#:   // 单行；/* 多行 */
来源：http://hz.9152youxi.cn/gtvlngasye.html

[A15] 空值判断与默认值
来源：http://hz.ydzc1.top/gtxydbwwve.html

Py:   value = data or "默认值"
来源：http://hz.tanke756.top/gtfpzjkdlz.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.chenlongwang.top/gtaywdstmw.html

JS:   const value = data ?? "默认值";
来源：http://hz.cashguo.top/gtvcsnoswa.html

TS:   const value = data ?? "默认值";
来源：http://hz.shuidangran.top/gtvgkzqqby.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.nanxuanxn.top/gtykutoyxh.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.snrcjt.cn/gtsgvgubne.html

Ruby: value = data || "默认值"
来源：http://hz.nanxuanxn.top/gtcsjomgaw.html

C#:   var value = data ?? "默认值";
来源：http://hz.hammf.cn/gtfgwnavhj.html

[A16] 真假值判断规则
来源：http://hz.xylfe.cn/gtkofupazi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.xuanzx.com/gtewasfbav.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.gaohongyu789.top/gtoismheew.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.birdmap.top/gthrrjfkos.html

TS:   if (!x) {}
来源：http://hz.shanyushiyangtech.top/gtewhmjxki.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.birdmap.top/gtdykutzjz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.smart0.xyz/gtodzjhjtm.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.dianchejie.cn/gtmvfwlvuk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hnxiangtu.top/gtznmkpkwr.html

[A17] 位运算
来源：http://hz.yueranfly.top/gtzemqumuh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cheryme.top/gtpgrjysje.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.shanyushiyangtech.top/gtlhpudhwp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jiagoushi.top/gtivfgifmx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.havefunace.top/gtecwjrsns.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ybcxt.top/gtuxaqhpse.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jinqigfzy.top/gtyqaftjkv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenzaomai.com/gtpgrntknq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cucudq.cn/gtdpeinryb.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ywan-chungtsiang.top/gtwsewgeov.html

Py:   ord("A"); chr(65)
来源：http://hz.fengsongda.top/gtdfpzqlaw.html

PHP:  ord("A"); chr(65)
来源：http://hz.yanxiufei.cn/gtceqxdipk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xinyue.icu/gtlxyzoika.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hammf.cn/gtjectjunh.html

Java: (int) 'A'; (char) 65
来源：http://hz.chenzaomai.com/gtsmwovxhp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.snrcjt.cn/gtuawojnew.html

Ruby: "A".ord; 65.chr
来源：http://hz.jqgufenzy.top/gthgwtaxcz.html

C#:   (int)'A'; (char)65
来源：http://hz.wangshuangyany.cn/gtqkvltsby.html

[A19] 交换两个变量
来源：http://hz.jinyuanbaomall.cn/gtfjxcnobz.html

Py:   a, b = b, a
来源：http://hz.jianghu66.top/gtgpuzsjwx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.shanyushiyangkeji.top/gtdskkczgg.html

JS:   [a, b] = [b, a];
来源：http://hz.sysykeji.top/gtvktzxeed.html

TS:   [a, b] = [b, a];
来源：http://hz.tianlin.xyz/gtmfvipgbe.html

Java: int t = a; a = b; b = t;
来源：http://hz.ehwqpu.com/gtxncomkkk.html

Go:   a, b = b, a
来源：http://hz.jqgfzy.top/gtkehbhrbp.html

Ruby: a, b = b, a
来源：http://hz.redwolf501.top/gtdeskbsfj.html

C#:   (a, b) = (b, a);
来源：http://hz.dashuyun.cn/gtdabqvnsp.html

[A20] 读取标准输入
来源：http://hz.shanyushiyangkeji.top/gtxvptzytf.html

Py:   name = input("请输入：")
来源：http://hz.hysaishi.cn/gtyclzcazu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.kuanghao11.cn/gtpeyaktzf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.aizwys.cn/gtqqhgsrws.html

TS:   // Node.js：readline 模块
来源：http://hz.svipenyu.cn/gtnyzmiphz.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.svipenyu.cn/gthhohqayk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhongyouzk.top/gtoppvnqte.html

Ruby: gets.chomp
来源：http://hz.yvedp.cn/gthgvwqwom.html

C#:   Console.ReadLine();
来源：http://hz.daria6918.cn/gtoikiohwy.html

[A21] 保留指定小数位输出
来源：http://hz.jlsjyb.cn/gtgplgwewf.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jqgfzy.top/gthfuvkytf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.gaohongyu789.top/gtxokauhmd.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ehwqpu.com/gtdtattyom.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtmjaevwtj.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ivvv.top/gtxpydscey.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.iojbl.cn/gtvgvdlhly.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.chenjidiqi.icu/gtaygidwms.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj202588.top/gtrrfkwvdg.html

[A22] 获取字符串长度
来源：http://hz.zycfv.cn/gtxfcgzsip.html

Py:   len(s)
来源：http://hz.yuanzhike.top/gtcmlwfhvf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.kuanghao11.cn/gtnvsktqao.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.tian-w.cn/gtzypjwirf.html

TS:   s.length
来源：http://hz.wangdashe.top/gtpqnjpesg.html

Java: s.length()
来源：http://hz.cheryme.top/gtisvnsakw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.xinyue.icu/gthukufzgi.html

Ruby: s.length
来源：http://hz.shangyingyoupin.top/gtwntypkrc.html

C#:   s.Length
来源：http://hz.c1oappe.top/gtvkmweila.html

[A23] 大小写转换
来源：http://hz.gaohongyu789.top/gtqzxqmumd.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hammf.cn/gtylqiilmu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.guannengcc.top/gttctbriob.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigfzy.top/gtjslgiczs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ydjk.org.cn/gtshwjypof.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.hongshengwenyu.top/gtkxoerflo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.sweek.top/gtvncyepcr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jianghu66.top/gtxlqtwfro.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.xingfuxueyuan.xyz/gtwijcgjuu.html

[A24] 去除首尾空白
来源：http://hz.feifeiyinyue.top/gtlisloeaf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.xuetiantiany.cn/gtaemptsvj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.birdmap.top/gthazgesaz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.nwbrower.top/gtlrdrujhd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigufen.top/gtphkajwje.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.cqqwz.cn/gtuuzmvzgi.html

Go:   strings.TrimSpace(s)
来源：http://hz.yangfankeji.com/gtpjjwyorj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.smart0.xyz/gtbpcxfsda.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhongyouzk.top/gteynvguci.html

[A25] 字符串比较
来源：http://hz.jinqigfzy.top/gtqamdawuv.html

Py:   s1 == s2; s1 != s2
来源：http://hz.hongshengwenyu.top/gtvrtnngme.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.chenzaomai.com/gtdkjlbwzk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.c1oappe.top/gtrbmfxlvv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jinghuilouyu.cn/gtgwzbmpru.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.birdmap.top/gtirzlrxqa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.chenzaomai.com/gtberwbbgl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ywan-chungtsiang.top/gtdkcgpadq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.haohaochexian.top/gtnkmybgyz.html

[A26] 类型转换总览
来源：http://hz.zdqjudy.top/gtqvmyhjmq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jqgfzy.top/gtsqsbrqgp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.wangshuangyany.cn/gtdypnikny.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinghuilouyu.cn/gtacudbodw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jqgufenzy.top/gtoaqcvzma.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.daria6918.cn/gteurvkqas.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.guannengcc.top/gtvbjeetzp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.cucudq.cn/gtaabsbscl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jqgfzy.top/gtyqieeodo.html

================================================================================
来源：http://hz.xuanzx.com/gtnddiqufi.html

B. 流程控制
来源：http://hz.xinyue.icu/gtzbimzyin.html

================================================================================
来源：http://hz.chenzaomai.com/gtsniuxeoj.html

[B01] 条件判断 if / else
来源：http://hz.yongpay.top/gtzlnpbfbh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.daria6918.cn/gtjwphrzcl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.snrcjt.cn/gtmlyibxho.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtlrbzxbgr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jianghu66.top/gtwfuhvaff.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.nanxinkj.top/gtrxgkctln.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.zhaomingkeji.xyz/gtxllarjwh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.ydzc1.top/gtrpuxntcg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.kuanghao11.cn/gtirpvvetg.html

[B02] 多分支 else if / elif
来源：http://hz.nanxuanxn.top/gtyjyohxlj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hongshengwenyu.top/gtxudvnaxs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.daxiang520.top/gtvmcwpmde.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.birdmap.top/gtpduhmbon.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.smart0.xyz/gtxykfewvx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ivvv.top/gtgysnvlld.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.guowangkeji.top/gthbtkarqh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hywenlv.cn/gtqfgeagpx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ybcxt.top/gtolicnosa.html

[B03] switch / match / case
来源：http://hz.snrcjt.cn/gtvcvajnty.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.52xcode.cn/gtozzstvgz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jyoumei.cn/gtrxadboqg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.iojbl.cn/gtbgwheril.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.nanxuanxn.top/gtbsvfmqcd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.bjfxy.top/gtxztwwfwu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jyoumei.cn/gtljtvaqlg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.fzhhl.top/gtkarzlbuf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.shuidangran.top/gtblojhuko.html

[B04] for 计数循环
来源：http://hz.svipenyu.cn/gtrbjoxfzk.html

Py:   for i in range(10): print(i)
来源：http://hz.dashuyun.cn/gtdfbcorgc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.dianchejie.cn/gtgqfsptap.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ybcxt.top/gtqlkdwpqu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.quarkkingdee.top/gthposhrqn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xuanzx.com/gtgfasehpq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.52xcode.cn/gtmtldodgo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhengqikj.top/gtablbrewz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.52xcode.cn/gtrkxgaoqd.html

[B05] 遍历数组 / 列表
来源：http://hz.tianlin.xyz/gtjxaiglew.html

Py:   for item in arr: print(item)
来源：http://hz.sysykeji.top/gtowhmjhmo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.sysykeji.top/gtpvsxyqlo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gttrduljrz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sxryk.cn/gtshrwlcwy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.snrcjt.cn/gtshrzjfvj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hnqzz.top/gtdcidvyzo.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tian-w.cn/gtnkyxrqyy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhixingplan.top/gtqgigyynk.html

[B06] 遍历字典 / 对象
来源：http://hz.shzxlz.cn/gtyuzxkrhk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.shuidangran.top/gtdwsblzpx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinqigufen.top/gtedbniaqq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xziqi.cn/gtifzpuytz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.fzhhl.top/gtauxlkrel.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yj202588.top/gtxxpaguoz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xinyue.icu/gtngherixi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.dianchejie.cn/gtlrvmkemz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yj20258888.top/gtjaagmwkg.html

[B07] while 循环
来源：http://hz.havefunace.top/gtqiurgocz.html

Py:   while i < 10: i += 1
来源：http://hz.zhoulong.xyz/gtszgpestt.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xuetiantiany.cn/gtpzybwvlk.html

JS:   while (i < 10) { i++; }
来源：http://hz.gogol.net.cn/gtxsfjvrdz.html

TS:   while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtrsefiwsb.html

Java: while (i < 10) { i++; }
来源：http://hz.havefunace.top/gtnhndufyk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yongpay.top/gtrqslqdvw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.9152youxi.cn/gtcpgoonto.html

C#:   while (i < 10) { i++; }
来源：http://hz.jqgufenzy.top/gtkmutccxb.html

[B08] do-while（至少执行一次）
来源：http://hz.haohaochexian.top/gtixmuoqrh.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cdnleiting.top/gtoavvstrm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shzxlz.cn/gtxxhgisyu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.mhx1999.top/gtgwyjhzmj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.sweek.top/gtuvijwojy.html

Java: do { i++; } while (i < 10);
来源：http://hz.pycfn.com/gtzlnvhvfe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.guannengcc.top/gtphluuxrg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenlongwang.top/gtochoibwt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.haohaochexian.top/gtexzxanxx.html

[B09] break 与 continue
来源：http://hz.hysaishi.cn/gtjurpfins.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ivvv.top/gtsrrrmtii.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.sysykeji.top/gtpvvjqwqv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtvmeblgih.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtvvmhhczk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gthryfwzcr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.316326.xyz/gtruomgavj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhengqikj.top/gtzvvdnats.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gthkomqkfl.html

[B10] 遍历同时拿索引
来源：http://hz.ehwqpu.com/gtvwlriivn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.ivvv.top/gtparfijpr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.hammf.cn/gtmksmvyod.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.iojbl.cn/gtagnhmigt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgufenzy.top/gtqsxkjozg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jinqigfzy.top/gtuzobymxh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.mhx1999.top/gtjpzgvrui.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.pycfn.com/gtvzqmhayq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yuxming.cn/gtudaoslng.html

[B11] 生成数字序列 / 区间
来源：http://hz.aizwys.cn/gtjxdvwiju.html

Py:   list(range(0, 10, 2))
来源：http://hz.shangyingyoupin.top/gtwhexatjm.html

PHP:  range(0, 10, 2);
来源：http://hz.zhijiandao.cn/gtedpkjlav.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dianchejie.cn/gtykhdcbvy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnxiangtu.top/gtuubvihew.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ivvv.top/gtkjszbefa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.chenjidiqi.icu/gttozqwvrz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.guowangkeji.top/gtncnbzxcr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ydjk.org.cn/gtulltagmn.html

[B12] 跳出多层循环
来源：http://hz.nwbrower.top/gtbxhvfjax.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yvedp.cn/gtfwyoxkky.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenjidiqi.icu/gtkeknnwra.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtranqhwrv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.redwolf501.top/gtpmpwabyw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtozrwywvw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.guannengcc.top/gtezjqvppi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jinqigfzy.top/gtecpqtcth.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.tianlin.xyz/gtqmnwlhdx.html

[B13] 判断是否为数字
来源：http://hz.pengpengdd.cyou/gtnlqbkdzo.html

Py:   isinstance(x, (int, float))
来源：http://hz.guannengcc.top/gtcejpxnxo.html

PHP:  is_numeric($x)
来源：http://hz.wangdashe.top/gtnptgcxbi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jyoumei.cn/gtkxajgsil.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj202588.top/gthedfqlun.html

Java: x instanceof Number
来源：http://hz.ywan-chungtsiang.top/gtlfrouivh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhoulong.xyz/gtxwyhehac.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ybcxt.top/gtyqnxtnxq.html

C#:   x is int or double or decimal
来源：http://hz.daria6918.cn/gtbnaadoow.html

[B14] 判断值是否在集合内
来源：http://hz.zhixingplan.top/gtnuvaldbq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sweek.top/gtilezbahq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cashguo.top/gtkpcchwdx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhongyouzk.top/gtgtjheyjj.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinyuanbaomall.cn/gtdxhsnfwz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinqigfzy.top/gtdtcdpztm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zycfv.cn/gtcuixzxxn.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yj202588.top/gtbeofetvr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtfqtnzpxs.html

[B15] 布尔运算与取反
来源：http://hz.52xcode.cn/gtmkoxrjnu.html

Py:   a and b or not c
来源：http://hz.snrcjt.cn/gtvbobddou.html

PHP:  $a && $b || !$c
来源：http://hz.jlsjyb.cn/gtwyukkubn.html

JS:   a && b || !c
来源：http://hz.nwbrower.top/gtfbjmhrey.html

TS:   a && b || !c
来源：http://hz.ppjwa.cn/gtkiiaxiuz.html

Java: a && b || !c
来源：http://hz.guannengcc.top/gtxfdugmsq.html

Go:   a && b || !c
来源：http://hz.mhx1999.top/gtzecxbfld.html

Ruby: a && b || !c
来源：http://hz.meibo888.top/gthlnnojlo.html

C#:   a && b || !c
来源：http://hz.zdqjudy.top/gtjhpqdnqk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhongyouzk.top/gtuwbtftul.html

Py:   if not data: return
来源：http://hz.wangshuangyany.cn/gtgvvdmsbv.html

PHP:  if (!$data) { return; }
来源：http://hz.gaohongyu789.top/gtbfrsyvwg.html

JS:   if (!data) return;
来源：http://hz.birdmap.top/gtttyniuae.html

TS:   if (!data) return;
来源：http://hz.jinghuilouyu.cn/gtdvetvtxt.html

Java: if (data == null) return;
来源：http://hz.wangdashe.top/gtcseoisaa.html

Go:   if data == nil { return }
来源：http://hz.xylfe.cn/gtguqsoxro.html

Ruby: return if data.nil?
来源：http://hz.wangdashe.top/gtzvulztie.html

C#:   if (data == null) return;
来源：http://hz.pycfn.com/gtouzapany.html

================================================================================
来源：http://hz.cheryme.top/gtlajwegxg.html

C. 函数与作用域
来源：http://hz.vqdsnc.cn/gtgcufshvq.html

================================================================================
来源：http://hz.nanxinkj.top/gtohrzjlgw.html

[C01] 定义函数
来源：http://hz.yanxiufei.cn/gtbcdxgbmi.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxinkj.top/gtmnmxzkdl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daxiang520.top/gtgqojnlit.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yangfankeji.com/gtbjtdoegp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gtjluaovkl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtrjftjnac.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.52xcode.cn/gtzfkelhdt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.guannengcc.top/gtsoqvrtzl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtfpnrofck.html

[C02] 默认参数
来源：http://hz.andypj.xyz/gtqvihbvfh.html

Py:   def greet(name="World"): return name
来源：http://hz.gogol.net.cn/gtyxvsafix.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jqgufenzy.top/gtpypcmzzk.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ppjwa.cn/gtbsshtgcr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.316326.xyz/gttyjagbjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shangyingyoupin.top/gtelttkwid.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sysykeji.top/gtebvaqudr.html

Ruby: def greet(name = "World") = name
来源：http://hz.cheryme.top/gtzmwoiszz.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shzxlz.cn/gtyoaaejqw.html

[C03] 可变参数
来源：http://hz.jinqigfzy.top/gtjjpscfpl.html

Py:   def total(*args): return sum(args)
来源：http://hz.chenzaomai.com/gtsrziceju.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangshuangyany.cn/gtdzzqkdgp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gttcoszbux.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tian-w.cn/gtqvftjnwc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hongshengwenyu.top/gtfrfbnlbi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.dianchejie.cn/gtwiypbgqu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jyoumei.cn/gtfqctdotd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gtajjvqntp.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtlrgfabbe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zhongyouzk.top/gtxfepwhvp.html


<!-- 参考信息 -->