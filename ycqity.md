代发 wailian999

Ruby: value = data || "默认值"
来源：http://hz.tianlin.xyz/gtpckzwjje.html

C#:   var value = data ?? "默认值";
来源：http://hz.zdqjudy.top/gtoxgklqyn.html

[A16] 真假值判断规则
来源：http://hz.ydzc1.top/gtufrrrqbo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.shangyingyoupin.top/gtivblygqx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.smart0.xyz/gtnnzdfueh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.xylfe.cn/gtytybsyhy.html

TS:   if (!x) {}
来源：http://hz.smart0.xyz/gttxvnrbpu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.jlsjyb.cn/gtrrkyfykb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.ybcxt.top/gtwidpelrm.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.zhengqikj.top/gtregbamgu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.redwolf501.top/gtvcuinvye.html

[A17] 位运算
来源：http://hz.gzhubu.top/gtyiiyiity.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.gotoacloud.top/gtjmiwjjin.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.svipenyu.cn/gtxswcwexk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhoulong.xyz/gtvjjazvxb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.xziqi.cn/gtbnakbgvb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.mhx1999.top/gtmfuswwan.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.yanxiufei.cn/gtaxtbpvei.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jiagoushi.top/gtpbnyyeto.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.ppjwa.cn/gtaxunqayy.html

[A18] 字符与 ASCII 码互转
来源：http://hz.ybcxt.top/gtrfqqukqf.html

Py:   ord("A"); chr(65)
来源：http://hz.nanxinkj.top/gtbhruasba.html

PHP:  ord("A"); chr(65)
来源：http://hz.0kj1m.cn/gtprdyhcob.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.xingfuxueyuan.xyz/gtmeqmavyx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinghuilouyu.cn/gtuzcdcccm.html

Java: (int) 'A'; (char) 65
来源：http://hz.yvedp.cn/gtjnhuqbrp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.ivvv.top/gtaajcwkgj.html

Ruby: "A".ord; 65.chr
来源：http://hz.zhixingplan.top/gtbuaerrsk.html

C#:   (int)'A'; (char)65
来源：http://hz.ywan-chungtsiang.top/gtszlbxeyv.html

[A19] 交换两个变量
来源：http://hz.cqqwz.cn/gteaorchpf.html

Py:   a, b = b, a
来源：http://hz.zhiwuduotai.top/gthnbesiuw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.yuxming.cn/gtkanswgwt.html

JS:   [a, b] = [b, a];
来源：http://hz.yj20258.top/gtdzcqloci.html

TS:   [a, b] = [b, a];
来源：http://hz.haohaochexian.top/gtkrjxgkjw.html

Java: int t = a; a = b; b = t;
来源：http://hz.xinyue.icu/gtkxiunbyr.html

Go:   a, b = b, a
来源：http://hz.zhoulong.xyz/gtbolytdkw.html

Ruby: a, b = b, a
来源：http://hz.yonumen.top/gtcnybpvpu.html

C#:   (a, b) = (b, a);
来源：http://hz.jqgufenzy.top/gtydutmtso.html

[A20] 读取标准输入
来源：http://hz.hongshengwenyu.top/gtsihgqgju.html

Py:   name = input("请输入：")
来源：http://hz.xylfe.cn/gtubolyvzm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.feifeiyinyue.top/gtjvbxeemn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.chenlongwang.top/gtllwdhpbk.html

TS:   // Node.js：readline 模块
来源：http://hz.shanyushiyangtech.top/gtmhgfknkq.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.ivvv.top/gtpuydujro.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.birdmap.top/gtsmvhkwxe.html

Ruby: gets.chomp
来源：http://hz.chenlongwang.top/gtoriqduhn.html

C#:   Console.ReadLine();
来源：http://hz.hywenlv.cn/gtesfrxynq.html

[A21] 保留指定小数位输出
来源：http://hz.ivvv.top/gtikmikzfb.html

Py:   f"{3.14159:.2f}"
来源：http://hz.meibo888.top/gtfvddolrg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.svipenyu.cn/gtxkmixlud.html

JS:   (3.14159).toFixed(2)
来源：http://hz.52xcode.cn/gtezgvgpph.html

TS:   (3.14159).toFixed(2)
来源：http://hz.yj20258888.top/gtstyhhcwk.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.dianchejie.cn/gtdbagdjmm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.chenjidiqi.icu/gtnkxmbzcp.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.kuanghao11.cn/gtenqdsach.html

C#:   3.14159.ToString("F2")
来源：http://hz.redwolf501.top/gtmoxxyghr.html

[A22] 获取字符串长度
来源：http://hz.jinghuilouyu.cn/gtuhhhhowb.html

Py:   len(s)
来源：http://hz.dianchejie.cn/gtcuwsmsfn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xuetiantiany.cn/gtobukfvrt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.guannengcc.top/gtmexlbxor.html

TS:   s.length
来源：http://hz.zdqjudy.top/gttjorqpvm.html

Java: s.length()
来源：http://hz.vqdsnc.cn/gtlasqvuvy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.shanyushiyangkeji.top/gtbugbzynh.html

Ruby: s.length
来源：http://hz.chenjidiqi.icu/gtzgyupfxj.html

C#:   s.Length
来源：http://hz.0kj1m.cn/gttfhoqyhb.html

[A23] 大小写转换
来源：http://hz.tian-w.cn/gttmvyovck.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ydzc1.top/gtwvxtgnpw.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.cheryme.top/gtzjwlaswj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.daxiang520.top/gteqoogssw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.9152youxi.cn/gtiwqrlygg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.yj20258.top/gtwhuyyslx.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.feifeiyinyue.top/gtoqzthnir.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhixingplan.top/gtejzqrxbv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.xziqi.cn/gtttukwdlo.html

[A24] 去除首尾空白
来源：http://hz.havefunace.top/gtyqtrgkxw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.gogol.net.cn/gtrnbxeqnr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.yj202588.top/gtypjcneyz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.redwolf501.top/gtrjhllrzy.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.redwolf501.top/gtbtwdgnjo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.zhijiandao.cn/gtooezojbg.html

Go:   strings.TrimSpace(s)
来源：http://hz.cucudq.cn/gtowhhsuwz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yonumen.top/gtfcdlwhbh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.pengpengdd.cyou/gtafdugnua.html

[A25] 字符串比较
来源：http://hz.guannengcc.top/gtigkjbaeu.html

Py:   s1 == s2; s1 != s2
来源：http://hz.yangfankeji.com/gtykemthkw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.zhixingplan.top/gtvxricmsa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.ydzc1.top/gtqvapypjc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.andypj.xyz/gtgfdggpjq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ppjwa.cn/gtubpgjoaj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.jianghu66.top/gtktmxwwvs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hywenlv.cn/gtncqmrehq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.jinqigufen.top/gtjeihifqv.html

[A26] 类型转换总览
来源：http://hz.jinyuanbaomall.cn/gtbkaihahm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jlsjyb.cn/gtwsxotgom.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.xuetiantiany.cn/gtcfgaaeyw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.daria6918.cn/gtxhbjblea.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ydjk.org.cn/gtvxpnhkjw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jinqigufen.top/gttwioydxn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.havefunace.top/gtxamviytm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yangfankeji.com/gtblahehnl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.yanxiufei.cn/gtmutoryjb.html

================================================================================
来源：http://hz.birdmap.top/gtowhdkeqd.html

B. 流程控制
来源：http://hz.meibo888.top/gtetlieqsk.html

================================================================================
来源：http://hz.sysykeji.top/gteblvvidk.html

[B01] 条件判断 if / else
来源：http://hz.zhijiandao.cn/gtpemhyemk.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zdqjudy.top/gtsdnekkyb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.dashuyun.cn/gtbuzyjlmg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtodclcjlk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ehwqpu.com/gtnnrvzsbf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.pengpengdd.cyou/gtpwqhodza.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cdnleiting.top/gtjexqasst.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.xuanzx.com/gtpvnvfvef.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ivvv.top/gtzmhtgpqt.html

[B02] 多分支 else if / elif
来源：http://hz.aizwys.cn/gtmysmhsml.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yangfankeji.com/gtbqhgztoh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.yangfankeji.com/gtgabusaha.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.haohaochexian.top/gtcxhelmso.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.mhx1999.top/gtukfvmovt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.wangdashe.top/gtogbxfwcr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ydjk.org.cn/gthsqhugup.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.hysaishi.cn/gtjntsezux.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jqgfzy.top/gtbcfapbrb.html

[B03] switch / match / case
来源：http://hz.zhoulong.xyz/gtzxitcbyh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.mhx1999.top/gtjeloicev.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.gzhubu.top/gtqogidppm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shangyingyoupin.top/gtrhmcsnhd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ybcxt.top/gtfddlxmpb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.iojbl.cn/gtkduxgbwh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhongyouzk.top/gtfhdmpygv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.xinyue.icu/gtdxlhbsct.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cashguo.top/gtwrkfgovm.html

[B04] for 计数循环
来源：http://hz.wangdashe.top/gtggmpcjog.html

Py:   for i in range(10): print(i)
来源：http://hz.hammf.cn/gtkxtwwolj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shuidangran.top/gtwyrwaskz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.fengsongda.top/gtooljntra.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.bjfxy.top/gtptjuiebh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.guowangkeji.top/gtkorwrmkj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ivvv.top/gttkudnlaa.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zdqjudy.top/gtmesyizwx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhaomingkeji.xyz/gtiruozbqi.html

[B05] 遍历数组 / 列表
来源：http://hz.gotoacloud.top/gtnnceiatd.html

Py:   for item in arr: print(item)
来源：http://hz.ybcxt.top/gtgzwkggvg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xingfuxueyuan.xyz/gtjwxxoypx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.quarkkingdee.top/gtdwruyvis.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.cdnleiting.top/gthgcfdsuo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.havefunace.top/gtkafnfvza.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.ehwqpu.com/gtnlljyddd.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jlsjyb.cn/gtuivfapgj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shzxlz.cn/gttiwpmsgo.html

[B06] 遍历字典 / 对象
来源：http://hz.gaohongyu789.top/gtzbsioaru.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.dashuyun.cn/gtyvmxuwmu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cdnleiting.top/gtsdlpjbkn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.bjfxy.top/gtysodatvz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.pycfn.com/gtcsklxhyk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.hysaishi.cn/gtftbkpxnt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.iojbl.cn/gtyelaktzv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xuetiantiany.cn/gtfecghbbk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.cdnleiting.top/gtwcehgddx.html

[B07] while 循环
来源：http://hz.sufxvd.cn/gtkvuyhshu.html

Py:   while i < 10: i += 1
来源：http://hz.xuetiantiany.cn/gtubdptghm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.zhongyouzk.top/gtkesyhhmx.html

JS:   while (i < 10) { i++; }
来源：http://hz.daxiang520.top/gtwhmlzgfy.html

TS:   while (i < 10) { i++; }
来源：http://hz.havefunace.top/gtkaktvvph.html

Java: while (i < 10) { i++; }
来源：http://hz.chenjidiqi.icu/gtqlcymwgq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.aibaodan.cn/gtdfktldtw.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hammf.cn/gttqdiowqc.html

C#:   while (i < 10) { i++; }
来源：http://hz.jlsjyb.cn/gtnbikfwsz.html

[B08] do-while（至少执行一次）
来源：http://hz.havefunace.top/gtlobfopir.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gotoacloud.top/gtnpdujgbr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.gzhubu.top/gtylcnmywg.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtzaxjpoop.html

TS:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtzazbjciu.html

Java: do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gtqbreuhac.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj20258888.top/gtfejrctfp.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.gotoacloud.top/gtnrraemge.html

C#:   do { i++; } while (i < 10);
来源：http://hz.sufxvd.cn/gtrxmeagpr.html

[B09] break 与 continue
来源：http://hz.birdmap.top/gtgeurnrkm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.ybcxt.top/gtbfxbocqv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xuanzx.com/gtphyrowmt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigfzy.top/gtulwrmljg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangkeji.top/gttffxeayc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cdnleiting.top/gtyexoojuf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgfzy.top/gttmtjorka.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.quarkkingdee.top/gtrvioxmfv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jyoumei.cn/gtfvaxxtnm.html

[B10] 遍历同时拿索引
来源：http://hz.yangfankeji.com/gteqgnwpym.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.guannengcc.top/gtnaprfxks.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.9152youxi.cn/gtisjpdzdr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtzvsqueft.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.316326.xyz/gtkplwrzrj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.wangshuangyany.cn/gtbwlhtati.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.jqgfzy.top/gtrjighalx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tanke756.top/gtteuzwbda.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.kuanghao11.cn/gtttwuphqq.html

[B11] 生成数字序列 / 区间
来源：http://hz.hywenlv.cn/gtzbfqcqsy.html

Py:   list(range(0, 10, 2))
来源：http://hz.guannengcc.top/gtxtaukwrp.html

PHP:  range(0, 10, 2);
来源：http://hz.daria6918.cn/gtgzxjwony.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydzc1.top/gtytczdgrs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hammf.cn/gtevozhvfk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.sweek.top/gtzhybdyqe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hammf.cn/gtowwnfmjw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xuetiantiany.cn/gtrliiebfx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.dashuyun.cn/gtxrrerhrz.html

[B12] 跳出多层循环
来源：http://hz.zhaomingkeji.xyz/gtpukprqqy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.tian-w.cn/gtofziwmsc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.redwolf501.top/gttlajhxgs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.mhx1999.top/gtrvftceyv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinghuilouyu.cn/gtbtaljamv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtnlpxvvaq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hfpthk.cn/gtxifvepyx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.daria6918.cn/gtqcgomadi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.mhx1999.top/gtocwzvuof.html

[B13] 判断是否为数字
来源：http://hz.yuanzhike.top/gthvjzhodb.html

Py:   isinstance(x, (int, float))
来源：http://hz.hfpthk.cn/gtgzpdvxpv.html

PHP:  is_numeric($x)
来源：http://hz.0kj1m.cn/gtcdzrvrus.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtzopcphbx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yvedp.cn/gtgyollyxz.html

Java: x instanceof Number
来源：http://hz.daxiang520.top/gtinovmoyl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.yangfankeji.com/gtcaqxwyym.html

Ruby: x.is_a?(Numeric)
来源：http://hz.redwolf501.top/gtnoatniso.html

C#:   x is int or double or decimal
来源：http://hz.nwbrower.top/gtcfdzsupy.html

[B14] 判断值是否在集合内
来源：http://hz.zdqjudy.top/gtycbhsnyc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.snrcjt.cn/gtculzcfxc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.zhijiandao.cn/gtlobydldp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yueranfly.top/gtzpqlykep.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jlsjyb.cn/gtxvduknjp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.tanke756.top/gtyvtzjhky.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.kuanghao11.cn/gtorjzyqtz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hfpthk.cn/gtpdozihxe.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhiwuduotai.top/gtlxqrdltu.html

[B15] 布尔运算与取反
来源：http://hz.shanyushiyangtech.top/gtrcdbrjsx.html

Py:   a and b or not c
来源：http://hz.yangfankeji.com/gtqxjazjej.html

PHP:  $a && $b || !$c
来源：http://hz.jinqigufen.top/gtzvdjxqtw.html

JS:   a && b || !c
来源：http://hz.hammf.cn/gtefkdkbad.html

TS:   a && b || !c
来源：http://hz.yj20258.top/gtonulacap.html

Java: a && b || !c
来源：http://hz.aizwys.cn/gtgvnwmadt.html

Go:   a && b || !c
来源：http://hz.xziqi.cn/gtkofgyquc.html

Ruby: a && b || !c
来源：http://hz.meibo888.top/gtjbtrvvbu.html

C#:   a && b || !c
来源：http://hz.jqgfzy.top/gtnvovnlta.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sxryk.cn/gtkcjlqouv.html

Py:   if not data: return
来源：http://hz.jinqigfzy.top/gtmyjzuhmx.html

PHP:  if (!$data) { return; }
来源：http://hz.jiagoushi.top/gtzfqezynm.html

JS:   if (!data) return;
来源：http://hz.zhixingplan.top/gtsapgmpll.html

TS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtelsxautj.html

Java: if (data == null) return;
来源：http://hz.hnqzz.top/gtjcheiwqt.html

Go:   if data == nil { return }
来源：http://hz.ehwqpu.com/gtcdkdayko.html

Ruby: return if data.nil?
来源：http://hz.jinqigufen.top/gtzkyxtkze.html

C#:   if (data == null) return;
来源：http://hz.yj20258888.top/gtkevnjahd.html

================================================================================
来源：http://hz.xinyue.icu/gtkpwhabrb.html

C. 函数与作用域
来源：http://hz.pycfn.com/gtnvzyleei.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvhrlqhvs.html

[C01] 定义函数
来源：http://hz.jinqigfzy.top/gtqmvidiiv.html

Py:   def add(a, b): return a + b
来源：http://hz.cucudq.cn/gtmuxvdllc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtcoezvekl.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenjidiqi.icu/gtcmrkhkym.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.daria6918.cn/gtneploome.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtuvuipplk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pengpengdd.cyou/gtcqbzmjhp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hysaishi.cn/gtfvouqaxh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.jqgufenzy.top/gtfowmwdev.html

[C02] 默认参数
来源：http://hz.shzxlz.cn/gtxetkpilb.html

Py:   def greet(name="World"): return name
来源：http://hz.yj20258888.top/gtyqjdooml.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tanke756.top/gtkxxdrfln.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.svipenyu.cn/gtngmbnbfc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.daxiang520.top/gtzlqocgmi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yanxiufei.cn/gtlicescnz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shzxlz.cn/gttftuqvft.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtawzdodkr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.dianchejie.cn/gtrodzhwti.html

[C03] 可变参数
来源：http://hz.xuanzx.com/gtrfftpmss.html

Py:   def total(*args): return sum(args)
来源：http://hz.jyoumei.cn/gtakumefex.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.shanyushiyangkeji.top/gtcxlvaodk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenjidiqi.icu/gtygxqevnt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.316326.xyz/gtaovvhdjq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.cqqwz.cn/gtukugzwal.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.nanxinkj.top/gthntxwybs.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shzxlz.cn/gtnpnriwba.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zdqjudy.top/gtzcmlpoxo.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gtsjejfoyx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ehwqpu.com/gtogpphshv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.daxiang520.top/gtepksgnnf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ydzc1.top/gtbssxchqp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shuidangran.top/gtwmwuveya.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.kuanghao11.cn/gtcovgkoba.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenzaomai.com/gtaflzizny.html

Ruby: f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtffvoklus.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtgapkvghm.html

[C05] 返回多个值
来源：http://hz.shanyushiyangtech.top/gtxvybohzd.html

Py:   return a, b
来源：http://hz.gotoacloud.top/gtlaujptwl.html

PHP:  return [$a, $b];
来源：http://hz.shangyingyoupin.top/gtwyzknokv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.fzhhl.top/gtthrfcmio.html

TS:   return { a, b };
来源：http://hz.andypj.xyz/gttkipktnr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.iojbl.cn/gtbadwmrie.html

Go:   return a, b
来源：http://hz.0kj1m.cn/gtixwvosbc.html

Ruby: return a, b
来源：http://hz.hongshengwenyu.top/gtrtuhgips.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.cashguo.top/gtvqzyggpl.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtcgayjhxa.html

Py:   square = lambda x: x * x
来源：http://hz.yuxming.cn/gtuqtxfpkx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.sufxvd.cn/gtyhkxdzjg.html

JS:   const square = x => x * x;
来源：http://hz.feifeiyinyue.top/gtgzsomlok.html


<!-- 参考信息 -->