代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.ybcxt.top/gtelizgcml.html

C#:   var value = data ?? "默认值";
来源：http://hz.cheryme.top/gthedeyeye.html

[A16] 真假值判断规则
来源：http://hz.zycfv.cn/gtgjfnzahq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.haohaochexian.top/gtnxzlalrm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.shanyushiyangkeji.top/gtamjqyksl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.chenzaomai.com/gtvargmiik.html

TS:   if (!x) {}
来源：http://hz.sweek.top/gtjpbeoqbw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.tian-w.cn/gtdmbdejtg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.hysaishi.cn/gtbcbbgewv.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.jqgfzy.top/gtadwwohjp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.daxiang520.top/gtcqfaduyz.html

[A17] 位运算
来源：http://hz.nwbrower.top/gtlbqjjrsl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.daria6918.cn/gtduxmudxc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.gaohongyu789.top/gtqacljwop.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ybcxt.top/gtudxlnlpg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.gaohongyu789.top/gtagzgtboc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yangfankeji.com/gtajluqvja.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtihfwcsko.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.cheryme.top/gtblauqjzm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.sufxvd.cn/gtiialfvqj.html

[A18] 字符与 ASCII 码互转
来源：http://hz.nanxinkj.top/gtdzkzpjcc.html

Py:   ord("A"); chr(65)
来源：http://hz.chenzaomai.com/gtyyryltxw.html

PHP:  ord("A"); chr(65)
来源：http://hz.vqdsnc.cn/gtibicldbf.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.nanxuanxn.top/gtrkffaija.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daxiang520.top/gtcfgzcmkw.html

Java: (int) 'A'; (char) 65
来源：http://hz.fengsongda.top/gtuwxbephp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.snrcjt.cn/gtpxzdijwv.html

Ruby: "A".ord; 65.chr
来源：http://hz.meibo888.top/gtasgvfcuv.html

C#:   (int)'A'; (char)65
来源：http://hz.gzhubu.top/gtbcwqizry.html

[A19] 交换两个变量
来源：http://hz.zhixingplan.top/gtrvjxfvzu.html

Py:   a, b = b, a
来源：http://hz.aizwys.cn/gtpdyhgair.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.zycfv.cn/gtxcvwmxuj.html

JS:   [a, b] = [b, a];
来源：http://hz.jinghuilouyu.cn/gtrfdygdbo.html

TS:   [a, b] = [b, a];
来源：http://hz.hongshengwenyu.top/gtfmleecai.html

Java: int t = a; a = b; b = t;
来源：http://hz.ivvv.top/gtlkuqtlrp.html

Go:   a, b = b, a
来源：http://hz.jinqigufen.top/gtvavzqrke.html

Ruby: a, b = b, a
来源：http://hz.redwolf501.top/gtzjyhhagt.html

C#:   (a, b) = (b, a);
来源：http://hz.jyoumei.cn/gtvlqzmewo.html

[A20] 读取标准输入
来源：http://hz.zdqjudy.top/gtrhwllwfb.html

Py:   name = input("请输入：")
来源：http://hz.tian-w.cn/gtuxifjwwd.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ydzc1.top/gtqvphvkva.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.wangshuangyany.cn/gtbljgmkuu.html

TS:   // Node.js：readline 模块
来源：http://hz.jianghu66.top/gtuahdxotj.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.jqgfzy.top/gtwpiqpemv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.xuanzx.com/gtizvnhjqh.html

Ruby: gets.chomp
来源：http://hz.meibo888.top/gtgdzugdqr.html

C#:   Console.ReadLine();
来源：http://hz.hammf.cn/gtcajplfro.html

[A21] 保留指定小数位输出
来源：http://hz.zhaomingkeji.xyz/gtqdsdtxxj.html

Py:   f"{3.14159:.2f}"
来源：http://hz.andypj.xyz/gtppwrsifm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jinyuanbaomall.cn/gtlgxxcxtt.html

JS:   (3.14159).toFixed(2)
来源：http://hz.fzhhl.top/gtwmqaoync.html

TS:   (3.14159).toFixed(2)
来源：http://hz.cucudq.cn/gtfrnljpxu.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.zhaomingkeji.xyz/gtnbbvabfu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.gzhubu.top/gtyejuwjoa.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.zhijiandao.cn/gtskqgfrfr.html

C#:   3.14159.ToString("F2")
来源：http://hz.redwolf501.top/gttlbdlusg.html

[A22] 获取字符串长度
来源：http://hz.zycfv.cn/gtprrunnzo.html

Py:   len(s)
来源：http://hz.hongshengwenyu.top/gtxkpzfsiy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.pengpengdd.cyou/gthhylwkym.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.nwbrower.top/gtnkiejrxh.html

TS:   s.length
来源：http://hz.wangshuangyany.cn/gtweppfbwe.html

Java: s.length()
来源：http://hz.quarkkingdee.top/gtaazoyszk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.shangyingyoupin.top/gtobwuryea.html

Ruby: s.length
来源：http://hz.zycfv.cn/gttukkaldz.html

C#:   s.Length
来源：http://hz.dashuyun.cn/gtmegbboov.html

[A23] 大小写转换
来源：http://hz.zhiwuduotai.top/gtkmucrgvl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jinqigfzy.top/gtadzasxow.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ivvv.top/gtnympghmq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xingfuxueyuan.xyz/gtrkkqhvtt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.tianlin.xyz/gtivaigzle.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangkeji.top/gteabvkqfa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.sufxvd.cn/gtxaiiqkrc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.tianlin.xyz/gtuopmcatw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.cucudq.cn/gtxhyzjeln.html

[A24] 去除首尾空白
来源：http://hz.yonumen.top/gteqpavywl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhixingplan.top/gtbenptjfc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.iojbl.cn/gthezinici.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xuetiantiany.cn/gtkuhxvelt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.xziqi.cn/gttfnxiajz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gotoacloud.top/gtniuhhhwr.html

Go:   strings.TrimSpace(s)
来源：http://hz.xingfuxueyuan.xyz/gtbxzunslb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.shanyushiyangtech.top/gtigexdvxm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.dianchejie.cn/gtaryumodk.html

[A25] 字符串比较
来源：http://hz.zycfv.cn/gturqqvdfm.html

Py:   s1 == s2; s1 != s2
来源：http://hz.cqqwz.cn/gterwcznnm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.cdnleiting.top/gtdmqrumlv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jianghu66.top/gtngwztbpk.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zycfv.cn/gtkaiqdbqz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.9152youxi.cn/gtiejqgecx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.vqdsnc.cn/gtxqdoobrj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yuanzhike.top/gtpywbcwsr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.cdnleiting.top/gtvsmiibit.html

[A26] 类型转换总览
来源：http://hz.dianchejie.cn/gtvovladsm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.andypj.xyz/gtsnvkukav.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xylfe.cn/gtrqcmbolg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.52xcode.cn/gtntahigzm.html

TS:   Number() String() Boolean() x as number
来源：http://hz.jyoumei.cn/gtkrwjntmf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.cqqwz.cn/gtchdpojxw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.jlsjyb.cn/gttxjcppqe.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.dashuyun.cn/gtloqoqchb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yj202588.top/gtxcrfbqhl.html

================================================================================
来源：http://hz.tianlin.xyz/gtbecehrkt.html

B. 流程控制
来源：http://hz.shzxlz.cn/gtnfxelwgo.html

================================================================================
来源：http://hz.iojbl.cn/gtqfuclifo.html

[B01] 条件判断 if / else
来源：http://hz.cqqwz.cn/gtgrdubfed.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.cheryme.top/gtjdajfhhd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.gaohongyu789.top/gtyjfrciop.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtrpikbsyo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jiagoushi.top/gtkwnnagqd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.redwolf501.top/gtkcylebgb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.yj20258.top/gtswlavtas.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.yvedp.cn/gtuhyjlsod.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhijiandao.cn/gtcuryeosy.html

[B02] 多分支 else if / elif
来源：http://hz.nanxinkj.top/gtrgzitsbq.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cashguo.top/gtzavtozij.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yj20258888.top/gtzphoxlcm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.mhx1999.top/gtbnpdmelf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.ppjwa.cn/gtpihpgfuz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtikdlsvny.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.hnqzz.top/gtftghvils.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.havefunace.top/gtnoftysfh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hfpthk.cn/gtihkvxxfu.html

[B03] switch / match / case
来源：http://hz.dashuyun.cn/gtqlpbdrwa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.vqdsnc.cn/gtysgmzudx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.yanxiufei.cn/gtpstcieyp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.zhijiandao.cn/gtdbqymhro.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.snrcjt.cn/gtkylnyysq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.andypj.xyz/gtmlqfelid.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yuxming.cn/gttsqbhmru.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yj20258.top/gtpjeihzaa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.bjfxy.top/gthaqgwftb.html

[B04] for 计数循环
来源：http://hz.xuanzx.com/gtzgliwwqk.html

Py:   for i in range(10): print(i)
来源：http://hz.pengpengdd.cyou/gtmwqoscvb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.svipenyu.cn/gtpxczuhpj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.pycfn.com/gtfffbkrzu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinyuanbaomall.cn/gtlhohrclj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.cashguo.top/gtnryxdkym.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.redwolf501.top/gtadpccvvx.html

Ruby: 10.times { |i| puts i }
来源：http://hz.chenlongwang.top/gtyxtiifjq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.52xcode.cn/gtjbglnhsl.html

[B05] 遍历数组 / 列表
来源：http://hz.iojbl.cn/gtxvwyeneg.html

Py:   for item in arr: print(item)
来源：http://hz.fengsongda.top/gtgckcwpld.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yj202588.top/gtrgnfzwym.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenjidiqi.icu/gtxtfhwikp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhengqikj.top/gtwajmnpkm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.chenjidiqi.icu/gtzztbqifr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ivvv.top/gticwkqpyq.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zdqjudy.top/gtrjmwdadi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.guowangkeji.top/gtjegkhshd.html

[B06] 遍历字典 / 对象
来源：http://hz.hammf.cn/gtwshfevas.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.316326.xyz/gtkrmuggng.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.pengpengdd.cyou/gtnipscphy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jyoumei.cn/gtksrwlodq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.birdmap.top/gtmkijztlk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.birdmap.top/gtlhhafsdr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hnqzz.top/gtvjiniehg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.guowangkeji.top/gtsdwzmnxt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.jinqigufen.top/gttwuhrsyc.html

[B07] while 循环
来源：http://hz.zhiwuduotai.top/gticoaivdy.html

Py:   while i < 10: i += 1
来源：http://hz.yonumen.top/gtzgbimlop.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yueranfly.top/gtulljmkjf.html

JS:   while (i < 10) { i++; }
来源：http://hz.cashguo.top/gtmwxowagu.html

TS:   while (i < 10) { i++; }
来源：http://hz.ywan-chungtsiang.top/gtajzsrmxn.html

Java: while (i < 10) { i++; }
来源：http://hz.cucudq.cn/gtvsinsfjc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cdnleiting.top/gteyibyuig.html

Ruby: while i < 10; i += 1; end
来源：http://hz.svipenyu.cn/gtwfpgrstr.html

C#:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gtvfmughsl.html

[B08] do-while（至少执行一次）
来源：http://hz.jinqigufen.top/gtzhiwncgs.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.cheryme.top/gtujmcsadn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.haohaochexian.top/gtrwsyuizu.html

JS:   do { i++; } while (i < 10);
来源：http://hz.guowangkeji.top/gtyibcndoo.html

TS:   do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtnqkfgsde.html

Java: do { i++; } while (i < 10);
来源：http://hz.pycfn.com/gtqfgpiuve.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.xinyue.icu/gtnbygkiyf.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhixingplan.top/gtzpctbgsa.html

C#:   do { i++; } while (i < 10);
来源：http://hz.gogol.net.cn/gtrfpjiark.html

[B09] break 与 continue
来源：http://hz.jinghuilouyu.cn/gtppubzmmq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xziqi.cn/gtlntdczvr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.guowangkeji.top/gtwpmfyjjx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hnxiangtu.top/gtviuowfqp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtiatwducy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxinkj.top/gtbmyvieof.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.wangshuangyany.cn/gtnrrhqhed.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yongpay.top/gtpbcmwqqf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.vqdsnc.cn/gtchoqoneh.html

[B10] 遍历同时拿索引
来源：http://hz.ywan-chungtsiang.top/gtarsnbzuv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuetiantiany.cn/gtxahqpqpz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.gogol.net.cn/gtdtucasit.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.0kj1m.cn/gtktzsvznk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.cdnleiting.top/gtjwerlzjb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhengqikj.top/gtgoqvithn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.fengsongda.top/gtqjsdagsd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.andypj.xyz/gtnmptqfmq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yonumen.top/gthytsywfu.html

[B11] 生成数字序列 / 区间
来源：http://hz.shuidangran.top/gtlxlebzaz.html

Py:   list(range(0, 10, 2))
来源：http://hz.pengpengdd.cyou/gtnfrlmxlg.html

PHP:  range(0, 10, 2);
来源：http://hz.mhx1999.top/gttezhcwio.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.pengpengdd.cyou/gtmdptxlxj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.quarkkingdee.top/gtrupgsbpg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.havefunace.top/gtvpklyjtu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.316326.xyz/gtoucgkykb.html

Ruby: (0...10).step(2).to_a
来源：http://hz.shanyushiyangkeji.top/gtbofjscym.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jiagoushi.top/gtxlfxfcut.html

[B12] 跳出多层循环
来源：http://hz.cashguo.top/gtixpleonx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yangfankeji.com/gtuugeocdv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gaohongyu789.top/gtyrwzyjxo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtefpytycp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sxryk.cn/gtpaqjtfjo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtvqwvznaj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinyuanbaomall.cn/gtxtjatezw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.kuanghao11.cn/gtckkpttdr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenlongwang.top/gtystsypax.html

[B13] 判断是否为数字
来源：http://hz.zhongyouzk.top/gtbkezagjo.html

Py:   isinstance(x, (int, float))
来源：http://hz.jlsjyb.cn/gtdggnnwbd.html

PHP:  is_numeric($x)
来源：http://hz.gzhubu.top/gtnvqdfjri.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.kuanghao11.cn/gtycdgrsuj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.daxiang520.top/gtvriekpeu.html

Java: x instanceof Number
来源：http://hz.zhengqikj.top/gtjgrqppcw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.guannengcc.top/gtworgyouc.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ydjk.org.cn/gthqevstsk.html

C#:   x is int or double or decimal
来源：http://hz.hnxiangtu.top/gtwsqsfigb.html

[B14] 判断值是否在集合内
来源：http://hz.gaohongyu789.top/gtqlxcuxwk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.tanke756.top/gtthmspuha.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenzaomai.com/gtsgohrcvc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.hywenlv.cn/gtoiirufae.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cucudq.cn/gtqlmdvner.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.gaohongyu789.top/gtjaaproik.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhiwuduotai.top/gtexxqmbul.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.wangshuangyany.cn/gtjstzvpfu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sufxvd.cn/gtkvjyhckq.html

[B15] 布尔运算与取反
来源：http://hz.dashuyun.cn/gtgyljzsro.html

Py:   a and b or not c
来源：http://hz.haohaochexian.top/gtabcvwenb.html

PHP:  $a && $b || !$c
来源：http://hz.cucudq.cn/gtrkxmamvg.html

JS:   a && b || !c
来源：http://hz.jiagoushi.top/gtrilvvgiu.html

TS:   a && b || !c
来源：http://hz.meibo888.top/gtzxubuhjj.html

Java: a && b || !c
来源：http://hz.yuxming.cn/gturcotnla.html

Go:   a && b || !c
来源：http://hz.jlsjyb.cn/gtgsdtgxbs.html

Ruby: a && b || !c
来源：http://hz.316326.xyz/gtniwnajtj.html

C#:   a && b || !c
来源：http://hz.yj202588.top/gthofzcaoy.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yvedp.cn/gtdxwvbbeq.html

Py:   if not data: return
来源：http://hz.hnqzz.top/gttfetgqwe.html

PHP:  if (!$data) { return; }
来源：http://hz.xuetiantiany.cn/gtomftkmmy.html

JS:   if (!data) return;
来源：http://hz.yvedp.cn/gtdouqgvhe.html

TS:   if (!data) return;
来源：http://hz.chenjidiqi.icu/gtavbzkomj.html

Java: if (data == null) return;
来源：http://hz.zhengqikj.top/gtxlzpdpae.html

Go:   if data == nil { return }
来源：http://hz.xingfuxueyuan.xyz/gtpbrlmlhh.html

Ruby: return if data.nil?
来源：http://hz.hywenlv.cn/gtdwtrtlof.html

C#:   if (data == null) return;
来源：http://hz.quarkkingdee.top/gtvnxlrarw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtttgbonmu.html

C. 函数与作用域
来源：http://hz.jinyuanbaomall.cn/gtssaxtkit.html

================================================================================
来源：http://hz.yangfankeji.com/gtfatwctin.html

[C01] 定义函数
来源：http://hz.chenlongwang.top/gttnjeadok.html

Py:   def add(a, b): return a + b
来源：http://hz.ywan-chungtsiang.top/gtpnojtsbb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.redwolf501.top/gtmsmcqobt.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtutibqmhr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jqgfzy.top/gthrlzyagq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigufen.top/gtzqpdwgej.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtfzunyzjz.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangkeji.top/gtqmvqibro.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtawrsewxj.html

[C02] 默认参数
来源：http://hz.9152youxi.cn/gtsgbcjpun.html

Py:   def greet(name="World"): return name
来源：http://hz.jqgfzy.top/gtbtgnartk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zdqjudy.top/gtsxgpxwsc.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dashuyun.cn/gtjcetgqpx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gotoacloud.top/gtixtvgjrz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.gzhubu.top/gtegoozmpn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aibaodan.cn/gtpdbddywe.html

Ruby: def greet(name = "World") = name
来源：http://hz.snrcjt.cn/gtczhiwirs.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.vqdsnc.cn/gtczowhbfh.html

[C03] 可变参数
来源：http://hz.ehwqpu.com/gtsognwtuo.html

Py:   def total(*args): return sum(args)
来源：http://hz.jlsjyb.cn/gtotxalyxj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sufxvd.cn/gteapbvrdq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhoulong.xyz/gtwyoozozp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtuhuripfx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cheryme.top/gtradbnllq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yongpay.top/gtxlvpxyut.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.sxryk.cn/gtcnosvkwi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nwbrower.top/gtcprhoyde.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shzxlz.cn/gtppwrofxi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ybcxt.top/gtbwczfkfz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xylfe.cn/gtrivsbmfp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhixingplan.top/gtydrlmjwd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhengqikj.top/gtbkpyjshu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenjidiqi.icu/gtoqghnpfy.html

Go:   // 无：用配置结构体参数
来源：http://hz.zdqjudy.top/gtadrxtkng.html

Ruby: f(a: 1, b: 2)
来源：http://hz.fengsongda.top/gtvcglfcvb.html

C#:   f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtjusziphx.html

[C05] 返回多个值
来源：http://hz.smart0.xyz/gtnxotwrql.html

Py:   return a, b
来源：http://hz.cqqwz.cn/gtqzdtfrem.html

PHP:  return [$a, $b];
来源：http://hz.zycfv.cn/gtpxmjtqly.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xuetiantiany.cn/gtmxpajpqd.html

TS:   return { a, b };
来源：http://hz.316326.xyz/gtkqupnyai.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zycfv.cn/gtvuzibskp.html

Go:   return a, b
来源：http://hz.jianghu66.top/gthghjuqrc.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtkxgwpefp.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ehwqpu.com/gtrceujrwe.html

[C06] 匿名函数 / lambda
来源：http://hz.yuxming.cn/gtityopuxh.html

Py:   square = lambda x: x * x
来源：http://hz.52xcode.cn/gthujsqson.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtfyzoucad.html

JS:   const square = x => x * x;
来源：http://hz.yj20258.top/gturtwxhay.html


<!-- 参考信息 -->