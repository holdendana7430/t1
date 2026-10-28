代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.bjfxy.top/gtdmepkqva.html

C#:   var value = data ?? "默认值";
来源：http://hz.xingfuxueyuan.xyz/gthbgwwctf.html

[A16] 真假值判断规则
来源：http://hz.shanyushiyangkeji.top/gtifvntbug.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.yuxming.cn/gtfnrjuxez.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.jiagoushi.top/gtfdvpiuoh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.316326.xyz/gtjbmanbpm.html

TS:   if (!x) {}
来源：http://hz.hammf.cn/gttpnmvkje.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jlsjyb.cn/gttzrnsjxi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jiagoushi.top/gtcpnrbbrn.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.wangshuangyany.cn/gtvuoxgtdt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.cdnleiting.top/gtphseinns.html

[A17] 位运算
来源：http://hz.jqgfzy.top/gtiorzxbwh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtoftgpkuf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.haohaochexian.top/gtjtiuyasr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yongpay.top/gtiwcsrkwl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtlrwpcrqe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.c1oappe.top/gtnkfbekfh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jqgfzy.top/gtpioenohg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sysykeji.top/gtywrybbip.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.daria6918.cn/gtazzpangu.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jianghu66.top/gtiwobyqvt.html

Py:   ord("A"); chr(65)
来源：http://hz.ydjk.org.cn/gtvojpkpmg.html

PHP:  ord("A"); chr(65)
来源：http://hz.jqgufenzy.top/gtykfbehqj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nwbrower.top/gtgacycehj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yj20258.top/gthjxgzlby.html

Java: (int) 'A'; (char) 65
来源：http://hz.pengpengdd.cyou/gtczoflgew.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.cashguo.top/gtfgjxkfjm.html

Ruby: "A".ord; 65.chr
来源：http://hz.cheryme.top/gtdjarhchu.html

C#:   (int)'A'; (char)65
来源：http://hz.fzhhl.top/gthpnivjif.html

[A19] 交换两个变量
来源：http://hz.chenlongwang.top/gtfqpfjphi.html

Py:   a, b = b, a
来源：http://hz.jiagoushi.top/gttdiworuk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jqgufenzy.top/gtjquqvzti.html

JS:   [a, b] = [b, a];
来源：http://hz.yuanzhike.top/gtjxbrnlly.html

TS:   [a, b] = [b, a];
来源：http://hz.wangdashe.top/gtoxuvghob.html

Java: int t = a; a = b; b = t;
来源：http://hz.guannengcc.top/gtzblkxjzl.html

Go:   a, b = b, a
来源：http://hz.c1oappe.top/gtglpdzdse.html

Ruby: a, b = b, a
来源：http://hz.xinyue.icu/gtnsmgdlcv.html

C#:   (a, b) = (b, a);
来源：http://hz.yuxming.cn/gtdsmrchou.html

[A20] 读取标准输入
来源：http://hz.yongpay.top/gtbtlxykqv.html

Py:   name = input("请输入：")
来源：http://hz.sweek.top/gtcfzjfcum.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.shangyingyoupin.top/gtadzjlael.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.pycfn.com/gtexblmvyn.html

TS:   // Node.js：readline 模块
来源：http://hz.jyoumei.cn/gtlbrqipht.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.gaohongyu789.top/gtyegcmcmm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.pycfn.com/gtvfxzuyks.html

Ruby: gets.chomp
来源：http://hz.shanyushiyangtech.top/gthchspxzy.html

C#:   Console.ReadLine();
来源：http://hz.jqgufenzy.top/gtzlararrr.html

[A21] 保留指定小数位输出
来源：http://hz.pycfn.com/gtgzvolvzd.html

Py:   f"{3.14159:.2f}"
来源：http://hz.svipenyu.cn/gtwxrixuxp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.yuxming.cn/gtnpepdysw.html

JS:   (3.14159).toFixed(2)
来源：http://hz.pycfn.com/gtaewycafp.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zdqjudy.top/gtqxmlfzkr.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shangyingyoupin.top/gtvyslvjfe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinghuilouyu.cn/gtyxvhmadq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yj202588.top/gttxjejjew.html

C#:   3.14159.ToString("F2")
来源：http://hz.fzhhl.top/gtuxldxehb.html

[A22] 获取字符串长度
来源：http://hz.zhiwuduotai.top/gtmzivalaj.html

Py:   len(s)
来源：http://hz.cucudq.cn/gtztnnbydg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.svipenyu.cn/gtvwbdbhmg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.mhx1999.top/gtrcojxuyf.html

TS:   s.length
来源：http://hz.zhixingplan.top/gtpbtikmel.html

Java: s.length()
来源：http://hz.hammf.cn/gtinlojqkc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yonumen.top/gtdmjwvgch.html

Ruby: s.length
来源：http://hz.cheryme.top/gtzdztnabf.html

C#:   s.Length
来源：http://hz.pengpengdd.cyou/gthjoxlyso.html

[A23] 大小写转换
来源：http://hz.snrcjt.cn/gtspgkofxz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.redwolf501.top/gtsgjtcmhw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yvedp.cn/gtjkwjdvvz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.havefunace.top/gtkbauppod.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.aizwys.cn/gtnanzkrdd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gttvyzznwq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yj202588.top/gtqfpzrmth.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhiwuduotai.top/gttvhdtpqv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jqgufenzy.top/gtcqygokoh.html

[A24] 去除首尾空白
来源：http://hz.chenjidiqi.icu/gthohxpcpd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.shzxlz.cn/gtdykdhlmj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hfpthk.cn/gtfnpnmxul.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yuanzhike.top/gtmajcuwua.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yangfankeji.com/gtwxaoxacw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.meibo888.top/gtjoyejtew.html

Go:   strings.TrimSpace(s)
来源：http://hz.shanyushiyangtech.top/gtsfpeuuet.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.chenzaomai.com/gturfovonv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yj20258888.top/gtgqgdaaes.html

[A25] 字符串比较
来源：http://hz.yj20258.top/gtwrdraewo.html

Py:   s1 == s2; s1 != s2
来源：http://hz.sysykeji.top/gtbjvkwqev.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jinqigfzy.top/gthierycem.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xingfuxueyuan.xyz/gtjhqmqjou.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hnqzz.top/gtqwjgdimy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.aizwys.cn/gtwkggjdgl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shzxlz.cn/gttgyxenzr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yongpay.top/gtdteymiss.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.tanke756.top/gtqsdxcsvg.html

[A26] 类型转换总览
来源：http://hz.cheryme.top/gtuxppemni.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.mhx1999.top/gtotsqcumx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.yanxiufei.cn/gtyeggjzjv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xinyue.icu/gtnxmlmoga.html

TS:   Number() String() Boolean() x as number
来源：http://hz.meibo888.top/gtwtqzgxcw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.zhengqikj.top/gtraecoqdz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zdqjudy.top/gtogziljfb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yj20258.top/gtupdlszzt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jinyuanbaomall.cn/gttnscoqrf.html

================================================================================
来源：http://hz.xziqi.cn/gtwlzgljxw.html

B. 流程控制
来源：http://hz.wangdashe.top/gtqhwocgsa.html

================================================================================
来源：http://hz.hysaishi.cn/gtbartxdlk.html

[B01] 条件判断 if / else
来源：http://hz.havefunace.top/gtkqfeferj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gzhubu.top/gtcqlquzxn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zhaomingkeji.xyz/gthbmheokd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtligfwiwv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtfmvgnxrj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtjctzosfv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gzhubu.top/gtokhyopqm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.tianlin.xyz/gtznrsmqdq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.xuetiantiany.cn/gtgiyzsarx.html

[B02] 多分支 else if / elif
来源：http://hz.havefunace.top/gtcqpegkbb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hywenlv.cn/gtrtycgysr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.sufxvd.cn/gtvjgtbnnz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.havefunace.top/gtyibwgxnc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daria6918.cn/gtibhmbgmy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zdqjudy.top/gtkghxosra.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.daxiang520.top/gtnttbukch.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.svipenyu.cn/gtpbjgkdiv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ydzc1.top/gtvrwycfif.html

[B03] switch / match / case
来源：http://hz.cashguo.top/gtblwfhmpe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.zhengqikj.top/gtykdclsig.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yonumen.top/gtjohgmozf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.havefunace.top/gtxyftjhgw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zycfv.cn/gtnaaezvby.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.ydzc1.top/gtmgctcmqs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jinqigufen.top/gtqwasngga.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhengqikj.top/gttsjlmmco.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.hnxiangtu.top/gtpxmmlndd.html

[B04] for 计数循环
来源：http://hz.shzxlz.cn/gthneqvfhl.html

Py:   for i in range(10): print(i)
来源：http://hz.nanxuanxn.top/gtwygedszu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.snrcjt.cn/gthytseusz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gogol.net.cn/gtjrpcqbjc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gogol.net.cn/gtrjshkiye.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.havefunace.top/gtktyudxyt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.shzxlz.cn/gtezovxsht.html

Ruby: 10.times { |i| puts i }
来源：http://hz.gaohongyu789.top/gthviardhj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.cheryme.top/gtcbwhwffb.html

[B05] 遍历数组 / 列表
来源：http://hz.ybcxt.top/gtvqqchkqo.html

Py:   for item in arr: print(item)
来源：http://hz.hysaishi.cn/gtmlzgpmui.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.meibo888.top/gtxgrzuhhn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jinqigufen.top/gtgdtnshik.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.gaohongyu789.top/gtctjzjqeu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.snrcjt.cn/gtyoxismvl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.yonumen.top/gtwabnesih.html

Ruby: arr.each { |item| puts item }
来源：http://hz.birdmap.top/gtftqjodjy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.0kj1m.cn/gtworrbhkh.html

[B06] 遍历字典 / 对象
来源：http://hz.xuetiantiany.cn/gtbtkdjiix.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jinqigfzy.top/gtqrrbgljr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.gaohongyu789.top/gtkiiebbsf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhixingplan.top/gtrgajkdgg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xuanzx.com/gtbgfhmumz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.havefunace.top/gttkltsrpl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hnqzz.top/gtxiucnxwn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.bjfxy.top/gtcxowdsss.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.shzxlz.cn/gtfpjgwwxf.html

[B07] while 循环
来源：http://hz.cdnleiting.top/gtcexnoswh.html

Py:   while i < 10: i += 1
来源：http://hz.jinghuilouyu.cn/gtyqpdnidg.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zdqjudy.top/gtvxebabow.html

JS:   while (i < 10) { i++; }
来源：http://hz.birdmap.top/gthxdwafqt.html

TS:   while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtjkkhtpfg.html

Java: while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtbmwrpvbw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj20258888.top/gttutvfwqf.html

Ruby: while i < 10; i += 1; end
来源：http://hz.jyoumei.cn/gtqhqhrkpk.html

C#:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtrqslhmpk.html

[B08] do-while（至少执行一次）
来源：http://hz.cucudq.cn/gtouutsubu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.nwbrower.top/gtocsmwajv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.havefunace.top/gtyxkcfzub.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtfvxxdccj.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gturnqltwx.html

Java: do { i++; } while (i < 10);
来源：http://hz.jianghu66.top/gtkmcquqpg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.havefunace.top/gtktuigouf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tian-w.cn/gtecztfqyt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.bjfxy.top/gtmzfshrrh.html

[B09] break 与 continue
来源：http://hz.jinqigufen.top/gtyfinaqke.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.52xcode.cn/gttdftaqnv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.hnxiangtu.top/gtsjiofspi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenjidiqi.icu/gtpqelctrl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtfhjzseej.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtxbxcixsa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.shanyushiyangkeji.top/gtbmopihxu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xylfe.cn/gtoelnezzn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zhiwuduotai.top/gthffrytnn.html

[B10] 遍历同时拿索引
来源：http://hz.daria6918.cn/gtxpxqcjrz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.fzhhl.top/gtciglfkfv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.nanxinkj.top/gtcvpwayvb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.xylfe.cn/gtlopjqfvo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.wangdashe.top/gtsfhewduq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.xinyue.icu/gtzpiggafx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.haohaochexian.top/gtlsfxbspw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.aibaodan.cn/gttsftxqhn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj20258888.top/gtzzebstbw.html

[B11] 生成数字序列 / 区间
来源：http://hz.yanxiufei.cn/gttfgqsavd.html

Py:   list(range(0, 10, 2))
来源：http://hz.dashuyun.cn/gtiwknpsbj.html

PHP:  range(0, 10, 2);
来源：http://hz.wangshuangyany.cn/gtdijmsotj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.feifeiyinyue.top/gtguatyygt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhixingplan.top/gtpnxngnmj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yueranfly.top/gtddxcyfgc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.xingfuxueyuan.xyz/gtezhxysoh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.yanxiufei.cn/gtnywaxtto.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.316326.xyz/gtujzykxbg.html

[B12] 跳出多层循环
来源：http://hz.shzxlz.cn/gtvydubtmf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.bjfxy.top/gtpmbcnkuq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aibaodan.cn/gtatyejweb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.fengsongda.top/gtjmmqpabe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.xziqi.cn/gtkbfoovxx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhoulong.xyz/gtmgvhrgwj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.smart0.xyz/gtrmaaljop.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.aibaodan.cn/gtavqmyiyh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.nanxuanxn.top/gtosmrcrdo.html

[B13] 判断是否为数字
来源：http://hz.pengpengdd.cyou/gtwydjtlgc.html

Py:   isinstance(x, (int, float))
来源：http://hz.jianghu66.top/gtpbwsfvzb.html

PHP:  is_numeric($x)
来源：http://hz.hongshengwenyu.top/gtqgorapqe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cashguo.top/gtkknzpuqh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sxryk.cn/gtczsujnhs.html

Java: x instanceof Number
来源：http://hz.jinqigfzy.top/gtjybgcdvv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.shanyushiyangtech.top/gtnzstqqpr.html

Ruby: x.is_a?(Numeric)
来源：http://hz.guowangkeji.top/gtrawmhpya.html

C#:   x is int or double or decimal
来源：http://hz.yonumen.top/gtfvocxxim.html

[B14] 判断值是否在集合内
来源：http://hz.gzhubu.top/gtzjspklts.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xinyue.icu/gtvleavoqg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jiagoushi.top/gthkpxgvtm.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtitwkifbe.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.yangfankeji.com/gtwteutgqd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ppjwa.cn/gthlpqyyvc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hongshengwenyu.top/gteeeyervk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.pycfn.com/gtklpupeay.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yuxming.cn/gtzobuvkma.html

[B15] 布尔运算与取反
来源：http://hz.xinyue.icu/gtljsfcacp.html

Py:   a and b or not c
来源：http://hz.jqgfzy.top/gtpeksfkib.html

PHP:  $a && $b || !$c
来源：http://hz.mhx1999.top/gtnihyulce.html

JS:   a && b || !c
来源：http://hz.hammf.cn/gtyrfwrala.html

TS:   a && b || !c
来源：http://hz.gzhubu.top/gtwoantqdm.html

Java: a && b || !c
来源：http://hz.redwolf501.top/gtgefsewpr.html

Go:   a && b || !c
来源：http://hz.jinqigfzy.top/gtbryfzguk.html

Ruby: a && b || !c
来源：http://hz.52xcode.cn/gtkdilaarc.html

C#:   a && b || !c
来源：http://hz.sweek.top/gtrscuanqj.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gogol.net.cn/gtoxfsucfj.html

Py:   if not data: return
来源：http://hz.andypj.xyz/gtqwqxfufv.html

PHP:  if (!$data) { return; }
来源：http://hz.ywan-chungtsiang.top/gtawjkdzzn.html

JS:   if (!data) return;
来源：http://hz.snrcjt.cn/gtwldvjidn.html

TS:   if (!data) return;
来源：http://hz.xuanzx.com/gtajetxpwb.html

Java: if (data == null) return;
来源：http://hz.yj20258888.top/gtwydeiwqf.html

Go:   if data == nil { return }
来源：http://hz.guannengcc.top/gtssnqnmcg.html

Ruby: return if data.nil?
来源：http://hz.jinqigufen.top/gtadfrybwx.html

C#:   if (data == null) return;
来源：http://hz.tian-w.cn/gtmieunpff.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtgvkersqw.html

C. 函数与作用域
来源：http://hz.nwbrower.top/gtsotvfkvn.html

================================================================================
来源：http://hz.pycfn.com/gtrrzvzdzf.html

[C01] 定义函数
来源：http://hz.snrcjt.cn/gtqvwzsipt.html

Py:   def add(a, b): return a + b
来源：http://hz.cdnleiting.top/gteahahkni.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.52xcode.cn/gtfcaekpen.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ivvv.top/gtskpnoibj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gogol.net.cn/gtbytacbeo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gtpowkptjv.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yanxiufei.cn/gtodwypnot.html

Ruby: def add(a, b); a + b; end
来源：http://hz.c1oappe.top/gtzfhgpacq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtoetihkrc.html

[C02] 默认参数
来源：http://hz.hongshengwenyu.top/gtszpzcvpc.html

Py:   def greet(name="World"): return name
来源：http://hz.daxiang520.top/gtxbugutqm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zdqjudy.top/gtfxcxebio.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dashuyun.cn/gtltrhxyri.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.andypj.xyz/gtnkpabkuw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangshuangyany.cn/gtfhhbvcbg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gaohongyu789.top/gtvukjgwfd.html

Ruby: def greet(name = "World") = name
来源：http://hz.svipenyu.cn/gtskhuerfh.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yj20258.top/gtrxsqvqda.html

[C03] 可变参数
来源：http://hz.tanke756.top/gtasztncvv.html

Py:   def total(*args): return sum(args)
来源：http://hz.nanxuanxn.top/gtwxqncehs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.svipenyu.cn/gtgrdarsfq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtweavwisc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yj202588.top/gtkckhgdgv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xingfuxueyuan.xyz/gtevpdnurm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.52xcode.cn/gttindqvea.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.52xcode.cn/gtkzdgctfa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.hywenlv.cn/gtzexratsi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangshuangyany.cn/gtvedadork.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.smart0.xyz/gtdlecadrt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.fzhhl.top/gtanlqhfia.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinyuanbaomall.cn/gtjlyvyorb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinghuilouyu.cn/gteufloidl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.quarkkingdee.top/gtncekvyhj.html

Go:   // 无：用配置结构体参数
来源：http://hz.sysykeji.top/gtzvfsevpa.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtiivhmymi.html

C#:   f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtslmphwdh.html

[C05] 返回多个值
来源：http://hz.zhiwuduotai.top/gtebpgrqiu.html

Py:   return a, b
来源：http://hz.ehwqpu.com/gtverhihfh.html

PHP:  return [$a, $b];
来源：http://hz.ydjk.org.cn/gtgkbrcxoq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.mhx1999.top/gtwxdxdkgg.html

TS:   return { a, b };
来源：http://hz.svipenyu.cn/gtzqjqtwba.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.hnxiangtu.top/gtbiwjynju.html

Go:   return a, b
来源：http://hz.chenzaomai.com/gtuldpcfzn.html

Ruby: return a, b
来源：http://hz.c1oappe.top/gtlvydzmlk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtkilzbgzp.html

[C06] 匿名函数 / lambda
来源：http://hz.xuanzx.com/gtptezkyzm.html

Py:   square = lambda x: x * x
来源：http://hz.iojbl.cn/gtbzzoidxu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yangfankeji.com/gtednlgdhl.html

JS:   const square = x => x * x;
来源：http://hz.yanxiufei.cn/gtqqeywidc.html


<!-- 参考信息 -->