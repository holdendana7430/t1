代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.hfpthk.cn/gtnxssqpsv.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.chenzaomai.com/gtfrcwpbpn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hywenlv.cn/gtkiztbrli.html

[A17] 位运算
来源：http://hz.jinghuilouyu.cn/gtwbjeeuvd.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuetiantiany.cn/gtgxqrvjeg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.sysykeji.top/gtkbjmpykv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtnkugdyws.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.316326.xyz/gteyieocrx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tanke756.top/gtekxuhijq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtzabmogqd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.iojbl.cn/gtjogvstyl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.chenlongwang.top/gtrnsjcysa.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ppjwa.cn/gtvfjaedaw.html

Py:   ord("A"); chr(65)
来源：http://hz.shanyushiyangtech.top/gtndeqtjxb.html

PHP:  ord("A"); chr(65)
来源：http://hz.jqgfzy.top/gtgfddcxdw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yueranfly.top/gtlxivxlmu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinghuilouyu.cn/gtbipasqqc.html

Java: (int) 'A'; (char) 65
来源：http://hz.daxiang520.top/gtybqciyws.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.sysykeji.top/gtsnzogsgw.html

Ruby: "A".ord; 65.chr
来源：http://hz.zdqjudy.top/gtsbyncesx.html

C#:   (int)'A'; (char)65
来源：http://hz.yueranfly.top/gtikxtswhu.html

[A19] 交换两个变量
来源：http://hz.hammf.cn/gtdxgfpmya.html

Py:   a, b = b, a
来源：http://hz.ybcxt.top/gtitztpalq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yangfankeji.com/gtucmbvqfq.html

JS:   [a, b] = [b, a];
来源：http://hz.birdmap.top/gtpgmptubf.html

TS:   [a, b] = [b, a];
来源：http://hz.chenjidiqi.icu/gtkbdayqen.html

Java: int t = a; a = b; b = t;
来源：http://hz.hnxiangtu.top/gtujfeutqt.html

Go:   a, b = b, a
来源：http://hz.jinyuanbaomall.cn/gtjckwubub.html

Ruby: a, b = b, a
来源：http://hz.zhiwuduotai.top/gtfmmidlwb.html

C#:   (a, b) = (b, a);
来源：http://hz.xylfe.cn/gtgnwbnpzr.html

[A20] 读取标准输入
来源：http://hz.smart0.xyz/gtvyaafeah.html

Py:   name = input("请输入：")
来源：http://hz.snrcjt.cn/gtwikwalmb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ywan-chungtsiang.top/gtreeldcfs.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.c1oappe.top/gtxqgqnnfv.html

TS:   // Node.js：readline 模块
来源：http://hz.hongshengwenyu.top/gtfskrwfia.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.quarkkingdee.top/gtifvfphif.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.mhx1999.top/gtwsujdaab.html

Ruby: gets.chomp
来源：http://hz.hywenlv.cn/gtnqciqinm.html

C#:   Console.ReadLine();
来源：http://hz.gaohongyu789.top/gtofedyoia.html

[A21] 保留指定小数位输出
来源：http://hz.hnqzz.top/gtkwlyotdk.html

Py:   f"{3.14159:.2f}"
来源：http://hz.0kj1m.cn/gtdcyhywir.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtsgrwkxrr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.sweek.top/gtprswivsu.html

TS:   (3.14159).toFixed(2)
来源：http://hz.c1oappe.top/gtcahblvwe.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.fengsongda.top/gtuwjfejiz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cqqwz.cn/gtsyjnuuwx.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.316326.xyz/gtxjpnwzkx.html

C#:   3.14159.ToString("F2")
来源：http://hz.yj202588.top/gtnkmtlzkw.html

[A22] 获取字符串长度
来源：http://hz.chenzaomai.com/gtvrfqcige.html

Py:   len(s)
来源：http://hz.pycfn.com/gtxbqegdkg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.bjfxy.top/gthakbrhao.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.xuanzx.com/gtlxigqumd.html

TS:   s.length
来源：http://hz.birdmap.top/gtpwdvpbkm.html

Java: s.length()
来源：http://hz.yj20258888.top/gtixqdfykb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.cucudq.cn/gtzdplxikx.html

Ruby: s.length
来源：http://hz.gotoacloud.top/gtttyhtlap.html

C#:   s.Length
来源：http://hz.yongpay.top/gtdwldnrdj.html

[A23] 大小写转换
来源：http://hz.ehwqpu.com/gtswbxwvvg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.hysaishi.cn/gtupdlguli.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.smart0.xyz/gtfccrcigl.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jqgufenzy.top/gtsfnnjkjb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jinqigfzy.top/gtcqzqwfta.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.sysykeji.top/gtjhcpntke.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.daxiang520.top/gtdderyvcq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.mhx1999.top/gthsevbghp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jianghu66.top/gtggaxluew.html

[A24] 去除首尾空白
来源：http://hz.hongshengwenyu.top/gtasvkiovu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.mhx1999.top/gtjpmbmzke.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.birdmap.top/gtpooyayvu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.cdnleiting.top/gtwbxtrdvc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.9152youxi.cn/gtjqerbjpg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.sxryk.cn/gtnlsspbdj.html

Go:   strings.TrimSpace(s)
来源：http://hz.feifeiyinyue.top/gtmngvznkv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.0kj1m.cn/gtdnayofys.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.gogol.net.cn/gtuzuacjei.html

[A25] 字符串比较
来源：http://hz.ivvv.top/gtsfudtwdz.html

Py:   s1 == s2; s1 != s2
来源：http://hz.pengpengdd.cyou/gtmxftpccc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.jinqigfzy.top/gtnajtwlcg.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.hysaishi.cn/gtrhuxkuqu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgufenzy.top/gtmrmmzaak.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yanxiufei.cn/gtcytqasso.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.iojbl.cn/gtdchdzfdx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.zhijiandao.cn/gtwwzvklkg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.birdmap.top/gtrpmjitbz.html

[A26] 类型转换总览
来源：http://hz.zhaomingkeji.xyz/gtotfunkzc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.dashuyun.cn/gtpeasbklq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.fengsongda.top/gtuoyzhtjc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.xingfuxueyuan.xyz/gtmlcdlpxv.html

TS:   Number() String() Boolean() x as number
来源：http://hz.svipenyu.cn/gtimvqitnh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jyoumei.cn/gtvxxvcmvj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hnqzz.top/gtonxmfjsh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.bjfxy.top/gtaxhgadmm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yvedp.cn/gtvhlhgsmc.html

================================================================================
来源：http://hz.gogol.net.cn/gtjgfnizsn.html

B. 流程控制
来源：http://hz.yj202588.top/gtovirouby.html

================================================================================
来源：http://hz.redwolf501.top/gtonxzzark.html

[B01] 条件判断 if / else
来源：http://hz.sufxvd.cn/gtzvlkegbf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.aizwys.cn/gtnrziishz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.guowangkeji.top/gtxwbljbfl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.shanyushiyangkeji.top/gtxsrfuvwt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.aibaodan.cn/gtlytasbuw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gtxhozodcc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.shangyingyoupin.top/gtlgsymsan.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.xingfuxueyuan.xyz/gtuqtrpiho.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.yuanzhike.top/gtnstnnwbs.html

[B02] 多分支 else if / elif
来源：http://hz.ywan-chungtsiang.top/gtrbntnpxn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.jinqigfzy.top/gtenhqsgvb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.tanke756.top/gtbydobcic.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xuanzx.com/gtrwiogsuf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xziqi.cn/gtqcnddcou.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgufenzy.top/gtznzvruwy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.sufxvd.cn/gtzhaerybu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.quarkkingdee.top/gtuidvtcqu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtmzjnscql.html

[B03] switch / match / case
来源：http://hz.gogol.net.cn/gtwbnawjll.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jinghuilouyu.cn/gtzqtxkstw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtgawsvede.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.yvedp.cn/gtuvyaahzt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenjidiqi.icu/gtivtazgwh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.0kj1m.cn/gtdkzqcpxe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cashguo.top/gtgrngliyx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.jqgfzy.top/gtnwxwegyq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jinqigfzy.top/gtnryfulzj.html

[B04] for 计数循环
来源：http://hz.chenlongwang.top/gteacdtwvs.html

Py:   for i in range(10): print(i)
来源：http://hz.tianlin.xyz/gtedomnsrg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zhixingplan.top/gtdnhhdiec.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.xylfe.cn/gtdegyeidu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.quarkkingdee.top/gtbwuoqrcp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xuanzx.com/gtabicfgpj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xuanzx.com/gtrvbuhvdx.html

Ruby: 10.times { |i| puts i }
来源：http://hz.tanke756.top/gtytvwnmoe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhoulong.xyz/gtmwmqjrdo.html

[B05] 遍历数组 / 列表
来源：http://hz.xinyue.icu/gtyhaduxgf.html

Py:   for item in arr: print(item)
来源：http://hz.fengsongda.top/gtcreistvu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yuxming.cn/gtxgabjzwi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hongshengwenyu.top/gtertsvtxu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xinyue.icu/gteighsxzx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ybcxt.top/gtswiscccb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cheryme.top/gtjmhtomer.html

Ruby: arr.each { |item| puts item }
来源：http://hz.hnqzz.top/gtmzeqypsj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ywan-chungtsiang.top/gtdeniepft.html

[B06] 遍历字典 / 对象
来源：http://hz.jinghuilouyu.cn/gtqwcyvzjz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.nanxuanxn.top/gtekrxfgxl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.chenlongwang.top/gtsyvcmhxh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jqgfzy.top/gtzzazdora.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gtuournohw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.ydjk.org.cn/gtysellomq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.kuanghao11.cn/gtmfjzczff.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hongshengwenyu.top/gtfcrglcjp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.9152youxi.cn/gtajfmrete.html

[B07] while 循环
来源：http://hz.tanke756.top/gtiwirpvnk.html

Py:   while i < 10: i += 1
来源：http://hz.yuxming.cn/gtbxzwmdgw.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jiagoushi.top/gthptcpdou.html

JS:   while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtxtcgaobh.html

TS:   while (i < 10) { i++; }
来源：http://hz.shangyingyoupin.top/gtjmyztjuf.html

Java: while (i < 10) { i++; }
来源：http://hz.bjfxy.top/gtcruxszka.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cqqwz.cn/gthyfjvull.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yueranfly.top/gtylsonsea.html

C#:   while (i < 10) { i++; }
来源：http://hz.tianlin.xyz/gtuonykryb.html

[B08] do-while（至少执行一次）
来源：http://hz.316326.xyz/gtjevypmnm.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.shzxlz.cn/gtjmyccyql.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gotoacloud.top/gtynjeizyo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.dashuyun.cn/gtnixjytci.html

TS:   do { i++; } while (i < 10);
来源：http://hz.feifeiyinyue.top/gtqgueodck.html

Java: do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtpbhhzwxl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.dashuyun.cn/gttjpvuyio.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.guannengcc.top/gtjpnprjxv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtqawfkbqk.html

[B09] break 与 continue
来源：http://hz.bjfxy.top/gtkqsjcwtg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.gzhubu.top/gtyxohvpba.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.kuanghao11.cn/gtybwqtwrt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.zdqjudy.top/gtymlteymd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.316326.xyz/gtlwghboxb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ehwqpu.com/gtitpxhmop.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.dianchejie.cn/gtkdvglrne.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.bjfxy.top/gtwxdwbtgl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guannengcc.top/gtekgybfik.html

[B10] 遍历同时拿索引
来源：http://hz.shanyushiyangkeji.top/gtzrkntaqj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.sweek.top/gtldofzvpf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ppjwa.cn/gtnpjutnfo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gogol.net.cn/gtlrwwvnhz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.tianlin.xyz/gtzykljyyl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.svipenyu.cn/gtpdtonmex.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.nwbrower.top/gtqwxvnavr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.smart0.xyz/gtijvztdgd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.ppjwa.cn/gtwtzoqeqd.html

[B11] 生成数字序列 / 区间
来源：http://hz.hywenlv.cn/gtybsebxqt.html

Py:   list(range(0, 10, 2))
来源：http://hz.birdmap.top/gtymcgqxxe.html

PHP:  range(0, 10, 2);
来源：http://hz.zhoulong.xyz/gttymcrhgr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtjkutgbsd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigfzy.top/gtyifodpcq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yongpay.top/gtniclkpny.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhixingplan.top/gtskqsxpzv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhixingplan.top/gtrognmjrz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.nanxinkj.top/gtddefalvn.html

[B12] 跳出多层循环
来源：http://hz.hnqzz.top/gtkpvbzmai.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.hnqzz.top/gtfannxgdo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gaohongyu789.top/gtqyqgvcyr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gtfztzbvwk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zdqjudy.top/gtgsmqncem.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtecbqzedo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shanyushiyangkeji.top/gtaagjyxgd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yanxiufei.cn/gtdlnzmkos.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.bjfxy.top/gtpdervugu.html

[B13] 判断是否为数字
来源：http://hz.cdnleiting.top/gtpsxvffla.html

Py:   isinstance(x, (int, float))
来源：http://hz.kuanghao11.cn/gtxibnzupp.html

PHP:  is_numeric($x)
来源：http://hz.guannengcc.top/gtjnozhuql.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nwbrower.top/gthlmwyhkh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xziqi.cn/gtazjtoeoz.html

Java: x instanceof Number
来源：http://hz.nanxinkj.top/gtovpqshlk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.dashuyun.cn/gtmpywmuvb.html

Ruby: x.is_a?(Numeric)
来源：http://hz.chenjidiqi.icu/gtoifsplew.html

C#:   x is int or double or decimal
来源：http://hz.chenzaomai.com/gtmcyuejdz.html

[B14] 判断值是否在集合内
来源：http://hz.hfpthk.cn/gtosebeemo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.daxiang520.top/gtctwivmkh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.dashuyun.cn/gtjrtdyahs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.dianchejie.cn/gtffbcubds.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtqwpwlzso.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.guowangkeji.top/gtnaiewjvh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daria6918.cn/gtxsuvfqdz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hysaishi.cn/gtsajbnjsu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.guowangkeji.top/gtglhksile.html

[B15] 布尔运算与取反
来源：http://hz.quarkkingdee.top/gtfxptnlay.html

Py:   a and b or not c
来源：http://hz.birdmap.top/gtxllmyusx.html

PHP:  $a && $b || !$c
来源：http://hz.gaohongyu789.top/gtjfwufiof.html

JS:   a && b || !c
来源：http://hz.xinyue.icu/gtxsdtepmp.html

TS:   a && b || !c
来源：http://hz.zhongyouzk.top/gtabyjlnuz.html

Java: a && b || !c
来源：http://hz.shanyushiyangtech.top/gtovsfnnnx.html

Go:   a && b || !c
来源：http://hz.yuxming.cn/gtmvatmeku.html

Ruby: a && b || !c
来源：http://hz.yj202588.top/gtzauadrjv.html

C#:   a && b || !c
来源：http://hz.mhx1999.top/gtlseowaev.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.quarkkingdee.top/gtrimntydm.html

Py:   if not data: return
来源：http://hz.fengsongda.top/gtgfsnwzce.html

PHP:  if (!$data) { return; }
来源：http://hz.shanyushiyangkeji.top/gtorszdzfl.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtrjmzchtn.html

TS:   if (!data) return;
来源：http://hz.pengpengdd.cyou/gtihppbfen.html

Java: if (data == null) return;
来源：http://hz.snrcjt.cn/gtnsivvans.html

Go:   if data == nil { return }
来源：http://hz.andypj.xyz/gtgicntwcm.html

Ruby: return if data.nil?
来源：http://hz.jiagoushi.top/gtxbcdmlqo.html

C#:   if (data == null) return;
来源：http://hz.daria6918.cn/gtnltemixq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtnfjzdahz.html

C. 函数与作用域
来源：http://hz.cucudq.cn/gtrglcrmqo.html

================================================================================
来源：http://hz.ppjwa.cn/gtnrknjrzq.html

[C01] 定义函数
来源：http://hz.xingfuxueyuan.xyz/gtcpwjqmqy.html

Py:   def add(a, b): return a + b
来源：http://hz.xuetiantiany.cn/gtvkkoecvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tanke756.top/gtlmyhbqrq.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ivvv.top/gthmrycaqs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtdwyyrxdc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtqyugaycx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xinyue.icu/gtnfaeeoff.html

Ruby: def add(a, b); a + b; end
来源：http://hz.andypj.xyz/gtigsivtya.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtdxeqlsdf.html

[C02] 默认参数
来源：http://hz.hysaishi.cn/gtulergxqd.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258.top/gtbuekjckf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jiagoushi.top/gtlpumkvks.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nanxinkj.top/gtalqjccnh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinghuilouyu.cn/gteexjcwfc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.iojbl.cn/gtdsrgowpj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinqigfzy.top/gttwtsiaui.html

Ruby: def greet(name = "World") = name
来源：http://hz.guannengcc.top/gtuuagllgb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hongshengwenyu.top/gtxubplnje.html

[C03] 可变参数
来源：http://hz.yj20258888.top/gturvqaiaq.html

Py:   def total(*args): return sum(args)
来源：http://hz.yueranfly.top/gtcidzieww.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.gzhubu.top/gtmpbsgcza.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtwqsoevxy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nanxuanxn.top/gtmgncempo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.pycfn.com/gtpjjadufr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jinqigfzy.top/gtrsteyhzp.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhengqikj.top/gtdcsjgvlr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fengsongda.top/gtsdlouzat.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yuanzhike.top/gtsyfwcxca.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daria6918.cn/gtgmkltwmu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sysykeji.top/gtijdcrjre.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.havefunace.top/gtwahyuhnx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.chenzaomai.com/gtffsqibst.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.pycfn.com/gttflllgcj.html

Go:   // 无：用配置结构体参数
来源：http://hz.jianghu66.top/gtcvsryqpw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtxtoqifwn.html

C#:   f(a: 1, b: 2)
来源：http://hz.chenlongwang.top/gtwlsodqnk.html

[C05] 返回多个值
来源：http://hz.daria6918.cn/gtwndjeyhf.html

Py:   return a, b
来源：http://hz.ppjwa.cn/gtjcwtdsbf.html

PHP:  return [$a, $b];
来源：http://hz.nanxuanxn.top/gtrqkliwwk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ppjwa.cn/gtwvkbvqij.html

TS:   return { a, b };
来源：http://hz.chenzaomai.com/gtooeqlriq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cucudq.cn/gtlwgfqzoz.html

Go:   return a, b
来源：http://hz.316326.xyz/gtlctdslvd.html

Ruby: return a, b
来源：http://hz.tanke756.top/gttbdpcgjl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.guowangkeji.top/gtxullwsph.html

[C06] 匿名函数 / lambda
来源：http://hz.dashuyun.cn/gtosribaaz.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258.top/gthzcxzwnu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.gogol.net.cn/gtrbtlkmuc.html

JS:   const square = x => x * x;
来源：http://hz.aizwys.cn/gtueezcqwx.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.haohaochexian.top/gtsnryxnvc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.daxiang520.top/gthjqmvcnv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.quarkkingdee.top/gtidgpzitf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.nanxinkj.top/gtntlnxrde.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gaohongyu789.top/gthkzdejqv.html

[C07] 把函数作为参数传入
来源：http://hz.svipenyu.cn/gtlzbfwchj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daxiang520.top/gtojkiscer.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xinyue.icu/gttuwrihzu.html


<!-- 参考信息 -->