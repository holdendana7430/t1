代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://hz.tanke756.top/gtaxdpwxil.html

TS:   const value = data ?? "默认值";
来源：http://hz.sweek.top/gtzokrauoz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.ppjwa.cn/gtmhlyimfx.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.yj202588.top/gtmhvfmshe.html

Ruby: value = data || "默认值"
来源：http://hz.hfpthk.cn/gtbvsculpz.html

C#:   var value = data ?? "默认值";
来源：http://hz.xingfuxueyuan.xyz/gtblnmswhk.html

[A16] 真假值判断规则
来源：http://hz.xziqi.cn/gtoffkvjyj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.fengsongda.top/gtdcampyan.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.svipenyu.cn/gtdoyatlrz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.tanke756.top/gtwqldoouj.html

TS:   if (!x) {}
来源：http://hz.yj202588.top/gtrizsfmga.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.ppjwa.cn/gtdbqczgpe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.tian-w.cn/gtdqjssftf.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.fengsongda.top/gtjykmdvaa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.hnxiangtu.top/gtwkdcujpz.html

[A17] 位运算
来源：http://hz.fzhhl.top/gtjqifbjnp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jiagoushi.top/gtttobbzwe.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.bjfxy.top/gtwpqpkdqq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.jianghu66.top/gtaxgiojli.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.kuanghao11.cn/gtvxlihnva.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtvwpwshdr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.guannengcc.top/gtrvovmgmu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.yj20258888.top/gttypgrnbe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hysaishi.cn/gtxfdeqadb.html

[A18] 字符与 ASCII 码互转
来源：http://hz.zhoulong.xyz/gtdaoyddmi.html

Py:   ord("A"); chr(65)
来源：http://hz.ppjwa.cn/gthmtbxyxu.html

PHP:  ord("A"); chr(65)
来源：http://hz.quarkkingdee.top/gtmthhiqpi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.daxiang520.top/gtkbzurqig.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.shzxlz.cn/gtldxgvvlr.html

Java: (int) 'A'; (char) 65
来源：http://hz.birdmap.top/gtiwaotops.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.nanxuanxn.top/gttpunqmka.html

Ruby: "A".ord; 65.chr
来源：http://hz.gogol.net.cn/gtzowfimbu.html

C#:   (int)'A'; (char)65
来源：http://hz.tanke756.top/gtsbzdfvis.html

[A19] 交换两个变量
来源：http://hz.ivvv.top/gtynxqfczh.html

Py:   a, b = b, a
来源：http://hz.aibaodan.cn/gtcjlgousi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.iojbl.cn/gtjxhwiktg.html

JS:   [a, b] = [b, a];
来源：http://hz.316326.xyz/gtxfdbregy.html

TS:   [a, b] = [b, a];
来源：http://hz.jiagoushi.top/gtbfneklgt.html

Java: int t = a; a = b; b = t;
来源：http://hz.hywenlv.cn/gtyjrqoxkc.html

Go:   a, b = b, a
来源：http://hz.wangdashe.top/gthhwnxvsr.html

Ruby: a, b = b, a
来源：http://hz.chenzaomai.com/gtsmpvnitv.html

C#:   (a, b) = (b, a);
来源：http://hz.shuidangran.top/gtwflwruzf.html

[A20] 读取标准输入
来源：http://hz.birdmap.top/gtggvomanr.html

Py:   name = input("请输入：")
来源：http://hz.xinyue.icu/gtstznstyc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yonumen.top/gttieasipj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.gogol.net.cn/gtfqhgwomn.html

TS:   // Node.js：readline 模块
来源：http://hz.xuetiantiany.cn/gtslqibzqm.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.bjfxy.top/gtihiagrkn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.yj20258.top/gtsliprbwg.html

Ruby: gets.chomp
来源：http://hz.jinyuanbaomall.cn/gtiyhqrqnw.html

C#:   Console.ReadLine();
来源：http://hz.cucudq.cn/gtiapoulhm.html

[A21] 保留指定小数位输出
来源：http://hz.gotoacloud.top/gtjfephdle.html

Py:   f"{3.14159:.2f}"
来源：http://hz.zhengqikj.top/gtnoybstfw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.pycfn.com/gtobbelkit.html

JS:   (3.14159).toFixed(2)
来源：http://hz.jqgufenzy.top/gtblzraicn.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zdqjudy.top/gtwfudywgy.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.ydzc1.top/gtowyslxev.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.pycfn.com/gtezfuccgz.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gtosftinjq.html

C#:   3.14159.ToString("F2")
来源：http://hz.fzhhl.top/gtkhifubaf.html

[A22] 获取字符串长度
来源：http://hz.guowangkeji.top/gtdypnwnxf.html

Py:   len(s)
来源：http://hz.nwbrower.top/gtrwhbjsrr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.nanxuanxn.top/gtvexmnxdy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.svipenyu.cn/gtcfbkzoqw.html

TS:   s.length
来源：http://hz.aizwys.cn/gtcmtnrdyr.html

Java: s.length()
来源：http://hz.yonumen.top/gtgfokaywd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.meibo888.top/gtwsofmrlf.html

Ruby: s.length
来源：http://hz.hnxiangtu.top/gtmioifvru.html

C#:   s.Length
来源：http://hz.ybcxt.top/gtpkjerjjz.html

[A23] 大小写转换
来源：http://hz.cucudq.cn/gtjigiztdm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.jqgufenzy.top/gtoitvkfzh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.pycfn.com/gtgdiryuco.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhongyouzk.top/gtjhehdomy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.sufxvd.cn/gtzdthhpng.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.birdmap.top/gtgdtyhtby.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.pycfn.com/gtdnwoxpjr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.zhixingplan.top/gtiozshyto.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.dianchejie.cn/gtzqjnenlt.html

[A24] 去除首尾空白
来源：http://hz.fengsongda.top/gtlkzzsbiw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yvedp.cn/gtkqmnxfnq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.gaohongyu789.top/gtrcijcsfu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinghuilouyu.cn/gtjkiuaeun.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shanyushiyangtech.top/gthuciuqvo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.gotoacloud.top/gtcibyzdhv.html

Go:   strings.TrimSpace(s)
来源：http://hz.daria6918.cn/gtszlmjjvw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yonumen.top/gtfgryvdzo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.yueranfly.top/gtnjfwiifg.html

[A25] 字符串比较
来源：http://hz.ydjk.org.cn/gtzadcsypd.html

Py:   s1 == s2; s1 != s2
来源：http://hz.hammf.cn/gtaebxjskg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.sxryk.cn/gtrpojhzaw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.redwolf501.top/gtgddsylqt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yongpay.top/gtzlqsffaa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.chenzaomai.com/gtbeaqmher.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.shanyushiyangkeji.top/gtgfhdfoyn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.andypj.xyz/gtcimjnwcg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.xinyue.icu/gtzslpzhpb.html

[A26] 类型转换总览
来源：http://hz.feifeiyinyue.top/gthluctjis.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.hnxiangtu.top/gtlmlnuwvy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.jyoumei.cn/gtaaxeamva.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.andypj.xyz/gtvdxobayo.html

TS:   Number() String() Boolean() x as number
来源：http://hz.dashuyun.cn/gtniqmcpfc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.svipenyu.cn/gtrzvwjzqj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hammf.cn/gtpfxwbrwj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.gotoacloud.top/gtjerpqsuu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.iojbl.cn/gtxkmbtonk.html

================================================================================
来源：http://hz.zhengqikj.top/gtzxcxkloy.html

B. 流程控制
来源：http://hz.guowangkeji.top/gtrfthgdem.html

================================================================================
来源：http://hz.ybcxt.top/gttujzfnby.html

[B01] 条件判断 if / else
来源：http://hz.jinghuilouyu.cn/gtxmvqeutq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.aibaodan.cn/gtvfryqqcw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xinyue.icu/gtarralasp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.0kj1m.cn/gtklzesgna.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.xylfe.cn/gttmlkwwov.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yueranfly.top/gtxbjklarq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.cucudq.cn/gtplfqaefe.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.52xcode.cn/gtiyctlzhy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtwfywufdm.html

[B02] 多分支 else if / elif
来源：http://hz.yueranfly.top/gtkhjdvpza.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.shuidangran.top/gtebptokym.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.vqdsnc.cn/gtxwkoiffk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nwbrower.top/gtxfxlpofp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.bjfxy.top/gtrjsglqvp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.daxiang520.top/gtkzzuisrj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.ybcxt.top/gtdowszdng.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.daxiang520.top/gtzdpocilh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.tanke756.top/gtoebezzms.html

[B03] switch / match / case
来源：http://hz.vqdsnc.cn/gtdorguuzh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.fengsongda.top/gtddqqnrte.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.wangdashe.top/gtkzzjacfd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.redwolf501.top/gtniyzyjpi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.pycfn.com/gtprgxqxev.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hnqzz.top/gtxaihprmj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.svipenyu.cn/gtrzjszqap.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zdqjudy.top/gtmmsaepkt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.daria6918.cn/gtuncyvdhd.html

[B04] for 计数循环
来源：http://hz.hongshengwenyu.top/gtmdkggfhm.html

Py:   for i in range(10): print(i)
来源：http://hz.wangshuangyany.cn/gtigylapum.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.cashguo.top/gtumlffnef.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jlsjyb.cn/gtzakiqadh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.wangdashe.top/gtydbjybeo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.zhaomingkeji.xyz/gtjofnnzaw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.yuxming.cn/gtictrxuik.html

Ruby: 10.times { |i| puts i }
来源：http://hz.daxiang520.top/gtgukejabo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.yueranfly.top/gtwhhuozil.html

[B05] 遍历数组 / 列表
来源：http://hz.cashguo.top/gtyavfxafi.html

Py:   for item in arr: print(item)
来源：http://hz.ppjwa.cn/gtfyeiuegm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.xuetiantiany.cn/gtntxftbsx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.yanxiufei.cn/gtdinlxkio.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.yuanzhike.top/gttpygdllh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.chenzaomai.com/gtdyiwcwmv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.hongshengwenyu.top/gtgqvnbbje.html

Ruby: arr.each { |item| puts item }
来源：http://hz.316326.xyz/gtgweudglc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jiagoushi.top/gtpitrnicm.html

[B06] 遍历字典 / 对象
来源：http://hz.gogol.net.cn/gtkwiltoes.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.xingfuxueyuan.xyz/gtcyhryinz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.tianlin.xyz/gtfalkqgra.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.feifeiyinyue.top/gtvikpuozo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.meibo888.top/gtakhqkzgt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.9152youxi.cn/gtrlaajuml.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinghuilouyu.cn/gtnmznibqc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.snrcjt.cn/gtytbangbe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.gzhubu.top/gtigqussxo.html

[B07] while 循环
来源：http://hz.redwolf501.top/gtjbqjwzws.html

Py:   while i < 10: i += 1
来源：http://hz.nanxinkj.top/gtloljxufm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.havefunace.top/gtkwjfolny.html

JS:   while (i < 10) { i++; }
来源：http://hz.meibo888.top/gtzykzxgao.html

TS:   while (i < 10) { i++; }
来源：http://hz.chenzaomai.com/gtixebbxxf.html

Java: while (i < 10) { i++; }
来源：http://hz.quarkkingdee.top/gtkdautldz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.cheryme.top/gtcwrhreey.html

Ruby: while i < 10; i += 1; end
来源：http://hz.guowangkeji.top/gtwucjqvsc.html

C#:   while (i < 10) { i++; }
来源：http://hz.redwolf501.top/gtqkbbguko.html

[B08] do-while（至少执行一次）
来源：http://hz.redwolf501.top/gtohebpfqi.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.pengpengdd.cyou/gtxktjodbl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shanyushiyangtech.top/gtbrpohxgo.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtprvofnpc.html

TS:   do { i++; } while (i < 10);
来源：http://hz.jqgfzy.top/gtlzjivhhj.html

Java: do { i++; } while (i < 10);
来源：http://hz.yuxming.cn/gtjgusnvda.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.wangdashe.top/gtpaqqwquw.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.tanke756.top/gtpgiyilof.html

C#:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtwslbfdux.html

[B09] break 与 continue
来源：http://hz.yongpay.top/gtgddbchky.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.xinyue.icu/gtzyzqlclt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinyuanbaomall.cn/gtpltjkaki.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shzxlz.cn/gtfypgqypo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.daria6918.cn/gtgwossbln.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gtelvxdmrz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jlsjyb.cn/gtoektrefm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.tanke756.top/gtlhpcrawe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gtzvwywnot.html

[B10] 遍历同时拿索引
来源：http://hz.hongshengwenyu.top/gtxbxakzwq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.chenzaomai.com/gtxmbtmixu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.mhx1999.top/gtfrdqyzbu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.jinqigfzy.top/gtkynqrfuu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.hysaishi.cn/gtqsddboaz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.jiagoushi.top/gtwndaiqjf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.guowangkeji.top/gtqbwesfhe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yueranfly.top/gtdrmxaocn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jianghu66.top/gtnucxmhbs.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuxming.cn/gthliwviap.html

Py:   list(range(0, 10, 2))
来源：http://hz.yanxiufei.cn/gtrftsqfin.html

PHP:  range(0, 10, 2);
来源：http://hz.yvedp.cn/gtyrasplth.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xziqi.cn/gtazjseyxz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hywenlv.cn/gtmnjjddbw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cheryme.top/gtszyldlff.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hfpthk.cn/gtcycgrgwa.html

Ruby: (0...10).step(2).to_a
来源：http://hz.vqdsnc.cn/gtyuatrhif.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.vqdsnc.cn/gtuxfmyqan.html

[B12] 跳出多层循环
来源：http://hz.dashuyun.cn/gtaiwsclfo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.sysykeji.top/gtahberumi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yueranfly.top/gtvnsuimkx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yanxiufei.cn/gtivpovzaa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shangyingyoupin.top/gtedxcbeza.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yueranfly.top/gtluerrbqz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ivvv.top/gtgluujbrm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.c1oappe.top/gtzvmrtqif.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.shanyushiyangkeji.top/gtjchekhcz.html

[B13] 判断是否为数字
来源：http://hz.guowangkeji.top/gtabkmdogn.html

Py:   isinstance(x, (int, float))
来源：http://hz.mhx1999.top/gtkuvxoqrq.html

PHP:  is_numeric($x)
来源：http://hz.yuanzhike.top/gtjdpirpbb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtlsimlltc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ivvv.top/gtceqmdwae.html

Java: x instanceof Number
来源：http://hz.ivvv.top/gtcdknhncj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.dianchejie.cn/gtodimgcqi.html

Ruby: x.is_a?(Numeric)
来源：http://hz.wangshuangyany.cn/gtjbowcjai.html

C#:   x is int or double or decimal
来源：http://hz.daxiang520.top/gthjfehfcd.html

[B14] 判断值是否在集合内
来源：http://hz.kuanghao11.cn/gtglagwpdw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shzxlz.cn/gthwfgphnl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jqgufenzy.top/gtsonffzcp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zdqjudy.top/gtzidracpu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nanxinkj.top/gtwljyveac.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.sufxvd.cn/gtjzjoqfou.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gzhubu.top/gtyvkrmlbo.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.sysykeji.top/gtmludydkw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.wangdashe.top/gthpzqxios.html

[B15] 布尔运算与取反
来源：http://hz.haohaochexian.top/gtezrlykbr.html

Py:   a and b or not c
来源：http://hz.tanke756.top/gtgjojxqzf.html

PHP:  $a && $b || !$c
来源：http://hz.chenlongwang.top/gtscakulyp.html

JS:   a && b || !c
来源：http://hz.shanyushiyangkeji.top/gtbcajhcxw.html

TS:   a && b || !c
来源：http://hz.jqgufenzy.top/gtbcgnjmbt.html

Java: a && b || !c
来源：http://hz.yuanzhike.top/gtfimblilj.html

Go:   a && b || !c
来源：http://hz.ydjk.org.cn/gtoqubvsal.html

Ruby: a && b || !c
来源：http://hz.yongpay.top/gtcgccurnj.html

C#:   a && b || !c
来源：http://hz.sweek.top/gtssqvewyo.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.gotoacloud.top/gtjuqfwenc.html

Py:   if not data: return
来源：http://hz.andypj.xyz/gtjcvscckf.html

PHP:  if (!$data) { return; }
来源：http://hz.smart0.xyz/gtlphxwzki.html

JS:   if (!data) return;
来源：http://hz.yuxming.cn/gtoffniqfa.html

TS:   if (!data) return;
来源：http://hz.hysaishi.cn/gtignjynqy.html

Java: if (data == null) return;
来源：http://hz.meibo888.top/gtzddjarnw.html

Go:   if data == nil { return }
来源：http://hz.ydjk.org.cn/gtxhegtkpw.html

Ruby: return if data.nil?
来源：http://hz.cashguo.top/gtgdrsuzxt.html

C#:   if (data == null) return;
来源：http://hz.yj20258888.top/gtihnyvpkn.html

================================================================================
来源：http://hz.yj202588.top/gtgdvukrvp.html

C. 函数与作用域
来源：http://hz.shangyingyoupin.top/gtkgavghlu.html

================================================================================
来源：http://hz.aizwys.cn/gtlehpledu.html

[C01] 定义函数
来源：http://hz.daria6918.cn/gtkdeuzwdw.html

Py:   def add(a, b): return a + b
来源：http://hz.smart0.xyz/gtqbbwxerd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aizwys.cn/gtqjrxgymh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ehwqpu.com/gtmfseeyid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtzpxkqsfu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yanxiufei.cn/gtvmwgajot.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shanyushiyangkeji.top/gtqirbmcrp.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shuidangran.top/gtxoybmqbp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtwdxdankx.html

[C02] 默认参数
来源：http://hz.pycfn.com/gtbhbacodh.html

Py:   def greet(name="World"): return name
来源：http://hz.iojbl.cn/gtiezhgczy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xingfuxueyuan.xyz/gtfmnlwrzz.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.fzhhl.top/gtwdbucvnp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtvtdnbgax.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangshuangyany.cn/gtrlnmingh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cucudq.cn/gtgygtsqdd.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinyuanbaomall.cn/gtiqnhseon.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ivvv.top/gttrafkdjh.html

[C03] 可变参数
来源：http://hz.xziqi.cn/gtpnfylczx.html

Py:   def total(*args): return sum(args)
来源：http://hz.316326.xyz/gtpdgtitdh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.zhijiandao.cn/gteheceaik.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xylfe.cn/gtuakeycqe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gtmbukmomd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hfpthk.cn/gtqpnutqct.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zycfv.cn/gtxkihdbjt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.ydjk.org.cn/gttyjsypys.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ybcxt.top/gtslprnezt.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yvedp.cn/gtgwdjzopd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.0kj1m.cn/gthvewkukw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xziqi.cn/gtqstabmay.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guannengcc.top/gttxiuvdko.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.c1oappe.top/gtgpixsqtb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jinqigfzy.top/gthmkpdrik.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinqigfzy.top/gtebxwtxlw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhiwuduotai.top/gtwhzpnrwq.html

C#:   f(a: 1, b: 2)
来源：http://hz.yueranfly.top/gtvzozxqca.html

[C05] 返回多个值
来源：http://hz.vqdsnc.cn/gtzxxvjoud.html

Py:   return a, b
来源：http://hz.sysykeji.top/gtlrmzwavw.html

PHP:  return [$a, $b];
来源：http://hz.aibaodan.cn/gtevlffaqs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnxiangtu.top/gtephpgalq.html

TS:   return { a, b };
来源：http://hz.wangdashe.top/gtysblnjht.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.gzhubu.top/gtuqygfpkt.html

Go:   return a, b
来源：http://hz.xuanzx.com/gtplrpbpsu.html

Ruby: return a, b
来源：http://hz.xylfe.cn/gtgauesgit.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.feifeiyinyue.top/gtmijpmxva.html


<!-- 参考信息 -->