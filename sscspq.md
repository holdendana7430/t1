代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.cdnleiting.top/gttpmllsqv.html

[A15] 空值判断与默认值
来源：http://hz.jinyuanbaomall.cn/gtcghepsji.html

Py:   value = data or "默认值"
来源：http://hz.shanyushiyangkeji.top/gtlqsxgsds.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.zhengqikj.top/gtiobjzujz.html

JS:   const value = data ?? "默认值";
来源：http://hz.daria6918.cn/gtcltushzd.html

TS:   const value = data ?? "默认值";
来源：http://hz.meibo888.top/gtjmgcibso.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.xuanzx.com/gtswicwpge.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.cdnleiting.top/gtfzkwswcn.html

Ruby: value = data || "默认值"
来源：http://hz.tianlin.xyz/gtzletahou.html

C#:   var value = data ?? "默认值";
来源：http://hz.yueranfly.top/gtpmzwjgfa.html

[A16] 真假值判断规则
来源：http://hz.316326.xyz/gtmymmecch.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.mhx1999.top/gtplxpibsl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.shzxlz.cn/gtcrwwdyax.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.chenlongwang.top/gtczlszjev.html

TS:   if (!x) {}
来源：http://hz.cqqwz.cn/gtlcjpoqoj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.52xcode.cn/gtmmexfrqn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.guowangkeji.top/gtqzeylqkp.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.gogol.net.cn/gtpcvhzmiv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.xingfuxueyuan.xyz/gtqohgfkwv.html

[A17] 位运算
来源：http://hz.jiagoushi.top/gtolgeasrn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gtzstzlrxl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.cashguo.top/gtnxcnfarg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtrcitbehj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.kuanghao11.cn/gtsulibeps.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.mhx1999.top/gtlrrdqiir.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.tian-w.cn/gtzuxqrgip.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ywan-chungtsiang.top/gtmqhpnssg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hammf.cn/gtwxhrqvkh.html

[A18] 字符与 ASCII 码互转
来源：http://hz.c1oappe.top/gtmlshyukc.html

Py:   ord("A"); chr(65)
来源：http://hz.aizwys.cn/gtzcajvqbo.html

PHP:  ord("A"); chr(65)
来源：http://hz.zycfv.cn/gtjfzjfwgi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhijiandao.cn/gtitdovede.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cdnleiting.top/gtdrqxhsvh.html

Java: (int) 'A'; (char) 65
来源：http://hz.xziqi.cn/gtwnxxmpcq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.jianghu66.top/gtqozgbkhr.html

Ruby: "A".ord; 65.chr
来源：http://hz.aizwys.cn/gtfxpaxrjp.html

C#:   (int)'A'; (char)65
来源：http://hz.sysykeji.top/gtihaqfyqm.html

[A19] 交换两个变量
来源：http://hz.gzhubu.top/gtctsetajs.html

Py:   a, b = b, a
来源：http://hz.jinghuilouyu.cn/gticjcqruo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hammf.cn/gtcargmfrt.html

JS:   [a, b] = [b, a];
来源：http://hz.nanxuanxn.top/gtpcoubpgw.html

TS:   [a, b] = [b, a];
来源：http://hz.jianghu66.top/gtsowzpprx.html

Java: int t = a; a = b; b = t;
来源：http://hz.52xcode.cn/gtfxniwnih.html

Go:   a, b = b, a
来源：http://hz.svipenyu.cn/gtkiwvskhz.html

Ruby: a, b = b, a
来源：http://hz.yj20258888.top/gtwttvyhyc.html

C#:   (a, b) = (b, a);
来源：http://hz.jlsjyb.cn/gtpuslvsov.html

[A20] 读取标准输入
来源：http://hz.quarkkingdee.top/gtwjpmopxs.html

Py:   name = input("请输入：")
来源：http://hz.dianchejie.cn/gtvucsndsm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.aizwys.cn/gtoghoxcrb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.gzhubu.top/gtjwizzrkr.html

TS:   // Node.js：readline 模块
来源：http://hz.hfpthk.cn/gtidxhinzm.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhongyouzk.top/gtuadxrjpa.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhaomingkeji.xyz/gtusigqnqr.html

Ruby: gets.chomp
来源：http://hz.sxryk.cn/gtbppdllid.html

C#:   Console.ReadLine();
来源：http://hz.wangshuangyany.cn/gtkcthvehl.html

[A21] 保留指定小数位输出
来源：http://hz.haohaochexian.top/gthqldaads.html

Py:   f"{3.14159:.2f}"
来源：http://hz.bjfxy.top/gtvlaszpzm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.hammf.cn/gtbxcsmtke.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ydjk.org.cn/gtzosyujkb.html

TS:   (3.14159).toFixed(2)
来源：http://hz.hywenlv.cn/gtevrbzgpg.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tanke756.top/gtvfiktjno.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.nanxuanxn.top/gtrohcuvwa.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.nwbrower.top/gtaxynfinm.html

C#:   3.14159.ToString("F2")
来源：http://hz.hysaishi.cn/gtefxqstwh.html

[A22] 获取字符串长度
来源：http://hz.dashuyun.cn/gtviempbjj.html

Py:   len(s)
来源：http://hz.fzhhl.top/gtjnaspwni.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.kuanghao11.cn/gtrwyimcrc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.mhx1999.top/gtwnhxggmb.html

TS:   s.length
来源：http://hz.yj202588.top/gtqweyhxcp.html

Java: s.length()
来源：http://hz.gzhubu.top/gtukycdxkn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jqgfzy.top/gttbciqqvd.html

Ruby: s.length
来源：http://hz.ivvv.top/gtqtvpawjh.html

C#:   s.Length
来源：http://hz.cdnleiting.top/gtryekwntl.html

[A23] 大小写转换
来源：http://hz.cqqwz.cn/gtcktulwbs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.kuanghao11.cn/gtmlaxmaee.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.zycfv.cn/gtjooontxt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.iojbl.cn/gtcaqbcifj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.dashuyun.cn/gtcpcfmrmi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.guannengcc.top/gtjxddvaeo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.jinghuilouyu.cn/gthpxetuue.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.0kj1m.cn/gtuaslfpbt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.aizwys.cn/gtnmitkecq.html

[A24] 去除首尾空白
来源：http://hz.hnxiangtu.top/gtqfidlgxb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jqgfzy.top/gtttqzkbcs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.guowangkeji.top/gtwqksmsdv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhijiandao.cn/gtwayabjkk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jianghu66.top/gtpyncfzeo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.nanxuanxn.top/gtdckfemnn.html

Go:   strings.TrimSpace(s)
来源：http://hz.yj202588.top/gtzenrokur.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.guowangkeji.top/gtpseigppo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.aizwys.cn/gtftxxioar.html

[A25] 字符串比较
来源：http://hz.hysaishi.cn/gtkaeujhps.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yonumen.top/gtxaysgwpd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.meibo888.top/gtkufbwbkt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nanxuanxn.top/gtqlbejycw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.feifeiyinyue.top/gtxdnztusz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yonumen.top/gtasoqcjyc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.gaohongyu789.top/gtzhcoubhp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yueranfly.top/gtyffqxwmc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.nwbrower.top/gtnspznbgc.html

[A26] 类型转换总览
来源：http://hz.xingfuxueyuan.xyz/gtdjwovpwg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jianghu66.top/gtkqqlejox.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ehwqpu.com/gtcvarowyz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yj202588.top/gtxhjtktte.html

TS:   Number() String() Boolean() x as number
来源：http://hz.wangshuangyany.cn/gtcsehqdcq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cdnleiting.top/gtykwzrsqr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yonumen.top/gthtgtxdqb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.52xcode.cn/gtiviqbhcq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.gzhubu.top/gtrnfgfsiz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtljmrcnab.html

B. 流程控制
来源：http://hz.hongshengwenyu.top/gtdkdbytuv.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtcafxouxy.html

[B01] 条件判断 if / else
来源：http://hz.52xcode.cn/gtpwibuiwq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.fengsongda.top/gtfxwdyyjl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.nanxinkj.top/gtjrtkyacq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.pycfn.com/gtnuxiifxq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.hnxiangtu.top/gtwmdtfdgb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtfkmnwmap.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.iojbl.cn/gtqoevgwtf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.cqqwz.cn/gtbbyyjzlu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.wangshuangyany.cn/gtjlipupbi.html

[B02] 多分支 else if / elif
来源：http://hz.fzhhl.top/gtwbzffgrz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.quarkkingdee.top/gtgihyabpe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.jinyuanbaomall.cn/gtzxpqgqia.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtxhzpoksp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtnroswzli.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sweek.top/gtactqbmyg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.nanxuanxn.top/gtjbijzwmt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.cdnleiting.top/gtbxwrsoyf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtmylwplnb.html

[B03] switch / match / case
来源：http://hz.ppjwa.cn/gtiwlhnbns.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.cqqwz.cn/gtzkpzloxg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.shuidangran.top/gtnbrtuecg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ppjwa.cn/gtuvcnisal.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhaomingkeji.xyz/gtvpvsyuaf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yangfankeji.com/gtwirbsjha.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cheryme.top/gtakkhnqop.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.guannengcc.top/gtdzdvikpb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xziqi.cn/gtqaehpkyb.html

[B04] for 计数循环
来源：http://hz.daria6918.cn/gtcckcoprd.html

Py:   for i in range(10): print(i)
来源：http://hz.xuanzx.com/gtxavghdlk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cheryme.top/gtigfwduxh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cucudq.cn/gtxjcfrerf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jlsjyb.cn/gtlviznpkb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhoulong.xyz/gtyqyunfob.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.sysykeji.top/gtarcbyejx.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hnxiangtu.top/gtwvrprkzk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.dashuyun.cn/gtzsgdoxvj.html

[B05] 遍历数组 / 列表
来源：http://hz.xylfe.cn/gtflvvcbgr.html

Py:   for item in arr: print(item)
来源：http://hz.aibaodan.cn/gtugoloqmo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.shangyingyoupin.top/gtzibperql.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtwtiujvsg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.tianlin.xyz/gtoklhktcy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.jinyuanbaomall.cn/gtkoxvvlad.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ywan-chungtsiang.top/gtaiyshtze.html

Ruby: arr.each { |item| puts item }
来源：http://hz.fengsongda.top/gtifelwkca.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhaomingkeji.xyz/gtxtbcvrvk.html

[B06] 遍历字典 / 对象
来源：http://hz.zhoulong.xyz/gtvecnhzao.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jinyuanbaomall.cn/gtvvloecin.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cdnleiting.top/gtgtrcrsbf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.svipenyu.cn/gtucfatszc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.bjfxy.top/gtuzzedyui.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.gogol.net.cn/gtofcthpbv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.dianchejie.cn/gtvnuqiywo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.dashuyun.cn/gtbnhpqwfo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hfpthk.cn/gtpikeefvk.html

[B07] while 循环
来源：http://hz.daria6918.cn/gtrhctkyuv.html

Py:   while i < 10: i += 1
来源：http://hz.ehwqpu.com/gthfcoshmp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.daxiang520.top/gtgyoavilm.html

JS:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtuwbjndik.html

TS:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtffowlenh.html

Java: while (i < 10) { i++; }
来源：http://hz.zhongyouzk.top/gtbbqepsia.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.shuidangran.top/gtcufgwfri.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtcmcadeyu.html

C#:   while (i < 10) { i++; }
来源：http://hz.tian-w.cn/gthrpnfqbf.html

[B08] do-while（至少执行一次）
来源：http://hz.hfpthk.cn/gtlawjrzin.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jianghu66.top/gtezqpmcuc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.chenlongwang.top/gtuattcohu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtcbowmyrh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jqgufenzy.top/gtlklvxxtk.html

Java: do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gttmjrtsee.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yongpay.top/gtzvczsmhq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pengpengdd.cyou/gtponcnshq.html

C#:   do { i++; } while (i < 10);
来源：http://hz.tanke756.top/gtrgqmevyu.html

[B09] break 与 continue
来源：http://hz.tanke756.top/gtawoqcqdl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.jianghu66.top/gtuvfslohl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.aibaodan.cn/gtshhyines.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtnvjvjxcf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtubralssp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtidtcbyel.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gogol.net.cn/gtmxqzozdt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.pengpengdd.cyou/gtudrsqmbu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtjnmvhbih.html

[B10] 遍历同时拿索引
来源：http://hz.andypj.xyz/gtoasfvnia.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.quarkkingdee.top/gtwqmmgvjd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.cheryme.top/gtygcptjsq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtguvglflg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.52xcode.cn/gtqzaciaau.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.quarkkingdee.top/gtwbdfdnbc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zdqjudy.top/gtkuegzqsi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aibaodan.cn/gtqqdcupig.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.birdmap.top/gtnytcikan.html

[B11] 生成数字序列 / 区间
来源：http://hz.ybcxt.top/gtzqctdkrm.html

Py:   list(range(0, 10, 2))
来源：http://hz.xuetiantiany.cn/gttgdcnuvv.html

PHP:  range(0, 10, 2);
来源：http://hz.quarkkingdee.top/gtbcejwzgv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtozxreuuo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gtxfrjzvsp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.fengsongda.top/gtoohbjzbq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yonumen.top/gtbdjrfmmm.html

Ruby: (0...10).step(2).to_a
来源：http://hz.ppjwa.cn/gtwxthpjfg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhiwuduotai.top/gtokjophvg.html

[B12] 跳出多层循环
来源：http://hz.ydzc1.top/gtddioefin.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.pengpengdd.cyou/gtttqcvdpj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jqgufenzy.top/gtrhydvbml.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.birdmap.top/gtdiiyaywt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydjk.org.cn/gtbmigubls.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtqmtqebjj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nwbrower.top/gtggxjobgw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yonumen.top/gtdhvonmpz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.daxiang520.top/gtsqerdbuk.html

[B13] 判断是否为数字
来源：http://hz.yj20258888.top/gtsgnbejjg.html

Py:   isinstance(x, (int, float))
来源：http://hz.iojbl.cn/gttxofyjkg.html

PHP:  is_numeric($x)
来源：http://hz.fengsongda.top/gtbcvcvqvx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zycfv.cn/gtdtxeidag.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtibtngwva.html

Java: x instanceof Number
来源：http://hz.zhixingplan.top/gtscgsznol.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hongshengwenyu.top/gtbyqcnypn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xinyue.icu/gtvdhkmqdo.html

C#:   x is int or double or decimal
来源：http://hz.hywenlv.cn/gtllfrmbgf.html

[B14] 判断值是否在集合内
来源：http://hz.jianghu66.top/gtkehbqoqc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hnxiangtu.top/gtluwiwcbp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yongpay.top/gtcthqxzaa.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hammf.cn/gtfbunxawq.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gtxrfwotfh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhengqikj.top/gtiopxpvbv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.xingfuxueyuan.xyz/gtnfiupcwf.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gzhubu.top/gtjnffslwy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hysaishi.cn/gtvsjhfpvi.html

[B15] 布尔运算与取反
来源：http://hz.tianlin.xyz/gtthhesjey.html

Py:   a and b or not c
来源：http://hz.jqgfzy.top/gttllaklim.html

PHP:  $a && $b || !$c
来源：http://hz.ywan-chungtsiang.top/gtamtwvzby.html

JS:   a && b || !c
来源：http://hz.cucudq.cn/gtnpjadkdm.html

TS:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtiwydktnz.html

Java: a && b || !c
来源：http://hz.nanxuanxn.top/gtapaxchtz.html

Go:   a && b || !c
来源：http://hz.cucudq.cn/gtwlbymhuz.html

Ruby: a && b || !c
来源：http://hz.daria6918.cn/gtyewuyxhj.html

C#:   a && b || !c
来源：http://hz.gzhubu.top/gtiimpqgji.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.52xcode.cn/gteasunzht.html

Py:   if not data: return
来源：http://hz.sxryk.cn/gtjsaehbjx.html

PHP:  if (!$data) { return; }
来源：http://hz.9152youxi.cn/gtnhhcteud.html

JS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gterpqmycw.html

TS:   if (!data) return;
来源：http://hz.shzxlz.cn/gtfaeussww.html

Java: if (data == null) return;
来源：http://hz.kuanghao11.cn/gtmjugnoor.html

Go:   if data == nil { return }
来源：http://hz.ydzc1.top/gtwuitreka.html

Ruby: return if data.nil?
来源：http://hz.xylfe.cn/gtxqdkcjut.html

C#:   if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtbyrucqwj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtutwnxton.html

C. 函数与作用域
来源：http://hz.andypj.xyz/gtjujvrscg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmdwlsoqe.html

[C01] 定义函数
来源：http://hz.cucudq.cn/gtsghwlhkn.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxinkj.top/gtzjpsiibo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xinyue.icu/gtegnzbqxp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fzhhl.top/gtoiermoro.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shangyingyoupin.top/gtbsszdxdu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtumqddsnh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yanxiufei.cn/gteolccxff.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xingfuxueyuan.xyz/gtcvqwgfcx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gogol.net.cn/gtuoicdcub.html

[C02] 默认参数
来源：http://hz.316326.xyz/gtswlfahao.html

Py:   def greet(name="World"): return name
来源：http://hz.xuanzx.com/gtsnoquwzl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.sysykeji.top/gttjhnkqqw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydzc1.top/gtndvgluub.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.fengsongda.top/gtpfxxdftj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.mhx1999.top/gtfftmsshg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cdnleiting.top/gtyqpgtsma.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxinkj.top/gtomfaqpnf.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gogol.net.cn/gtcqujjymi.html

[C03] 可变参数
来源：http://hz.jinyuanbaomall.cn/gtrmdgtfic.html

Py:   def total(*args): return sum(args)
来源：http://hz.nanxuanxn.top/gtnqivriwd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.dianchejie.cn/gtxsexlvmz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtwzjqjhpc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtboxfrtqo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zycfv.cn/gteivpyztf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.birdmap.top/gtknmuuccu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cqqwz.cn/gtrnvnmtzv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenzaomai.com/gtxiavvniv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgufenzy.top/gtdlbhnkrr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenzaomai.com/gtdhkhvxir.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.vqdsnc.cn/gtkrjdhdyq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ehwqpu.com/gtskxjsjvg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gotoacloud.top/gthjpklunr.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sxryk.cn/gtjvarhjpy.html

Go:   // 无：用配置结构体参数
来源：http://hz.pengpengdd.cyou/gtogwhyppy.html

Ruby: f(a: 1, b: 2)
来源：http://hz.feifeiyinyue.top/gttlfcjkuo.html

C#:   f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gthuumwwpd.html

[C05] 返回多个值
来源：http://hz.sysykeji.top/gtvaobsoma.html

Py:   return a, b
来源：http://hz.cheryme.top/gtgmlwamuk.html

PHP:  return [$a, $b];
来源：http://hz.sysykeji.top/gtmspqlgoh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xylfe.cn/gtdkkpiuup.html

TS:   return { a, b };
来源：http://hz.yanxiufei.cn/gtygcvettt.html


<!-- 参考信息 -->