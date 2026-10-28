代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.gotoacloud.top/gtyygmeayf.html

[A15] 空值判断与默认值
来源：http://hz.meibo888.top/gtmqtseskc.html

Py:   value = data or "默认值"
来源：http://hz.yonumen.top/gtrxboiobc.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.hnxiangtu.top/gtygbiqkfs.html

JS:   const value = data ?? "默认值";
来源：http://hz.ppjwa.cn/gtoambnidv.html

TS:   const value = data ?? "默认值";
来源：http://hz.nanxuanxn.top/gttdszxaet.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.redwolf501.top/gtrclcwtqi.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cqqwz.cn/gtoecdcubq.html

Ruby: value = data || "默认值"
来源：http://hz.cashguo.top/gtgxjdatek.html

C#:   var value = data ?? "默认值";
来源：http://hz.shuidangran.top/gtngzpsdtp.html

[A16] 真假值判断规则
来源：http://hz.fengsongda.top/gtfrvfncsr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.nanxinkj.top/gththwxnvk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.zdqjudy.top/gtypkbehei.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.yanxiufei.cn/gtwiqvpwyl.html

TS:   if (!x) {}
来源：http://hz.havefunace.top/gtnkapbzdr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.zhixingplan.top/gtmrxxpjpt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.pengpengdd.cyou/gtwouugxvy.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.daxiang520.top/gtqeqxwbwi.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zhiwuduotai.top/gtzvzbnftc.html

[A17] 位运算
来源：http://hz.zhaomingkeji.xyz/gteidkhmnn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shzxlz.cn/gtnlyfqtez.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.52xcode.cn/gtbtvvvmdr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtmhnbhlql.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.jinqigfzy.top/gtpsvmbzro.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj202588.top/gttwgqqrdt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtjjxhhnur.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gtoipfaqtu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtxzdinrkc.html

[A18] 字符与 ASCII 码互转
来源：http://hz.gotoacloud.top/gtyfonmafs.html

Py:   ord("A"); chr(65)
来源：http://hz.wangdashe.top/gtmvzwskxu.html

PHP:  ord("A"); chr(65)
来源：http://hz.zhixingplan.top/gtejpkfvzb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.iojbl.cn/gthaxlgggz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhoulong.xyz/gtwtajyown.html

Java: (int) 'A'; (char) 65
来源：http://hz.hnxiangtu.top/gtqwfmlywc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.chenlongwang.top/gtvnxzmpwr.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhijiandao.cn/gtieumyzff.html

C#:   (int)'A'; (char)65
来源：http://hz.zhongyouzk.top/gtrzxwiork.html

[A19] 交换两个变量
来源：http://hz.yongpay.top/gtqldobvyo.html

Py:   a, b = b, a
来源：http://hz.hongshengwenyu.top/gtqteiyikb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.meibo888.top/gtnwyofzli.html

JS:   [a, b] = [b, a];
来源：http://hz.dianchejie.cn/gtakjknqwc.html

TS:   [a, b] = [b, a];
来源：http://hz.hnxiangtu.top/gtfoowmiks.html

Java: int t = a; a = b; b = t;
来源：http://hz.dashuyun.cn/gtzuxtdwkk.html

Go:   a, b = b, a
来源：http://hz.jinyuanbaomall.cn/gtobnlnjmp.html

Ruby: a, b = b, a
来源：http://hz.xziqi.cn/gtnsqqdhqc.html

C#:   (a, b) = (b, a);
来源：http://hz.sxryk.cn/gtylwsitjg.html

[A20] 读取标准输入
来源：http://hz.haohaochexian.top/gtaiqgjicn.html

Py:   name = input("请输入：")
来源：http://hz.xylfe.cn/gtfdxuxfhz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.jiagoushi.top/gtwwywcmsp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.cashguo.top/gtvrrqmpjl.html

TS:   // Node.js：readline 模块
来源：http://hz.chenlongwang.top/gtaybcvrmv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.ywan-chungtsiang.top/gtzasvbspe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.daria6918.cn/gtausdxdqc.html

Ruby: gets.chomp
来源：http://hz.cheryme.top/gtvbzywphx.html

C#:   Console.ReadLine();
来源：http://hz.aibaodan.cn/gtupslvzod.html

[A21] 保留指定小数位输出
来源：http://hz.sysykeji.top/gtlyaairxb.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yonumen.top/gtxltarsol.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.hammf.cn/gtqyfquwjf.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ydzc1.top/gtmwykyhom.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jqgufenzy.top/gtgnwghqff.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.cucudq.cn/gtcdyzmtke.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.nwbrower.top/gtofstiqld.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zhiwuduotai.top/gtuwqeprel.html

C#:   3.14159.ToString("F2")
来源：http://hz.hammf.cn/gtycxnhxwt.html

[A22] 获取字符串长度
来源：http://hz.zhengqikj.top/gtlyrxtavw.html

Py:   len(s)
来源：http://hz.ybcxt.top/gtlzsokjop.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jianghu66.top/gtbkzgyyqn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.haohaochexian.top/gtnqllhrkw.html

TS:   s.length
来源：http://hz.316326.xyz/gtfzzcpewu.html

Java: s.length()
来源：http://hz.zhaomingkeji.xyz/gtnhcubsgc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.ywan-chungtsiang.top/gtxjfcrxal.html

Ruby: s.length
来源：http://hz.zhixingplan.top/gtpkpdhyhd.html

C#:   s.Length
来源：http://hz.xuanzx.com/gtisbzmbzs.html

[A23] 大小写转换
来源：http://hz.jinqigufen.top/gtuckzecsa.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.aibaodan.cn/gtroqrlshz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.pycfn.com/gtuoytcxzi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jiagoushi.top/gtvcjvmryg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cqqwz.cn/gtunfgtwel.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangtech.top/gtnshaksik.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.iojbl.cn/gtjalvaspk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.hammf.cn/gtpfbvoosf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.chenjidiqi.icu/gthnzjgovz.html

[A24] 去除首尾空白
来源：http://hz.0kj1m.cn/gtbtrfuhey.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.gzhubu.top/gtofoootmv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ehwqpu.com/gtcjrwjaag.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sxryk.cn/gtmhwmqobf.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuanzx.com/gtddqvjeof.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.nanxuanxn.top/gtcgmwbcro.html

Go:   strings.TrimSpace(s)
来源：http://hz.jianghu66.top/gtptdskxte.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ehwqpu.com/gtchxtwtsb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.tanke756.top/gtbiqitoen.html

[A25] 字符串比较
来源：http://hz.cdnleiting.top/gtnjyxszxt.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zdqjudy.top/gtjweutceu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cucudq.cn/gtxcteafav.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtwywkygxr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgufenzy.top/gtopqlzdgk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hywenlv.cn/gtcftwystu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.chenlongwang.top/gttjabfyro.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ehwqpu.com/gtvdkeiqsf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.pycfn.com/gtyvebezpo.html

[A26] 类型转换总览
来源：http://hz.hammf.cn/gtftvewzrw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yj20258.top/gtosrkqljj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.sysykeji.top/gtbqwfomlx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhaomingkeji.xyz/gtoypsxrbw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhixingplan.top/gtbwtjursp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.daxiang520.top/gthaaipiai.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhixingplan.top/gtvfthigkz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yj202588.top/gtofniaife.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jyoumei.cn/gtxfckzkda.html

================================================================================
来源：http://hz.hnxiangtu.top/gtuulpsomr.html

B. 流程控制
来源：http://hz.nwbrower.top/gtgikyozdd.html

================================================================================
来源：http://hz.xuanzx.com/gtstayjmbx.html

[B01] 条件判断 if / else
来源：http://hz.sysykeji.top/gtestwykgc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.svipenyu.cn/gtqxotafwl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.hnqzz.top/gtsfektozr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zdqjudy.top/gtetwwadnu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtpkddxbhe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.zhixingplan.top/gtvmqwxkeh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.fengsongda.top/gtwznksxlv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cucudq.cn/gtfldwanvj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xziqi.cn/gtraauyime.html

[B02] 多分支 else if / elif
来源：http://hz.chenlongwang.top/gtcxvqgcjk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.9152youxi.cn/gtgdunnjte.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.nanxinkj.top/gtefasgyqz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtanmuuowf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cdnleiting.top/gtkhdlceps.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinqigfzy.top/gtfqpudjuy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.cheryme.top/gtmwwcvwmk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.nanxuanxn.top/gtxbhleova.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.pycfn.com/gtjxouaqgh.html

[B03] switch / match / case
来源：http://hz.gotoacloud.top/gtwrputfmh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cdnleiting.top/gtufhmhmjo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.c1oappe.top/gtzsgwxnre.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yueranfly.top/gtnhpntwmq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.tianlin.xyz/gtpshloedi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenzaomai.com/gtcpzdiyvk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.dianchejie.cn/gtbvryocwm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.havefunace.top/gtjgcvppml.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xinyue.icu/gtlshxuxne.html

[B04] for 计数循环
来源：http://hz.yj20258.top/gtrkoofibz.html

Py:   for i in range(10): print(i)
来源：http://hz.shanyushiyangkeji.top/gtqqukjzgk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.aibaodan.cn/gtnjjrcbww.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.fzhhl.top/gtwigcwdfa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yuxming.cn/gtqehurjxi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hysaishi.cn/gtqcobfnlf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xuanzx.com/gtyfhmcwip.html

Ruby: 10.times { |i| puts i }
来源：http://hz.sufxvd.cn/gtbovpiono.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.meibo888.top/gtlicyodzl.html

[B05] 遍历数组 / 列表
来源：http://hz.sweek.top/gtbvwgwttu.html

Py:   for item in arr: print(item)
来源：http://hz.mhx1999.top/gtdxruatqd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.316326.xyz/gtomqsvvqp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.ydzc1.top/gtiqsvqtbn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.daxiang520.top/gtanyuzuoa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yj20258.top/gtqyitowvr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.meibo888.top/gtspipwccc.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zycfv.cn/gtlpqlzsrw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.guowangkeji.top/gtcrczavlt.html

[B06] 遍历字典 / 对象
来源：http://hz.zhijiandao.cn/gtobmxpals.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ydzc1.top/gtywzaisso.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jinyuanbaomall.cn/gtsnsjqaxi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xylfe.cn/gtjdrkakib.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sufxvd.cn/gtjjanywog.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hammf.cn/gtxmqcchev.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.svipenyu.cn/gtjlbchndn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hnqzz.top/gtmkimwsln.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xingfuxueyuan.xyz/gtjeihnxog.html

[B07] while 循环
来源：http://hz.hnxiangtu.top/gthoyftxba.html

Py:   while i < 10: i += 1
来源：http://hz.gaohongyu789.top/gtfkqsfbhw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.xuetiantiany.cn/gtlcmfsjzv.html

JS:   while (i < 10) { i++; }
来源：http://hz.zhaomingkeji.xyz/gtameldzya.html

TS:   while (i < 10) { i++; }
来源：http://hz.guowangkeji.top/gthenzcsjv.html

Java: while (i < 10) { i++; }
来源：http://hz.gaohongyu789.top/gtautfphno.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shanyushiyangtech.top/gtqqcayvvi.html

Ruby: while i < 10; i += 1; end
来源：http://hz.pycfn.com/gtstvktjls.html

C#:   while (i < 10) { i++; }
来源：http://hz.tian-w.cn/gthujrisne.html

[B08] do-while（至少执行一次）
来源：http://hz.cashguo.top/gtryxlkjpu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.havefunace.top/gtnrqfocqm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.pengpengdd.cyou/gtselpazyt.html

JS:   do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gtqkaawyem.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhongyouzk.top/gtwtrbztzs.html

Java: do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtfujhchtw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hnqzz.top/gtpixegnkp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.feifeiyinyue.top/gtjermftgp.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gthgrsomhv.html

[B09] break 与 continue
来源：http://hz.cheryme.top/gtyiqbijne.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xziqi.cn/gtplsnaofc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtgkqtjvwa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yonumen.top/gtbdsjpwbi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.snrcjt.cn/gtxpwkujzc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtwvgqbwiy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.zhijiandao.cn/gtnzippppn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gthpvntvmm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtgncufkai.html

[B10] 遍历同时拿索引
来源：http://hz.jinghuilouyu.cn/gtngoofiue.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenlongwang.top/gtfxalpnyj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.feifeiyinyue.top/gtsejstrqz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hongshengwenyu.top/gturcpvkbj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtqpnfrowi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jyoumei.cn/gtrnoawgcj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jinyuanbaomall.cn/gtisxhsrxv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhijiandao.cn/gtigqiqnth.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ydjk.org.cn/gtgrueunye.html

[B11] 生成数字序列 / 区间
来源：http://hz.sufxvd.cn/gtflwfytig.html

Py:   list(range(0, 10, 2))
来源：http://hz.aibaodan.cn/gtvnlwtmsk.html

PHP:  range(0, 10, 2);
来源：http://hz.gzhubu.top/gtapijlomr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sufxvd.cn/gtnxzklgkq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.cashguo.top/gtelwfovzt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.svipenyu.cn/gtlaosrjfl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gtlmjbionc.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xylfe.cn/gtnnyxxhwg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.haohaochexian.top/gtshhzzgro.html

[B12] 跳出多层循环
来源：http://hz.jinghuilouyu.cn/gtdpmdmtpx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jiagoushi.top/gtjxrcrxwl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.sysykeji.top/gtoqwsgerc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gtvpqrqrnf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.mhx1999.top/gtmwylzdqt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zycfv.cn/gtmovsocsd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.meibo888.top/gtxghwoqvf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ydjk.org.cn/gtppzrsnme.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenzaomai.com/gtgowekyua.html

[B13] 判断是否为数字
来源：http://hz.cucudq.cn/gtnqturtvh.html

Py:   isinstance(x, (int, float))
来源：http://hz.xuetiantiany.cn/gtrarsxlxa.html

PHP:  is_numeric($x)
来源：http://hz.gaohongyu789.top/gthkadsylk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sufxvd.cn/gtpjiuoqdc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gttmwfvgys.html

Java: x instanceof Number
来源：http://hz.gogol.net.cn/gtmygqvjxm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sweek.top/gtwybvsfks.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hongshengwenyu.top/gtngslqqtw.html

C#:   x is int or double or decimal
来源：http://hz.ybcxt.top/gtremtobiq.html

[B14] 判断值是否在集合内
来源：http://hz.jinqigfzy.top/gtxciwcspu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hongshengwenyu.top/gtyyrteduo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shuidangran.top/gtqsiybvst.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ydzc1.top/gtmewdnmxl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gaohongyu789.top/gtkfkfpjjc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sxryk.cn/gtqhheyphr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhengqikj.top/gtwevziwtr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.dianchejie.cn/gtgujtkqoq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.mhx1999.top/gtrlacockv.html

[B15] 布尔运算与取反
来源：http://hz.yj20258.top/gtwzlojmtq.html

Py:   a and b or not c
来源：http://hz.iojbl.cn/gtzmxinkay.html

PHP:  $a && $b || !$c
来源：http://hz.tianlin.xyz/gtmdxyjjtu.html

JS:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtuqoygzez.html

TS:   a && b || !c
来源：http://hz.cashguo.top/gtjmfpbnqe.html

Java: a && b || !c
来源：http://hz.sysykeji.top/gtwsafwent.html

Go:   a && b || !c
来源：http://hz.52xcode.cn/gtmcqcsivd.html

Ruby: a && b || !c
来源：http://hz.cucudq.cn/gturgdfceo.html

C#:   a && b || !c
来源：http://hz.aibaodan.cn/gtxatwkwhp.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shangyingyoupin.top/gttojlgmrl.html

Py:   if not data: return
来源：http://hz.zhoulong.xyz/gtuewwekmp.html

PHP:  if (!$data) { return; }
来源：http://hz.sweek.top/gtmdpnpkfo.html

JS:   if (!data) return;
来源：http://hz.jianghu66.top/gtmmaulbsk.html

TS:   if (!data) return;
来源：http://hz.jinghuilouyu.cn/gtqirhorvb.html

Java: if (data == null) return;
来源：http://hz.yvedp.cn/gtdgjugvsz.html

Go:   if data == nil { return }
来源：http://hz.tanke756.top/gtxswsisgn.html

Ruby: return if data.nil?
来源：http://hz.yuxming.cn/gtzvbagysr.html

C#:   if (data == null) return;
来源：http://hz.yueranfly.top/gtiyglrnwx.html

================================================================================
来源：http://hz.yueranfly.top/gtpytpamxs.html

C. 函数与作用域
来源：http://hz.aibaodan.cn/gtaqqxvtaa.html

================================================================================
来源：http://hz.cheryme.top/gtcycffpin.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gtavbqntzj.html

Py:   def add(a, b): return a + b
来源：http://hz.tianlin.xyz/gtytuonscy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtikyvpemg.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xuanzx.com/gtzqsnzdhf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtocdqbzbr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtfwmjzpel.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtadofzuhj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.vqdsnc.cn/gtafrqojjn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtbxrhblwa.html

[C02] 默认参数
来源：http://hz.sysykeji.top/gthguvppvn.html

Py:   def greet(name="World"): return name
来源：http://hz.daxiang520.top/gtnonopeys.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.dashuyun.cn/gtjauujvrf.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ybcxt.top/gtbdqbpedu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.svipenyu.cn/gtzcfgcbdl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yangfankeji.com/gttvupjytl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.kuanghao11.cn/gtmraegkhx.html

Ruby: def greet(name = "World") = name
来源：http://hz.ppjwa.cn/gtdfhfvhwm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnxiangtu.top/gtwwqphffc.html

[C03] 可变参数
来源：http://hz.mhx1999.top/gtvatfqiek.html

Py:   def total(*args): return sum(args)
来源：http://hz.shangyingyoupin.top/gtjvgvparm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.aibaodan.cn/gttlkpxtdc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cheryme.top/gtgvkqhumx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tanke756.top/gtanevgezc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jianghu66.top/gtlmozrerk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.redwolf501.top/gtvaatrhrv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ivvv.top/gtkpnjrryl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenlongwang.top/gtzpkrzjan.html

[C04] 命名参数 / 关键字参数
来源：http://hz.gotoacloud.top/gtfnutyvwf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sysykeji.top/gtqfplbjyl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.316326.xyz/gtdelqtzjg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.iojbl.cn/gtfhemiqjl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.nwbrower.top/gtsngfgsmv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sufxvd.cn/gtnskxunij.html

Go:   // 无：用配置结构体参数
来源：http://hz.vqdsnc.cn/gtaljfavkl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuxming.cn/gtvpxhbyds.html

C#:   f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtzvkbuysy.html

[C05] 返回多个值
来源：http://hz.shzxlz.cn/gtqwqkfner.html

Py:   return a, b
来源：http://hz.xinyue.icu/gtrwmlvbol.html

PHP:  return [$a, $b];
来源：http://hz.0kj1m.cn/gtrdxxshgh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.snrcjt.cn/gtpyeqempm.html

TS:   return { a, b };
来源：http://hz.zhoulong.xyz/gtyivjvygr.html


<!-- 参考信息 -->