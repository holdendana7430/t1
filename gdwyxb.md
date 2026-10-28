代发 wailian999

Ruby: a, b = b, a
来源：http://hz.chenzaomai.com/gtfnnetwex.html

C#:   (a, b) = (b, a);
来源：http://hz.ehwqpu.com/gtnaecuzjn.html

[A20] 读取标准输入
来源：http://hz.zhoulong.xyz/gtzgprwgii.html

Py:   name = input("请输入：")
来源：http://hz.hysaishi.cn/gthxpgluoz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.yvedp.cn/gtcfuimkez.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.fengsongda.top/gtjftptemy.html

TS:   // Node.js：readline 模块
来源：http://hz.sweek.top/gtuyotmtja.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.zhengqikj.top/gtlxitsode.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.zhijiandao.cn/gtcdtbhwhm.html

Ruby: gets.chomp
来源：http://hz.vqdsnc.cn/gtanzpolsc.html

C#:   Console.ReadLine();
来源：http://hz.aibaodan.cn/gthcxiddyg.html

[A21] 保留指定小数位输出
来源：http://hz.tianlin.xyz/gtnfatorjn.html

Py:   f"{3.14159:.2f}"
来源：http://hz.52xcode.cn/gtpvqcshml.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.aizwys.cn/gtdmwozaca.html

JS:   (3.14159).toFixed(2)
来源：http://hz.shzxlz.cn/gtitpehxgc.html

TS:   (3.14159).toFixed(2)
来源：http://hz.fzhhl.top/gtarcreaom.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.shanyushiyangkeji.top/gtutmnxghz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.hysaishi.cn/gtkjixxovk.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.hammf.cn/gtockgdqtg.html

C#:   3.14159.ToString("F2")
来源：http://hz.cqqwz.cn/gtfjzyiurj.html

[A22] 获取字符串长度
来源：http://hz.meibo888.top/gtvpmveomp.html

Py:   len(s)
来源：http://hz.hammf.cn/gtlldphbnu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.hysaishi.cn/gtcggukxhi.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.svipenyu.cn/gtnkmhimxr.html

TS:   s.length
来源：http://hz.xingfuxueyuan.xyz/gtuvwugxzy.html

Java: s.length()
来源：http://hz.yuanzhike.top/gtzuhgoxxh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.sufxvd.cn/gtizmpztpb.html

Ruby: s.length
来源：http://hz.sweek.top/gtamdfmlkb.html

C#:   s.Length
来源：http://hz.sysykeji.top/gtqbexbpmb.html

[A23] 大小写转换
来源：http://hz.svipenyu.cn/gthrrnknom.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.aizwys.cn/gtehowskcd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.yuxming.cn/gtutscoacs.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.cucudq.cn/gtfoiqqvux.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.ehwqpu.com/gtfnzskcju.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.ppjwa.cn/gtxskkajyi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.ybcxt.top/gtjrrogjvz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.smart0.xyz/gtsavycsbl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yj20258.top/gtkvyowenn.html

[A24] 去除首尾空白
来源：http://hz.jinqigfzy.top/gtsddwvryl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.jianghu66.top/gtzwsjhbum.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zhengqikj.top/gtpgdlyjkz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.yj202588.top/gthmzjztem.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.jinqigufen.top/gtzohsdrux.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.yanxiufei.cn/gthnsseggk.html

Go:   strings.TrimSpace(s)
来源：http://hz.dashuyun.cn/gtcmhwikcg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.daria6918.cn/gtxherotbf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.xuanzx.com/gtkgttljph.html

[A25] 字符串比较
来源：http://hz.jinghuilouyu.cn/gtlzzjhmgp.html

Py:   s1 == s2; s1 != s2
来源：http://hz.pengpengdd.cyou/gtzqehxonc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.shuidangran.top/gtwvkkvoxe.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.fengsongda.top/gtkiyvkpsr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jlsjyb.cn/gtcngjvrxi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.iojbl.cn/gtbmbploxj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.sysykeji.top/gtbbznquzv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hnqzz.top/gtwyvaerva.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.yuxming.cn/gthezsgkpy.html

[A26] 类型转换总览
来源：http://hz.xinyue.icu/gtjumltejm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.sufxvd.cn/gtqftjyrzn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.dashuyun.cn/gtyubhewfj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.zhiwuduotai.top/gtggwqvupp.html

TS:   Number() String() Boolean() x as number
来源：http://hz.iojbl.cn/gtssdcprju.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.ydjk.org.cn/gtovklhhod.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.cashguo.top/gtynxxpman.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.pengpengdd.cyou/gtqygmkodk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.iojbl.cn/gtwgvjlzhh.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqcrveghg.html

B. 流程控制
来源：http://hz.chenlongwang.top/gtvcziaeoi.html

================================================================================
来源：http://hz.xylfe.cn/gttfburmbp.html

[B01] 条件判断 if / else
来源：http://hz.cdnleiting.top/gtidjcusnp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.hammf.cn/gttvktyvxi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.xuetiantiany.cn/gtcobtuxzd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.fengsongda.top/gtcljnwdmg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.tianlin.xyz/gtffaivlou.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jianghu66.top/gttsljbxrr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.nwbrower.top/gtdutdpplc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.chenlongwang.top/gtbwobcnlc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigfzy.top/gtvtiaseob.html

[B02] 多分支 else if / elif
来源：http://hz.hywenlv.cn/gtfirsxmpr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.cucudq.cn/gtscgzgwnr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.xylfe.cn/gtwqphtoje.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cqqwz.cn/gttufhwuqo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.gogol.net.cn/gtcqjimwvt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.chenlongwang.top/gtwadnwrmx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.wangdashe.top/gtkpdtrdzz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.vqdsnc.cn/gtvykfckcm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hnqzz.top/gtfvkbvvvn.html

[B03] switch / match / case
来源：http://hz.sweek.top/gtkrajrcui.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.jqgufenzy.top/gtdirrhpxi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhengqikj.top/gtcfhkonqs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.mhx1999.top/gttiuhelvv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.haohaochexian.top/gtmdfrokbm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.yonumen.top/gtjacwyazb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.jyoumei.cn/gttbbjzcfq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.zhaomingkeji.xyz/gtosztxrkf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.zhijiandao.cn/gteacfzqeb.html

[B04] for 计数循环
来源：http://hz.zhiwuduotai.top/gttxmhsbqn.html

Py:   for i in range(10): print(i)
来源：http://hz.yuanzhike.top/gtkfakvtfz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.shanyushiyangtech.top/gtshnhqwur.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zhengqikj.top/gtkrdunmdj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj202588.top/gtdhiqvjze.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yueranfly.top/gthkmajufr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.ivvv.top/gtmodhwtdf.html

Ruby: 10.times { |i| puts i }
来源：http://hz.iojbl.cn/gtlymixtqi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.gzhubu.top/gtzgnsjcjg.html

[B05] 遍历数组 / 列表
来源：http://hz.snrcjt.cn/gtequzzdoc.html

Py:   for item in arr: print(item)
来源：http://hz.pycfn.com/gtbhsmqxbq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.nanxuanxn.top/gtcufwgsvb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.aizwys.cn/gtaceoarxk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.jlsjyb.cn/gtobsakcxk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hnqzz.top/gtnbhhjpae.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.aibaodan.cn/gtpqjfmewj.html

Ruby: arr.each { |item| puts item }
来源：http://hz.vqdsnc.cn/gtlzvtkfum.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.iojbl.cn/gtziyquikw.html

[B06] 遍历字典 / 对象
来源：http://hz.cdnleiting.top/gtvthjackk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.yuxming.cn/gtcmpuvdzz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.sufxvd.cn/gtczqszgqq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.sysykeji.top/gtojcfbyef.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shzxlz.cn/gtfpjjwfgw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.shanyushiyangtech.top/gtnilgrmgq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.tianlin.xyz/gthdrwiyka.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xuanzx.com/gtevekmnff.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.pengpengdd.cyou/gtmwnkplzt.html

[B07] while 循环
来源：http://hz.shangyingyoupin.top/gtjgimsviq.html

Py:   while i < 10: i += 1
来源：http://hz.tianlin.xyz/gtecrgrgvu.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.mhx1999.top/gtiaxtumxo.html

JS:   while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtitclkypi.html

TS:   while (i < 10) { i++; }
来源：http://hz.316326.xyz/gthifjltcv.html

Java: while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtcsrwlngk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tanke756.top/gthjtmyxil.html

Ruby: while i < 10; i += 1; end
来源：http://hz.wangdashe.top/gtxvduglcw.html

C#:   while (i < 10) { i++; }
来源：http://hz.yonumen.top/gtagvbkqxe.html

[B08] do-while（至少执行一次）
来源：http://hz.chenlongwang.top/gtvjoswnau.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ydjk.org.cn/gtvnsfjnkv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yj20258888.top/gtlvsrubyc.html

JS:   do { i++; } while (i < 10);
来源：http://hz.kuanghao11.cn/gtmgoyrgmq.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtgsjxgctj.html

Java: do { i++; } while (i < 10);
来源：http://hz.yongpay.top/gtkflqqrpw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.nwbrower.top/gtscdpxcvi.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.chenlongwang.top/gtnoxtrvsv.html

C#:   do { i++; } while (i < 10);
来源：http://hz.jianghu66.top/gthzzeiuup.html

[B09] break 与 continue
来源：http://hz.zhengqikj.top/gtnlgihwmb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.sweek.top/gtpmlzayrt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jinqigfzy.top/gterxcxcqq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtrborkmjd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gtojntbjdv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gttbibmujt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.jiagoushi.top/gtqmuhvlem.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.daxiang520.top/gtqmoznkwp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtxxxpoqjk.html

[B10] 遍历同时拿索引
来源：http://hz.pengpengdd.cyou/gtijmppfht.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xziqi.cn/gtvnflljzk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.pycfn.com/gtizzptzzq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.daxiang520.top/gtrbmevwtm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.vqdsnc.cn/gtnrowqnsf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sweek.top/gtlewvqddg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.sweek.top/gtpmenswgq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yj20258.top/gtsylmhneg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.sufxvd.cn/gtmuziqwcw.html

[B11] 生成数字序列 / 区间
来源：http://hz.zhijiandao.cn/gtxbrpmuua.html

Py:   list(range(0, 10, 2))
来源：http://hz.hfpthk.cn/gtnslnzopb.html

PHP:  range(0, 10, 2);
来源：http://hz.cdnleiting.top/gtuenvpflh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhengqikj.top/gthjhgescl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sweek.top/gtvkxopfiq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.chenlongwang.top/gtzmpxznlu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.cucudq.cn/gtlswtpemg.html

Ruby: (0...10).step(2).to_a
来源：http://hz.xingfuxueyuan.xyz/gtwnalrxnf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj20258.top/gthnghldvx.html

[B12] 跳出多层循环
来源：http://hz.zhijiandao.cn/gtpszmeoyp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.bjfxy.top/gtvqhuqdnz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.bjfxy.top/gtwmcffoij.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yuxming.cn/gtrnznthcp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtzfniwkvh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jiagoushi.top/gthuonxceo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.svipenyu.cn/gtrfjymqcd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.nanxuanxn.top/gtagqbsdjc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.chenzaomai.com/gtnqovyxaf.html

[B13] 判断是否为数字
来源：http://hz.jinghuilouyu.cn/gtlpcnezla.html

Py:   isinstance(x, (int, float))
来源：http://hz.hywenlv.cn/gtseytpcxj.html

PHP:  is_numeric($x)
来源：http://hz.hongshengwenyu.top/gtxapvcjnj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aibaodan.cn/gtavzzqwvw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hysaishi.cn/gtjaqqzfkr.html

Java: x instanceof Number
来源：http://hz.aibaodan.cn/gtnczmhiti.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jinqigfzy.top/gtjtrxmlsg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.nwbrower.top/gtthyhteut.html

C#:   x is int or double or decimal
来源：http://hz.zhijiandao.cn/gtnwidlrie.html

[B14] 判断值是否在集合内
来源：http://hz.9152youxi.cn/gtkttqnsms.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.gaohongyu789.top/gtnmdirwyc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.yj20258888.top/gtvyjsfxno.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.ppjwa.cn/gtcncrslva.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.9152youxi.cn/gtvqjjyemx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinqigfzy.top/gtgdrsnein.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.mhx1999.top/gtbovsjmzz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.cashguo.top/gtjrgsejfy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.316326.xyz/gtqjyzoxwj.html

[B15] 布尔运算与取反
来源：http://hz.sxryk.cn/gtbcajpcvm.html

Py:   a and b or not c
来源：http://hz.yanxiufei.cn/gtsberglow.html

PHP:  $a && $b || !$c
来源：http://hz.haohaochexian.top/gtyglrmcps.html

JS:   a && b || !c
来源：http://hz.yangfankeji.com/gtclpnaete.html

TS:   a && b || !c
来源：http://hz.zhongyouzk.top/gtzxvvmali.html

Java: a && b || !c
来源：http://hz.gaohongyu789.top/gtcsfdnhli.html

Go:   a && b || !c
来源：http://hz.meibo888.top/gttmrgowap.html

Ruby: a && b || !c
来源：http://hz.cheryme.top/gtulevtxyv.html

C#:   a && b || !c
来源：http://hz.kuanghao11.cn/gttzttvhfm.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.cheryme.top/gtbhthehqt.html

Py:   if not data: return
来源：http://hz.hongshengwenyu.top/gtzmmzsrlv.html

PHP:  if (!$data) { return; }
来源：http://hz.dianchejie.cn/gtwxhjsfbn.html

JS:   if (!data) return;
来源：http://hz.jyoumei.cn/gtksjmbqiu.html

TS:   if (!data) return;
来源：http://hz.xinyue.icu/gtztehigqp.html

Java: if (data == null) return;
来源：http://hz.ivvv.top/gtubofyttj.html

Go:   if data == nil { return }
来源：http://hz.sweek.top/gtigxedzyj.html

Ruby: return if data.nil?
来源：http://hz.cqqwz.cn/gttilndppz.html

C#:   if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtkjoofwms.html

================================================================================
来源：http://hz.bjfxy.top/gtnsphgjlz.html

C. 函数与作用域
来源：http://hz.yvedp.cn/gtnsduqbxh.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtynwublqt.html

[C01] 定义函数
来源：http://hz.sufxvd.cn/gtkberigjq.html

Py:   def add(a, b): return a + b
来源：http://hz.zhijiandao.cn/gtwtsikdex.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtdbbpphgb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xuanzx.com/gttqurqwad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gtzpygnhsx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtmijtbsap.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.shzxlz.cn/gtxjtwcsro.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jlsjyb.cn/gtqtfdtwzc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.bjfxy.top/gtmbzvjsau.html

[C02] 默认参数
来源：http://hz.zhiwuduotai.top/gtmnovvqse.html

Py:   def greet(name="World"): return name
来源：http://hz.ydzc1.top/gtvvjmbvmh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tian-w.cn/gtqltvygyg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.kuanghao11.cn/gtlqmudmht.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtajjcfzjg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.pycfn.com/gtpvedkkgu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.shzxlz.cn/gtdxjcvyff.html

Ruby: def greet(name = "World") = name
来源：http://hz.redwolf501.top/gtoykjkqmi.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.chenjidiqi.icu/gtmspntkdt.html

[C03] 可变参数
来源：http://hz.ppjwa.cn/gtwctujond.html

Py:   def total(*args): return sum(args)
来源：http://hz.0kj1m.cn/gtlmihaate.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.0kj1m.cn/gtmvkdmhka.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtgszfuoia.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gtlduhkyul.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jqgufenzy.top/gtrdobcofc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.fengsongda.top/gtvbhnaesz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.dashuyun.cn/gtppwpxcis.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shanyushiyangkeji.top/gtnlwcpvbc.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xziqi.cn/gtdavmlnfb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.daria6918.cn/gthyaybuzc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cheryme.top/gtpzyvtmxq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.sufxvd.cn/gtklwsfwtd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xingfuxueyuan.xyz/gtdshztade.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenjidiqi.icu/gtfedssfks.html

Go:   // 无：用配置结构体参数
来源：http://hz.andypj.xyz/gtnjgkgvka.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ybcxt.top/gtcxyhddiv.html

C#:   f(a: 1, b: 2)
来源：http://hz.zdqjudy.top/gtvzwbflep.html

[C05] 返回多个值
来源：http://hz.jqgufenzy.top/gterzznbrg.html

Py:   return a, b
来源：http://hz.ivvv.top/gtbsiryrmi.html

PHP:  return [$a, $b];
来源：http://hz.9152youxi.cn/gtsoaxyqkw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.nanxinkj.top/gtexlurchc.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtnoirrsfl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtrjjjuhel.html

Go:   return a, b
来源：http://hz.ywan-chungtsiang.top/gtmojrjhbt.html

Ruby: return a, b
来源：http://hz.feifeiyinyue.top/gtgzdeahxn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gzhubu.top/gteqptemwq.html

[C06] 匿名函数 / lambda
来源：http://hz.aibaodan.cn/gtlxybjprx.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtndtfaxmj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhixingplan.top/gtvemmaxzd.html

JS:   const square = x => x * x;
来源：http://hz.hammf.cn/gtryrjmysi.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cqqwz.cn/gtyxkdkono.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.ydjk.org.cn/gtfbiduzlz.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.gaohongyu789.top/gttqbroned.html

Ruby: square = ->(x) { x * x }
来源：http://hz.gogol.net.cn/gtadtykpxk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnqzz.top/gtkpscomto.html

[C07] 把函数作为参数传入
来源：http://hz.nanxuanxn.top/gtnnditibh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.0kj1m.cn/gtsedttujy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.kuanghao11.cn/gtzdddnzzp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yj202588.top/gtounyllck.html

TS:   arr.map(String)
来源：http://hz.nanxuanxn.top/gtfwydeadr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jinghuilouyu.cn/gtpsnybeia.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.sysykeji.top/gtlzpwxnid.html

Ruby: arr.map(&:upcase)
来源：http://hz.xingfuxueyuan.xyz/gtrrhdexfm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.smart0.xyz/gtuxtorxdy.html

[C08] 闭包
来源：http://hz.gzhubu.top/gtlzgkfqyk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.bjfxy.top/gtszjlouwb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.chenlongwang.top/gticimetqj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtvxvjlwjv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jinqigufen.top/gtllcupkis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.iojbl.cn/gtjvcwieyy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.aibaodan.cn/gtzqxxmisq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xziqi.cn/gtgkihzeve.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.sweek.top/gtroxhieks.html

[C09] 递归
来源：http://hz.shzxlz.cn/gtffxhjzdo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtmguotayi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtaopfgfky.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtrjayhipw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gtkblxqhbk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.daria6918.cn/gtmtgiyvsb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydjk.org.cn/gtzmuzuwxy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jinqigfzy.top/gtwefeojfh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.smart0.xyz/gtemmvrcnt.html

[C10] 变量作用域
来源：http://hz.ywan-chungtsiang.top/gtyqpttkvh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yangfankeji.com/gtwmsbzqyh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.kuanghao11.cn/gtoyugmuux.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.yanxiufei.cn/gtgfgivmut.html


<!-- 参考信息 -->