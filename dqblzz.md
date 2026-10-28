代发 wailian999

Java: "第一行\n第二行"
来源：http://hz.yangfankeji.com/gtumuqzuew.html

Go:   "第一行\n第二行"
来源：http://hz.yj20258.top/gtvogtlgos.html

Ruby: "第一行\n第二行"
来源：http://hz.zhengqikj.top/gtcnlbqyqq.html

C#:   "第一行\n第二行"
来源：http://hz.gzhubu.top/gtaipknqgw.html

[A14] 注释写法
来源：http://hz.jianghu66.top/gtbtelgqgp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.xziqi.cn/gtzbfoklwo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.kuanghao11.cn/gtucmaxmoz.html

JS:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtuubrxixw.html

TS:   // 单行；/* 多行 */
来源：http://hz.yj202588.top/gtzqnfhjwo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhongyouzk.top/gtbxjyuugj.html

Go:   // 单行；/* 多行 */
来源：http://hz.c1oappe.top/gtltfyqqcw.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.jianghu66.top/gtycouexkg.html

C#:   // 单行；/* 多行 */
来源：http://hz.zhiwuduotai.top/gtwefjpnwg.html

[A15] 空值判断与默认值
来源：http://hz.guannengcc.top/gtlgsoekuv.html

Py:   value = data or "默认值"
来源：http://hz.zhengqikj.top/gthxoylqyj.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.gotoacloud.top/gtuwatsqsw.html

JS:   const value = data ?? "默认值";
来源：http://hz.hongshengwenyu.top/gtvpackqjr.html

TS:   const value = data ?? "默认值";
来源：http://hz.fzhhl.top/gtmmcvtlvi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.zhengqikj.top/gttrkslpoi.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.ivvv.top/gtvlurolor.html

Ruby: value = data || "默认值"
来源：http://hz.zycfv.cn/gteyjiulup.html

C#:   var value = data ?? "默认值";
来源：http://hz.jiagoushi.top/gtwhipfisi.html

[A16] 真假值判断规则
来源：http://hz.jqgufenzy.top/gtvkmbnkmu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.hnxiangtu.top/gthtwoxafs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.zhengqikj.top/gtjjtjsqbi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.hnxiangtu.top/gtpfbvrpyo.html

TS:   if (!x) {}
来源：http://hz.tian-w.cn/gtbfmjscks.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.redwolf501.top/gtzhgublfl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.meibo888.top/gteaneiznr.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.gzhubu.top/gthqstvxxh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.cdnleiting.top/gtcgztcaor.html

[A17] 位运算
来源：http://hz.jinqigufen.top/gtvlhsvmmo.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hywenlv.cn/gteyjdddwx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yvedp.cn/gtzpbmbsdn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jinghuilouyu.cn/gtwzykxion.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.chenjidiqi.icu/gtdmsaepzf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.bjfxy.top/gthzgvyxwc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hnxiangtu.top/gtngufgqvz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sweek.top/gtvxanxzth.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtpeonbkfi.html

[A18] 字符与 ASCII 码互转
来源：http://hz.nanxinkj.top/gtjvubrgjp.html

Py:   ord("A"); chr(65)
来源：http://hz.hnxiangtu.top/gtfdnhglnw.html

PHP:  ord("A"); chr(65)
来源：http://hz.316326.xyz/gtvzdfivay.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.zhijiandao.cn/gtfwynqzjk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinyuanbaomall.cn/gtzivtmhzq.html

Java: (int) 'A'; (char) 65
来源：http://hz.redwolf501.top/gtdztyksxv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.yuanzhike.top/gtsobigmkr.html

Ruby: "A".ord; 65.chr
来源：http://hz.havefunace.top/gtsktgvdgq.html

C#:   (int)'A'; (char)65
来源：http://hz.nanxinkj.top/gtnfgxhtzw.html

[A19] 交换两个变量
来源：http://hz.tian-w.cn/gtxhrpllfn.html

Py:   a, b = b, a
来源：http://hz.jqgfzy.top/gtxoronqhi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.cdnleiting.top/gtfzlqgzya.html

JS:   [a, b] = [b, a];
来源：http://hz.havefunace.top/gtocbqoayi.html

TS:   [a, b] = [b, a];
来源：http://hz.xinyue.icu/gtlqcgmbtt.html

Java: int t = a; a = b; b = t;
来源：http://hz.pycfn.com/gtzhcvpzev.html

Go:   a, b = b, a
来源：http://hz.hywenlv.cn/gtpktsftao.html

Ruby: a, b = b, a
来源：http://hz.dianchejie.cn/gtoufyjjzl.html

C#:   (a, b) = (b, a);
来源：http://hz.zhijiandao.cn/gtdwxmctcz.html

[A20] 读取标准输入
来源：http://hz.sufxvd.cn/gtidbjzygq.html

Py:   name = input("请输入：")
来源：http://hz.fengsongda.top/gtqqzukhfq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cqqwz.cn/gtagxmsnal.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.shanyushiyangkeji.top/gtnitgtoay.html

TS:   // Node.js：readline 模块
来源：http://hz.redwolf501.top/gtvacyyfdb.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yj20258.top/gtwltwgkap.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ppjwa.cn/gtqkzkhjqv.html

Ruby: gets.chomp
来源：http://hz.cqqwz.cn/gtntnzkwgc.html

C#:   Console.ReadLine();
来源：http://hz.daxiang520.top/gtcbcgixck.html

[A21] 保留指定小数位输出
来源：http://hz.ehwqpu.com/gthbkcqkrs.html

Py:   f"{3.14159:.2f}"
来源：http://hz.meibo888.top/gtrscqxndi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jqgfzy.top/gtuujrklwg.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sweek.top/gtcxyxmwuq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yuanzhike.top/gtzfukqjzk.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.smart0.xyz/gttbuvtbwn.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gtslnicusm.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.cheryme.top/gtwkxkavis.html

C#:   3.14159.ToString("F2")
来源：http://hz.xylfe.cn/gtkukhxcwk.html

[A22] 获取字符串长度
来源：http://hz.yvedp.cn/gtznrkoawc.html

Py:   len(s)
来源：http://hz.hysaishi.cn/gtjtrxvdfy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jyoumei.cn/gtpedlmplq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.316326.xyz/gttqhgjpop.html

TS:   s.length
来源：http://hz.yongpay.top/gtzmwltpdp.html

Java: s.length()
来源：http://hz.gaohongyu789.top/gtsstndqir.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.iojbl.cn/gtpbyauclx.html

Ruby: s.length
来源：http://hz.meibo888.top/gtyioahnjo.html

C#:   s.Length
来源：http://hz.quarkkingdee.top/gtibikiiyu.html

[A23] 大小写转换
来源：http://hz.316326.xyz/gtbzywvgal.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ehwqpu.com/gtpxavkxfx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.gzhubu.top/gtnktzdvxr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.nanxinkj.top/gtowalyzhy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ywan-chungtsiang.top/gtvqbtxwnk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.guowangkeji.top/gtyqzllabi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ywan-chungtsiang.top/gtcrgytwnp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhongyouzk.top/gtwkybzzsq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yuxming.cn/gtlheqtqad.html

[A24] 去除首尾空白
来源：http://hz.hongshengwenyu.top/gtjkromkaj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yanxiufei.cn/gtjmarnsjt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.ivvv.top/gtsgftpxss.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.gzhubu.top/gtonxxqseg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.svipenyu.cn/gtqpclfvcl.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.hywenlv.cn/gtmsamwvbw.html

Go:   strings.TrimSpace(s)
来源：http://hz.jqgufenzy.top/gtyvgrjzcz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.quarkkingdee.top/gtsupshehw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.dashuyun.cn/gthlbihcjh.html

[A25] 字符串比较
来源：http://hz.yj202588.top/gtvualvjsu.html

Py:   s1 == s2; s1 != s2
来源：http://hz.ydjk.org.cn/gtwvbglhyl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cdnleiting.top/gtksidyvin.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daria6918.cn/gtvknvnbfk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.0kj1m.cn/gtnsnsypqv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.guannengcc.top/gtonazobnt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.tanke756.top/gtgtllebcj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.iojbl.cn/gtdueyqrdu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.nanxuanxn.top/gtghubozdk.html

[A26] 类型转换总览
来源：http://hz.hongshengwenyu.top/gtgiuqpkhh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.xuetiantiany.cn/gtuskgoqdl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.ppjwa.cn/gtyubwdcjl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinghuilouyu.cn/gtoqgeonwo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xuetiantiany.cn/gtpgpyvzex.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yuanzhike.top/gtcjzblrzb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.daxiang520.top/gtqpklffsi.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dianchejie.cn/gtzktxullo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.shuidangran.top/gtbpikhhdp.html

================================================================================
来源：http://hz.hywenlv.cn/gtmpxqtryl.html

B. 流程控制
来源：http://hz.havefunace.top/gtmcptgjcm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtscovyvaq.html

[B01] 条件判断 if / else
来源：http://hz.jqgfzy.top/gtmlwyniyq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.shanyushiyangtech.top/gtpfigoxig.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.cheryme.top/gtvrtualjf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtckyyfnof.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jiagoushi.top/gttzrynjpf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.hnqzz.top/gtbtjcahfx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.shzxlz.cn/gtopatvsto.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.gotoacloud.top/gtyiaiiszq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtjxdbvqod.html

[B02] 多分支 else if / elif
来源：http://hz.jinghuilouyu.cn/gtrmckamtr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.gotoacloud.top/gtngyhccva.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ywan-chungtsiang.top/gtqvcdjcah.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gthzwhbjjn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhoulong.xyz/gtmydusrdo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtodzyvmqa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.xziqi.cn/gtxgowqoqp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hysaishi.cn/gthgfjlwhn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenzaomai.com/gtslcetvwl.html

[B03] switch / match / case
来源：http://hz.chenlongwang.top/gtfjhhfmyz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jlsjyb.cn/gtohmwcetr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gzhubu.top/gtdebxoqat.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenzaomai.com/gtpgilzedm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aizwys.cn/gtvwdhvohu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cdnleiting.top/gtfuhczbvq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ywan-chungtsiang.top/gtklmeprew.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jlsjyb.cn/gtvmrvkkyp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.nwbrower.top/gtfprbafrb.html

[B04] for 计数循环
来源：http://hz.yueranfly.top/gtilzqdgjp.html

Py:   for i in range(10): print(i)
来源：http://hz.shzxlz.cn/gtbjvcuasl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yongpay.top/gtkhvltqsp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hnxiangtu.top/gtkglfxwcn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.iojbl.cn/gtudxqwvbu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hnqzz.top/gtmcnrsydg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.316326.xyz/gtqgvwocpm.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shangyingyoupin.top/gtmuujbxfj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.tianlin.xyz/gtbsrkfaxc.html

[B05] 遍历数组 / 列表
来源：http://hz.0kj1m.cn/gtwhnzhyje.html

Py:   for item in arr: print(item)
来源：http://hz.gaohongyu789.top/gtafkpkdwj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.redwolf501.top/gtruwibmay.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jianghu66.top/gtslednowr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hysaishi.cn/gtulvpwrip.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.vqdsnc.cn/gthrjyidop.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.sweek.top/gtkcxvwyzi.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yj20258.top/gtlogxueyi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.9152youxi.cn/gtsxqwxgrj.html

[B06] 遍历字典 / 对象
来源：http://hz.meibo888.top/gtsqllyvqw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.fengsongda.top/gtbhiqbvmi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.feifeiyinyue.top/gtljwmysxb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hywenlv.cn/gthpieeaer.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.cheryme.top/gtuqzjyhyd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.sysykeji.top/gtnzlhtwtd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hnxiangtu.top/gtskekynrx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.svipenyu.cn/gttmifgrfh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.iojbl.cn/gtwlitczie.html

[B07] while 循环
来源：http://hz.hywenlv.cn/gtdpkahbqz.html

Py:   while i < 10: i += 1
来源：http://hz.meibo888.top/gtwjymcqxz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.kuanghao11.cn/gtskghqiwj.html

JS:   while (i < 10) { i++; }
来源：http://hz.yangfankeji.com/gtjvrgtjly.html

TS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtgckvecxf.html

Java: while (i < 10) { i++; }
来源：http://hz.cqqwz.cn/gtjttcecoo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hnqzz.top/gtkforonuj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.mhx1999.top/gtdtucstse.html

C#:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtzjkzuvie.html

[B08] do-while（至少执行一次）
来源：http://hz.shangyingyoupin.top/gtcojbfjww.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinqigufen.top/gtiweoupav.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gaohongyu789.top/gtbkhntdex.html

JS:   do { i++; } while (i < 10);
来源：http://hz.ppjwa.cn/gtsqhcnttg.html

TS:   do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtvveulteq.html

Java: do { i++; } while (i < 10);
来源：http://hz.cdnleiting.top/gtajakxquo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.shuidangran.top/gtjmlloezx.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.52xcode.cn/gtfaxxcpup.html

C#:   do { i++; } while (i < 10);
来源：http://hz.wangdashe.top/gtgpjuzsqw.html

[B09] break 与 continue
来源：http://hz.dashuyun.cn/gtblbmgumh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tian-w.cn/gtxtxlgabh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.yonumen.top/gtaevtsfly.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.smart0.xyz/gtbbethouy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtmnuodcik.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtnmazlrfv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xziqi.cn/gtssdsapyn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yj202588.top/gtumwgefss.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtunfgthsz.html

[B10] 遍历同时拿索引
来源：http://hz.jinghuilouyu.cn/gtifbaavde.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zhijiandao.cn/gtkjbrzivk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.xuanzx.com/gtrjtzvqqm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.iojbl.cn/gtaznzvrsh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.smart0.xyz/gttzhjthyn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.bjfxy.top/gtrkeqcsfu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.ydzc1.top/gtcpmmgije.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jiagoushi.top/gttzjasnvl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jinqigufen.top/gtowhqsmyo.html

[B11] 生成数字序列 / 区间
来源：http://hz.gotoacloud.top/gtdwsclqyh.html

Py:   list(range(0, 10, 2))
来源：http://hz.vqdsnc.cn/gtnwybmfqb.html

PHP:  range(0, 10, 2);
来源：http://hz.hysaishi.cn/gtzillurzm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.shuidangran.top/gtkflfufyb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yvedp.cn/gtjjsnwkil.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ybcxt.top/gtnjajxuhi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xziqi.cn/gthjuvwozi.html

Ruby: (0...10).step(2).to_a
来源：http://hz.pengpengdd.cyou/gtzfouscbq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.gzhubu.top/gtkdmkyhpe.html

[B12] 跳出多层循环
来源：http://hz.chenzaomai.com/gtpvfeleen.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxinkj.top/gtektshspf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.svipenyu.cn/gtlrhjbaox.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jlsjyb.cn/gtbavrazuv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtdtykhqyh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.mhx1999.top/gtuschadvv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cqqwz.cn/gtayarhret.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.jyoumei.cn/gtaxemiwbb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jinqigufen.top/gtcmblxkqw.html

[B13] 判断是否为数字
来源：http://hz.aizwys.cn/gtgbcjxwej.html

Py:   isinstance(x, (int, float))
来源：http://hz.tanke756.top/gtkoicnfct.html

PHP:  is_numeric($x)
来源：http://hz.cqqwz.cn/gtrpfvwefk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shangyingyoupin.top/gtwnkzotme.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gtjmtmzvlh.html

Java: x instanceof Number
来源：http://hz.zhongyouzk.top/gtdxiycnen.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xuanzx.com/gtvwimhucn.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zycfv.cn/gtczdtftxb.html

C#:   x is int or double or decimal
来源：http://hz.yanxiufei.cn/gtgqozlhhh.html

[B14] 判断值是否在集合内
来源：http://hz.pycfn.com/gtcdezoukr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.guowangkeji.top/gthukhowme.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.cashguo.top/gttldvmxvs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hongshengwenyu.top/gtmoolmuyk.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigufen.top/gtanwhreib.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gtwlhjdmgb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hywenlv.cn/gtjylikptt.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xziqi.cn/gtptpygogq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cheryme.top/gtbzzcxkud.html

[B15] 布尔运算与取反
来源：http://hz.jinghuilouyu.cn/gttkgxylgd.html

Py:   a and b or not c
来源：http://hz.redwolf501.top/gtdptexggi.html

PHP:  $a && $b || !$c
来源：http://hz.jqgfzy.top/gtjdhzktdy.html

JS:   a && b || !c
来源：http://hz.bjfxy.top/gtmsamzqid.html

TS:   a && b || !c
来源：http://hz.zhijiandao.cn/gtyjrhexui.html

Java: a && b || !c
来源：http://hz.wangdashe.top/gtwlwjdmle.html

Go:   a && b || !c
来源：http://hz.zhixingplan.top/gtwznlutvj.html

Ruby: a && b || !c
来源：http://hz.jianghu66.top/gtlicobepq.html

C#:   a && b || !c
来源：http://hz.hammf.cn/gtnljzuior.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cheryme.top/gtugrwubfy.html

Py:   if not data: return
来源：http://hz.jinqigfzy.top/gtofvuhxpg.html

PHP:  if (!$data) { return; }
来源：http://hz.hnqzz.top/gtlsgbkvoi.html

JS:   if (!data) return;
来源：http://hz.cucudq.cn/gtxydbzccp.html

TS:   if (!data) return;
来源：http://hz.nanxinkj.top/gtvnntrbmb.html

Java: if (data == null) return;
来源：http://hz.kuanghao11.cn/gtgdtxmnpl.html

Go:   if data == nil { return }
来源：http://hz.nwbrower.top/gtyvrxsrae.html

Ruby: return if data.nil?
来源：http://hz.pycfn.com/gtdybtaapr.html

C#:   if (data == null) return;
来源：http://hz.aizwys.cn/gtlzbrjkkf.html

================================================================================
来源：http://hz.0kj1m.cn/gtqbmanvvz.html

C. 函数与作用域
来源：http://hz.iojbl.cn/gtowbeaexu.html

================================================================================
来源：http://hz.nanxinkj.top/gtdhdylqdb.html

[C01] 定义函数
来源：http://hz.daxiang520.top/gtjchfvlbd.html

Py:   def add(a, b): return a + b
来源：http://hz.pycfn.com/gtrfhyymat.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gotoacloud.top/gtjcjetnov.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.redwolf501.top/gtxzboykou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtkorrwxqm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtamilhwit.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.guannengcc.top/gttrtmupur.html

Ruby: def add(a, b); a + b; end
来源：http://hz.andypj.xyz/gtxxrilaug.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtecpkcewr.html

[C02] 默认参数
来源：http://hz.yuxming.cn/gtnvnscbjm.html

Py:   def greet(name="World"): return name
来源：http://hz.bjfxy.top/gtunvwiemg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.smart0.xyz/gtlzkppibg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ppjwa.cn/gtnimkwfbf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhongyouzk.top/gtsbylsdwp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yj202588.top/gtjqwxblve.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.chenlongwang.top/gtqfnmvqhz.html

Ruby: def greet(name = "World") = name
来源：http://hz.nanxuanxn.top/gtxfxraaou.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hnxiangtu.top/gtftkncwwz.html

[C03] 可变参数
来源：http://hz.wangshuangyany.cn/gthqyxsdir.html

Py:   def total(*args): return sum(args)
来源：http://hz.tian-w.cn/gtvejrlfxi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.snrcjt.cn/gtnsmhdwia.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.feifeiyinyue.top/gtvtzaawio.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhoulong.xyz/gtcfucfkqo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cheryme.top/gtsxyxegqy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuanzhike.top/gtggjwgntl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tanke756.top/gtoleghafh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ydzc1.top/gtfqqrvisi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cucudq.cn/gtzssfylks.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenzaomai.com/gthzpiuhfv.html


<!-- 参考信息 -->