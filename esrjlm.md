代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://hz.shangyingyoupin.top/gtbhsiutny.html

[A15] 空值判断与默认值
来源：http://hz.yongpay.top/gtymladqkq.html

Py:   value = data or "默认值"
来源：http://hz.zhoulong.xyz/gtkknsfnnp.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.gzhubu.top/gtobthvvnh.html

JS:   const value = data ?? "默认值";
来源：http://hz.zdqjudy.top/gtnelombpt.html

TS:   const value = data ?? "默认值";
来源：http://hz.guannengcc.top/gtaeuwxcvu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shuidangran.top/gtgnzxnjnu.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.feifeiyinyue.top/gtgoilsysi.html

Ruby: value = data || "默认值"
来源：http://hz.zycfv.cn/gtixkpfdmk.html

C#:   var value = data ?? "默认值";
来源：http://hz.shuidangran.top/gtfvbgwkex.html

[A16] 真假值判断规则
来源：http://hz.yj20258888.top/gtycrzerid.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.xylfe.cn/gtcxvjbdln.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.zhijiandao.cn/gtpvkclywp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xylfe.cn/gtuwxylgnx.html

TS:   if (!x) {}
来源：http://hz.jinyuanbaomall.cn/gttwqwovtk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yj20258888.top/gtxfxhcggx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jyoumei.cn/gtbcaietuw.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.yj20258888.top/gtyvxyrcoj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.jinyuanbaomall.cn/gtafiezjhn.html

[A17] 位运算
来源：http://hz.hongshengwenyu.top/gtrncbfcjr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yangfankeji.com/gtyaxlpavm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yuxming.cn/gtvwkvbmpm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gtvgqhxmvb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.316326.xyz/gtvymubhdy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinqigufen.top/gtgwytswjs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtujeybeor.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ehwqpu.com/gtjhnygkvf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtnctubsum.html

[A18] 字符与 ASCII 码互转
来源：http://hz.smart0.xyz/gtkvdhkxxy.html

Py:   ord("A"); chr(65)
来源：http://hz.cucudq.cn/gtdqrojfcj.html

PHP:  ord("A"); chr(65)
来源：http://hz.yanxiufei.cn/gtotvywpty.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinqigfzy.top/gtwoorhrfs.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ydjk.org.cn/gtievkkjlc.html

Java: (int) 'A'; (char) 65
来源：http://hz.pycfn.com/gtsrsujybf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.andypj.xyz/gtrahnjglb.html

Ruby: "A".ord; 65.chr
来源：http://hz.jqgfzy.top/gtmgnagmax.html

C#:   (int)'A'; (char)65
来源：http://hz.ivvv.top/gtckmibfpn.html

[A19] 交换两个变量
来源：http://hz.cashguo.top/gtxfcrrlfx.html

Py:   a, b = b, a
来源：http://hz.bjfxy.top/gtyyvrnhhy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.pycfn.com/gtqdweaxwc.html

JS:   [a, b] = [b, a];
来源：http://hz.cheryme.top/gtbmwsjtnn.html

TS:   [a, b] = [b, a];
来源：http://hz.daxiang520.top/gtkzaywetq.html

Java: int t = a; a = b; b = t;
来源：http://hz.cheryme.top/gtygeqdyna.html

Go:   a, b = b, a
来源：http://hz.yonumen.top/gtzyylhpin.html

Ruby: a, b = b, a
来源：http://hz.cqqwz.cn/gtnbkiwpbq.html

C#:   (a, b) = (b, a);
来源：http://hz.pycfn.com/gtqmoryatl.html

[A20] 读取标准输入
来源：http://hz.daxiang520.top/gtouhleuol.html

Py:   name = input("请输入：")
来源：http://hz.xuetiantiany.cn/gtscerksxm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hfpthk.cn/gthjzawhbe.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.gzhubu.top/gtrcjziydw.html

TS:   // Node.js：readline 模块
来源：http://hz.xuetiantiany.cn/gtunjklayv.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.bjfxy.top/gtzghksbxc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhongyouzk.top/gtdwfejfte.html

Ruby: gets.chomp
来源：http://hz.wangshuangyany.cn/gthaukjtyt.html

C#:   Console.ReadLine();
来源：http://hz.zhijiandao.cn/gtxdtpfmub.html

[A21] 保留指定小数位输出
来源：http://hz.hammf.cn/gtdozxbgfb.html

Py:   f"{3.14159:.2f}"
来源：http://hz.andypj.xyz/gtxqegenky.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ydzc1.top/gtpruspjti.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ppjwa.cn/gtjbtyomkc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yj20258888.top/gtvosivoma.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.andypj.xyz/gtvuwzpeyt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.daria6918.cn/gtqlqyavze.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.wangdashe.top/gtbuqxsupy.html

C#:   3.14159.ToString("F2")
来源：http://hz.yangfankeji.com/gttdpqacsq.html

[A22] 获取字符串长度
来源：http://hz.9152youxi.cn/gtguvkgzxs.html

Py:   len(s)
来源：http://hz.iojbl.cn/gtjfqyyqmy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zhongyouzk.top/gtlyutijkc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.vqdsnc.cn/gthvqpbuce.html

TS:   s.length
来源：http://hz.jiagoushi.top/gtdzhmonum.html

Java: s.length()
来源：http://hz.ppjwa.cn/gtmrwutlwa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.jinghuilouyu.cn/gtncydfhze.html

Ruby: s.length
来源：http://hz.hywenlv.cn/gtrwizvpyz.html

C#:   s.Length
来源：http://hz.guannengcc.top/gtczjodqkr.html

[A23] 大小写转换
来源：http://hz.ehwqpu.com/gtmuzhnkmy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.cqqwz.cn/gtvmbgdwgi.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.shzxlz.cn/gtybogviad.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ivvv.top/gtzdefupgr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.havefunace.top/gtivmwltsw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.tian-w.cn/gtpdyeqypb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ywan-chungtsiang.top/gtvtkfckzv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.yongpay.top/gtvwiqnplp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.wangdashe.top/gtdslnxxah.html

[A24] 去除首尾空白
来源：http://hz.ehwqpu.com/gttkxmvezy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.ydzc1.top/gtyojrmncf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.cheryme.top/gtfarriuez.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.hnqzz.top/gtronwkgco.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.bjfxy.top/gtwotllpum.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.xingfuxueyuan.xyz/gtfgwlfogi.html

Go:   strings.TrimSpace(s)
来源：http://hz.snrcjt.cn/gtkteafumx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yongpay.top/gtxborxvxl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shangyingyoupin.top/gtzdwztmtv.html

[A25] 字符串比较
来源：http://hz.chenlongwang.top/gtuihehyka.html

Py:   s1 == s2; s1 != s2
来源：http://hz.wangshuangyany.cn/gteqclmniu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.dashuyun.cn/gtfqkwcrxs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.gogol.net.cn/gtymbfjvwb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.aibaodan.cn/gtojlvsrvd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.chenzaomai.com/gtjozimojh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yangfankeji.com/gtxvpakjqk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.quarkkingdee.top/gtgbfvxoaa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yanxiufei.cn/gtzidozclk.html

[A26] 类型转换总览
来源：http://hz.yueranfly.top/gtgybxblzv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.chenzaomai.com/gtfunogoqa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jinqigufen.top/gtpshpnnlc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yangfankeji.com/gtdxmarpfx.html

TS:   Number() String() Boolean() x as number
来源：http://hz.dianchejie.cn/gtncopvcsr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.bjfxy.top/gtnioqmjnz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.ydjk.org.cn/gtosncehht.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.shanyushiyangtech.top/gthafcvmki.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jlsjyb.cn/gtevlbybtw.html

================================================================================
来源：http://hz.xylfe.cn/gtntixplem.html

B. 流程控制
来源：http://hz.feifeiyinyue.top/gtmiadcpwu.html

================================================================================
来源：http://hz.jiagoushi.top/gthpesrjgz.html

[B01] 条件判断 if / else
来源：http://hz.ywan-chungtsiang.top/gtuokpwdpc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.jiagoushi.top/gtgdzthyay.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.daria6918.cn/gtvkyqxjpa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yueranfly.top/gthkcncvwy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhiwuduotai.top/gtuhuadobe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shuidangran.top/gtfjyoyihx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yj20258888.top/gthicwxkkb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yvedp.cn/gtcmfiqbum.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.0kj1m.cn/gtwpnpdksi.html

[B02] 多分支 else if / elif
来源：http://hz.hywenlv.cn/gtawdxleun.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.zhijiandao.cn/gtudlpcuvo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.chenzaomai.com/gtnmrqsxsn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgufenzy.top/gtkrxawcoe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cheryme.top/gtcokwellr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtaheprlzf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xingfuxueyuan.xyz/gtpvmcaidp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.shanyushiyangtech.top/gtlbkbabci.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ehwqpu.com/gtxcxntwkc.html

[B03] switch / match / case
来源：http://hz.yvedp.cn/gtsclbpnpk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.fengsongda.top/gtpadkuuki.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhixingplan.top/gtaznxfqoa.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.guowangkeji.top/gtghfqvmky.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj20258888.top/gtehcjixxu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.feifeiyinyue.top/gtlfadqyxu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hammf.cn/gtgheywynb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hysaishi.cn/gtkmozqxwa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.shanyushiyangtech.top/gteuqkgiok.html

[B04] for 计数循环
来源：http://hz.hnqzz.top/gtblppuvyt.html

Py:   for i in range(10): print(i)
来源：http://hz.daria6918.cn/gtawvfuper.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.hnqzz.top/gtlqojqnhn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhijiandao.cn/gtzrnwajza.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.sweek.top/gtmbmcdrto.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xziqi.cn/gtgvgxqvhj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ivvv.top/gtsmbordhr.html

Ruby: 10.times { |i| puts i }
来源：http://hz.hongshengwenyu.top/gtbreybnkr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.xylfe.cn/gtpzrskxsb.html

[B05] 遍历数组 / 列表
来源：http://hz.xingfuxueyuan.xyz/gtfswdarza.html

Py:   for item in arr: print(item)
来源：http://hz.zhixingplan.top/gtigfdghig.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.hnxiangtu.top/gtvfdhmzjp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenjidiqi.icu/gtxnvvnqaj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.guannengcc.top/gtwnyxeoey.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.wangshuangyany.cn/gtscuqigxu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.daria6918.cn/gtltjccauu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zycfv.cn/gtozibnpzs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.yangfankeji.com/gtkainrvtv.html

[B06] 遍历字典 / 对象
来源：http://hz.gogol.net.cn/gtxeeiwewq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.nwbrower.top/gtbmfmelqi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.meibo888.top/gtegkzepfb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.smart0.xyz/gtuizyptvi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.snrcjt.cn/gtmznxadwh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hnxiangtu.top/gtnjapkfpd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hnqzz.top/gtyiooxrwt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.fzhhl.top/gtlkohbzth.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sufxvd.cn/gtimyjivjz.html

[B07] while 循环
来源：http://hz.daxiang520.top/gtmswrpalu.html

Py:   while i < 10: i += 1
来源：http://hz.guowangkeji.top/gtxdxgfsls.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.tianlin.xyz/gtgytwoeut.html

JS:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gthmqdmiqt.html

TS:   while (i < 10) { i++; }
来源：http://hz.tanke756.top/gttlwnfhkk.html

Java: while (i < 10) { i++; }
来源：http://hz.yanxiufei.cn/gtogjtuvna.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jinqigufen.top/gtqaueulfu.html

Ruby: while i < 10; i += 1; end
来源：http://hz.aizwys.cn/gtzabaocop.html

C#:   while (i < 10) { i++; }
来源：http://hz.xylfe.cn/gtbtsiqcqf.html

[B08] do-while（至少执行一次）
来源：http://hz.guannengcc.top/gtcmcjwvld.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenzaomai.com/gtavttxzuv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.daria6918.cn/gtcwidrskc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.redwolf501.top/gtnpxsjxdp.html

TS:   do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtpsmktpep.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhaomingkeji.xyz/gtkrlrwizm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhengqikj.top/gtialsmdue.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhaomingkeji.xyz/gtogehbtcb.html

C#:   do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtstocurms.html

[B09] break 与 continue
来源：http://hz.pengpengdd.cyou/gteuehmpcw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gotoacloud.top/gtexvsbbep.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cucudq.cn/gtzxwzwklo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ybcxt.top/gtyaymiorz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hammf.cn/gtxxegswjd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtyinoykei.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.yuxming.cn/gtbuorrhri.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.feifeiyinyue.top/gtsiunkpre.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cqqwz.cn/gtltvtjbyb.html

[B10] 遍历同时拿索引
来源：http://hz.yj20258.top/gtpynhtxnr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hongshengwenyu.top/gtxpymjhpu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gogol.net.cn/gtwnjyrjbp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gotoacloud.top/gtojtzwtob.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.smart0.xyz/gtqcbyolot.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shanyushiyangtech.top/gtkikanxlf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.vqdsnc.cn/gtaxhqqfcp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.gzhubu.top/gtxrnuvdle.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj20258.top/gtpaqfkagv.html

[B11] 生成数字序列 / 区间
来源：http://hz.meibo888.top/gtybnxfayq.html

Py:   list(range(0, 10, 2))
来源：http://hz.yanxiufei.cn/gthiugfhij.html

PHP:  range(0, 10, 2);
来源：http://hz.yvedp.cn/gtkjxvkjxw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhixingplan.top/gtzuttyrur.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.birdmap.top/gthyrfvhhs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.snrcjt.cn/gtuhtktvre.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhijiandao.cn/gtfbjoosho.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sxryk.cn/gtgmuagmdo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.pycfn.com/gtlxwfsmfm.html

[B12] 跳出多层循环
来源：http://hz.daxiang520.top/gtktlpwktu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.mhx1999.top/gttmzjsigo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yueranfly.top/gtpulspbpy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yangfankeji.com/gtukbjhbpk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cqqwz.cn/gtzojhllxx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtkkraspvm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cdnleiting.top/gtwprwhfsv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhiwuduotai.top/gtwhdchzej.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.mhx1999.top/gtmblwhzap.html

[B13] 判断是否为数字
来源：http://hz.yonumen.top/gtkoizdugz.html

Py:   isinstance(x, (int, float))
来源：http://hz.guowangkeji.top/gtedoeymxj.html

PHP:  is_numeric($x)
来源：http://hz.sxryk.cn/gtasdmukhk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhongyouzk.top/gtbsaljxis.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtusvoqoou.html

Java: x instanceof Number
来源：http://hz.zhijiandao.cn/gtxzyeojry.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinyuanbaomall.cn/gtjbztwwov.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenjidiqi.icu/gtnraqqqxj.html

C#:   x is int or double or decimal
来源：http://hz.wangshuangyany.cn/gtoydcrbtt.html

[B14] 判断值是否在集合内
来源：http://hz.cdnleiting.top/gtogdyoaah.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.316326.xyz/gtknbzqecl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shangyingyoupin.top/gtpohncszd.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ywan-chungtsiang.top/gtpnukdjav.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gogol.net.cn/gtilobtmea.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.haohaochexian.top/gtwvqszppu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ppjwa.cn/gtbtbnjhwt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.fzhhl.top/gtxezugjte.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shanyushiyangkeji.top/gtatrugusj.html

[B15] 布尔运算与取反
来源：http://hz.jyoumei.cn/gtgojrsytp.html

Py:   a and b or not c
来源：http://hz.nanxuanxn.top/gtjxyivneu.html

PHP:  $a && $b || !$c
来源：http://hz.sysykeji.top/gtekfyfaky.html

JS:   a && b || !c
来源：http://hz.ppjwa.cn/gtkaqzxfik.html

TS:   a && b || !c
来源：http://hz.svipenyu.cn/gtdateqbkp.html

Java: a && b || !c
来源：http://hz.tanke756.top/gtrldxyvkd.html

Go:   a && b || !c
来源：http://hz.yanxiufei.cn/gtfiwjazho.html

Ruby: a && b || !c
来源：http://hz.cucudq.cn/gtghhdcayl.html

C#:   a && b || !c
来源：http://hz.jinqigfzy.top/gtoqpajniv.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hywenlv.cn/gtyzzuqqrw.html

Py:   if not data: return
来源：http://hz.vqdsnc.cn/gtnumgimmj.html

PHP:  if (!$data) { return; }
来源：http://hz.zhongyouzk.top/gtduhmkayb.html

JS:   if (!data) return;
来源：http://hz.xuetiantiany.cn/gtndddnkqt.html

TS:   if (!data) return;
来源：http://hz.zhongyouzk.top/gtquuyycfa.html

Java: if (data == null) return;
来源：http://hz.sysykeji.top/gtwuchljiv.html

Go:   if data == nil { return }
来源：http://hz.jqgufenzy.top/gtzwuywybn.html

Ruby: return if data.nil?
来源：http://hz.quarkkingdee.top/gtixbrtmod.html

C#:   if (data == null) return;
来源：http://hz.wangdashe.top/gtdhlxqeyk.html

================================================================================
来源：http://hz.yvedp.cn/gtvfqtngwo.html

C. 函数与作用域
来源：http://hz.wangdashe.top/gtmnfruwut.html

================================================================================
来源：http://hz.shuidangran.top/gtqswcsubg.html

[C01] 定义函数
来源：http://hz.sweek.top/gtreatcxty.html

Py:   def add(a, b): return a + b
来源：http://hz.hnqzz.top/gtfmmuqsnj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.iojbl.cn/gtyqmetdea.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.redwolf501.top/gtitmamsco.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gtlggcmkmv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj20258.top/gtmcievhnc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinyuanbaomall.cn/gttmtahiex.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jianghu66.top/gtrudyhhew.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtufcneblh.html

[C02] 默认参数
来源：http://hz.xinyue.icu/gttpexcjqe.html

Py:   def greet(name="World"): return name
来源：http://hz.feifeiyinyue.top/gtqyplkewl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.meibo888.top/gthvnqljes.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.52xcode.cn/gtrizcgwsi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.meibo888.top/gtmpdttxin.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yangfankeji.com/gtmoqenekq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sxryk.cn/gtdgjqryxd.html

Ruby: def greet(name = "World") = name
来源：http://hz.sysykeji.top/gtgdtyzoup.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.c1oappe.top/gteqptfzsb.html

[C03] 可变参数
来源：http://hz.ywan-chungtsiang.top/gtesuvfpgc.html

Py:   def total(*args): return sum(args)
来源：http://hz.andypj.xyz/gtkibnenyh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhaomingkeji.xyz/gtqxizrkjk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtkpglacda.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gotoacloud.top/gtafuqouqj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ivvv.top/gttootjxaf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xylfe.cn/gtevokmjdv.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jianghu66.top/gthnajhcze.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zhiwuduotai.top/gtrxhctrxh.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jianghu66.top/gtjbifhjty.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hnqzz.top/gtczbdjovp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.52xcode.cn/gtcrjxfyqd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtodbmfhgf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhengqikj.top/gtgngbhrif.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nanxuanxn.top/gtpsudwjhs.html

Go:   // 无：用配置结构体参数
来源：http://hz.guannengcc.top/gtlxqjwtmt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtkhxkhqlo.html

C#:   f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gteqciksiz.html

[C05] 返回多个值
来源：http://hz.gaohongyu789.top/gtfbpcabuj.html

Py:   return a, b
来源：http://hz.nanxuanxn.top/gtuavtjwbx.html

PHP:  return [$a, $b];
来源：http://hz.jianghu66.top/gtmdyfikih.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tanke756.top/gtgiucdukk.html

TS:   return { a, b };
来源：http://hz.hfpthk.cn/gtniitjqgc.html


<!-- 参考信息 -->