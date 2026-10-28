代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.haohaochexian.top/gtnglywzjg.html

Go:   "第一行\n第二行"
来源：http://hz.aizwys.cn/gttkthqdds.html

Ruby: "第一行\n第二行"
来源：http://hz.mhx1999.top/gtyftfbplj.html

C#:   "第一行\n第二行"
来源：http://hz.52xcode.cn/gteuvlqgfa.html

[A14] 注释写法
来源：http://hz.fzhhl.top/gtspqfhkda.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.hysaishi.cn/gtxeepqcms.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.meibo888.top/gtzzbwxbwn.html

JS:   // 单行；/* 多行 */
来源：http://hz.ybcxt.top/gtbaiombrf.html

TS:   // 单行；/* 多行 */
来源：http://hz.yueranfly.top/gtnlhnfvug.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.hammf.cn/gtblnstyor.html

Go:   // 单行；/* 多行 */
来源：http://hz.xuetiantiany.cn/gtcuwehvkg.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.yj202588.top/gtuxpvfukv.html

C#:   // 单行；/* 多行 */
来源：http://hz.tianlin.xyz/gtsvcgzhrn.html

[A15] 空值判断与默认值
来源：http://hz.svipenyu.cn/gtlkktcsei.html

Py:   value = data or "默认值"
来源：http://hz.birdmap.top/gtcpggewjy.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.guowangkeji.top/gtevnrtwcb.html

JS:   const value = data ?? "默认值";
来源：http://hz.daxiang520.top/gthkxoinvx.html

TS:   const value = data ?? "默认值";
来源：http://hz.sxryk.cn/gtegraypru.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.nwbrower.top/gtazbtgcjz.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.shanyushiyangtech.top/gtqjpstpev.html

Ruby: value = data || "默认值"
来源：http://hz.cucudq.cn/gttsbyrzpp.html

C#:   var value = data ?? "默认值";
来源：http://hz.redwolf501.top/gtpztlbafc.html

[A16] 真假值判断规则
来源：http://hz.jinqigfzy.top/gtnszfphui.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.guannengcc.top/gtrjiryknl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.0kj1m.cn/gtjauvjojh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hysaishi.cn/gtcuamqsmp.html

TS:   if (!x) {}
来源：http://hz.jinqigfzy.top/gtbnlavryb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.gogol.net.cn/gtiudawigs.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jinqigfzy.top/gthbqyhhgc.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.xuanzx.com/gtxyqgteil.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.yuxming.cn/gtzrnlavim.html

[A17] 位运算
来源：http://hz.tianlin.xyz/gtpvcxluoa.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yueranfly.top/gtuhxrvrob.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yueranfly.top/gtzzaomkul.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xinyue.icu/gtroqakcnd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.ppjwa.cn/gtshfnpdqw.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.wangshuangyany.cn/gtbnkstmmj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.dianchejie.cn/gtzycltwzu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gttbjjuaim.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yanxiufei.cn/gtbiucjxcb.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ywan-chungtsiang.top/gtkomixymt.html

Py:   ord("A"); chr(65)
来源：http://hz.fengsongda.top/gtldmwvddb.html

PHP:  ord("A"); chr(65)
来源：http://hz.yonumen.top/gtrexegqcd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xuetiantiany.cn/gtstdeefsk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhijiandao.cn/gteccmtsgx.html

Java: (int) 'A'; (char) 65
来源：http://hz.hnqzz.top/gtjjdrrjrb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.ybcxt.top/gtcnbzprfn.html

Ruby: "A".ord; 65.chr
来源：http://hz.pengpengdd.cyou/gtrmiwotno.html

C#:   (int)'A'; (char)65
来源：http://hz.xziqi.cn/gtnpeknxhw.html

[A19] 交换两个变量
来源：http://hz.gaohongyu789.top/gtifkfnyrf.html

Py:   a, b = b, a
来源：http://hz.yongpay.top/gtlhttcagw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.wangdashe.top/gtajknxrux.html

JS:   [a, b] = [b, a];
来源：http://hz.fzhhl.top/gtsxnbefox.html

TS:   [a, b] = [b, a];
来源：http://hz.fengsongda.top/gtwtkorpen.html

Java: int t = a; a = b; b = t;
来源：http://hz.fzhhl.top/gtnustxkmv.html

Go:   a, b = b, a
来源：http://hz.pycfn.com/gthitsdmfi.html

Ruby: a, b = b, a
来源：http://hz.tanke756.top/gtcrpincee.html

C#:   (a, b) = (b, a);
来源：http://hz.ydjk.org.cn/gtpjbzedib.html

[A20] 读取标准输入
来源：http://hz.shzxlz.cn/gtsixshqik.html

Py:   name = input("请输入：")
来源：http://hz.daxiang520.top/gtbphcfgnh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hnqzz.top/gtsprwrarc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.ivvv.top/gtoccghdqm.html

TS:   // Node.js：readline 模块
来源：http://hz.jlsjyb.cn/gtroriiyuq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.gaohongyu789.top/gtzpqsxhoq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.feifeiyinyue.top/gtcxbvdwfz.html

Ruby: gets.chomp
来源：http://hz.iojbl.cn/gtmxkmcxvl.html

C#:   Console.ReadLine();
来源：http://hz.mhx1999.top/gtaedxjqxb.html

[A21] 保留指定小数位输出
来源：http://hz.jiagoushi.top/gtlqumkgvb.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cheryme.top/gthbetdvoq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.snrcjt.cn/gtzikpfggz.html

JS:   (3.14159).toFixed(2)
来源：http://hz.tanke756.top/gtojzrftdi.html

TS:   (3.14159).toFixed(2)
来源：http://hz.daria6918.cn/gtnfebapgh.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jqgfzy.top/gtssippokh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.birdmap.top/gtreqpvtxq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.nanxinkj.top/gtfwgwpwsz.html

C#:   3.14159.ToString("F2")
来源：http://hz.jyoumei.cn/gtscquazqd.html

[A22] 获取字符串长度
来源：http://hz.feifeiyinyue.top/gtckcprnyx.html

Py:   len(s)
来源：http://hz.ydjk.org.cn/gtjatwgner.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.smart0.xyz/gtvugkjzoi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.yonumen.top/gtveywsztz.html

TS:   s.length
来源：http://hz.xylfe.cn/gtuwulvozq.html

Java: s.length()
来源：http://hz.haohaochexian.top/gttamnuvpl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cashguo.top/gtwzwvhpbq.html

Ruby: s.length
来源：http://hz.pengpengdd.cyou/gtgaqnckvl.html

C#:   s.Length
来源：http://hz.zhongyouzk.top/gthtbyxmsu.html

[A23] 大小写转换
来源：http://hz.zhoulong.xyz/gttczorbks.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.sweek.top/gtrqchltnh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xuanzx.com/gtdvlgtfds.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hammf.cn/gtsrumqhav.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.dianchejie.cn/gtbplfhzyt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.tian-w.cn/gtoimvqpjp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.hongshengwenyu.top/gtzeqcgnvq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.jinghuilouyu.cn/gtlggagmyt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.andypj.xyz/gtooevvhev.html

[A24] 去除首尾空白
来源：http://hz.gzhubu.top/gtspoexxjl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yongpay.top/gtlympeffn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xziqi.cn/gtufaysftt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuetiantiany.cn/gtfbgefyws.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jlsjyb.cn/gtnehotmtd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jinqigfzy.top/gtctsxukem.html

Go:   strings.TrimSpace(s)
来源：http://hz.jinghuilouyu.cn/gtixskrxrr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.316326.xyz/gtqueqhjyj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.svipenyu.cn/gtgpvfucmh.html

[A25] 字符串比较
来源：http://hz.shangyingyoupin.top/gtqnzmxsxj.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhixingplan.top/gtzakohamd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.nanxuanxn.top/gtgmgzkuko.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.fzhhl.top/gtmsurybfe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.smart0.xyz/gtnisnzkhc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.hnqzz.top/gtxhxhyagr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.xylfe.cn/gturthwmhh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.c1oappe.top/gtosupfdfq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.kuanghao11.cn/gtlbopirtx.html

[A26] 类型转换总览
来源：http://hz.daxiang520.top/gtqavneleb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.svipenyu.cn/gtkdkzrika.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jqgufenzy.top/gtfurtpghq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hysaishi.cn/gtdxzfojyj.html

TS:   Number() String() Boolean() x as number
来源：http://hz.zhaomingkeji.xyz/gtqfwuafsb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shanyushiyangkeji.top/gtusnruvqj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.havefunace.top/gtggpsinas.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hywenlv.cn/gtggzxxcrx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhijiandao.cn/gtojeeuhxk.html

================================================================================
来源：http://hz.ybcxt.top/gtwbaqwnoh.html

B. 流程控制
来源：http://hz.xylfe.cn/gtqmfbuuac.html

================================================================================
来源：http://hz.quarkkingdee.top/gtegshmbyc.html

[B01] 条件判断 if / else
来源：http://hz.xinyue.icu/gtrtxstaja.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shanyushiyangtech.top/gthufqtwaq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.jqgufenzy.top/gtratxvuos.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtsuhcfdcb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yj202588.top/gtslbgajbe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.shzxlz.cn/gtjavcmgfv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.shuidangran.top/gtovxkzpre.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.ydjk.org.cn/gtxaxdyrkx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhaomingkeji.xyz/gtyeuixxva.html

[B02] 多分支 else if / elif
来源：http://hz.tanke756.top/gtlrtnwdfi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.wangshuangyany.cn/gtlpxabhyy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.chenzaomai.com/gtvvbsgevt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtmhaovzoq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtxeukpocc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gtgdoezfwi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hfpthk.cn/gtmsqbdjpf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zycfv.cn/gtlldoscjt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gtortnaxmh.html

[B03] switch / match / case
来源：http://hz.ybcxt.top/gtddaribej.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.yj20258.top/gthtywticx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gaohongyu789.top/gtcoapcoyh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.wangdashe.top/gtyzvlkdxo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yj202588.top/gtxldxuvtt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.svipenyu.cn/gtmhlxveii.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhaomingkeji.xyz/gtsaujwcze.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cdnleiting.top/gtmajxnjis.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.pycfn.com/gtucsybutu.html

[B04] for 计数循环
来源：http://hz.jiagoushi.top/gtmhvrmnhq.html

Py:   for i in range(10): print(i)
来源：http://hz.andypj.xyz/gthfbywfxs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.sysykeji.top/gtdkpcdpbb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yueranfly.top/gtvvownovd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cdnleiting.top/gtgageebkd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.sweek.top/gtugccyyra.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.tanke756.top/gtydtonaca.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jyoumei.cn/gtfmnephef.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.svipenyu.cn/gtjqbisimj.html

[B05] 遍历数组 / 列表
来源：http://hz.yvedp.cn/gtcavcgldf.html

Py:   for item in arr: print(item)
来源：http://hz.ehwqpu.com/gtdohhydat.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.316326.xyz/gtqveilvmn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.xylfe.cn/gtjpvrtegy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinghuilouyu.cn/gtofxdjumr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zycfv.cn/gtbbljnsuq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.pengpengdd.cyou/gtslsadelv.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hywenlv.cn/gtbltszonm.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ybcxt.top/gtipgspeyp.html

[B06] 遍历字典 / 对象
来源：http://hz.ybcxt.top/gtbxeigkxu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sweek.top/gtcpmqqrvz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.ppjwa.cn/gtwsncuvoz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cucudq.cn/gtykyaxpgd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ivvv.top/gtrwnjecug.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.fengsongda.top/gtytwqqate.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinqigufen.top/gtnvqsgctv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.svipenyu.cn/gtqqtconlz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.hywenlv.cn/gtmmptsugr.html

[B07] while 循环
来源：http://hz.aizwys.cn/gtuzpafjft.html

Py:   while i < 10: i += 1
来源：http://hz.aizwys.cn/gtcpdwmgtc.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.bjfxy.top/gterkafbem.html

JS:   while (i < 10) { i++; }
来源：http://hz.guowangkeji.top/gtsuuyzthw.html

TS:   while (i < 10) { i++; }
来源：http://hz.c1oappe.top/gtbbcdaanl.html

Java: while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtnffjwpyn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hywenlv.cn/gtniazxcfj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ehwqpu.com/gtlxnwdevk.html

C#:   while (i < 10) { i++; }
来源：http://hz.sufxvd.cn/gtopoghyji.html

[B08] do-while（至少执行一次）
来源：http://hz.tianlin.xyz/gtutclexmr.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.haohaochexian.top/gtcqrivzha.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yonumen.top/gtnlfyohdc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.svipenyu.cn/gtgsvgxsrc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.wangshuangyany.cn/gtwpkymmmc.html

Java: do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtzzcwwjzv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhijiandao.cn/gtiemjkeqd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhaomingkeji.xyz/gtxajywxmc.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gtdqxpwqmo.html

[B09] break 与 continue
来源：http://hz.sweek.top/gtwphjkjsn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.hywenlv.cn/gtcbrojlve.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.andypj.xyz/gttqwhvwqc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtgqynhujb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yuxming.cn/gtooamqtlk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtyyyunnfu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ivvv.top/gtmgjieili.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.ppjwa.cn/gtrssetgel.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.bjfxy.top/gtedarcuzi.html

[B10] 遍历同时拿索引
来源：http://hz.ydzc1.top/gtfuowimcz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sufxvd.cn/gtfwxnhvgs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tianlin.xyz/gtlemrbtom.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.ehwqpu.com/gtxjkdkrxi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.aibaodan.cn/gtdrsejqkc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.redwolf501.top/gtbdyeytjn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.havefunace.top/gtmknlhcvh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sweek.top/gtwbwwgpjq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.fzhhl.top/gtdfbxbgzq.html

[B11] 生成数字序列 / 区间
来源：http://hz.daria6918.cn/gtvvhorghb.html

Py:   list(range(0, 10, 2))
来源：http://hz.yueranfly.top/gtyhsjyuxr.html

PHP:  range(0, 10, 2);
来源：http://hz.daria6918.cn/gtwomjraxe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hongshengwenyu.top/gtckigsgdd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtwaxdbohg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigfzy.top/gtcqjxyvsz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.fzhhl.top/gtqvfvxvbi.html

Ruby: (0...10).step(2).to_a
来源：http://hz.guannengcc.top/gtxaeqfrsz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zdqjudy.top/gtvyujyepq.html

[B12] 跳出多层循环
来源：http://hz.yj20258888.top/gtojjusrku.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.aibaodan.cn/gtcatcevvg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.chenzaomai.com/gtryfhnorm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhixingplan.top/gtkdsaniwu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ivvv.top/gtvrjrwkyb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtziitoqeb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.zhixingplan.top/gtglnmqpqb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yueranfly.top/gtqonehiil.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.svipenyu.cn/gtapxbvmfn.html

[B13] 判断是否为数字
来源：http://hz.jlsjyb.cn/gtebtcoawa.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinghuilouyu.cn/gtiagslsjb.html

PHP:  is_numeric($x)
来源：http://hz.redwolf501.top/gtbweftpsr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shangyingyoupin.top/gtiemeysky.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.9152youxi.cn/gtedheaykk.html

Java: x instanceof Number
来源：http://hz.hammf.cn/gthtpfqvlj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.tianlin.xyz/gtksrmkfqs.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jyoumei.cn/gtdxzubhfg.html

C#:   x is int or double or decimal
来源：http://hz.yonumen.top/gtasrsqgyq.html

[B14] 判断值是否在集合内
来源：http://hz.yuxming.cn/gttbpaxdbp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.hongshengwenyu.top/gtggyonjfh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jlsjyb.cn/gtnhjgipfy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yonumen.top/gtjrbxjdup.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yangfankeji.com/gtbiaasvuq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gtkqrmvtnr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yanxiufei.cn/gtmwwgyzjd.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinqigufen.top/gtwhqtmadz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.ydzc1.top/gtvkmknlzf.html

[B15] 布尔运算与取反
来源：http://hz.shuidangran.top/gtubqtuhkj.html

Py:   a and b or not c
来源：http://hz.ydjk.org.cn/gtalqugbes.html

PHP:  $a && $b || !$c
来源：http://hz.dianchejie.cn/gtaickyutu.html

JS:   a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtevstzhro.html

TS:   a && b || !c
来源：http://hz.havefunace.top/gtispkklmd.html

Java: a && b || !c
来源：http://hz.wangshuangyany.cn/gtexxirytk.html

Go:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtiqxssypo.html

Ruby: a && b || !c
来源：http://hz.havefunace.top/gtzxbnsfdd.html

C#:   a && b || !c
来源：http://hz.jiagoushi.top/gtfdyofqvl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.zhoulong.xyz/gtvvfkqull.html

Py:   if not data: return
来源：http://hz.yj20258.top/gtkwtbpkrx.html

PHP:  if (!$data) { return; }
来源：http://hz.cdnleiting.top/gtsffzwsyx.html

JS:   if (!data) return;
来源：http://hz.wangdashe.top/gtngrnsqba.html

TS:   if (!data) return;
来源：http://hz.yongpay.top/gtmlquprxp.html

Java: if (data == null) return;
来源：http://hz.xuanzx.com/gtbpucqpix.html

Go:   if data == nil { return }
来源：http://hz.feifeiyinyue.top/gtgbmcqteo.html

Ruby: return if data.nil?
来源：http://hz.zhixingplan.top/gtcupyxhgk.html

C#:   if (data == null) return;
来源：http://hz.pengpengdd.cyou/gtxlkifaep.html

================================================================================
来源：http://hz.jyoumei.cn/gtcdelzdoa.html

C. 函数与作用域
来源：http://hz.smart0.xyz/gtqgbaqhbr.html

================================================================================
来源：http://hz.guannengcc.top/gtqbczfbna.html

[C01] 定义函数
来源：http://hz.hfpthk.cn/gtjntfhjgv.html

Py:   def add(a, b): return a + b
来源：http://hz.daxiang520.top/gtabbghuey.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hfpthk.cn/gtvhjhheqq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yvedp.cn/gtrefgryzx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gtfxddoqkc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtshgbubso.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.vqdsnc.cn/gtasldfapb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.gogol.net.cn/gtcdlxkfbt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtduamadxd.html

[C02] 默认参数
来源：http://hz.shanyushiyangtech.top/gtwvznozxk.html

Py:   def greet(name="World"): return name
来源：http://hz.gotoacloud.top/gtexoolciq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cheryme.top/gtqlmmqmrw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.smart0.xyz/gtsvzujnfo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.cdnleiting.top/gtfpjnlyzb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.tianlin.xyz/gtjklqjxrj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhengqikj.top/gtbkmwvqtt.html

Ruby: def greet(name = "World") = name
来源：http://hz.redwolf501.top/gtwpurbcaq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yongpay.top/gtghmlvrei.html

[C03] 可变参数
来源：http://hz.cashguo.top/gtfbybyfno.html

Py:   def total(*args): return sum(args)
来源：http://hz.yuanzhike.top/gtfadwopns.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinqigufen.top/gtpwurpwen.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jyoumei.cn/gtewiniglk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hfpthk.cn/gtabuedkhp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xinyue.icu/gtsgfgsidu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhoulong.xyz/gtvspgyohr.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yueranfly.top/gtpuratdwe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hnxiangtu.top/gtpjkndxea.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yueranfly.top/gtyusqwovv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gaohongyu789.top/gtdneetdfz.html


<!-- 参考信息 -->