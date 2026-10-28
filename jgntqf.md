代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.ppjwa.cn/gtdaqpjgvy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.snrcjt.cn/gtipkjrvcy.html

TS:   if (!x) {}
来源：http://hz.daria6918.cn/gtrkmfrgdc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.bjfxy.top/gtdcbamyiq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.hammf.cn/gtjxdotgvs.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.ywan-chungtsiang.top/gtucqmvcyg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.smart0.xyz/gtezyeaugt.html

[A17] 位运算
来源：http://hz.zhiwuduotai.top/gtmqvfwezu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jyoumei.cn/gtepvxdpsn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.yj20258888.top/gttoawebuk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fengsongda.top/gtfzomxaao.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.daxiang520.top/gtxhaxiotq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ybcxt.top/gtnsborste.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.nanxuanxn.top/gtpjtngjbu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.shanyushiyangtech.top/gtwmsjrots.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj202588.top/gtiwvtyulr.html

[A18] 字符与 ASCII 码互转
来源：http://hz.c1oappe.top/gtizdyecck.html

Py:   ord("A"); chr(65)
来源：http://hz.kuanghao11.cn/gtptfkpmmx.html

PHP:  ord("A"); chr(65)
来源：http://hz.cucudq.cn/gtgstssqyy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xziqi.cn/gtbuhjpohu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.yuxming.cn/gteysgoetb.html

Java: (int) 'A'; (char) 65
来源：http://hz.wangdashe.top/gteijxlfpz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.haohaochexian.top/gtryqpjrud.html

Ruby: "A".ord; 65.chr
来源：http://hz.fzhhl.top/gtiyioyzxe.html

C#:   (int)'A'; (char)65
来源：http://hz.ywan-chungtsiang.top/gtslkxikea.html

[A19] 交换两个变量
来源：http://hz.52xcode.cn/gtmvhmseai.html

Py:   a, b = b, a
来源：http://hz.yonumen.top/gtfgmpxxqw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hnxiangtu.top/gtemfbgicd.html

JS:   [a, b] = [b, a];
来源：http://hz.yj202588.top/gthgabcwxx.html

TS:   [a, b] = [b, a];
来源：http://hz.havefunace.top/gtdbyrxbpg.html

Java: int t = a; a = b; b = t;
来源：http://hz.meibo888.top/gtlslofcsr.html

Go:   a, b = b, a
来源：http://hz.ivvv.top/gtrpszsjuv.html

Ruby: a, b = b, a
来源：http://hz.dashuyun.cn/gtzwvsgdlt.html

C#:   (a, b) = (b, a);
来源：http://hz.gaohongyu789.top/gtesvacfdh.html

[A20] 读取标准输入
来源：http://hz.yvedp.cn/gtbpkyyijq.html

Py:   name = input("请输入：")
来源：http://hz.jyoumei.cn/gtlyswtbjk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.hammf.cn/gtvuqgacpz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.yj202588.top/gtedfdvtwp.html

TS:   // Node.js：readline 模块
来源：http://hz.ywan-chungtsiang.top/gtzvwjhhim.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.yj20258.top/gtgxdktgxo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yj20258.top/gtvlfffble.html

Ruby: gets.chomp
来源：http://hz.shanyushiyangkeji.top/gtlwjvtibd.html

C#:   Console.ReadLine();
来源：http://hz.redwolf501.top/gttwhcrmrq.html

[A21] 保留指定小数位输出
来源：http://hz.nanxinkj.top/gtzgirjabv.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zhijiandao.cn/gtytwscifo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gthhmvdnzg.html

JS:   (3.14159).toFixed(2)
来源：http://hz.hongshengwenyu.top/gtqqjeaabx.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zhoulong.xyz/gtjkxrsjsf.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.gzhubu.top/gtsdchgzee.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.cdnleiting.top/gtgdnchdiq.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.nanxinkj.top/gtsjzlxdwh.html

C#:   3.14159.ToString("F2")
来源：http://hz.hammf.cn/gtxiytmcux.html

[A22] 获取字符串长度
来源：http://hz.yj20258888.top/gtufipdiwk.html

Py:   len(s)
来源：http://hz.hfpthk.cn/gtakmkorfu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.tanke756.top/gttdvyjduk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.zhixingplan.top/gtlnqgvgmo.html

TS:   s.length
来源：http://hz.gotoacloud.top/gtoiiegbuq.html

Java: s.length()
来源：http://hz.guannengcc.top/gtuovswxnt.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.gzhubu.top/gtnodaovqs.html

Ruby: s.length
来源：http://hz.aibaodan.cn/gtyzgnztja.html

C#:   s.Length
来源：http://hz.cashguo.top/gtodgfpcbq.html

[A23] 大小写转换
来源：http://hz.tian-w.cn/gtpgdkczrb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.yvedp.cn/gtdxbaclig.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.guannengcc.top/gtutelkaoa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.hysaishi.cn/gtaxebzwkv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.meibo888.top/gtrpzsxjjn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gtgbsouumz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.gogol.net.cn/gtlaevmkfe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xingfuxueyuan.xyz/gtbasusgir.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yangfankeji.com/gthfupyzsx.html

[A24] 去除首尾空白
来源：http://hz.chenjidiqi.icu/gtptfkglps.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.daxiang520.top/gteoeeuspz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.hammf.cn/gtwcehtfuj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.aizwys.cn/gtuuirdsik.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.tanke756.top/gtayrrqfqo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gotoacloud.top/gtuygkyjjg.html

Go:   strings.TrimSpace(s)
来源：http://hz.xinyue.icu/gtzqwftloy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.kuanghao11.cn/gtfqqwlumv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.cashguo.top/gtyuhtdjuo.html

[A25] 字符串比较
来源：http://hz.jinqigfzy.top/gtchirnsss.html

Py:   s1 == s2; s1 != s2
来源：http://hz.zhiwuduotai.top/gtdxiwtthr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.gotoacloud.top/gtniixgsyl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.pycfn.com/gtovxsxmjc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.52xcode.cn/gtosmyjevd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.snrcjt.cn/gtwddnvvgy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cheryme.top/gtdfnzlqbm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.chenzaomai.com/gtqzqtvdxb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jqgufenzy.top/gtldbyytsu.html

[A26] 类型转换总览
来源：http://hz.chenlongwang.top/gtmmjehubw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zhengqikj.top/gtiirlktvj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jqgfzy.top/gtynnvnydp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.gzhubu.top/gtrvpmxugw.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jyoumei.cn/gtyixetmfw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.shanyushiyangkeji.top/gtwovwuzub.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.zhixingplan.top/gtrvdqpber.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.sufxvd.cn/gtnzhqccmt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xuanzx.com/gtcnpakthm.html

================================================================================
来源：http://hz.tanke756.top/gthqinyvym.html

B. 流程控制
来源：http://hz.ybcxt.top/gtfgwaleeg.html

================================================================================
来源：http://hz.kuanghao11.cn/gtbgfzxgae.html

[B01] 条件判断 if / else
来源：http://hz.yuxming.cn/gteelnyzii.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.ehwqpu.com/gttqmpjiui.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.shuidangran.top/gthdsiwrdm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtmnqnwslc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jyoumei.cn/gtdlmtrmwc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.sweek.top/gtveqynfyx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.nwbrower.top/gtppqkbcwh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.jiagoushi.top/gtycfgnzcq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.316326.xyz/gtssirwaax.html

[B02] 多分支 else if / elif
来源：http://hz.andypj.xyz/gtdyxxekje.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.xziqi.cn/gtatgawddv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.chenjidiqi.icu/gtpdcppgjq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenzaomai.com/gtwuhrfjju.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yvedp.cn/gtwrpscbcp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.sufxvd.cn/gtffpduwor.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.cqqwz.cn/gtnabmsspv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinqigfzy.top/gtjihbvcvk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangshuangyany.cn/gthhlapzrx.html

[B03] switch / match / case
来源：http://hz.guannengcc.top/gtyrgtvitp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.xuanzx.com/gtprlttrop.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.ivvv.top/gtchidgvmn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.vqdsnc.cn/gtgtiwgrfj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.xingfuxueyuan.xyz/gtpigcpilu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.chenlongwang.top/gtwzvhbhjv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yonumen.top/gtuamsfvoj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.haohaochexian.top/gtlcortdpx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.nanxuanxn.top/gtrddkcixy.html

[B04] for 计数循环
来源：http://hz.guannengcc.top/gtpeivbxot.html

Py:   for i in range(10): print(i)
来源：http://hz.andypj.xyz/gtkrvcbwmd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.tianlin.xyz/gtyikauucx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.dianchejie.cn/gtkawcstir.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhongyouzk.top/gtjljpshxt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.hnxiangtu.top/gtimbryzqc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jianghu66.top/gtqugmgabh.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shuidangran.top/gtdyiazssb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.fengsongda.top/gtusjpyfnt.html

[B05] 遍历数组 / 列表
来源：http://hz.birdmap.top/gtnommqdng.html

Py:   for item in arr: print(item)
来源：http://hz.andypj.xyz/gtxiggtpig.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.daxiang520.top/gtfvhdenzm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.haohaochexian.top/gtfzbdjjcq.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.cashguo.top/gtztjhshfw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.ehwqpu.com/gtaogkpghj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.chenzaomai.com/gtrglufola.html

Ruby: arr.each { |item| puts item }
来源：http://hz.sweek.top/gtdvynmgen.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.zhoulong.xyz/gtsfjxjqcy.html

[B06] 遍历字典 / 对象
来源：http://hz.cqqwz.cn/gtxvslslmc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.guannengcc.top/gttkximepd.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.xuanzx.com/gtifburqtn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jinqigfzy.top/gtaicmvafc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yongpay.top/gtcsljzmoh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.wangshuangyany.cn/gtytpnjvzv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.xingfuxueyuan.xyz/gtjvdkliru.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.fzhhl.top/gtinshnxgd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.bjfxy.top/gtldzlvvjv.html

[B07] while 循环
来源：http://hz.zycfv.cn/gtjeqyxqlb.html

Py:   while i < 10: i += 1
来源：http://hz.mhx1999.top/gtdmzzsvjn.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ybcxt.top/gtixznuqkq.html

JS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangkeji.top/gtvgrjdibp.html

TS:   while (i < 10) { i++; }
来源：http://hz.shzxlz.cn/gtldwsyhep.html

Java: while (i < 10) { i++; }
来源：http://hz.yueranfly.top/gthcjeioet.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.xinyue.icu/gtsghhobka.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhoulong.xyz/gtwwpumtwl.html

C#:   while (i < 10) { i++; }
来源：http://hz.pycfn.com/gtpqrlikyh.html

[B08] do-while（至少执行一次）
来源：http://hz.yj20258.top/gtkxnqrybl.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.sxryk.cn/gtsrdksqyp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hnqzz.top/gtmdmpsimg.html

JS:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtvazjldvx.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jlsjyb.cn/gtbknvrxow.html

Java: do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gtjunbbvlg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj20258888.top/gtquywxvzf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.xziqi.cn/gtqioyqapu.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yuanzhike.top/gtreektzpe.html

[B09] break 与 continue
来源：http://hz.hfpthk.cn/gtjfayijoz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.feifeiyinyue.top/gtqacrupuw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xingfuxueyuan.xyz/gtwoerliye.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cashguo.top/gtmdfvkocc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gzhubu.top/gtebgihiyb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xuetiantiany.cn/gtaxpbiuog.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.tanke756.top/gtupitppru.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.chenzaomai.com/gtsuzvwqwr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.guowangkeji.top/gtmvfhsmpw.html

[B10] 遍历同时拿索引
来源：http://hz.gzhubu.top/gtphvpjape.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenlongwang.top/gtjurctfox.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.zhaomingkeji.xyz/gtypypkukt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hywenlv.cn/gtrjcyvewl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.fengsongda.top/gtcknicuov.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jiagoushi.top/gtisqnnnfu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhengqikj.top/gtjomtjjsn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.zhongyouzk.top/gtwycblzlu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.fengsongda.top/gtppuogsvz.html

[B11] 生成数字序列 / 区间
来源：http://hz.jqgufenzy.top/gtaiagpopb.html

Py:   list(range(0, 10, 2))
来源：http://hz.0kj1m.cn/gtsmbzucfa.html

PHP:  range(0, 10, 2);
来源：http://hz.yangfankeji.com/gtmddixmxx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.andypj.xyz/gthjuvlrjn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ywan-chungtsiang.top/gtnwcxsixy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.vqdsnc.cn/gtuukahoop.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yanxiufei.cn/gtjkwusrbr.html

Ruby: (0...10).step(2).to_a
来源：http://hz.aizwys.cn/gtrwkpdtbe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.snrcjt.cn/gtpsrxsbjc.html

[B12] 跳出多层循环
来源：http://hz.ivvv.top/gtrbgcagto.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhongyouzk.top/gttvimnghb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jyoumei.cn/gttylymjkg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenlongwang.top/gtyxpvgdkt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.cdnleiting.top/gtpijsywvm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.hysaishi.cn/gtbzhykken.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.cdnleiting.top/gtmhymjdjy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.andypj.xyz/gtnjhfjdvw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.wangdashe.top/gtphcbnlxk.html

[B13] 判断是否为数字
来源：http://hz.52xcode.cn/gtroyftjuv.html

Py:   isinstance(x, (int, float))
来源：http://hz.birdmap.top/gtdwxjmxxw.html

PHP:  is_numeric($x)
来源：http://hz.zdqjudy.top/gtrdirxqsf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gtuqjztljs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sxryk.cn/gtmwsiuhii.html

Java: x instanceof Number
来源：http://hz.fzhhl.top/gtezlwednu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ywan-chungtsiang.top/gtnafglnhd.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhiwuduotai.top/gtwzpyxuss.html

C#:   x is int or double or decimal
来源：http://hz.nwbrower.top/gtdkqrltee.html

[B14] 判断值是否在集合内
来源：http://hz.xziqi.cn/gtlbjtdgsj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.nwbrower.top/gtnmubzaxx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.shanyushiyangtech.top/gtthznhtcf.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtsxbflpgw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.pycfn.com/gtemxknbks.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.ybcxt.top/gtrgbnujhf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guowangkeji.top/gtfuulnahe.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinghuilouyu.cn/gtmgrzrhqy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.chenzaomai.com/gtzbjplxfr.html

[B15] 布尔运算与取反
来源：http://hz.gogol.net.cn/gthiizdjnj.html

Py:   a and b or not c
来源：http://hz.xuanzx.com/gtnpzvfguj.html

PHP:  $a && $b || !$c
来源：http://hz.svipenyu.cn/gtydclerex.html

JS:   a && b || !c
来源：http://hz.cdnleiting.top/gtydlvjfny.html

TS:   a && b || !c
来源：http://hz.nwbrower.top/gtzdugbzxv.html

Java: a && b || !c
来源：http://hz.svipenyu.cn/gtttnkgefs.html

Go:   a && b || !c
来源：http://hz.sweek.top/gteazhellv.html

Ruby: a && b || !c
来源：http://hz.kuanghao11.cn/gtbtdqcwba.html

C#:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtbkchpbfe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yvedp.cn/gtxlinyghx.html

Py:   if not data: return
来源：http://hz.feifeiyinyue.top/gtqjpzlegf.html

PHP:  if (!$data) { return; }
来源：http://hz.andypj.xyz/gtllzugkbr.html

JS:   if (!data) return;
来源：http://hz.ehwqpu.com/gtcwlwmjmv.html

TS:   if (!data) return;
来源：http://hz.xylfe.cn/gtefwxlxmv.html

Java: if (data == null) return;
来源：http://hz.fzhhl.top/gtzkukbonl.html

Go:   if data == nil { return }
来源：http://hz.dashuyun.cn/gthcydozxh.html

Ruby: return if data.nil?
来源：http://hz.kuanghao11.cn/gtznwcgnxf.html

C#:   if (data == null) return;
来源：http://hz.yj20258.top/gtbgbpuzzs.html

================================================================================
来源：http://hz.hysaishi.cn/gtcbzkduou.html

C. 函数与作用域
来源：http://hz.dianchejie.cn/gtttmluqwr.html

================================================================================
来源：http://hz.sweek.top/gtivegodsw.html

[C01] 定义函数
来源：http://hz.shanyushiyangkeji.top/gtgkhklzul.html

Py:   def add(a, b): return a + b
来源：http://hz.jinyuanbaomall.cn/gtsgduqwco.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guowangkeji.top/gtamhtgnfn.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtscsadiex.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gtdkkktbld.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yonumen.top/gtvyttoibo.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yanxiufei.cn/gtwqxsuecl.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nwbrower.top/gtipiienfw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtxbmrviaw.html

[C02] 默认参数
来源：http://hz.yuanzhike.top/gtoglziuoj.html

Py:   def greet(name="World"): return name
来源：http://hz.chenlongwang.top/gtbbdfszjw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.aibaodan.cn/gtagmgqnoq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtotrseebk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtafzdqrfz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.birdmap.top/gtyhncwsii.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.snrcjt.cn/gtqfvinusx.html

Ruby: def greet(name = "World") = name
来源：http://hz.chenlongwang.top/gtidpqbldb.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhiwuduotai.top/gtarebiwkj.html

[C03] 可变参数
来源：http://hz.xinyue.icu/gttzirrmor.html

Py:   def total(*args): return sum(args)
来源：http://hz.xingfuxueyuan.xyz/gtllpbosuj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xylfe.cn/gtrwudeili.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gtrevezwlk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gtgrbadtju.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.iojbl.cn/gtfdmwurpr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tianlin.xyz/gtxswfqted.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigfzy.top/gtacyiyust.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.andypj.xyz/gtrbfbbbam.html

[C04] 命名参数 / 关键字参数
来源：http://hz.aizwys.cn/gtgarvlsvx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.andypj.xyz/gtdbjaycqx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhixingplan.top/gthuaejvjf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sweek.top/gtljhucgeu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xinyue.icu/gtakqikybo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhijiandao.cn/gtdxgfhkqs.html

Go:   // 无：用配置结构体参数
来源：http://hz.pycfn.com/gtmfwopeuk.html

Ruby: f(a: 1, b: 2)
来源：http://hz.sufxvd.cn/gtoichgryu.html

C#:   f(a: 1, b: 2)
来源：http://hz.c1oappe.top/gthhjjtihl.html

[C05] 返回多个值
来源：http://hz.chenlongwang.top/gtauzgvkwo.html

Py:   return a, b
来源：http://hz.316326.xyz/gtvgfhndvw.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gthcwfcjym.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.daxiang520.top/gtthmianpd.html

TS:   return { a, b };
来源：http://hz.zhijiandao.cn/gtdfdifxup.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ywan-chungtsiang.top/gtvgurhgvn.html

Go:   return a, b
来源：http://hz.pycfn.com/gtzmkcqptz.html

Ruby: return a, b
来源：http://hz.haohaochexian.top/gtegtomiok.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.smart0.xyz/gtyuwmhvle.html

[C06] 匿名函数 / lambda
来源：http://hz.shzxlz.cn/gtvhegcrls.html

Py:   square = lambda x: x * x
来源：http://hz.ybcxt.top/gtfvhuoids.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.andypj.xyz/gtfqrcjjqa.html

JS:   const square = x => x * x;
来源：http://hz.gzhubu.top/gtyoxeqidw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jinghuilouyu.cn/gtekikvglq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.bjfxy.top/gtuecdnedd.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.smart0.xyz/gtzvrhyvtv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.fengsongda.top/gtxwisurjx.html


<!-- 参考信息 -->