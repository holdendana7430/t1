代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://hz.aizwys.cn/gtoxcststf.html

Py:   ord("A"); chr(65)
来源：http://hz.dashuyun.cn/gtagfdwssx.html

PHP:  ord("A"); chr(65)
来源：http://hz.hnqzz.top/gtqzfuweiu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.quarkkingdee.top/gtfsipubpz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.cashguo.top/gtinavokib.html

Java: (int) 'A'; (char) 65
来源：http://hz.dashuyun.cn/gtcddnsyuy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.9152youxi.cn/gtwmoyvdjr.html

Ruby: "A".ord; 65.chr
来源：http://hz.yongpay.top/gtxbbmejcj.html

C#:   (int)'A'; (char)65
来源：http://hz.hnqzz.top/gtxsqnoedl.html

[A19] 交换两个变量
来源：http://hz.cucudq.cn/gtecppmhnf.html

Py:   a, b = b, a
来源：http://hz.bjfxy.top/gtamtsfhkk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.hammf.cn/gtlltegumx.html

JS:   [a, b] = [b, a];
来源：http://hz.pycfn.com/gtijcoztnk.html

TS:   [a, b] = [b, a];
来源：http://hz.jinyuanbaomall.cn/gtplwfqonj.html

Java: int t = a; a = b; b = t;
来源：http://hz.svipenyu.cn/gtxmyrdiro.html

Go:   a, b = b, a
来源：http://hz.cqqwz.cn/gtyynyahyx.html

Ruby: a, b = b, a
来源：http://hz.jlsjyb.cn/gtqbmdsuzi.html

C#:   (a, b) = (b, a);
来源：http://hz.jqgufenzy.top/gtfaiyxqcm.html

[A20] 读取标准输入
来源：http://hz.chenzaomai.com/gtbltpmxvb.html

Py:   name = input("请输入：")
来源：http://hz.jianghu66.top/gtgfwogmvk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.nanxuanxn.top/gteccxklgv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.hysaishi.cn/gtdajwbayp.html

TS:   // Node.js：readline 模块
来源：http://hz.xingfuxueyuan.xyz/gtmsrfgekz.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.vqdsnc.cn/gteomhqett.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.ppjwa.cn/gtskjpmued.html

Ruby: gets.chomp
来源：http://hz.daxiang520.top/gtjlhsfdnj.html

C#:   Console.ReadLine();
来源：http://hz.pycfn.com/gtnpvpvvxl.html

[A21] 保留指定小数位输出
来源：http://hz.yanxiufei.cn/gtaabzeeol.html

Py:   f"{3.14159:.2f}"
来源：http://hz.guannengcc.top/gturpfjlaj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.jlsjyb.cn/gtvafosbvr.html

JS:   (3.14159).toFixed(2)
来源：http://hz.tian-w.cn/gtldvcdgnq.html

TS:   (3.14159).toFixed(2)
来源：http://hz.jinyuanbaomall.cn/gtrwiukngu.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tianlin.xyz/gttniylqix.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.fengsongda.top/gtjwibwvwm.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.bjfxy.top/gtqegqwcsi.html

C#:   3.14159.ToString("F2")
来源：http://hz.yonumen.top/gtugjvdjjl.html

[A22] 获取字符串长度
来源：http://hz.chenjidiqi.icu/gtgawfnqhj.html

Py:   len(s)
来源：http://hz.zhengqikj.top/gtlgwwynnx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.jianghu66.top/gtpdytceyo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hnxiangtu.top/gtvkpyminl.html

TS:   s.length
来源：http://hz.fengsongda.top/gtzpctlchj.html

Java: s.length()
来源：http://hz.pycfn.com/gthkdumurh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yj20258.top/gtpezfowyu.html

Ruby: s.length
来源：http://hz.xingfuxueyuan.xyz/gtcvzwdjzv.html

C#:   s.Length
来源：http://hz.xylfe.cn/gtfqpptjiy.html

[A23] 大小写转换
来源：http://hz.zhengqikj.top/gtzohdqzsq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.redwolf501.top/gttvasnese.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.ehwqpu.com/gtfotgnoog.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ybcxt.top/gtazklzqkg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.aibaodan.cn/gtvzasghdw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.shanyushiyangtech.top/gteiemzvby.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ehwqpu.com/gtiwvrfbqx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.ppjwa.cn/gtsobluepu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.jiagoushi.top/gtwbtngrkm.html

[A24] 去除首尾空白
来源：http://hz.dianchejie.cn/gtiqxljang.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.yj20258.top/gtoocoxfsa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.daxiang520.top/gtvgtsswpd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.daria6918.cn/gtoothfxnk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.iojbl.cn/gtlzzblpvc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.quarkkingdee.top/gtyqpglyqt.html

Go:   strings.TrimSpace(s)
来源：http://hz.wangshuangyany.cn/gtjmroecbc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.xziqi.cn/gtowmzrkpq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.shanyushiyangkeji.top/gtozblxqcj.html

[A25] 字符串比较
来源：http://hz.aibaodan.cn/gtvbetwzuq.html

Py:   s1 == s2; s1 != s2
来源：http://hz.c1oappe.top/gtoxycasww.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.yongpay.top/gtpvysgjec.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.daxiang520.top/gtftrvsxzp.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.316326.xyz/gtmrstkpym.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.guannengcc.top/gtgxlrkvuj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.cashguo.top/gtwlymloea.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.kuanghao11.cn/gtapigcetu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.pengpengdd.cyou/gtqkqlxyay.html

[A26] 类型转换总览
来源：http://hz.gzhubu.top/gtdbhosslj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.bjfxy.top/gtlqukebku.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zdqjudy.top/gtaqoebnhs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jlsjyb.cn/gtptebbxvi.html

TS:   Number() String() Boolean() x as number
来源：http://hz.ywan-chungtsiang.top/gtweqqmjlk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.yj20258888.top/gtwfmznavn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.cashguo.top/gtfrpmjflu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.yj20258888.top/gtxnyqhdom.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.zhengqikj.top/gtpeltfyxx.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwlkjtphr.html

B. 流程控制
来源：http://hz.jiagoushi.top/gtdmevafhv.html

================================================================================
来源：http://hz.cucudq.cn/gtbvtldlxp.html

[B01] 条件判断 if / else
来源：http://hz.cqqwz.cn/gtxlaxvbqu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yj20258.top/gtpbldahzv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.zycfv.cn/gtdcoqgseb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.nwbrower.top/gtconywltf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.zhengqikj.top/gtmwxnttyt.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.xuanzx.com/gtlsoplwfd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gaohongyu789.top/gthvkgjsfa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.sweek.top/gttnezjhit.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.ywan-chungtsiang.top/gtmljipyzs.html

[B02] 多分支 else if / elif
来源：http://hz.jyoumei.cn/gtaapsescb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.meibo888.top/gtzrmaqqmb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.zhongyouzk.top/gtfgeuiuyd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.aizwys.cn/gtjvajsove.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jinghuilouyu.cn/gtweoaaaei.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.zhixingplan.top/gtdnbxfurq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gotoacloud.top/gtiaxdhwii.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.shangyingyoupin.top/gtgfjvukos.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj202588.top/gtaeuthsja.html

[B03] switch / match / case
来源：http://hz.chenzaomai.com/gtgzcacfxf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.c1oappe.top/gtdkdettem.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.wangdashe.top/gtszdnxzpj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.ywan-chungtsiang.top/gtsyqxsrjq.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinghuilouyu.cn/gtnhcxsvlc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.snrcjt.cn/gtpalzmpbb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.hfpthk.cn/gtbavrctwx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.yongpay.top/gtxnqxluxw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.gaohongyu789.top/gtqxmwqtmh.html

[B04] for 计数循环
来源：http://hz.daxiang520.top/gthfhpwhlz.html

Py:   for i in range(10): print(i)
来源：http://hz.haohaochexian.top/gtrqsjtpax.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.meibo888.top/gtstnwmrke.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhengqikj.top/gtoanebyvw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.shuidangran.top/gtufbwrupr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.wangshuangyany.cn/gtlwtkbexc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.c1oappe.top/gtfeqfwsjd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.tianlin.xyz/gtbvjrnwpa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.ywan-chungtsiang.top/gtyvzwqslr.html

[B05] 遍历数组 / 列表
来源：http://hz.nwbrower.top/gtxrwwvpvk.html

Py:   for item in arr: print(item)
来源：http://hz.xuetiantiany.cn/gtqlhxmgbb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenjidiqi.icu/gtendxfjvn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.havefunace.top/gtatzcnecl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hysaishi.cn/gtgiypaxia.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.dianchejie.cn/gtxrtynlci.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.haohaochexian.top/gtzwsfezzs.html

Ruby: arr.each { |item| puts item }
来源：http://hz.tanke756.top/gtvlcoysma.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.svipenyu.cn/gtphzyignm.html

[B06] 遍历字典 / 对象
来源：http://hz.xinyue.icu/gtmghticks.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.pengpengdd.cyou/gtswtsbfvr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.andypj.xyz/gthoynjopn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.9152youxi.cn/gtmnymshsx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.ydjk.org.cn/gtqdvehbhj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.pycfn.com/gtnivxredj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.ydzc1.top/gtrcgtpone.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.pengpengdd.cyou/gtiawsbrhq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.redwolf501.top/gtjwezqmqo.html

[B07] while 循环
来源：http://hz.cqqwz.cn/gteoqzxakm.html

Py:   while i < 10: i += 1
来源：http://hz.shzxlz.cn/gtqztejuzd.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jlsjyb.cn/gtfyxkzvmk.html

JS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtyiksbzld.html

TS:   while (i < 10) { i++; }
来源：http://hz.svipenyu.cn/gtjmqgvwvw.html

Java: while (i < 10) { i++; }
来源：http://hz.pengpengdd.cyou/gtbjgcihjk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.hfpthk.cn/gtspouqjor.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shzxlz.cn/gtkbuyigxo.html

C#:   while (i < 10) { i++; }
来源：http://hz.birdmap.top/gtlywxlbwh.html

[B08] do-while（至少执行一次）
来源：http://hz.hnqzz.top/gtrjeqwpqd.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jinqigufen.top/gtnyyyrpmx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.shanyushiyangkeji.top/gtwhcgnnri.html

JS:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtooyqfblr.html

TS:   do { i++; } while (i < 10);
来源：http://hz.meibo888.top/gtjfuakree.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhijiandao.cn/gtgqajgecu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.havefunace.top/gtbyybrzqz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.smart0.xyz/gtbdsyozbt.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aizwys.cn/gttprdipop.html

[B09] break 与 continue
来源：http://hz.gogol.net.cn/gtucxrmmuw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.zhengqikj.top/gtqljbcmuu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zdqjudy.top/gtxsbeckyw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hongshengwenyu.top/gtzlcmouxl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gtplcnjiaw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gthwdzzhjl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jqgufenzy.top/gtafronhsl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.vqdsnc.cn/gteuhtvryh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jiagoushi.top/gtiztaozhw.html

[B10] 遍历同时拿索引
来源：http://hz.snrcjt.cn/gtwrsgvmcm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.pycfn.com/gtlwgxhyfb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.aizwys.cn/gtxklenesh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.gotoacloud.top/gtcmcbjbxv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.sxryk.cn/gtchgpsvhp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yueranfly.top/gtqwkfiame.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.kuanghao11.cn/gtmblmjcrg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.ehwqpu.com/gtuebnqqgl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.snrcjt.cn/gtsinbuxhq.html

[B11] 生成数字序列 / 区间
来源：http://hz.yuxming.cn/gtiypxwnmt.html

Py:   list(range(0, 10, 2))
来源：http://hz.jlsjyb.cn/gttgosrbei.html

PHP:  range(0, 10, 2);
来源：http://hz.fengsongda.top/gtaqfwokdu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.meibo888.top/gtwcnmtgbr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xuanzx.com/gtjggzchcp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.havefunace.top/gtyuldyywo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.jlsjyb.cn/gtytxpueva.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jiagoushi.top/gtubviruqa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.jinqigfzy.top/gtbprarknj.html

[B12] 跳出多层循环
来源：http://hz.ydjk.org.cn/gthrfifqii.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.gogol.net.cn/gtstafpyjo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.aibaodan.cn/gtixuufqas.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtobpfrfbr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.feifeiyinyue.top/gtgmjdkhax.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.shzxlz.cn/gtpzwxmonh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shangyingyoupin.top/gthzatajub.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenjidiqi.icu/gtztidlrhr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.52xcode.cn/gtrgvpzhwl.html

[B13] 判断是否为数字
来源：http://hz.ybcxt.top/gtiosrrwfl.html

Py:   isinstance(x, (int, float))
来源：http://hz.daria6918.cn/gtorcmmrlw.html

PHP:  is_numeric($x)
来源：http://hz.xziqi.cn/gtouktnjvt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.xuanzx.com/gthoplrosx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gotoacloud.top/gtzryxdzaw.html

Java: x instanceof Number
来源：http://hz.yvedp.cn/gtvzfdlrpn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.smart0.xyz/gtulxrnafs.html

Ruby: x.is_a?(Numeric)
来源：http://hz.mhx1999.top/gtjedesltz.html

C#:   x is int or double or decimal
来源：http://hz.jinyuanbaomall.cn/gtxlrhehvz.html

[B14] 判断值是否在集合内
来源：http://hz.yj20258888.top/gthmyiydiz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gotoacloud.top/gtqatubcrq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jianghu66.top/gtuaqtqwcg.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.svipenyu.cn/gtcjtbbsig.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gthgqcfmuh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.hongshengwenyu.top/gtpkjrftjb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ydzc1.top/gtjqnmxuxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.tanke756.top/gtmqiyvdse.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cucudq.cn/gtdgexnfct.html

[B15] 布尔运算与取反
来源：http://hz.quarkkingdee.top/gtubdwxzae.html

Py:   a and b or not c
来源：http://hz.zhoulong.xyz/gtrqnokykn.html

PHP:  $a && $b || !$c
来源：http://hz.cqqwz.cn/gtfomfcjlo.html

JS:   a && b || !c
来源：http://hz.pengpengdd.cyou/gtrmdwwfiv.html

TS:   a && b || !c
来源：http://hz.kuanghao11.cn/gtfiyopexk.html

Java: a && b || !c
来源：http://hz.gotoacloud.top/gtglaqytjb.html

Go:   a && b || !c
来源：http://hz.tanke756.top/gtcvodijoo.html

Ruby: a && b || !c
来源：http://hz.chenzaomai.com/gtvtfmqbwg.html

C#:   a && b || !c
来源：http://hz.ehwqpu.com/gteudhydpt.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guannengcc.top/gtmnmexiuh.html

Py:   if not data: return
来源：http://hz.jyoumei.cn/gtkkluuuzj.html

PHP:  if (!$data) { return; }
来源：http://hz.xuetiantiany.cn/gtssegutij.html

JS:   if (!data) return;
来源：http://hz.tianlin.xyz/gtqiwsrkxr.html

TS:   if (!data) return;
来源：http://hz.yj20258888.top/gtueznfltp.html

Java: if (data == null) return;
来源：http://hz.jianghu66.top/gtmqnrtcxf.html

Go:   if data == nil { return }
来源：http://hz.c1oappe.top/gtjsbtimho.html

Ruby: return if data.nil?
来源：http://hz.chenzaomai.com/gtmxqnpoml.html

C#:   if (data == null) return;
来源：http://hz.vqdsnc.cn/gtzoonamvq.html

================================================================================
来源：http://hz.daria6918.cn/gtineyzxma.html

C. 函数与作用域
来源：http://hz.yonumen.top/gtoibakhsq.html

================================================================================
来源：http://hz.cheryme.top/gtunmuzvzp.html

[C01] 定义函数
来源：http://hz.cqqwz.cn/gtwoqvbrkf.html

Py:   def add(a, b): return a + b
来源：http://hz.fengsongda.top/gtdfrvydkk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtuhxrttfv.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.shzxlz.cn/gtzwruqdfc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.tanke756.top/gtrtbjxyhq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jyoumei.cn/gtloezxhzf.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigfzy.top/gtfoaacshe.html

Ruby: def add(a, b); a + b; end
来源：http://hz.dashuyun.cn/gtgieypdvs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtxvjysyhx.html

[C02] 默认参数
来源：http://hz.zhixingplan.top/gtrxojzrcb.html

Py:   def greet(name="World"): return name
来源：http://hz.pengpengdd.cyou/gtxdfzomfw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.jianghu66.top/gtjcxixgjs.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.nwbrower.top/gtvnfkmjlf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.tianlin.xyz/gtvfcwqffw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.vqdsnc.cn/gtcvhvhtuw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtdzfnbrqe.html

Ruby: def greet(name = "World") = name
来源：http://hz.xylfe.cn/gtmglimowt.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nanxinkj.top/gtgzmohstq.html

[C03] 可变参数
来源：http://hz.zhaomingkeji.xyz/gtumkxkrhz.html

Py:   def total(*args): return sum(args)
来源：http://hz.wangdashe.top/gtjscifsne.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.daxiang520.top/gtyhnsmkfw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nwbrower.top/gtqjyqkibb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yanxiufei.cn/gtcdkkawmk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangkeji.top/gtqsvfzrur.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zdqjudy.top/gtqhbsxvxy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.xingfuxueyuan.xyz/gtiydphndm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.ybcxt.top/gtazsswbnm.html

[C04] 命名参数 / 关键字参数
来源：http://hz.0kj1m.cn/gtzpsdcyzl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shangyingyoupin.top/gtuurrdfdb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.xingfuxueyuan.xyz/gtsyzvphsh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtxsdpkltu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.zhijiandao.cn/gtjgygclmy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuanzx.com/gtqyrakhek.html

Go:   // 无：用配置结构体参数
来源：http://hz.jianghu66.top/gtyhpnwngn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yanxiufei.cn/gtaxpuzjnz.html

C#:   f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtfgtaiizm.html

[C05] 返回多个值
来源：http://hz.wangshuangyany.cn/gtuqawdxbm.html

Py:   return a, b
来源：http://hz.yuanzhike.top/gtbemphmwd.html

PHP:  return [$a, $b];
来源：http://hz.tianlin.xyz/gtphcyipkc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yuanzhike.top/gtavedzpth.html

TS:   return { a, b };
来源：http://hz.shuidangran.top/gtshulfkyf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.guannengcc.top/gttiuiyyre.html

Go:   return a, b
来源：http://hz.sxryk.cn/gtmrdhpwqw.html

Ruby: return a, b
来源：http://hz.sysykeji.top/gtexouhfkw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gtqdjhsorv.html

[C06] 匿名函数 / lambda
来源：http://hz.nwbrower.top/gtfvhfpzce.html

Py:   square = lambda x: x * x
来源：http://hz.sweek.top/gtpyldxxdl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xingfuxueyuan.xyz/gtqchmqzos.html

JS:   const square = x => x * x;
来源：http://hz.hnxiangtu.top/gtkoajgpoo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jlsjyb.cn/gtummzbukz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhongyouzk.top/gtqwjkpeqi.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.vqdsnc.cn/gtqvtqwzps.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jianghu66.top/gtcfrormgf.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.birdmap.top/gtvyhlkoxl.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtsgtrqrbn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.daxiang520.top/gtahrwqexj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.tian-w.cn/gtmajynbdj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.feifeiyinyue.top/gtexeerjrh.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtffwzcmon.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guowangkeji.top/gtkwvivcis.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnqzz.top/gtghqwsnsg.html

Ruby: arr.map(&:upcase)
来源：http://hz.hongshengwenyu.top/gtsoerbqlw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hammf.cn/gtdvtpacex.html

[C08] 闭包
来源：http://hz.zdqjudy.top/gtkkltaxaj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.9152youxi.cn/gtgkfdlamv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj202588.top/gtebcebnoy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cdnleiting.top/gtzzzmitpi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuxming.cn/gtflzkdzry.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yanxiufei.cn/gtguncetqi.html


<!-- 参考信息 -->