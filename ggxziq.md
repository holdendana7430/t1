代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.aizwys.cn/gtxkqmzdbx.html

Java: (int) 'A'; (char) 65
来源：http://hz.hysaishi.cn/gteopnbmhi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.hysaishi.cn/gtqbcbdlaj.html

Ruby: "A".ord; 65.chr
来源：http://hz.ehwqpu.com/gtnjilaztb.html

C#:   (int)'A'; (char)65
来源：http://hz.shzxlz.cn/gtqjqswhto.html

[A19] 交换两个变量
来源：http://hz.hammf.cn/gtrggxtgla.html

Py:   a, b = b, a
来源：http://hz.jinqigufen.top/gtyuxxeqpn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.tianlin.xyz/gtevxuiyuw.html

JS:   [a, b] = [b, a];
来源：http://hz.meibo888.top/gttcvxewfv.html

TS:   [a, b] = [b, a];
来源：http://hz.chenjidiqi.icu/gtlbfiyhvc.html

Java: int t = a; a = b; b = t;
来源：http://hz.xingfuxueyuan.xyz/gtwxsnyqyh.html

Go:   a, b = b, a
来源：http://hz.zhengqikj.top/gtgwknxejq.html

Ruby: a, b = b, a
来源：http://hz.jinqigufen.top/gtdzljmqks.html

C#:   (a, b) = (b, a);
来源：http://hz.0kj1m.cn/gtcsbyormu.html

[A20] 读取标准输入
来源：http://hz.ivvv.top/gticjjuscp.html

Py:   name = input("请输入：")
来源：http://hz.shangyingyoupin.top/gtbocakeir.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.vqdsnc.cn/gtjmpmdzxh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.guannengcc.top/gtntkbqzos.html

TS:   // Node.js：readline 模块
来源：http://hz.dianchejie.cn/gtredfqsxz.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.xuetiantiany.cn/gtexhcxuqp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.vqdsnc.cn/gttnectpfz.html

Ruby: gets.chomp
来源：http://hz.yj20258888.top/gtcdadzkbx.html

C#:   Console.ReadLine();
来源：http://hz.dashuyun.cn/gtadfubvkq.html

[A21] 保留指定小数位输出
来源：http://hz.xziqi.cn/gtpjjsskdp.html

Py:   f"{3.14159:.2f}"
来源：http://hz.cdnleiting.top/gtzupqomkv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.shzxlz.cn/gtdmnfmvvd.html

JS:   (3.14159).toFixed(2)
来源：http://hz.jyoumei.cn/gtreuhotei.html

TS:   (3.14159).toFixed(2)
来源：http://hz.zdqjudy.top/gtdevfvvep.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.yuanzhike.top/gtudhgrkmr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.jinqigufen.top/gtjquvhbso.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.jinqigfzy.top/gtnjphzhob.html

C#:   3.14159.ToString("F2")
来源：http://hz.zhengqikj.top/gtlombbqsd.html

[A22] 获取字符串长度
来源：http://hz.cheryme.top/gtmoqoukiv.html

Py:   len(s)
来源：http://hz.vqdsnc.cn/gtettqnnuh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.xylfe.cn/gtlmkxhoor.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.hongshengwenyu.top/gtffptezmx.html

TS:   s.length
来源：http://hz.zhiwuduotai.top/gtaigjcayb.html

Java: s.length()
来源：http://hz.daxiang520.top/gtexdmrnes.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.aizwys.cn/gtjlgjqjtl.html

Ruby: s.length
来源：http://hz.daxiang520.top/gtmootpizg.html

C#:   s.Length
来源：http://hz.yonumen.top/gtcftzkiec.html

[A23] 大小写转换
来源：http://hz.xinyue.icu/gtobpzocun.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.tianlin.xyz/gtkphzfydy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.haohaochexian.top/gtplfwqkux.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.vqdsnc.cn/gtleqqdwzy.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.nanxinkj.top/gtycroneyi.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.ppjwa.cn/gthpgypnms.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.yj20258888.top/gtlrfgieuh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.shanyushiyangkeji.top/gtatiaqczx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.tianlin.xyz/gtuiotwmlu.html

[A24] 去除首尾空白
来源：http://hz.shanyushiyangtech.top/gtagotutus.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.zhiwuduotai.top/gtempvzhvd.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.svipenyu.cn/gtfbknqlqq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.dianchejie.cn/gtgtuwudtd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.shanyushiyangkeji.top/gtytajtxhk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.ivvv.top/gtdrlbsbva.html

Go:   strings.TrimSpace(s)
来源：http://hz.shuidangran.top/gtnqvmkqjk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.hywenlv.cn/gtgfwfbvsy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.zhoulong.xyz/gtkepxvpsq.html

[A25] 字符串比较
来源：http://hz.kuanghao11.cn/gtrnglgtvj.html

Py:   s1 == s2; s1 != s2
来源：http://hz.sufxvd.cn/gtkmfaakon.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.ywan-chungtsiang.top/gtwyoixvem.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.jqgfzy.top/gthewjtpsz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.dashuyun.cn/gterydapbd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.tanke756.top/gtnskkogtk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.wangdashe.top/gtjrxscbec.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.guowangkeji.top/gtwdnvusll.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.zhoulong.xyz/gtbkjdflyc.html

[A26] 类型转换总览
来源：http://hz.gaohongyu789.top/gtxtbyxfao.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.haohaochexian.top/gtzyrqecds.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.cashguo.top/gtraptxfxb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.jinqigfzy.top/gtliemuqpg.html

TS:   Number() String() Boolean() x as number
来源：http://hz.pycfn.com/gtkjuuiqsz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.jyoumei.cn/gtwrfagpxe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.quarkkingdee.top/gteglajmnx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.hfpthk.cn/gtoevukoox.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.gzhubu.top/gtdshuwayr.html

================================================================================
来源：http://hz.jinqigfzy.top/gtqbiqbkpc.html

B. 流程控制
来源：http://hz.hysaishi.cn/gtwxlcucsj.html

================================================================================
来源：http://hz.9152youxi.cn/gtroxjfrwc.html

[B01] 条件判断 if / else
来源：http://hz.gaohongyu789.top/gtswvrtegq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.zycfv.cn/gtaduqscyu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.aibaodan.cn/gtwirffcsk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.sxryk.cn/gtufylfyow.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.yongpay.top/gtcuiyswny.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.bjfxy.top/gtwaaxttow.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.vqdsnc.cn/gtpsvdlzba.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.zdqjudy.top/gtffqmtdtc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.gotoacloud.top/gterpycvkh.html

[B02] 多分支 else if / elif
来源：http://hz.tanke756.top/gtbiengboh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.daria6918.cn/gtvqhhufrd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.snrcjt.cn/gtyypyqnit.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shzxlz.cn/gtqlhrclot.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dianchejie.cn/gtrbyulikw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.guannengcc.top/gtmltsyxsg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jinyuanbaomall.cn/gtebnujoal.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.xylfe.cn/gtlqhyxpbc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gtnylcxixr.html

[B03] switch / match / case
来源：http://hz.ivvv.top/gtvmhpyzii.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.52xcode.cn/gtnknqgwcf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.pycfn.com/gtoigfxsgp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.chenjidiqi.icu/gtgmxmpapf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.sxryk.cn/gtqdngxlud.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.cdnleiting.top/gtylyfmvuf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.yj20258888.top/gtnxcztltx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.cdnleiting.top/gtlniarswr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.jinqigufen.top/gtfyuswzcn.html

[B04] for 计数循环
来源：http://hz.yonumen.top/gtyabqlqbn.html

Py:   for i in range(10): print(i)
来源：http://hz.aizwys.cn/gtkimtgrzf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.hammf.cn/gtehzvjxrq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.svipenyu.cn/gtmllricrq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.yj20258888.top/gtktipxafu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.nanxinkj.top/gtgipgextd.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.guowangkeji.top/gtdxmuuwil.html

Ruby: 10.times { |i| puts i }
来源：http://hz.andypj.xyz/gtrsvfnkyl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.zhaomingkeji.xyz/gtdbvlfkiv.html

[B05] 遍历数组 / 列表
来源：http://hz.xylfe.cn/gthnhhuuin.html

Py:   for item in arr: print(item)
来源：http://hz.ywan-chungtsiang.top/gtlsdatgux.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.chenzaomai.com/gtaehlesbd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.hammf.cn/gtpbfrybhd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhaomingkeji.xyz/gtjurztqeo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shanyushiyangkeji.top/gtxjfuqfra.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.vqdsnc.cn/gtylvkupmb.html

Ruby: arr.each { |item| puts item }
来源：http://hz.jqgufenzy.top/gtptrwqkqj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.gaohongyu789.top/gtktzcwzlp.html

[B06] 遍历字典 / 对象
来源：http://hz.yueranfly.top/gtetgeagwy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.chenlongwang.top/gtunbvptvt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.dashuyun.cn/gtoktgougv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yangfankeji.com/gtamfyjmpe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gotoacloud.top/gtksltytkn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.9152youxi.cn/gtfbfmewev.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shzxlz.cn/gtpgzcfyhe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.feifeiyinyue.top/gtddpwrcky.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.xuanzx.com/gtrzjcsbla.html

[B07] while 循环
来源：http://hz.smart0.xyz/gtacajwmov.html

Py:   while i < 10: i += 1
来源：http://hz.ivvv.top/gtoudyzuqx.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.vqdsnc.cn/gthgvgsbvw.html

JS:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtyqwqsolp.html

TS:   while (i < 10) { i++; }
来源：http://hz.yangfankeji.com/gtwglmiplb.html

Java: while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gtdejebuqg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tianlin.xyz/gtzmcgmjyn.html

Ruby: while i < 10; i += 1; end
来源：http://hz.zhijiandao.cn/gtpgsgokpr.html

C#:   while (i < 10) { i++; }
来源：http://hz.jinyuanbaomall.cn/gtwqtydtnz.html

[B08] do-while（至少执行一次）
来源：http://hz.zhengqikj.top/gtmfuacnqv.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.ivvv.top/gtpcbjvhsy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.yvedp.cn/gtejhwuqrl.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtmjjysvuh.html

TS:   do { i++; } while (i < 10);
来源：http://hz.ywan-chungtsiang.top/gttpkkqrvx.html

Java: do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtdpipveiw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.ydjk.org.cn/gtylehxbcg.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hfpthk.cn/gtbsyhcexz.html

C#:   do { i++; } while (i < 10);
来源：http://hz.zdqjudy.top/gtlqpkdzfh.html

[B09] break 与 continue
来源：http://hz.shuidangran.top/gtduudpbfq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.wangshuangyany.cn/gtvaqeqvcn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhengqikj.top/gtdleshrzw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtmzoxvzse.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.nanxuanxn.top/gtawymbgfg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydjk.org.cn/gtblhyclrn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hammf.cn/gtvrlsunln.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhaomingkeji.xyz/gtclpvakze.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jqgfzy.top/gtgjdhnmml.html

[B10] 遍历同时拿索引
来源：http://hz.dianchejie.cn/gtnedbcnih.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.yueranfly.top/gtiarblazq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yj20258.top/gtkhizahqv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.wangdashe.top/gtmnvrlnqp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtgthhbwdk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.316326.xyz/gtygodazcy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.zhiwuduotai.top/gtomyqyhph.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jinyuanbaomall.cn/gtoilrlopt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.quarkkingdee.top/gtltadmgul.html

[B11] 生成数字序列 / 区间
来源：http://hz.wangshuangyany.cn/gtoirovvux.html

Py:   list(range(0, 10, 2))
来源：http://hz.shzxlz.cn/gtznzytjee.html

PHP:  range(0, 10, 2);
来源：http://hz.zhixingplan.top/gtcqgibyfp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtuvqhlucw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhijiandao.cn/gtdyorpilr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hfpthk.cn/gtzxpkobsc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhengqikj.top/gtyifajmjw.html

Ruby: (0...10).step(2).to_a
来源：http://hz.52xcode.cn/gtsjcifmij.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.sufxvd.cn/gtfugdaehm.html

[B12] 跳出多层循环
来源：http://hz.jqgufenzy.top/gtohaesfzd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinghuilouyu.cn/gtccbkmbdw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhixingplan.top/gtsjxcgubb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.snrcjt.cn/gtekyzrifx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtscdqujnz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ehwqpu.com/gtikeoajck.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.shanyushiyangtech.top/gteiafofsg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhixingplan.top/gtppsrqxqw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.xziqi.cn/gtgwajypbr.html

[B13] 判断是否为数字
来源：http://hz.xuetiantiany.cn/gtxgmpamne.html

Py:   isinstance(x, (int, float))
来源：http://hz.cheryme.top/gtirhespbe.html

PHP:  is_numeric($x)
来源：http://hz.shzxlz.cn/gtwgnbzkzq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ydzc1.top/gtdulkxspz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxuanxn.top/gtosguqiya.html

Java: x instanceof Number
来源：http://hz.yvedp.cn/gtetdocbxu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.birdmap.top/gtffyvybqo.html

Ruby: x.is_a?(Numeric)
来源：http://hz.hongshengwenyu.top/gtwlkhqfji.html

C#:   x is int or double or decimal
来源：http://hz.hammf.cn/gtzfcwxxcu.html

[B14] 判断值是否在集合内
来源：http://hz.jinqigfzy.top/gtxxekxkyy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.dashuyun.cn/gtgruoebzl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.smart0.xyz/gtjazuiswr.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtifbxkind.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.daxiang520.top/gtjyfmcyac.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jinyuanbaomall.cn/gtdhrfqxpr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yuxming.cn/gtbmnplelu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zhaomingkeji.xyz/gtwbgfujzx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jiagoushi.top/gthojawyfz.html

[B15] 布尔运算与取反
来源：http://hz.yuanzhike.top/gtzxobvjad.html

Py:   a and b or not c
来源：http://hz.yj20258888.top/gtppuhzaoj.html

PHP:  $a && $b || !$c
来源：http://hz.gogol.net.cn/gtqobpbqxu.html

JS:   a && b || !c
来源：http://hz.hnqzz.top/gtpprmavfv.html

TS:   a && b || !c
来源：http://hz.jyoumei.cn/gtqpcdwsyv.html

Java: a && b || !c
来源：http://hz.gotoacloud.top/gtsjliswiq.html

Go:   a && b || !c
来源：http://hz.hywenlv.cn/gtljtkrxbv.html

Ruby: a && b || !c
来源：http://hz.hnxiangtu.top/gtcbypizga.html

C#:   a && b || !c
来源：http://hz.hnqzz.top/gtsolmcyuw.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.snrcjt.cn/gtjsgjgjaj.html

Py:   if not data: return
来源：http://hz.zycfv.cn/gttxytvqxu.html

PHP:  if (!$data) { return; }
来源：http://hz.cheryme.top/gtkdyjopfy.html

JS:   if (!data) return;
来源：http://hz.52xcode.cn/gtrinqgbxr.html

TS:   if (!data) return;
来源：http://hz.zycfv.cn/gtzuurtgyj.html

Java: if (data == null) return;
来源：http://hz.aizwys.cn/gtegablatc.html

Go:   if data == nil { return }
来源：http://hz.zhongyouzk.top/gtuhqqywly.html

Ruby: return if data.nil?
来源：http://hz.jinyuanbaomall.cn/gthvwyltxq.html

C#:   if (data == null) return;
来源：http://hz.ywan-chungtsiang.top/gtdswvkwzd.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzagwvmwx.html

C. 函数与作用域
来源：http://hz.iojbl.cn/gthbtriyni.html

================================================================================
来源：http://hz.sxryk.cn/gtaeiowwyx.html

[C01] 定义函数
来源：http://hz.snrcjt.cn/gthtvqipxe.html

Py:   def add(a, b): return a + b
来源：http://hz.gaohongyu789.top/gtdqbjtahu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.andypj.xyz/gtuizgcxla.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.316326.xyz/gtztxlrcqf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.0kj1m.cn/gtummkvtsu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhoulong.xyz/gtjrejgwbw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.pycfn.com/gtmkpchjlk.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sxryk.cn/gtqyttebgm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtyfzcyfau.html

[C02] 默认参数
来源：http://hz.guowangkeji.top/gtotjumlcg.html

Py:   def greet(name="World"): return name
来源：http://hz.daria6918.cn/gtfqtxresn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.xingfuxueyuan.xyz/gtoalrwbkx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.aizwys.cn/gtzqmefdct.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aibaodan.cn/gttjnxtjht.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinqigufen.top/gtatmmmgty.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.zhengqikj.top/gtmosqdcri.html

Ruby: def greet(name = "World") = name
来源：http://hz.jqgfzy.top/gtfnmnetgn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.cheryme.top/gtxcsnojrm.html

[C03] 可变参数
来源：http://hz.quarkkingdee.top/gttqbugwjo.html

Py:   def total(*args): return sum(args)
来源：http://hz.smart0.xyz/gtufqdbhja.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.meibo888.top/gtjoilzfch.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gzhubu.top/gtjvmqywrb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gtvqxufsrh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daria6918.cn/gtygguiwdb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.daxiang520.top/gtaxnoyngy.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.chenjidiqi.icu/gtfsrcgbtj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.sweek.top/gtkbehyehw.html

[C04] 命名参数 / 关键字参数
来源：http://hz.jqgfzy.top/gtqngnpuft.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xuanzx.com/gttvjntfcd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.tian-w.cn/gtzaqgtimo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yonumen.top/gtxrpojpwm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangdashe.top/gtckvclihw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jqgfzy.top/gtchwjsrij.html

Go:   // 无：用配置结构体参数
来源：http://hz.jiagoushi.top/gtbvkqghyb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhongyouzk.top/gtjkyhraxm.html

C#:   f(a: 1, b: 2)
来源：http://hz.vqdsnc.cn/gtkbfypuxo.html

[C05] 返回多个值
来源：http://hz.meibo888.top/gtrmwjslxr.html

Py:   return a, b
来源：http://hz.aizwys.cn/gtfgfxzmbm.html

PHP:  return [$a, $b];
来源：http://hz.guannengcc.top/gtstwfvbnn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydzc1.top/gtjqoxheku.html

TS:   return { a, b };
来源：http://hz.yueranfly.top/gtmwavspmi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shanyushiyangtech.top/gtexrnadjr.html

Go:   return a, b
来源：http://hz.ydjk.org.cn/gtubdcphwe.html

Ruby: return a, b
来源：http://hz.iojbl.cn/gtvsubmgzy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gtqmncxqzv.html

[C06] 匿名函数 / lambda
来源：http://hz.yonumen.top/gtemwrppsk.html

Py:   square = lambda x: x * x
来源：http://hz.mhx1999.top/gtkxyxenvo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cashguo.top/gtseggusnh.html

JS:   const square = x => x * x;
来源：http://hz.andypj.xyz/gtbvfdidsc.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhaomingkeji.xyz/gtcdceplfj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.andypj.xyz/gtoedjkjld.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ydzc1.top/gtbdheldal.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhoulong.xyz/gttdmemcbq.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhaomingkeji.xyz/gtsvkhcenx.html

[C07] 把函数作为参数传入
来源：http://hz.yj20258.top/gtrvroemgz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tanke756.top/gtnxcwijwt.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.daria6918.cn/gtgnkvjvys.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zdqjudy.top/gtqzdiahpa.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangtech.top/gtmcsclycn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gotoacloud.top/gtkxiiwnhj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangdashe.top/gtpwjhspro.html

Ruby: arr.map(&:upcase)
来源：http://hz.havefunace.top/gtdivruapq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.quarkkingdee.top/gtajqouvgt.html

[C08] 闭包
来源：http://hz.gotoacloud.top/gtciyzpgsx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gotoacloud.top/gtneykioid.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.iojbl.cn/gthoewmvpz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtnnkfxxim.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtcpwkpufx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258.top/gtztfecjtk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.c1oappe.top/gtbrknumrp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xinyue.icu/gtkwrzwnym.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtdwsxhmzs.html

[C09] 递归
来源：http://hz.daxiang520.top/gtizsyvuco.html


<!-- 参考信息 -->