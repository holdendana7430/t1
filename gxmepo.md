代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.ydzc1.top/gtgzyypwvz.html

Java: (int) 'A'; (char) 65
来源：http://hz.gotoacloud.top/gtiilvnuet.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.pengpengdd.cyou/gtviygxfqi.html

Ruby: "A".ord; 65.chr
来源：http://hz.jinghuilouyu.cn/gtunzqxthx.html

C#:   (int)'A'; (char)65
来源：http://hz.nwbrower.top/gtzpkqjmzc.html

[A19] 交换两个变量
来源：http://hz.yuanzhike.top/gtbefubxxj.html

Py:   a, b = b, a
来源：http://hz.fengsongda.top/gtpycvcfug.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.jianghu66.top/gtwdgwxxjc.html

JS:   [a, b] = [b, a];
来源：http://hz.vqdsnc.cn/gtrxwicmua.html

TS:   [a, b] = [b, a];
来源：http://hz.wangshuangyany.cn/gtmvchtene.html

Java: int t = a; a = b; b = t;
来源：http://hz.svipenyu.cn/gtmtscepml.html

Go:   a, b = b, a
来源：http://hz.jinqigufen.top/gtbgvifckb.html

Ruby: a, b = b, a
来源：http://hz.ppjwa.cn/gtzwvhdqkk.html

C#:   (a, b) = (b, a);
来源：http://hz.jyoumei.cn/gtiinilwxq.html

[A20] 读取标准输入
来源：http://hz.jinqigfzy.top/gtsmmxticm.html

Py:   name = input("请输入：")
来源：http://hz.zdqjudy.top/gtxalsrhbl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.ydzc1.top/gtdibmbskz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.shuidangran.top/gtrqscfazz.html

TS:   // Node.js：readline 模块
来源：http://hz.cucudq.cn/gtpdlpevhu.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.shangyingyoupin.top/gtkeimkerw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jqgfzy.top/gtadqbvpoy.html

Ruby: gets.chomp
来源：http://hz.daria6918.cn/gtwpxgxalz.html

C#:   Console.ReadLine();
来源：http://hz.wangdashe.top/gtnwolrkvn.html

[A21] 保留指定小数位输出
来源：http://hz.ywan-chungtsiang.top/gtblcgaocw.html

Py:   f"{3.14159:.2f}"
来源：http://hz.jlsjyb.cn/gtlyifsbdj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.birdmap.top/gtacthsmhh.html

JS:   (3.14159).toFixed(2)
来源：http://hz.ybcxt.top/gtlpkcaedb.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jiagoushi.top/gtovtywhnm.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yvedp.cn/gtrjggvhmr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hammf.cn/gtkyjadrmo.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jlsjyb.cn/gtairlwdwf.html

C#:   3.14159.ToString("F2")
来源：http://hz.meibo888.top/gtrxzhrmoe.html

[A22] 获取字符串长度
来源：http://hz.kuanghao11.cn/gtpiyfpxyo.html

Py:   len(s)
来源：http://hz.shzxlz.cn/gtbjblekiz.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.yueranfly.top/gteegavqbu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.guannengcc.top/gtkchowunp.html

TS:   s.length
来源：http://hz.zhaomingkeji.xyz/gtarbwgqjs.html

Java: s.length()
来源：http://hz.chenjidiqi.icu/gtvlxhddfc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yj202588.top/gtynuaaydb.html

Ruby: s.length
来源：http://hz.shanyushiyangkeji.top/gtbxotlgnc.html

C#:   s.Length
来源：http://hz.yvedp.cn/gtspvfsytn.html

[A23] 大小写转换
来源：http://hz.aibaodan.cn/gtfishamnt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.ivvv.top/gtpahskqht.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.xziqi.cn/gttapwzedx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.xuetiantiany.cn/gtabpbqsnv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.daxiang520.top/gtngxwzrxk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.dashuyun.cn/gtkikbmyqa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ywan-chungtsiang.top/gtbhotrqec.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.xuanzx.com/gtjjsbynno.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.svipenyu.cn/gtjiqnfsul.html

[A24] 去除首尾空白
来源：http://hz.yj20258888.top/gtgukmtxgd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.xinyue.icu/gtjszylisa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.fzhhl.top/gttgyxhlyt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dianchejie.cn/gtqbrpbwcz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.sxryk.cn/gtulzistju.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.iojbl.cn/gtbxrzwhxk.html

Go:   strings.TrimSpace(s)
来源：http://hz.tian-w.cn/gttnpvxbho.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.tianlin.xyz/gtbwwivxmc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhixingplan.top/gtpzftwutw.html

[A25] 字符串比较
来源：http://hz.zhoulong.xyz/gtjzkecfko.html

Py:   s1 == s2; s1 != s2
来源：http://hz.jyoumei.cn/gtxsxcuope.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.hongshengwenyu.top/gtnazjpdyb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.mhx1999.top/gtcpjgxibu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nanxinkj.top/gtrawgcxzf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.yj20258888.top/gtcnhevnmo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.zdqjudy.top/gtfsvjmatz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.316326.xyz/gtplgxedtm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.dianchejie.cn/gttmnpovjc.html

[A26] 类型转换总览
来源：http://hz.snrcjt.cn/gtplisijri.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yj202588.top/gtnvlingzk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.c1oappe.top/gtjndcyaaa.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.aizwys.cn/gtryfcnmbc.html

TS:   Number() String() Boolean() x as number
来源：http://hz.xuetiantiany.cn/gtwixsyquk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.gotoacloud.top/gtsvcdbgcq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.wangshuangyany.cn/gtsbugjvvf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.pycfn.com/gtbanoauwv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.jianghu66.top/gtklasvsrp.html

================================================================================
来源：http://hz.yj202588.top/gtdlfkordl.html

B. 流程控制
来源：http://hz.meibo888.top/gtgilbcfnr.html

================================================================================
来源：http://hz.aibaodan.cn/gteqzittkl.html

[B01] 条件判断 if / else
来源：http://hz.zhengqikj.top/gtrrejrmsq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.gzhubu.top/gtqkmgxupy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.daria6918.cn/gtowbigwqs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.iojbl.cn/gtrzvrgmjc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtefdskjdc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.yj20258888.top/gtzfwtszgg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.jqgfzy.top/gtbijnbkky.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.pengpengdd.cyou/gtrzlytyda.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.gaohongyu789.top/gtucrgoelc.html

[B02] 多分支 else if / elif
来源：http://hz.yuanzhike.top/gtaikewbfr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.hysaishi.cn/gtghqbwysy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.ppjwa.cn/gtidcvxzby.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yueranfly.top/gtvqruwcxe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.nanxinkj.top/gtixtduokf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.snrcjt.cn/gtlxuiclse.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yuanzhike.top/gtbmbobdqi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.chenlongwang.top/gtodgmfpyh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cdnleiting.top/gtxtxxifak.html

[B03] switch / match / case
来源：http://hz.bjfxy.top/gtwdvlirfm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.kuanghao11.cn/gtvoufelcc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.9152youxi.cn/gtvdrtbojf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.cqqwz.cn/gtrjrfafzw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jiagoushi.top/gtvlkchrgl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.shuidangran.top/gtnsxvjuxs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.52xcode.cn/gttyvwovvw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zdqjudy.top/gtsqtpwmnu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jianghu66.top/gtqfdjwowq.html

[B04] for 计数循环
来源：http://hz.jiagoushi.top/gteogttkan.html

Py:   for i in range(10): print(i)
来源：http://hz.zhoulong.xyz/gtvbrikxmf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yj202588.top/gtrssqrmwv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.gogol.net.cn/gtdxexnqfm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.aibaodan.cn/gtmbnfttgt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.daxiang520.top/gtwbngozql.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.xylfe.cn/gtimtjgpzo.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhixingplan.top/gtvikunajo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.aibaodan.cn/gthdzleklq.html

[B05] 遍历数组 / 列表
来源：http://hz.jianghu66.top/gtvetnpjbj.html

Py:   for item in arr: print(item)
来源：http://hz.hywenlv.cn/gtcidmrwdp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenjidiqi.icu/gtbzdldvqb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.jqgufenzy.top/gtiaihvwlj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.shanyushiyangkeji.top/gtogzulpyd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.zhengqikj.top/gtxrflvmhx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.snrcjt.cn/gtmuflyhcl.html

Ruby: arr.each { |item| puts item }
来源：http://hz.zhaomingkeji.xyz/gtqvrbdlkh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ydzc1.top/gtfuzczieb.html

[B06] 遍历字典 / 对象
来源：http://hz.ywan-chungtsiang.top/gtdfskfkby.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cashguo.top/gttaqqnbsn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.pycfn.com/gtcuuhivey.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.chenlongwang.top/gtkthteqya.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.chenjidiqi.icu/gtoyopgzpu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.fengsongda.top/gtaxclirdz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.zhongyouzk.top/gturraxnzr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yongpay.top/gtefgphkqm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.ivvv.top/gtyltrvgaq.html

[B07] while 循环
来源：http://hz.jqgufenzy.top/gtktowraut.html

Py:   while i < 10: i += 1
来源：http://hz.andypj.xyz/gtyjagylsm.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.ydjk.org.cn/gtwxjmbypt.html

JS:   while (i < 10) { i++; }
来源：http://hz.hfpthk.cn/gtsseomghy.html

TS:   while (i < 10) { i++; }
来源：http://hz.yuxming.cn/gtasabzfcn.html

Java: while (i < 10) { i++; }
来源：http://hz.aizwys.cn/gtgcmboahj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.pengpengdd.cyou/gttquhaqpd.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhiwuduotai.top/gtbiosdoft.html

C#:   while (i < 10) { i++; }
来源：http://hz.ybcxt.top/gtgeucltsu.html

[B08] do-while（至少执行一次）
来源：http://hz.gotoacloud.top/gtsveprcqz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.chenlongwang.top/gtstntnlqz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shangyingyoupin.top/gtlsiopbfe.html

JS:   do { i++; } while (i < 10);
来源：http://hz.sysykeji.top/gtkzqoowux.html

TS:   do { i++; } while (i < 10);
来源：http://hz.fengsongda.top/gtpzmpejxq.html

Java: do { i++; } while (i < 10);
来源：http://hz.ivvv.top/gtigwxhphy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhixingplan.top/gtbjgxmlip.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hysaishi.cn/gtzvaxbcor.html

C#:   do { i++; } while (i < 10);
来源：http://hz.hnxiangtu.top/gttfokiyqe.html

[B09] break 与 continue
来源：http://hz.hammf.cn/gtbapguljk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sysykeji.top/gthsewkodd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhoulong.xyz/gttkcfocku.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.52xcode.cn/gtqbsvwcal.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jianghu66.top/gtgiubvjqp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ywan-chungtsiang.top/gteaiwnlbs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hywenlv.cn/gtakhchzjv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.hnxiangtu.top/gtxaalwpmd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtofmqhcdx.html

[B10] 遍历同时拿索引
来源：http://hz.chenzaomai.com/gtaseyulwl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xinyue.icu/gtjfdduxke.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.daxiang520.top/gtghuegmbd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zycfv.cn/gtmefcwmup.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.ydjk.org.cn/gtrxazsrji.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.hongshengwenyu.top/gtsbuqwncv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.cqqwz.cn/gtgyausbjb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.c1oappe.top/gtsegtqxqs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jlsjyb.cn/gtossezerm.html

[B11] 生成数字序列 / 区间
来源：http://hz.shzxlz.cn/gtouclofel.html

Py:   list(range(0, 10, 2))
来源：http://hz.birdmap.top/gtwwirskfh.html

PHP:  range(0, 10, 2);
来源：http://hz.0kj1m.cn/gtheswluvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xinyue.icu/gtzboyinju.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xingfuxueyuan.xyz/gtsumguctw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.cqqwz.cn/gtnbfolakn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.52xcode.cn/gtzfudvbpd.html

Ruby: (0...10).step(2).to_a
来源：http://hz.redwolf501.top/gtqjkcklmq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.ppjwa.cn/gtiqyesdwz.html

[B12] 跳出多层循环
来源：http://hz.shanyushiyangkeji.top/gtkeqfaeya.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.xinyue.icu/gtshplqklq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.vqdsnc.cn/gtkselmjkj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.wangshuangyany.cn/gttfdvmtnr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.dashuyun.cn/gtyojjhrql.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtwfjqddsi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shzxlz.cn/gtbtvywasf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.shanyushiyangkeji.top/gtqxzabbcf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.bjfxy.top/gtjnwcgbez.html

[B13] 判断是否为数字
来源：http://hz.hywenlv.cn/gtkawfaawm.html

Py:   isinstance(x, (int, float))
来源：http://hz.gaohongyu789.top/gtvavwpxkm.html

PHP:  is_numeric($x)
来源：http://hz.316326.xyz/gtpknlskpl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtwtldcdzj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.pengpengdd.cyou/gtwthkexwn.html

Java: x instanceof Number
来源：http://hz.zhengqikj.top/gtrehwyqoa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigufen.top/gtbzdisujm.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinyuanbaomall.cn/gthseraugb.html

C#:   x is int or double or decimal
来源：http://hz.cashguo.top/gtkdfljsef.html

[B14] 判断值是否在集合内
来源：http://hz.aizwys.cn/gteuatibzu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sysykeji.top/gtcpucnezf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.gotoacloud.top/gtocevvmqa.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.xinyue.icu/gtytauepzz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cheryme.top/gtzkoewhcr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.52xcode.cn/gtcwgheaow.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dashuyun.cn/gtztzmwvhc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shzxlz.cn/gtfgjahnbw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yangfankeji.com/gtecwnxpeb.html

[B15] 布尔运算与取反
来源：http://hz.hammf.cn/gtjspxxvue.html

Py:   a and b or not c
来源：http://hz.yueranfly.top/gtyiytjytl.html

PHP:  $a && $b || !$c
来源：http://hz.zhaomingkeji.xyz/gtmmbzshss.html

JS:   a && b || !c
来源：http://hz.wangdashe.top/gthfcmqcfh.html

TS:   a && b || !c
来源：http://hz.redwolf501.top/gtfsuqcokr.html

Java: a && b || !c
来源：http://hz.yj20258888.top/gtadvownee.html

Go:   a && b || !c
来源：http://hz.jyoumei.cn/gtuibkctjm.html

Ruby: a && b || !c
来源：http://hz.cucudq.cn/gtaljdcvgs.html

C#:   a && b || !c
来源：http://hz.cashguo.top/gtkfaupgdm.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.sufxvd.cn/gtqezippof.html

Py:   if not data: return
来源：http://hz.wangdashe.top/gttfvxsjfd.html

PHP:  if (!$data) { return; }
来源：http://hz.birdmap.top/gtmulkcnmt.html

JS:   if (!data) return;
来源：http://hz.zhaomingkeji.xyz/gthzpohdqx.html

TS:   if (!data) return;
来源：http://hz.yj20258888.top/gteniyqdpl.html

Java: if (data == null) return;
来源：http://hz.hysaishi.cn/gtkkbhuyzk.html

Go:   if data == nil { return }
来源：http://hz.daria6918.cn/gtcnmmoirf.html

Ruby: return if data.nil?
来源：http://hz.nanxuanxn.top/gtgmasitqy.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gtfitwpwuk.html

================================================================================
来源：http://hz.tianlin.xyz/gtbxaklviu.html

C. 函数与作用域
来源：http://hz.hammf.cn/gttlilxjxb.html

================================================================================
来源：http://hz.0kj1m.cn/gtgzgmzhqp.html

[C01] 定义函数
来源：http://hz.daxiang520.top/gtlgqhohfz.html

Py:   def add(a, b): return a + b
来源：http://hz.zhijiandao.cn/gtasvsgvgw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhongyouzk.top/gttcissziy.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hfpthk.cn/gthhtgmgsj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cucudq.cn/gtryxfitdv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gthtbtiqcq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.fengsongda.top/gtvzmxcjsq.html

Ruby: def add(a, b); a + b; end
来源：http://hz.xingfuxueyuan.xyz/gtbzxemhyq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.quarkkingdee.top/gtmaapghlg.html

[C02] 默认参数
来源：http://hz.shzxlz.cn/gttmnnldzr.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtkpwekftj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xinyue.icu/gtsvvrzxmr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.wangshuangyany.cn/gtgtfclpeg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tian-w.cn/gthutfsvmo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yuanzhike.top/gtupolieqh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.pycfn.com/gtklfjnyxs.html

Ruby: def greet(name = "World") = name
来源：http://hz.vqdsnc.cn/gtfyhuoqlr.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xylfe.cn/gtivgwopzx.html

[C03] 可变参数
来源：http://hz.havefunace.top/gtkoohhhnb.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhijiandao.cn/gtsgmromdp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.mhx1999.top/gtryfgpswv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.mhx1999.top/gtxekhsnhr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuanzhike.top/gtcxxsqive.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.kuanghao11.cn/gthzazborp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sxryk.cn/gtgvefcach.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.kuanghao11.cn/gtkdxcuxwm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aibaodan.cn/gtocczytad.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangdashe.top/gtxxtudkhn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guowangkeji.top/gtiqxcujca.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.shzxlz.cn/gtcxhxqqvl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.mhx1999.top/gtwbypzbhk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yj20258888.top/gtbyhwvqud.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.tanke756.top/gtxdnrvtdz.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinyuanbaomall.cn/gtkneclzqo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yuanzhike.top/gtykiyktuh.html

C#:   f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtshqsbfvc.html

[C05] 返回多个值
来源：http://hz.chenjidiqi.icu/gtqmgpcmop.html

Py:   return a, b
来源：http://hz.jinqigufen.top/gtjouzcoii.html

PHP:  return [$a, $b];
来源：http://hz.dashuyun.cn/gtdkfylpfw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.hnxiangtu.top/gtksqcabuq.html

TS:   return { a, b };
来源：http://hz.yj20258.top/gtapthakbo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhixingplan.top/gtsffpcmef.html

Go:   return a, b
来源：http://hz.ybcxt.top/gtsmpahvam.html

Ruby: return a, b
来源：http://hz.zycfv.cn/gtqjdpljuu.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jyoumei.cn/gtptvgnbhu.html

[C06] 匿名函数 / lambda
来源：http://hz.tianlin.xyz/gtwgenvmvi.html

Py:   square = lambda x: x * x
来源：http://hz.daxiang520.top/gtabogmmbs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.pengpengdd.cyou/gtpnetwxme.html

JS:   const square = x => x * x;
来源：http://hz.iojbl.cn/gtpjfcyzls.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.kuanghao11.cn/gttusxinzw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jlsjyb.cn/gtubmoofio.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.sysykeji.top/gtvkbnmqjm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sufxvd.cn/gtdkbfinsq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sxryk.cn/gtrirynkvk.html

[C07] 把函数作为参数传入
来源：http://hz.aibaodan.cn/gtiieeffzc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.andypj.xyz/gtutucgqpu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cucudq.cn/gtoytynlve.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.fengsongda.top/gtjyitlvyh.html

TS:   arr.map(String)
来源：http://hz.jiagoushi.top/gtnxzumirs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hysaishi.cn/gtmtubjpjv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.smart0.xyz/gtbyyalqah.html

Ruby: arr.map(&:upcase)
来源：http://hz.jianghu66.top/gtttkbaggr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.birdmap.top/gtqgbdxucd.html

[C08] 闭包
来源：http://hz.gzhubu.top/gtxpvstfsn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.fzhhl.top/gtonhjhiac.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.aizwys.cn/gtfjsltylx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.snrcjt.cn/gtjudjgtki.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhoulong.xyz/gtjzrhkfwc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jqgufenzy.top/gtfwdnkgiw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.redwolf501.top/gtbhyjzakb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangdashe.top/gtlyujfkhn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yanxiufei.cn/gtweosgtpi.html

[C09] 递归
来源：http://hz.zhengqikj.top/gtwihkxbmg.html


<!-- 参考信息 -->