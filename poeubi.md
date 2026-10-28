代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.ydjk.org.cn/gtljlyctts.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.nwbrower.top/gtmyrkltdl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.tianlin.xyz/gtqlvwozbv.html

[A17] 位运算
来源：http://hz.nwbrower.top/gtmjejvjnx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yuanzhike.top/gtpgpwigom.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.ybcxt.top/gtfhntmfhc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.nwbrower.top/gtamdioyek.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.zdqjudy.top/gtkbymzhwk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fengsongda.top/gtdshaxsgb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.ydjk.org.cn/gtqrrkgknm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zycfv.cn/gtjoeonjur.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zycfv.cn/gtfxakxwqx.html

[A18] 字符与 ASCII 码互转
来源：http://hz.guannengcc.top/gtbovfxmvn.html

Py:   ord("A"); chr(65)
来源：http://hz.zhengqikj.top/gtmczrgypm.html

PHP:  ord("A"); chr(65)
来源：http://hz.wangshuangyany.cn/gtkoaxubvw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.hnxiangtu.top/gtzupmaasl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.aizwys.cn/gtvaluafbo.html

Java: (int) 'A'; (char) 65
来源：http://hz.jianghu66.top/gtgkzommsz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.tanke756.top/gtygiqekpb.html

Ruby: "A".ord; 65.chr
来源：http://hz.dianchejie.cn/gtzizxvieg.html

C#:   (int)'A'; (char)65
来源：http://hz.shangyingyoupin.top/gthnfkwymd.html

[A19] 交换两个变量
来源：http://hz.52xcode.cn/gtmekwiiur.html

Py:   a, b = b, a
来源：http://hz.yj202588.top/gthqfncukt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.tianlin.xyz/gteqnwwekl.html

JS:   [a, b] = [b, a];
来源：http://hz.zhongyouzk.top/gtkwmpsxqn.html

TS:   [a, b] = [b, a];
来源：http://hz.xuanzx.com/gtrxtnnsta.html

Java: int t = a; a = b; b = t;
来源：http://hz.jinqigfzy.top/gtbzcjrosm.html

Go:   a, b = b, a
来源：http://hz.nanxuanxn.top/gtcngerpdi.html

Ruby: a, b = b, a
来源：http://hz.daxiang520.top/gtqcanesfc.html

C#:   (a, b) = (b, a);
来源：http://hz.jinqigfzy.top/gtvrbrfsim.html

[A20] 读取标准输入
来源：http://hz.hnqzz.top/gtcwbrucsa.html

Py:   name = input("请输入：")
来源：http://hz.vqdsnc.cn/gtnhnddifx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.cucudq.cn/gtmmdyzerf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.pengpengdd.cyou/gtclradxvo.html

TS:   // Node.js：readline 模块
来源：http://hz.shanyushiyangtech.top/gtsyyvzqjg.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yj202588.top/gtwyxujaap.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.meibo888.top/gthuiiftue.html

Ruby: gets.chomp
来源：http://hz.gotoacloud.top/gtljxbmask.html

C#:   Console.ReadLine();
来源：http://hz.zhoulong.xyz/gtolnofgdo.html

[A21] 保留指定小数位输出
来源：http://hz.aibaodan.cn/gtkasnwamm.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ivvv.top/gtkxowjsoc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.zhoulong.xyz/gtajzgoamu.html

JS:   (3.14159).toFixed(2)
来源：http://hz.yvedp.cn/gtxjrywaih.html

TS:   (3.14159).toFixed(2)
来源：http://hz.mhx1999.top/gtdtwwhnvs.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.haohaochexian.top/gtccbdyfcb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.shanyushiyangtech.top/gtluqlkgut.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zhoulong.xyz/gtkpawcrjf.html

C#:   3.14159.ToString("F2")
来源：http://hz.haohaochexian.top/gtnhtiromz.html

[A22] 获取字符串长度
来源：http://hz.nanxinkj.top/gtdzcxmijo.html

Py:   len(s)
来源：http://hz.pengpengdd.cyou/gthbyzfypa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.zhijiandao.cn/gttcyaxbnv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.haohaochexian.top/gtunzxcivu.html

TS:   s.length
来源：http://hz.c1oappe.top/gtvxkcqrub.html

Java: s.length()
来源：http://hz.shuidangran.top/gtqlbqoiis.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.xingfuxueyuan.xyz/gtrtaaulre.html

Ruby: s.length
来源：http://hz.sweek.top/gtegllsgvi.html

C#:   s.Length
来源：http://hz.zhixingplan.top/gtzztgvmnf.html

[A23] 大小写转换
来源：http://hz.tian-w.cn/gtzuxqgwyx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.guowangkeji.top/gtvzcelfec.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.hongshengwenyu.top/gtcoyggpnf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sufxvd.cn/gtytevouoj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuanzx.com/gtwpyorxfd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.snrcjt.cn/gtejketnch.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.tian-w.cn/gtakpfmzoe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.mhx1999.top/gtccnucyhv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.ydzc1.top/gtxuxjvxxa.html

[A24] 去除首尾空白
来源：http://hz.yanxiufei.cn/gtlzjtmrny.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.nanxuanxn.top/gtcefdyndg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.xylfe.cn/gtciinzawf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuanzx.com/gtcfqllhoj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tian-w.cn/gtbzchcmgd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.jqgfzy.top/gttpjntqtg.html

Go:   strings.TrimSpace(s)
来源：http://hz.jqgufenzy.top/gtajyqgmeg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.ivvv.top/gtnvuikmea.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yuxming.cn/gtoojpzdqh.html

[A25] 字符串比较
来源：http://hz.zdqjudy.top/gtdqpgddgd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.pengpengdd.cyou/gtjikbjckl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.xingfuxueyuan.xyz/gtgezhnfof.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.pengpengdd.cyou/gtlmdiklvv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydjk.org.cn/gtkqalwjjh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.c1oappe.top/gtikxfjiot.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sxryk.cn/gtvhscugjq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhoulong.xyz/gtsnacvkfh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.cucudq.cn/gtchayaeqj.html

[A26] 类型转换总览
来源：http://hz.chenjidiqi.icu/gttjxmustz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.vqdsnc.cn/gtlhfkrokb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.kuanghao11.cn/gttbmgiden.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.hongshengwenyu.top/gtzrjklfay.html

TS:   Number() String() Boolean() x as number
来源：http://hz.tanke756.top/gtspricrqm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.c1oappe.top/gtnyxkmsel.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.sxryk.cn/gtpcbfwyqc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yonumen.top/gtduvhscsn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jiagoushi.top/gtvgqafrri.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtfnskbuge.html

B. 流程控制
来源：http://hz.gzhubu.top/gtwvuossug.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtjkckygvf.html

[B01] 条件判断 if / else
来源：http://hz.shuidangran.top/gtarflbvmk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.vqdsnc.cn/gtqzvhhmrv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.aizwys.cn/gtuyccxolo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.birdmap.top/gtuezdfeen.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shuidangran.top/gtmmtnntgr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258.top/gtevulplri.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.nanxinkj.top/gtvkwmmesu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.sufxvd.cn/gtlgaqntkl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yangfankeji.com/gtgruabffo.html

[B02] 多分支 else if / elif
来源：http://hz.gaohongyu789.top/gtiylnhjcs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.fengsongda.top/gtfhufpnqc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.snrcjt.cn/gtktisszaf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gaohongyu789.top/gthhvwbaur.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangshuangyany.cn/gttomcjnbs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtniwbsskr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ywan-chungtsiang.top/gtopvesgxf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.zhoulong.xyz/gtwlwjejyw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gthcmmkttc.html

[B03] switch / match / case
来源：http://hz.yongpay.top/gtxlibvwmd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.tianlin.xyz/gticnkpjws.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.jinqigfzy.top/gtledsoudb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jiagoushi.top/gtsnanpxje.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigfzy.top/gtmfrcjagw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.sysykeji.top/gtybmzusqc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.52xcode.cn/gtbbhvpkxq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.tianlin.xyz/gtvdidfxvb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.xziqi.cn/gtwwkaecmr.html

[B04] for 计数循环
来源：http://hz.xylfe.cn/gtvamadupi.html

Py:   for i in range(10): print(i)
来源：http://hz.jlsjyb.cn/gtxmzozhta.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yueranfly.top/gtmquecotj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinghuilouyu.cn/gtelyhkxwk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.ppjwa.cn/gticjsafmh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hnxiangtu.top/gtfroxojdv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.cheryme.top/gtygrtdwru.html

Ruby: 10.times { |i| puts i }
来源：http://hz.wangshuangyany.cn/gtostvitft.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.redwolf501.top/gtfexxselu.html

[B05] 遍历数组 / 列表
来源：http://hz.jinyuanbaomall.cn/gtnhmeefhx.html

Py:   for item in arr: print(item)
来源：http://hz.xziqi.cn/gtdoatshuy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.jinghuilouyu.cn/gtrwvfkbyr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuxming.cn/gtrttnekqq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sufxvd.cn/gtrqbavwvr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hfpthk.cn/gtmsysoiid.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.guowangkeji.top/gtnzomknfx.html

Ruby: arr.each { |item| puts item }
来源：http://hz.yuxming.cn/gtojpgwqgj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zdqjudy.top/gtccwneysu.html

[B06] 遍历字典 / 对象
来源：http://hz.hammf.cn/gtcphqgboy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jinqigfzy.top/gtukorkhge.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.jlsjyb.cn/gtjszuxrow.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.zhaomingkeji.xyz/gtqijkrtmt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.aizwys.cn/gttxinaffs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cqqwz.cn/gtneesebds.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.kuanghao11.cn/gtujewkfhj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yueranfly.top/gtbvxventl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.bjfxy.top/gtwopdzdvp.html

[B07] while 循环
来源：http://hz.yonumen.top/gtlikjihpz.html

Py:   while i < 10: i += 1
来源：http://hz.yueranfly.top/gtmafttmuw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.snrcjt.cn/gtkqmerabi.html

JS:   while (i < 10) { i++; }
来源：http://hz.wangshuangyany.cn/gtznprqyod.html

TS:   while (i < 10) { i++; }
来源：http://hz.9152youxi.cn/gtyagaxlwv.html

Java: while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtxytbnqjz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.yj20258888.top/gtfknirvtd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhaomingkeji.xyz/gtrxoovfan.html

C#:   while (i < 10) { i++; }
来源：http://hz.tianlin.xyz/gtjjagykvr.html

[B08] do-while（至少执行一次）
来源：http://hz.ehwqpu.com/gtzigzrmdo.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.hongshengwenyu.top/gtrgdvelbt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.9152youxi.cn/gtwiapdxic.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gteheuujvb.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtjglqqbvx.html

Java: do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtutosycin.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ivvv.top/gtvthiunbp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.nanxuanxn.top/gtfljzejib.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenjidiqi.icu/gtpkzowdyi.html

[B09] break 与 continue
来源：http://hz.sweek.top/gtsokaqnxn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.shzxlz.cn/gtpvbuyvqs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.nanxuanxn.top/gtynlvbngk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.dashuyun.cn/gtjdrqsmmf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gthvsnqlgv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sysykeji.top/gtqanzvbrj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.daxiang520.top/gtxaqjvips.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.52xcode.cn/gtmuggicia.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.meibo888.top/gtdzhtnozk.html

[B10] 遍历同时拿索引
来源：http://hz.cdnleiting.top/gtlelluxfo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.gzhubu.top/gtlnwcfdut.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.sweek.top/gthtzwqyrq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhijiandao.cn/gtdokoqblj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.xziqi.cn/gtlvsblyrf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.shangyingyoupin.top/gtnrdsiegd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hfpthk.cn/gtncndztji.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhongyouzk.top/gtqfznwuya.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangkeji.top/gtoycqmtqn.html

[B11] 生成数字序列 / 区间
来源：http://hz.c1oappe.top/gtzltfdaie.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtyzkbiwoj.html

PHP:  range(0, 10, 2);
来源：http://hz.jqgfzy.top/gtsszmmhow.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sufxvd.cn/gtpwuiinev.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhiwuduotai.top/gtzjtzmpqo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhaomingkeji.xyz/gtirduzdbe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.9152youxi.cn/gtbegvsndo.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sxryk.cn/gtojnbjjjk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xuanzx.com/gtjfvsswqp.html

[B12] 跳出多层循环
来源：http://hz.yongpay.top/gtrkatxwxq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.chenjidiqi.icu/gtmxwjxlrw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.smart0.xyz/gtdclzmxda.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.316326.xyz/gtjzomenej.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gthcrxugvp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gttaevkcdf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yuxming.cn/gtncihgcat.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.ppjwa.cn/gtfbeurkyu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.52xcode.cn/gtwfqmimca.html

[B13] 判断是否为数字
来源：http://hz.0kj1m.cn/gtomkurlol.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhongyouzk.top/gtbbkhedvc.html

PHP:  is_numeric($x)
来源：http://hz.xziqi.cn/gtwzyldohb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtgwfilkfd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtyghnnask.html

Java: x instanceof Number
来源：http://hz.yonumen.top/gtqxmplfvx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.xziqi.cn/gtuhnrovto.html

Ruby: x.is_a?(Numeric)
来源：http://hz.pengpengdd.cyou/gtrferkisf.html

C#:   x is int or double or decimal
来源：http://hz.daxiang520.top/gttixdhuox.html

[B14] 判断值是否在集合内
来源：http://hz.cqqwz.cn/gtapvatzzv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.kuanghao11.cn/gtnlnktwlf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shanyushiyangkeji.top/gtsopactpj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xziqi.cn/gtexnehycy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jinghuilouyu.cn/gthbhjbalt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gaohongyu789.top/gtefsdoreo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.meibo888.top/gtoenoxewo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.nanxuanxn.top/gtwsbdvtkz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.snrcjt.cn/gtfuukjzoz.html

[B15] 布尔运算与取反
来源：http://hz.yvedp.cn/gtduhcpnvo.html

Py:   a and b or not c
来源：http://hz.tian-w.cn/gtcwfgruvh.html

PHP:  $a && $b || !$c
来源：http://hz.hnxiangtu.top/gtsbufeveg.html

JS:   a && b || !c
来源：http://hz.nanxinkj.top/gtyyqzmgub.html

TS:   a && b || !c
来源：http://hz.c1oappe.top/gtcufcryas.html

Java: a && b || !c
来源：http://hz.gogol.net.cn/gtrrfxillr.html

Go:   a && b || !c
来源：http://hz.daria6918.cn/gtpbcduxfy.html

Ruby: a && b || !c
来源：http://hz.mhx1999.top/gtlzlvbrnb.html

C#:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtwddwmnwx.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shuidangran.top/gtmyvaeuhs.html

Py:   if not data: return
来源：http://hz.ybcxt.top/gtdspbloza.html

PHP:  if (!$data) { return; }
来源：http://hz.quarkkingdee.top/gtvimhnasq.html

JS:   if (!data) return;
来源：http://hz.tian-w.cn/gtbxwcruck.html

TS:   if (!data) return;
来源：http://hz.hysaishi.cn/gtctunepim.html

Java: if (data == null) return;
来源：http://hz.xingfuxueyuan.xyz/gtmaqshtvq.html

Go:   if data == nil { return }
来源：http://hz.sufxvd.cn/gtewfsqgzv.html

Ruby: return if data.nil?
来源：http://hz.tian-w.cn/gtyiywjkzs.html

C#:   if (data == null) return;
来源：http://hz.fengsongda.top/gtamagopjo.html

================================================================================
来源：http://hz.smart0.xyz/gttshcztzo.html

C. 函数与作用域
来源：http://hz.ybcxt.top/gtdrxdviyz.html

================================================================================
来源：http://hz.xinyue.icu/gtgvgjvjzw.html

[C01] 定义函数
来源：http://hz.vqdsnc.cn/gtghngdtty.html

Py:   def add(a, b): return a + b
来源：http://hz.jinqigfzy.top/gtwadifofz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtieapkefb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.yj202588.top/gtnesnvror.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cqqwz.cn/gtezmewxhp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtvuzfdnpa.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258.top/gtvoxdfrlu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hammf.cn/gtfykvcdgw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtuhsekzsl.html

[C02] 默认参数
来源：http://hz.jinyuanbaomall.cn/gtivthsigl.html

Py:   def greet(name="World"): return name
来源：http://hz.tanke756.top/gttmoeswac.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yj20258.top/gtgyofxxua.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.chenjidiqi.icu/gtaohvvvgy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jyoumei.cn/gtuxqswjfv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.cheryme.top/gtvusxsmln.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yanxiufei.cn/gtaczplywn.html

Ruby: def greet(name = "World") = name
来源：http://hz.sxryk.cn/gtclwjmkjv.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.tianlin.xyz/gtscvhardy.html

[C03] 可变参数
来源：http://hz.c1oappe.top/gtdldshzvg.html

Py:   def total(*args): return sum(args)
来源：http://hz.yj20258.top/gtcqzpglat.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jlsjyb.cn/gtccxqrfng.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gtzfendcvv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtznbpwncx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhaomingkeji.xyz/gtjluxnhix.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xinyue.icu/gtlxdijcti.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cashguo.top/gtfegvpnum.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xuanzx.com/gtpprzwhmt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ppjwa.cn/gtqdkalunn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxuanxn.top/gteldwlmnv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gtvnzvxvfy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.havefunace.top/gtdcmoyncq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinqigfzy.top/gtqcaadxod.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gzhubu.top/gthrhwwkou.html

Go:   // 无：用配置结构体参数
来源：http://hz.xuetiantiany.cn/gtgorwjqqx.html

Ruby: f(a: 1, b: 2)
来源：http://hz.fzhhl.top/gtqmmpktfk.html

C#:   f(a: 1, b: 2)
来源：http://hz.jianghu66.top/gtvgfgkmsw.html

[C05] 返回多个值
来源：http://hz.xinyue.icu/gtflbxmggn.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtnomvjmcz.html

PHP:  return [$a, $b];
来源：http://hz.havefunace.top/gtxixvlrec.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cqqwz.cn/gtfmxudasz.html

TS:   return { a, b };
来源：http://hz.316326.xyz/gtxmttzdlj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.havefunace.top/gthfyeqspi.html

Go:   return a, b
来源：http://hz.hammf.cn/gtnycsthax.html

Ruby: return a, b
来源：http://hz.hfpthk.cn/gtxluyorty.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jiagoushi.top/gtneknxrlx.html

[C06] 匿名函数 / lambda
来源：http://hz.yongpay.top/gtcuuckhoa.html

Py:   square = lambda x: x * x
来源：http://hz.xingfuxueyuan.xyz/gtshurxywr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangdashe.top/gtmfzevket.html

JS:   const square = x => x * x;
来源：http://hz.andypj.xyz/gtfvmpqskd.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.c1oappe.top/gtkqsfvyph.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yonumen.top/gtwxnvqdrk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yuxming.cn/gtkkqqffws.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fengsongda.top/gtlitbiwjd.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj202588.top/gthuwpgryo.html

[C07] 把函数作为参数传入
来源：http://hz.gotoacloud.top/gtbywrtnia.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daria6918.cn/gtqtceuvxd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.gogol.net.cn/gtkvtcuscp.html


<!-- 参考信息 -->