代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://hz.pycfn.com/gtcstvjvsc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.jinghuilouyu.cn/gthejqvpzh.html

Go:   // 单行；/* 多行 */
来源：http://hz.gzhubu.top/gtdivmhynf.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yuanzhike.top/gtkzcfuxiv.html

C#:   // 单行；/* 多行 */
来源：http://hz.fzhhl.top/gtlulbtyjj.html

[A15] 空值判断与默认值
来源：http://hz.guowangkeji.top/gtuzmbhoih.html

Py:   value = data or "默认值"
来源：http://hz.dianchejie.cn/gthzuprhcy.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.pengpengdd.cyou/gttaiiyyji.html

JS:   const value = data ?? "默认值";
来源：http://hz.gaohongyu789.top/gtthsqveal.html

TS:   const value = data ?? "默认值";
来源：http://hz.hfpthk.cn/gtvlmbmxtn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.cqqwz.cn/gtirnhiusl.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.nanxuanxn.top/gtbuetthmd.html

Ruby: value = data || "默认值"
来源：http://hz.zhongyouzk.top/gtmamudfjk.html

C#:   var value = data ?? "默认值";
来源：http://hz.hysaishi.cn/gtcsnrjhwa.html

[A16] 真假值判断规则
来源：http://hz.fengsongda.top/gtxhptermv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.dashuyun.cn/gtxfpuycoh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.hammf.cn/gtaoitljcd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.jinghuilouyu.cn/gtesyhyrip.html

TS:   if (!x) {}
来源：http://hz.smart0.xyz/gtgzfbqwld.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yj20258.top/gtdjaaveos.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.yonumen.top/gtayhzektr.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zhengqikj.top/gtoncsjzik.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.zhongyouzk.top/gthzgctmwl.html

[A17] 位运算
来源：http://hz.jyoumei.cn/gthsxbvvnv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ivvv.top/gtdknzcvza.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.nanxuanxn.top/gtweitfghq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.pengpengdd.cyou/gtktetkxtl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.guowangkeji.top/gtwqpyvosk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cashguo.top/gtfifpjzyw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtvtdyjloh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gotoacloud.top/gtnttbhcde.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.snrcjt.cn/gtwqlqprcu.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jinghuilouyu.cn/gtqnqmcayh.html

Py:   ord("A"); chr(65)
来源：http://hz.nanxuanxn.top/gtzinbryaz.html

PHP:  ord("A"); chr(65)
来源：http://hz.fengsongda.top/gtkoersgrb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhoulong.xyz/gtarhdyvyt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yj20258.top/gttpqxivjb.html

Java: (int) 'A'; (char) 65
来源：http://hz.iojbl.cn/gtsuqnwlfq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.meibo888.top/gtmaziadcu.html

Ruby: "A".ord; 65.chr
来源：http://hz.snrcjt.cn/gtxzccoamy.html

C#:   (int)'A'; (char)65
来源：http://hz.shangyingyoupin.top/gtwhoaejev.html

[A19] 交换两个变量
来源：http://hz.shanyushiyangtech.top/gtovxzbqck.html

Py:   a, b = b, a
来源：http://hz.pycfn.com/gtgathhedu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.gzhubu.top/gtokbcurlw.html

JS:   [a, b] = [b, a];
来源：http://hz.ehwqpu.com/gtkdmfatft.html

TS:   [a, b] = [b, a];
来源：http://hz.yj20258.top/gtcipqmjdi.html

Java: int t = a; a = b; b = t;
来源：http://hz.cheryme.top/gtdqunugqe.html

Go:   a, b = b, a
来源：http://hz.wangdashe.top/gtptfwmspe.html

Ruby: a, b = b, a
来源：http://hz.vqdsnc.cn/gtugdyhdtu.html

C#:   (a, b) = (b, a);
来源：http://hz.hywenlv.cn/gtkqwfypxl.html

[A20] 读取标准输入
来源：http://hz.yvedp.cn/gtyzvzlzcj.html

Py:   name = input("请输入：")
来源：http://hz.cqqwz.cn/gtkkcxhjvl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.jianghu66.top/gtkyupqhvm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.hfpthk.cn/gtyehpmtrl.html

TS:   // Node.js：readline 模块
来源：http://hz.hammf.cn/gtttzqqkvi.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhengqikj.top/gtebdanxhc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ivvv.top/gtutwiojuq.html

Ruby: gets.chomp
来源：http://hz.daxiang520.top/gtekpsmstb.html

C#:   Console.ReadLine();
来源：http://hz.havefunace.top/gtojtbatfj.html

[A21] 保留指定小数位输出
来源：http://hz.cheryme.top/gtdsbhhzgu.html

Py:   f"{3.14159:.2f}"
来源：http://hz.nanxinkj.top/gtqcbhtnpg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.mhx1999.top/gtxwwljref.html

JS:   (3.14159).toFixed(2)
来源：http://hz.snrcjt.cn/gtrswsrbwc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zdqjudy.top/gtbiwbasuv.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yj20258.top/gthetuyvmq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtlblrkudb.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.ydjk.org.cn/gtbbrheftb.html

C#:   3.14159.ToString("F2")
来源：http://hz.nanxuanxn.top/gtfyzjyfbp.html

[A22] 获取字符串长度
来源：http://hz.chenjidiqi.icu/gtijuvqiph.html

Py:   len(s)
来源：http://hz.jinqigufen.top/gtvyavnhja.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.fengsongda.top/gtmhobvltb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.gzhubu.top/gtiuoqombm.html

TS:   s.length
来源：http://hz.jqgfzy.top/gtjqwkxheb.html

Java: s.length()
来源：http://hz.sufxvd.cn/gtvagnbhye.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.c1oappe.top/gtehfndwul.html

Ruby: s.length
来源：http://hz.ppjwa.cn/gtgxgefvba.html

C#:   s.Length
来源：http://hz.nwbrower.top/gtnbmpwnlm.html

[A23] 大小写转换
来源：http://hz.jyoumei.cn/gtnuamrawt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zdqjudy.top/gtwlpbbqnt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.shanyushiyangkeji.top/gtoptnjwvy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xziqi.cn/gtewctnicj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ivvv.top/gtminibnlo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.cdnleiting.top/gtxehmrmym.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.nwbrower.top/gtrnyglnka.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.gotoacloud.top/gtxkvasdtc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yvedp.cn/gtzoccfgeo.html

[A24] 去除首尾空白
来源：http://hz.xziqi.cn/gtzwcubhyh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.havefunace.top/gtzrkmjfme.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.guowangkeji.top/gtffypzzhl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.pycfn.com/gtflpvfwyo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yueranfly.top/gtmrffjyee.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.52xcode.cn/gtbypkccqg.html

Go:   strings.TrimSpace(s)
来源：http://hz.jlsjyb.cn/gtooudbdpu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.jqgufenzy.top/gttupjkxqw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.svipenyu.cn/gtmhdzfbtj.html

[A25] 字符串比较
来源：http://hz.yuanzhike.top/gthbiqqoff.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yueranfly.top/gtnmjntxkj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ywan-chungtsiang.top/gtoxxotlim.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yvedp.cn/gtrqlyjccp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yueranfly.top/gtftauldvb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.zhijiandao.cn/gtikgbtekz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yanxiufei.cn/gtdgazlgdl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.ppjwa.cn/gttklsiknk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xuetiantiany.cn/gthmkiocev.html

[A26] 类型转换总览
来源：http://hz.dianchejie.cn/gthopwtleb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.ehwqpu.com/gtiqssvhgk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gotoacloud.top/gtqrfjpwnt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hammf.cn/gtldriapes.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jinghuilouyu.cn/gtcmjtxirv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.nanxuanxn.top/gtweydfbrh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hysaishi.cn/gtzzharmcm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yanxiufei.cn/gtdwsxfrup.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.hnqzz.top/gtdgpbwrwc.html

================================================================================
来源：http://hz.bjfxy.top/gtimvfvivl.html

B. 流程控制
来源：http://hz.sxryk.cn/gtjpojhasv.html

================================================================================
来源：http://hz.jianghu66.top/gtvigmrele.html

[B01] 条件判断 if / else
来源：http://hz.ydzc1.top/gttqohjeiy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zhaomingkeji.xyz/gtafwncvhe.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhaomingkeji.xyz/gttjtelegn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.gogol.net.cn/gtkpbuctry.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.52xcode.cn/gtjkfdften.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.meibo888.top/gtqiuiqhzc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yj202588.top/gtmrobkhyw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jinqigfzy.top/gtzvmjibze.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.pycfn.com/gtumizpsrk.html

[B02] 多分支 else if / elif
来源：http://hz.0kj1m.cn/gtlinyttdb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.daria6918.cn/gtkymoatfe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tanke756.top/gtlffxzjuz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cashguo.top/gtxoduztio.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yangfankeji.com/gtkzithfbt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.meibo888.top/gtracqylkz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yongpay.top/gtdputbqwx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.sufxvd.cn/gtimoxkabr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tian-w.cn/gtgkjdvolm.html

[B03] switch / match / case
来源：http://hz.iojbl.cn/gtpcaazmty.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.ivvv.top/gtepihlhws.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yangfankeji.com/gtegkarwle.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jyoumei.cn/gtadkybibm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xuetiantiany.cn/gtyjdcgtnz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.zhoulong.xyz/gtyqlyfhlv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yvedp.cn/gtwinkzyei.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cheryme.top/gtltxmndaf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.tanke756.top/gtsxanfefc.html

[B04] for 计数循环
来源：http://hz.jinyuanbaomall.cn/gtgenfudkg.html

Py:   for i in range(10): print(i)
来源：http://hz.tianlin.xyz/gtskqzoqxs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.pycfn.com/gtmmjoqwus.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.fengsongda.top/gtcfqeedcw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gotoacloud.top/gtcyzlzjug.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.jlsjyb.cn/gtbhnrfsqa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ydzc1.top/gtwafbplja.html

Ruby: 10.times { |i| puts i }
来源：http://hz.iojbl.cn/gtcyzarhkk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ppjwa.cn/gtuoidelpm.html

[B05] 遍历数组 / 列表
来源：http://hz.aibaodan.cn/gtfjkohmcz.html

Py:   for item in arr: print(item)
来源：http://hz.shanyushiyangtech.top/gtjgefxytc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yueranfly.top/gtypbyprit.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.guannengcc.top/gtzaugtnyk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgufenzy.top/gtmuvwyfsi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yongpay.top/gthjphpkqc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ywan-chungtsiang.top/gttmpkbnez.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sufxvd.cn/gthkdtnsst.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.0kj1m.cn/gtbijkqibo.html

[B06] 遍历字典 / 对象
来源：http://hz.wangshuangyany.cn/gtfhuhhwhy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.ehwqpu.com/gtrjelzcgd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.yj20258.top/gthoaowexa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhixingplan.top/gtkcijwshh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.daxiang520.top/gtolzcrqzd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hongshengwenyu.top/gtzxuohmnt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.sxryk.cn/gtqyeeedtf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yj20258888.top/gtibplleyv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hywenlv.cn/gtimajrrtb.html

[B07] while 循环
来源：http://hz.kuanghao11.cn/gtkvfmnsir.html

Py:   while i < 10: i += 1
来源：http://hz.zhongyouzk.top/gticajaoqv.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinqigfzy.top/gtfvfyxsgt.html

JS:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtvpwapwdp.html

TS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtlfoexufe.html

Java: while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtnbkcgfge.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.zhixingplan.top/gtqvztcxhb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hywenlv.cn/gtmcithzjr.html

C#:   while (i < 10) { i++; }
来源：http://hz.nwbrower.top/gtzkwpchvp.html

[B08] do-while（至少执行一次）
来源：http://hz.vqdsnc.cn/gtedxluxoz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jiagoushi.top/gtuciuaxsd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.9152youxi.cn/gtfvsbynev.html

JS:   do { i++; } while (i < 10);
来源：http://hz.9152youxi.cn/gtuvzaqhpw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtvtizhibq.html

Java: do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gtnvitgyun.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.wangshuangyany.cn/gtxaiswfcn.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhongyouzk.top/gtcnnexahd.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jyoumei.cn/gtmulnaebh.html

[B09] break 与 continue
来源：http://hz.chenjidiqi.icu/gtfsamcavg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhixingplan.top/gtdsxwgppc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.aibaodan.cn/gtmrmdzfxr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhoulong.xyz/gtpmphuabj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tian-w.cn/gtzczunsws.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtxqqjnslb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jyoumei.cn/gtxdazouhq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.9152youxi.cn/gtrwblerwj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tianlin.xyz/gtwncwvtew.html

[B10] 遍历同时拿索引
来源：http://hz.shangyingyoupin.top/gtrolobroa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shanyushiyangkeji.top/gtxpfjqyvb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhengqikj.top/gtxphvqhky.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xingfuxueyuan.xyz/gtdnpveikc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.gaohongyu789.top/gtkiohbhoo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shanyushiyangtech.top/gttrctxjsd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yj20258888.top/gtylslbcel.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aibaodan.cn/gtnjkuurcp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.havefunace.top/gtifyibkic.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhijiandao.cn/gtdpkzvepf.html

Py:   list(range(0, 10, 2))
来源：http://hz.yueranfly.top/gtgjoqamdz.html

PHP:  range(0, 10, 2);
来源：http://hz.c1oappe.top/gtpmfdijwk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangshuangyany.cn/gtyjakhnzh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.redwolf501.top/gtpfobhpse.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.nanxinkj.top/gtabbbcbow.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.havefunace.top/gttgzwpuoe.html

Ruby: (0...10).step(2).to_a
来源：http://hz.vqdsnc.cn/gtkrdnepqp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigufen.top/gtxdnaducu.html

[B12] 跳出多层循环
来源：http://hz.316326.xyz/gttnrcrhvd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.cucudq.cn/gtwapvewoy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yanxiufei.cn/gtzclrgupu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gtqddiyqom.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtcggewqce.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shanyushiyangtech.top/gtfecjfoug.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yonumen.top/gtwalvvubp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.gaohongyu789.top/gttdnbjutx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.vqdsnc.cn/gtakxrlcln.html

[B13] 判断是否为数字
来源：http://hz.chenlongwang.top/gtmkfbsnlq.html

Py:   isinstance(x, (int, float))
来源：http://hz.smart0.xyz/gtoshlkvjx.html

PHP:  is_numeric($x)
来源：http://hz.daria6918.cn/gtpdfhtkdw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gogol.net.cn/gtbaokhbgo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yuanzhike.top/gtkubwwadj.html

Java: x instanceof Number
来源：http://hz.shanyushiyangkeji.top/gtasawxlrq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.sysykeji.top/gtqxrjnklx.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yvedp.cn/gtcoyajbmw.html

C#:   x is int or double or decimal
来源：http://hz.sysykeji.top/gtseszylno.html

[B14] 判断值是否在集合内
来源：http://hz.wangshuangyany.cn/gtpnwvejaw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinqigfzy.top/gtidlkeyrs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shangyingyoupin.top/gtqhvrymyi.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigfzy.top/gtaokoklpm.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nanxinkj.top/gtcxmlexir.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gtssytator.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cucudq.cn/gtfndkyxym.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.yangfankeji.com/gtingvymxu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.c1oappe.top/gthmmcxsba.html

[B15] 布尔运算与取反
来源：http://hz.hywenlv.cn/gtpuyfcvyx.html

Py:   a and b or not c
来源：http://hz.jqgfzy.top/gtisbxeddt.html

PHP:  $a && $b || !$c
来源：http://hz.jinqigfzy.top/gtmamhunib.html

JS:   a && b || !c
来源：http://hz.cqqwz.cn/gtnmvfmugk.html

TS:   a && b || !c
来源：http://hz.dianchejie.cn/gtanwlxrqs.html

Java: a && b || !c
来源：http://hz.xuetiantiany.cn/gtdnvpczha.html

Go:   a && b || !c
来源：http://hz.hysaishi.cn/gtccyehrke.html

Ruby: a && b || !c
来源：http://hz.xuanzx.com/gtaagszgwm.html

C#:   a && b || !c
来源：http://hz.haohaochexian.top/gtzmusltps.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.mhx1999.top/gtwhdarqie.html

Py:   if not data: return
来源：http://hz.quarkkingdee.top/gtjixjroul.html

PHP:  if (!$data) { return; }
来源：http://hz.cucudq.cn/gtydbvrrcw.html

JS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gteydvpcsy.html

TS:   if (!data) return;
来源：http://hz.xinyue.icu/gthulwjhlv.html

Java: if (data == null) return;
来源：http://hz.yj20258.top/gtlzsszdhl.html

Go:   if data == nil { return }
来源：http://hz.mhx1999.top/gtrsrywtpz.html

Ruby: return if data.nil?
来源：http://hz.wangdashe.top/gtmyxenzva.html

C#:   if (data == null) return;
来源：http://hz.wangdashe.top/gtkbxalfui.html

================================================================================
来源：http://hz.316326.xyz/gtlyrrwifr.html

C. 函数与作用域
来源：http://hz.chenzaomai.com/gtglykhmuu.html

================================================================================
来源：http://hz.xziqi.cn/gtzkgtlokw.html

[C01] 定义函数
来源：http://hz.ydzc1.top/gtrqspruon.html

Py:   def add(a, b): return a + b
来源：http://hz.zhijiandao.cn/gtousjxrzt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtuoocwhgf.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.aibaodan.cn/gtyqlzdywz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gttefywulg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtvvisbdyp.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinyuanbaomall.cn/gtiseejknn.html

Ruby: def add(a, b); a + b; end
来源：http://hz.tian-w.cn/gtwvukyopp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xziqi.cn/gtxfvunnqs.html

[C02] 默认参数
来源：http://hz.sysykeji.top/gtnbmntgtf.html

Py:   def greet(name="World"): return name
来源：http://hz.pengpengdd.cyou/gttashhlyl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.daria6918.cn/gtemvdmfcd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.svipenyu.cn/gtsibxqosn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhengqikj.top/gtgulgllcx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.vqdsnc.cn/gtyttqkbrm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.hywenlv.cn/gtqucqsgqx.html

Ruby: def greet(name = "World") = name
来源：http://hz.iojbl.cn/gtlgfdboim.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gotoacloud.top/gtolhngoac.html

[C03] 可变参数
来源：http://hz.yueranfly.top/gtwhqdrqwm.html

Py:   def total(*args): return sum(args)
来源：http://hz.yonumen.top/gtwqgrtpcw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xylfe.cn/gtnapkzyxe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gtpvysjbkk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cqqwz.cn/gtgbbttwoi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.sysykeji.top/gtkcfmrgtg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxuanxn.top/gtszlkfftw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtebambpmy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xziqi.cn/gtycbndjqf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhengqikj.top/gtwoesguiz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xylfe.cn/gtcbzwufgp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.gogol.net.cn/gtmoujngfc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtpsvyuzwq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhiwuduotai.top/gtwhuwcvog.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sweek.top/gtttlfsllt.html

Go:   // 无：用配置结构体参数
来源：http://hz.andypj.xyz/gtlvvdsxyt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ppjwa.cn/gtaqsnzgjh.html

C#:   f(a: 1, b: 2)
来源：http://hz.nanxinkj.top/gtffdbuwkt.html

[C05] 返回多个值
来源：http://hz.hammf.cn/gtwuefcrpe.html


<!-- 参考信息 -->