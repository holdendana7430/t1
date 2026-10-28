代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.meibo888.top/gtvfzlbnle.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.fzhhl.top/gtzkmdwjpn.html

TS:   if (!x) {}
来源：http://hz.guowangkeji.top/gtciifyxbl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.yongpay.top/gtrheejgbi.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.kuanghao11.cn/gtfyfxlesy.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.gaohongyu789.top/gtsjqnfclv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.svipenyu.cn/gtgkozocms.html

[A17] 位运算
来源：http://hz.nanxinkj.top/gtklehwhbf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shuidangran.top/gtyioyobml.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yongpay.top/gtyiiakbjt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gtmjcnwqhg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.hnqzz.top/gtqiobqatc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.52xcode.cn/gtsvumrpoe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hywenlv.cn/gtoojhnqye.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhixingplan.top/gtdrynalku.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuanzx.com/gtxwkkespi.html

[A18] 字符与 ASCII 码互转
来源：http://hz.9152youxi.cn/gtsxmmiioi.html

Py:   ord("A"); chr(65)
来源：http://hz.xuetiantiany.cn/gttqdzwpku.html

PHP:  ord("A"); chr(65)
来源：http://hz.vqdsnc.cn/gtqcepwtsa.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.316326.xyz/gthsbglmtt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.andypj.xyz/gtnlfiqrrr.html

Java: (int) 'A'; (char) 65
来源：http://hz.meibo888.top/gthcmspyyw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.wangshuangyany.cn/gtfkgimdeh.html

Ruby: "A".ord; 65.chr
来源：http://hz.gogol.net.cn/gtdqdjeuhf.html

C#:   (int)'A'; (char)65
来源：http://hz.tanke756.top/gtkhdzzvlf.html

[A19] 交换两个变量
来源：http://hz.havefunace.top/gtwytkfcje.html

Py:   a, b = b, a
来源：http://hz.sufxvd.cn/gtfgcmjmhf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.guannengcc.top/gtkfboqiau.html

JS:   [a, b] = [b, a];
来源：http://hz.tianlin.xyz/gthzjlxdyf.html

TS:   [a, b] = [b, a];
来源：http://hz.chenjidiqi.icu/gtdooydmbq.html

Java: int t = a; a = b; b = t;
来源：http://hz.yanxiufei.cn/gthuofinrj.html

Go:   a, b = b, a
来源：http://hz.guowangkeji.top/gtomwjlisx.html

Ruby: a, b = b, a
来源：http://hz.ivvv.top/gthjvudfpf.html

C#:   (a, b) = (b, a);
来源：http://hz.hnxiangtu.top/gtrzjisjqc.html

[A20] 读取标准输入
来源：http://hz.zhijiandao.cn/gtahbcqfga.html

Py:   name = input("请输入：")
来源：http://hz.pycfn.com/gtrlhqphks.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.mhx1999.top/gtkdwnturq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.daxiang520.top/gtwgdelack.html

TS:   // Node.js：readline 模块
来源：http://hz.gogol.net.cn/gtbonsdgfc.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhijiandao.cn/gtieolsyan.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xinyue.icu/gtvahiyzpz.html

Ruby: gets.chomp
来源：http://hz.yvedp.cn/gtxlioloyj.html

C#:   Console.ReadLine();
来源：http://hz.ybcxt.top/gtomopmdjk.html

[A21] 保留指定小数位输出
来源：http://hz.ppjwa.cn/gtumgsccla.html

Py:   f"{3.14159:.2f}"
来源：http://hz.yueranfly.top/gtnybbihvg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.sxryk.cn/gtodfdhhtf.html

JS:   (3.14159).toFixed(2)
来源：http://hz.quarkkingdee.top/gtphhohyep.html

TS:   (3.14159).toFixed(2)
来源：http://hz.guannengcc.top/gtfuxulrej.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gtdybmkyqk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.pengpengdd.cyou/gtndzpdcvl.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.yongpay.top/gtyrauniwb.html

C#:   3.14159.ToString("F2")
来源：http://hz.chenzaomai.com/gtarnezlff.html

[A22] 获取字符串长度
来源：http://hz.nanxinkj.top/gtttmmfrbs.html

Py:   len(s)
来源：http://hz.yonumen.top/gtdkxfgvla.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jinqigufen.top/gtkxlamzsc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.c1oappe.top/gtmogfhseu.html

TS:   s.length
来源：http://hz.chenjidiqi.icu/gtgukqmwyv.html

Java: s.length()
来源：http://hz.hnqzz.top/gtmqdswwfa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cashguo.top/gtqybpeajg.html

Ruby: s.length
来源：http://hz.yvedp.cn/gtzcqensxg.html

C#:   s.Length
来源：http://hz.cheryme.top/gtsukrsdgw.html

[A23] 大小写转换
来源：http://hz.9152youxi.cn/gtpxsuvvzr.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.cdnleiting.top/gthmxqvzdx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.316326.xyz/gtmjgjjjdw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.daria6918.cn/gtminhfjvq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sweek.top/gtrqjdhtax.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.hongshengwenyu.top/gtxeftxhof.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.pycfn.com/gtivqigdow.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.daxiang520.top/gtpcmmgjmt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.vqdsnc.cn/gtxbxappum.html

[A24] 去除首尾空白
来源：http://hz.ppjwa.cn/gtcsqrqbrn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhaomingkeji.xyz/gtgnstqiot.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.gaohongyu789.top/gtqtoioknk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shzxlz.cn/gthycbvzpj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.meibo888.top/gtthhpmrct.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yuxming.cn/gtyjijinqg.html

Go:   strings.TrimSpace(s)
来源：http://hz.xuanzx.com/gtmmltombn.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.birdmap.top/gtjumfxfpx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.jiagoushi.top/gtigwjhsns.html

[A25] 字符串比较
来源：http://hz.316326.xyz/gtgpjsfocj.html

Py:   s1 == s2; s1 != s2
来源：http://hz.pycfn.com/gtttemfukw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.gogol.net.cn/gtqvveekxf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hywenlv.cn/gtaahqoiud.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yuanzhike.top/gtuqdpaqmg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.vqdsnc.cn/gtsjvfyqsf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cashguo.top/gtaijagxrw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.gogol.net.cn/gtmjaublqv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.ybcxt.top/gtomlwcyph.html

[A26] 类型转换总览
来源：http://hz.sxryk.cn/gtmfobyemt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhixingplan.top/gtqwftbtny.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.wangdashe.top/gtmmnwfvnw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinghuilouyu.cn/gtbseynwhv.html

TS:   Number() String() Boolean() x as number
来源：http://hz.wangshuangyany.cn/gthskndxco.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.dashuyun.cn/gttauuqmla.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.sweek.top/gtbzjglong.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.jinghuilouyu.cn/gtlzfbqxrg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhengqikj.top/gtdouzxzlq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkkfwrknk.html

B. 流程控制
来源：http://hz.hywenlv.cn/gtybqbbllx.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwugvhpgj.html

[B01] 条件判断 if / else
来源：http://hz.fengsongda.top/gtnkdfyecz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gaohongyu789.top/gtswlcztee.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.ywan-chungtsiang.top/gtinmwibuo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.0kj1m.cn/gtbnfmaaho.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tian-w.cn/gtejslayjp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtqocpmxgb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cashguo.top/gtzoxbrevq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jinghuilouyu.cn/gtwjhvqotw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.chenjidiqi.icu/gttielsldr.html

[B02] 多分支 else if / elif
来源：http://hz.fzhhl.top/gtovnygepl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.feifeiyinyue.top/gthexrceov.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.feifeiyinyue.top/gtczobmwfv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtzcagrcch.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.feifeiyinyue.top/gtlgnsfppm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gotoacloud.top/gtdfjtlwwl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.chenlongwang.top/gtqukynrpy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.nwbrower.top/gtbjavyvqa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nwbrower.top/gtotjgfehc.html

[B03] switch / match / case
来源：http://hz.xinyue.icu/gtauowdnui.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.guannengcc.top/gtjrfcilyx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jlsjyb.cn/gtooadepys.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.aizwys.cn/gtagymupez.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.9152youxi.cn/gtywvngjgc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jlsjyb.cn/gtwovsxlnj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.tianlin.xyz/gtjcyrsltu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ywan-chungtsiang.top/gtgnlqkhep.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhoulong.xyz/gtrsrblogo.html

[B04] for 计数循环
来源：http://hz.jianghu66.top/gtzkabxknu.html

Py:   for i in range(10): print(i)
来源：http://hz.yj20258.top/gtlzjkvhbk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhixingplan.top/gthwrqxjhk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.cashguo.top/gtwmgnfheh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.nanxuanxn.top/gtslaokxns.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.guannengcc.top/gtletvntai.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.svipenyu.cn/gtopqedpwb.html

Ruby: 10.times { |i| puts i }
来源：http://hz.pycfn.com/gtpkyiszpd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.fengsongda.top/gtpbkqbygd.html

[B05] 遍历数组 / 列表
来源：http://hz.yj202588.top/gtyyyilnbh.html

Py:   for item in arr: print(item)
来源：http://hz.zhongyouzk.top/gtwoavyulv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.pycfn.com/gthjkzwwkp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jianghu66.top/gtmfadnkmv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuanzhike.top/gtmforkpkf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.wangdashe.top/gtntoknipv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.jqgfzy.top/gtssmurvwh.html

Ruby: arr.each { |item| puts item }
来源：http://hz.cdnleiting.top/gtcfntudjl.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.daria6918.cn/gtlmaekhdf.html

[B06] 遍历字典 / 对象
来源：http://hz.nwbrower.top/gtyfsacmyw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.fzhhl.top/gtcbnzaiem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cashguo.top/gtsonxiyul.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.birdmap.top/gtkjvwtykz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yj20258888.top/gtabecltov.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.nanxuanxn.top/gtqkgagwcu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.yuanzhike.top/gtltmdeyoj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.feifeiyinyue.top/gtflocnpzp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.quarkkingdee.top/gtgoxtierc.html

[B07] while 循环
来源：http://hz.hongshengwenyu.top/gtywdrvvsm.html

Py:   while i < 10: i += 1
来源：http://hz.xylfe.cn/gtqdepkanm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jlsjyb.cn/gtidprargr.html

JS:   while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtmvpkceyc.html

TS:   while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtypqkjivb.html

Java: while (i < 10) { i++; }
来源：http://hz.iojbl.cn/gtgldymuto.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.chenlongwang.top/gtlaebakge.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yvedp.cn/gtzstvsrtb.html

C#:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtxhkqltka.html

[B08] do-while（至少执行一次）
来源：http://hz.tanke756.top/gtcuxxugri.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jyoumei.cn/gtntxbyxyu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shanyushiyangkeji.top/gtrokbxrit.html

JS:   do { i++; } while (i < 10);
来源：http://hz.c1oappe.top/gtzojvnjxh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ydjk.org.cn/gtecgpuovb.html

Java: do { i++; } while (i < 10);
来源：http://hz.haohaochexian.top/gtuatfwtdo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.bjfxy.top/gttbrlgbrs.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ybcxt.top/gtmgbokkei.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shanyushiyangkeji.top/gtjrfdsmri.html

[B09] break 与 continue
来源：http://hz.jinqigfzy.top/gtgepjdiwc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sufxvd.cn/gtrqjlxhmg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhongyouzk.top/gtfhalymxr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtgksksmxy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gtlbdruiyl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jiagoushi.top/gtttklafyd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.ppjwa.cn/gtqwafsnpz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.havefunace.top/gtlrvicybq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sufxvd.cn/gtizvixtsn.html

[B10] 遍历同时拿索引
来源：http://hz.cqqwz.cn/gtmeoyqgfe.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinqigufen.top/gtokjsgcyt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhaomingkeji.xyz/gtjwvupvca.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shangyingyoupin.top/gtsezikmot.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tianlin.xyz/gtqfxrtuql.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jqgufenzy.top/gtjsdutwbo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.dianchejie.cn/gtvrxztrhb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shanyushiyangtech.top/gtkkgaqxdm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.zhiwuduotai.top/gtmrhyxpmb.html

[B11] 生成数字序列 / 区间
来源：http://hz.ehwqpu.com/gtsfofiflr.html

Py:   list(range(0, 10, 2))
来源：http://hz.haohaochexian.top/gtumawfqyg.html

PHP:  range(0, 10, 2);
来源：http://hz.cqqwz.cn/gtlbyupqkl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.aibaodan.cn/gtnqvkmilu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhaomingkeji.xyz/gtjsealzov.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cucudq.cn/gttkcsuixb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.kuanghao11.cn/gtpzwavopt.html

Ruby: (0...10).step(2).to_a
来源：http://hz.gogol.net.cn/gtlofovpur.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.zhongyouzk.top/gtwyuhwojz.html

[B12] 跳出多层循环
来源：http://hz.nanxuanxn.top/gteclgmmzw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenjidiqi.icu/gttqkmxkgr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtissyqvfz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.tianlin.xyz/gtzqniahmf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gthfvhqktm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuanzx.com/gtlzspyfst.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.dianchejie.cn/gtrcmqjspn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zdqjudy.top/gtlixefxpz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gogol.net.cn/gtnfsrokax.html

[B13] 判断是否为数字
来源：http://hz.jlsjyb.cn/gthjjcajhg.html

Py:   isinstance(x, (int, float))
来源：http://hz.pycfn.com/gtlgfhqdgk.html

PHP:  is_numeric($x)
来源：http://hz.shangyingyoupin.top/gtuxqwjyqf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xinyue.icu/gtiksogzyk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yuanzhike.top/gtghhqxrov.html

Java: x instanceof Number
来源：http://hz.shuidangran.top/gtaqlxkmbd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhijiandao.cn/gtexrtyxug.html

Ruby: x.is_a?(Numeric)
来源：http://hz.yongpay.top/gtzmacycod.html

C#:   x is int or double or decimal
来源：http://hz.chenlongwang.top/gtfornghoi.html

[B14] 判断值是否在集合内
来源：http://hz.yj20258888.top/gthaqbnerp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zycfv.cn/gtzuvialsn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenzaomai.com/gttsdgegzv.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtxeeleibo.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.fengsongda.top/gtvpwxsgeu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ydjk.org.cn/gtdpggfqgg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yj202588.top/gtxxhqcdli.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.feifeiyinyue.top/gteigpeaxb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhiwuduotai.top/gtxwkdhfmx.html

[B15] 布尔运算与取反
来源：http://hz.sufxvd.cn/gtomzzkscl.html

Py:   a and b or not c
来源：http://hz.tanke756.top/gtveduexko.html

PHP:  $a && $b || !$c
来源：http://hz.ydzc1.top/gtngiffuyq.html

JS:   a && b || !c
来源：http://hz.feifeiyinyue.top/gtwasjgwgu.html

TS:   a && b || !c
来源：http://hz.zhongyouzk.top/gtyqyofmpi.html

Java: a && b || !c
来源：http://hz.yuxming.cn/gttqaqsqfx.html

Go:   a && b || !c
来源：http://hz.snrcjt.cn/gtleukkodd.html

Ruby: a && b || !c
来源：http://hz.jlsjyb.cn/gtfwfzpxgg.html

C#:   a && b || !c
来源：http://hz.sweek.top/gtpesafzmy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hysaishi.cn/gtdvkkcqul.html

Py:   if not data: return
来源：http://hz.zhaomingkeji.xyz/gttvokwlqf.html

PHP:  if (!$data) { return; }
来源：http://hz.wangshuangyany.cn/gtzudrcjjm.html

JS:   if (!data) return;
来源：http://hz.bjfxy.top/gtfgcmsijf.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtxfgvxayb.html

Java: if (data == null) return;
来源：http://hz.sufxvd.cn/gtdhqrqktc.html

Go:   if data == nil { return }
来源：http://hz.fzhhl.top/gtvlhhnapj.html

Ruby: return if data.nil?
来源：http://hz.haohaochexian.top/gtmbfdnjyc.html

C#:   if (data == null) return;
来源：http://hz.xuanzx.com/gtgopqvnnx.html

================================================================================
来源：http://hz.zhengqikj.top/gtmauqcunv.html

C. 函数与作用域
来源：http://hz.jqgfzy.top/gtgkxzdcuw.html

================================================================================
来源：http://hz.daxiang520.top/gtfkdtmgqe.html

[C01] 定义函数
来源：http://hz.yongpay.top/gtlavdqmjp.html

Py:   def add(a, b): return a + b
来源：http://hz.sysykeji.top/gtmohickwg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cqqwz.cn/gtemyolhth.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jqgfzy.top/gtwjsdzfah.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtigpwovru.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.birdmap.top/gtbvyymgmd.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cheryme.top/gtjngtmeer.html

Ruby: def add(a, b); a + b; end
来源：http://hz.dianchejie.cn/gtpsfivqxc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shanyushiyangkeji.top/gtckgeplpa.html

[C02] 默认参数
来源：http://hz.daria6918.cn/gtelxnzdls.html

Py:   def greet(name="World"): return name
来源：http://hz.chenlongwang.top/gtdknjxdue.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tian-w.cn/gtegekfvwj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.guowangkeji.top/gtlkoybhfi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtiyvzowoh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shangyingyoupin.top/gtvrnqdzuz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.mhx1999.top/gthfcndrwm.html

Ruby: def greet(name = "World") = name
来源：http://hz.andypj.xyz/gttkhothzw.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.smart0.xyz/gtgsssywex.html

[C03] 可变参数
来源：http://hz.nanxuanxn.top/gtdsfmpicn.html

Py:   def total(*args): return sum(args)
来源：http://hz.sufxvd.cn/gtyiqusecr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sysykeji.top/gtqovsskqp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pengpengdd.cyou/gtedqwkczt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sxryk.cn/gtgwqqozda.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hammf.cn/gtpmziekqn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jianghu66.top/gtfopevwjw.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yongpay.top/gtazqyjrkc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.wangshuangyany.cn/gtsroaprtd.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hammf.cn/gtoisoiqgj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenlongwang.top/gtobakzuxx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.feifeiyinyue.top/gtgbykjfbz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.c1oappe.top/gtnlbixgqv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.smart0.xyz/gtkbwgvdhi.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.vqdsnc.cn/gtgvftpklk.html

Go:   // 无：用配置结构体参数
来源：http://hz.sweek.top/gtafvtbrgg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.cdnleiting.top/gthkfyvezs.html

C#:   f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtsgikiyqg.html

[C05] 返回多个值
来源：http://hz.hysaishi.cn/gtlffcbieo.html

Py:   return a, b
来源：http://hz.gaohongyu789.top/gtvqkghqvv.html

PHP:  return [$a, $b];
来源：http://hz.sufxvd.cn/gtksuudbup.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.iojbl.cn/gtzcblzdkt.html

TS:   return { a, b };
来源：http://hz.shuidangran.top/gtmoagdioj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yuanzhike.top/gthwzztfly.html

Go:   return a, b
来源：http://hz.quarkkingdee.top/gtavzfnady.html

Ruby: return a, b
来源：http://hz.nanxuanxn.top/gttmzqfaji.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinyuanbaomall.cn/gtvfnjvwaw.html

[C06] 匿名函数 / lambda
来源：http://hz.sufxvd.cn/gtkkhjxdog.html

Py:   square = lambda x: x * x
来源：http://hz.smart0.xyz/gtrsreipzn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hysaishi.cn/gtojrueble.html

JS:   const square = x => x * x;
来源：http://hz.xziqi.cn/gtsyiuotwu.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pengpengdd.cyou/gtddjyveyk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhongyouzk.top/gtocpmejvp.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.9152youxi.cn/gtgjqlcikm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydzc1.top/gtkezugmyo.html


<!-- 参考信息 -->