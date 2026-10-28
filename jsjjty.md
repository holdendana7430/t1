代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.sufxvd.cn/gtyclilaor.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.xuetiantiany.cn/gtysvhqnun.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.zhoulong.xyz/gtcpmhohft.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.andypj.xyz/gtxxixtnma.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.gotoacloud.top/gtrkvllypx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ydzc1.top/gtitcvastg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.cashguo.top/gtbbhcsjsk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.daria6918.cn/gtrptnyxrv.html

[A26] 类型转换总览
来源：http://hz.feifeiyinyue.top/gtdpvzchur.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.yongpay.top/gtuskpcfbe.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.mhx1999.top/gtxgcsizvc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yj202588.top/gtghjqirob.html

TS:   Number() String() Boolean() x as number
来源：http://hz.nwbrower.top/gtxhxqxlwm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.9152youxi.cn/gtjkrnsqpl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.hnqzz.top/gtlsjoajmq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.tanke756.top/gtcgstxhfg.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.ywan-chungtsiang.top/gtmbehzdxi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtyfupmafc.html

B. 流程控制
来源：http://hz.cqqwz.cn/gtzyfspbse.html

================================================================================
来源：http://hz.meibo888.top/gtehdnwydp.html

[B01] 条件判断 if / else
来源：http://hz.zhaomingkeji.xyz/gtdebhhcwy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.tanke756.top/gtzpkgrred.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.yueranfly.top/gtmniyygit.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.ydjk.org.cn/gtaxpwjeyn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.smart0.xyz/gtapnqheod.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.jinghuilouyu.cn/gtjvnckpnf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.sufxvd.cn/gtpqcjqlbb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.haohaochexian.top/gtjpwktvsh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jlsjyb.cn/gtwbgkchsj.html

[B02] 多分支 else if / elif
来源：http://hz.gaohongyu789.top/gtnwedultc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.ydjk.org.cn/gtrbhpvudo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.fzhhl.top/gtdldgsuri.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtcfwrnark.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yongpay.top/gtcadrjlwr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.svipenyu.cn/gtddjeneep.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.jlsjyb.cn/gtcjatfktg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.meibo888.top/gtdgskpvmn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.xingfuxueyuan.xyz/gttldxtgdc.html

[B03] switch / match / case
来源：http://hz.xingfuxueyuan.xyz/gtrhmarnzr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.sxryk.cn/gtfbspgffz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.zhixingplan.top/gtcogswnyr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.hnqzz.top/gtupmwxrjj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gogol.net.cn/gtnbpxvpkk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.daxiang520.top/gtcoafmckv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.zhijiandao.cn/gtoswiseyo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.hnxiangtu.top/gtkairxowb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.snrcjt.cn/gtdbawdpwr.html

[B04] for 计数循环
来源：http://hz.wangshuangyany.cn/gtaruilkyw.html

Py:   for i in range(10): print(i)
来源：http://hz.ivvv.top/gttdzqusya.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.fzhhl.top/gthgmyiflw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.hongshengwenyu.top/gtbwkvprto.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.9152youxi.cn/gtbxtkgdfs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.yuanzhike.top/gtksxnlxzn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.smart0.xyz/gtshhrwlpd.html

Ruby: 10.times { |i| puts i }
来源：http://hz.gaohongyu789.top/gtetafdvmn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.316326.xyz/gtnytoscya.html

[B05] 遍历数组 / 列表
来源：http://hz.zhoulong.xyz/gtijwexvdr.html

Py:   for item in arr: print(item)
来源：http://hz.yonumen.top/gtorqqlwhi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.yj20258888.top/gttfvkphbv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.svipenyu.cn/gtazcnbknk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.xziqi.cn/gtigfwaxyx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.hfpthk.cn/gtnmwgmgfa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.shangyingyoupin.top/gtuqrrsume.html

Ruby: arr.each { |item| puts item }
来源：http://hz.ydzc1.top/gtylkycqrz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.chenzaomai.com/gtzqxxcrix.html

[B06] 遍历字典 / 对象
来源：http://hz.gogol.net.cn/gtbvrhtqnx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.sysykeji.top/gtvdgwogai.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.hammf.cn/gtxyrirofe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.feifeiyinyue.top/gtyrcwoyyy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hysaishi.cn/gtyahhgdfo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.guowangkeji.top/gtpqpxkoxu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.jinqigufen.top/gtcnwzybmn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.xuetiantiany.cn/gtfdppulgi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.sxryk.cn/gtmwejlrsv.html

[B07] while 循环
来源：http://hz.cheryme.top/gtzmtvzmxi.html

Py:   while i < 10: i += 1
来源：http://hz.gzhubu.top/gtqdxjntms.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jianghu66.top/gtzelcyaxl.html

JS:   while (i < 10) { i++; }
来源：http://hz.xuetiantiany.cn/gtbukgfcfp.html

TS:   while (i < 10) { i++; }
来源：http://hz.zdqjudy.top/gtbcuhrjwh.html

Java: while (i < 10) { i++; }
来源：http://hz.yj20258888.top/gtkhbvtpma.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.guowangkeji.top/gtgnxookgn.html

Ruby: while i < 10; i += 1; end
来源：http://hz.shuidangran.top/gtdgvasnso.html

C#:   while (i < 10) { i++; }
来源：http://hz.jyoumei.cn/gturovpqzo.html

[B08] do-while（至少执行一次）
来源：http://hz.hammf.cn/gthsdiwrgu.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.jqgufenzy.top/gtdnpjdxiq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.andypj.xyz/gtlhxzlcbi.html

JS:   do { i++; } while (i < 10);
来源：http://hz.gzhubu.top/gtkynfvjue.html

TS:   do { i++; } while (i < 10);
来源：http://hz.xylfe.cn/gtjrqnoycg.html

Java: do { i++; } while (i < 10);
来源：http://hz.yonumen.top/gtggffuhyl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.hysaishi.cn/gtqsatpjso.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.fzhhl.top/gtasjktfwg.html

C#:   do { i++; } while (i < 10);
来源：http://hz.shuidangran.top/gtsxvqpoav.html

[B09] break 与 continue
来源：http://hz.9152youxi.cn/gtpnnurejf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yuanzhike.top/gtbwgamdno.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.andypj.xyz/gtxbxbvsxg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtwimekuip.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shanyushiyangtech.top/gtiqkqciuz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hysaishi.cn/gtmlrhjjfr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.dianchejie.cn/gtwhyqgjvy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xylfe.cn/gtzjnpqwpw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtjeqqrkcz.html

[B10] 遍历同时拿索引
来源：http://hz.jiagoushi.top/gtwewwrurm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.hnqzz.top/gtloklahyo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.yueranfly.top/gthrjpptxk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.bjfxy.top/gtemsymbzw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jqgfzy.top/gtkqtuwxei.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zycfv.cn/gtbfhbzsls.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yuanzhike.top/gtxocizqqz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.tian-w.cn/gtohunicpw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yj202588.top/gtwazrlyiz.html

[B11] 生成数字序列 / 区间
来源：http://hz.ywan-chungtsiang.top/gtornykzkj.html

Py:   list(range(0, 10, 2))
来源：http://hz.ppjwa.cn/gtnlfpvolz.html

PHP:  range(0, 10, 2);
来源：http://hz.jianghu66.top/gtarbiwffw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.ydzc1.top/gtzxxjvxgo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigfzy.top/gtbhmajhzl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.jinqigfzy.top/gtrbpqbnld.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.haohaochexian.top/gtmgnxanpj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.gaohongyu789.top/gtqrqypbdv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.mhx1999.top/gtswlbyjyd.html

[B12] 跳出多层循环
来源：http://hz.zhixingplan.top/gtdxmuhruv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yvedp.cn/gtjgwmzfyv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.gzhubu.top/gtdxgyltej.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.guowangkeji.top/gtymbtqzkm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenzaomai.com/gtlzajxzmx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.pengpengdd.cyou/gtqkczbfsf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.nwbrower.top/gtvksmgmze.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258.top/gtcfjafgvu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.guowangkeji.top/gtsjgjipze.html

[B13] 判断是否为数字
来源：http://hz.yj20258.top/gtcjzkjadc.html

Py:   isinstance(x, (int, float))
来源：http://hz.pycfn.com/gtzyyvhdde.html

PHP:  is_numeric($x)
来源：http://hz.jiagoushi.top/gtyfdisdlh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hongshengwenyu.top/gtthytjqxx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxinkj.top/gtaabfbrqt.html

Java: x instanceof Number
来源：http://hz.ivvv.top/gtwsrxarrl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cheryme.top/gtgmddmgxa.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sxryk.cn/gtgvuxemsw.html

C#:   x is int or double or decimal
来源：http://hz.zhengqikj.top/gtudfsrvki.html

[B14] 判断值是否在集合内
来源：http://hz.ydjk.org.cn/gtzhszpfcj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.sysykeji.top/gttplermwq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.316326.xyz/gtveqqxjdy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtdplhmidb.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.guannengcc.top/gtutepnwur.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhiwuduotai.top/gtbzxigygp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhengqikj.top/gtvtnudsvv.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.shuidangran.top/gtasrtsytm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.iojbl.cn/gtdjqdzfxj.html

[B15] 布尔运算与取反
来源：http://hz.yanxiufei.cn/gtiyffwfvd.html

Py:   a and b or not c
来源：http://hz.guowangkeji.top/gtytdrbnmv.html

PHP:  $a && $b || !$c
来源：http://hz.zhengqikj.top/gtxgoasbdw.html

JS:   a && b || !c
来源：http://hz.cucudq.cn/gtgejzaaey.html

TS:   a && b || !c
来源：http://hz.c1oappe.top/gtxdqxqhqo.html

Java: a && b || !c
来源：http://hz.redwolf501.top/gtyjomohhn.html

Go:   a && b || !c
来源：http://hz.chenzaomai.com/gtqdptpomk.html

Ruby: a && b || !c
来源：http://hz.shuidangran.top/gtjqlgomms.html

C#:   a && b || !c
来源：http://hz.xuanzx.com/gtojztnmcz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.andypj.xyz/gtuuftnmzi.html

Py:   if not data: return
来源：http://hz.quarkkingdee.top/gtbhkrokpr.html

PHP:  if (!$data) { return; }
来源：http://hz.yangfankeji.com/gtwkldizke.html

JS:   if (!data) return;
来源：http://hz.316326.xyz/gthwayglvz.html

TS:   if (!data) return;
来源：http://hz.ywan-chungtsiang.top/gtbjzzwtqv.html

Java: if (data == null) return;
来源：http://hz.quarkkingdee.top/gtsseunwwp.html

Go:   if data == nil { return }
来源：http://hz.ybcxt.top/gtpgwvzbsn.html

Ruby: return if data.nil?
来源：http://hz.yj20258.top/gtrobxawaf.html

C#:   if (data == null) return;
来源：http://hz.havefunace.top/gtzvqxxoea.html

================================================================================
来源：http://hz.ehwqpu.com/gtlwkzgftp.html

C. 函数与作用域
来源：http://hz.shuidangran.top/gttqfxvlqp.html

================================================================================
来源：http://hz.smart0.xyz/gtvqcxvxax.html

[C01] 定义函数
来源：http://hz.jqgufenzy.top/gtmocvdgui.html

Py:   def add(a, b): return a + b
来源：http://hz.ydjk.org.cn/gtoiuvbhii.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.wangshuangyany.cn/gtukjgjexj.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.bjfxy.top/gtioqlxshr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ehwqpu.com/gtumoipheo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtrmwbxxwa.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.dianchejie.cn/gtlnaxvrnd.html

Ruby: def add(a, b); a + b; end
来源：http://hz.chenjidiqi.icu/gtfwzcmirb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtomeolalw.html

[C02] 默认参数
来源：http://hz.jlsjyb.cn/gtjmjbgwsp.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtasuvagai.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.c1oappe.top/gtwukbtgzd.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtrqlgykhh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtgrmajztg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yanxiufei.cn/gtourtxxlx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jqgfzy.top/gtthadxwpe.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnqzz.top/gtwglzltzn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.haohaochexian.top/gtnibtoefi.html

[C03] 可变参数
来源：http://hz.haohaochexian.top/gtudchqsol.html

Py:   def total(*args): return sum(args)
来源：http://hz.dashuyun.cn/gtqhrowvdd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.chenlongwang.top/gtkhqblvqr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gtoamgyfae.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgfzy.top/gtyxbqwlcb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.vqdsnc.cn/gtmqpxqrnm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sysykeji.top/gtvcrjikgh.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.quarkkingdee.top/gtkznbczmb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fzhhl.top/gtshgxgkvi.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhixingplan.top/gtkmunfdes.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.hongshengwenyu.top/gtzupphgrw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.meibo888.top/gtxdhwgoxm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtdjcvylws.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.svipenyu.cn/gtmpxdjsez.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.wangdashe.top/gtgpyomiro.html

Go:   // 无：用配置结构体参数
来源：http://hz.jinghuilouyu.cn/gtlzaizykj.html

Ruby: f(a: 1, b: 2)
来源：http://hz.wangshuangyany.cn/gtulttwvnv.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258888.top/gtkxvcevaz.html

[C05] 返回多个值
来源：http://hz.quarkkingdee.top/gttfgqvtrz.html

Py:   return a, b
来源：http://hz.smart0.xyz/gtgaefxats.html

PHP:  return [$a, $b];
来源：http://hz.jinqigufen.top/gtfsipmsmq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.tian-w.cn/gtpcqufmtc.html

TS:   return { a, b };
来源：http://hz.yvedp.cn/gtwuowcjpe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.iojbl.cn/gtuejhomrg.html

Go:   return a, b
来源：http://hz.sweek.top/gtusgmykfs.html

Ruby: return a, b
来源：http://hz.zhiwuduotai.top/gtlajrmnze.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangdashe.top/gtldxsvwlb.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gtvaqxtvvb.html

Py:   square = lambda x: x * x
来源：http://hz.jqgufenzy.top/gtlmaxckvk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xingfuxueyuan.xyz/gtokjrbilc.html

JS:   const square = x => x * x;
来源：http://hz.ybcxt.top/gtqdotivvz.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenlongwang.top/gtcpyxduke.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.gogol.net.cn/gtxwojrbju.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cqqwz.cn/gtbibjgndu.html

Ruby: square = ->(x) { x * x }
来源：http://hz.pengpengdd.cyou/gtoenpsosr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zdqjudy.top/gtdkfblgnp.html

[C07] 把函数作为参数传入
来源：http://hz.jinyuanbaomall.cn/gtmapzgdyr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gotoacloud.top/gtngcankdm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ivvv.top/gtllqtbopl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cashguo.top/gtnvmlpqpf.html

TS:   arr.map(String)
来源：http://hz.xinyue.icu/gtmslznyfk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jqgufenzy.top/gtogdlxrxx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.daxiang520.top/gtnxxiduak.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenjidiqi.icu/gtvoyphwpe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shuidangran.top/gtkrqcyzup.html

[C08] 闭包
来源：http://hz.ybcxt.top/gtdqupfgeo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.9152youxi.cn/gtckroxckg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sweek.top/gtasynvgxg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtpwzvdmud.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtsrsxqqjl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fzhhl.top/gtxohxxyhb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.chenzaomai.com/gtgnvxmigo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj20258.top/gtguuscfus.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtmyowbnxb.html

[C09] 递归
来源：http://hz.smart0.xyz/gtmuswunla.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gtdzlnsnhy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gtygxirapp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gthzojhpvp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.redwolf501.top/gtbenlrrts.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.quarkkingdee.top/gtyqbrqjic.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhoulong.xyz/gtwuwkyrzr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sweek.top/gtjhdqssfb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yueranfly.top/gtqylxuxva.html

[C10] 变量作用域
来源：http://hz.kuanghao11.cn/gtnyztoqcu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhijiandao.cn/gtpanowvmg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jinqigfzy.top/gtclgszeed.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.52xcode.cn/gtrarzesej.html

TS:   同 JS
来源：http://hz.yanxiufei.cn/gtktiqqnaz.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gttqehrjbo.html

Go:   花括号块级作用域
来源：http://hz.chenzaomai.com/gtgyhvgmjx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.316326.xyz/gtcmzlrgto.html

C#:   块级作用域
来源：http://hz.snrcjt.cn/gtrsyeufyr.html

[C11] 模块导入与导出
来源：http://hz.guannengcc.top/gtsulmzusf.html

Py:   from module import func
来源：http://hz.tianlin.xyz/gtkgheoqdt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zycfv.cn/gttqdfaqvf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtkcvztkld.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.0kj1m.cn/gtzbnwdkst.html

Java: import java.util.List;
来源：http://hz.redwolf501.top/gtdujfqvbs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.andypj.xyz/gtpvzlsduu.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.redwolf501.top/gtlzypqwkd.html

C#:   using System.Text;
来源：http://hz.gaohongyu789.top/gtcdzuumdp.html

[C12] 立即执行函数 IIFE
来源：http://hz.316326.xyz/gtelwavdab.html

Py:   (lambda: print("run"))()
来源：http://hz.mhx1999.top/gtyoartiin.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yuanzhike.top/gtaxzjiedl.html

JS:   (() => { console.log("run"); })();
来源：http://hz.redwolf501.top/gthaaahxfv.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yvedp.cn/gtvlwvqhbg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtddcbspiz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.dashuyun.cn/gtaaeeemdf.html

Ruby: -> { puts "run" }.call
来源：http://hz.guannengcc.top/gtbsmegppt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ehwqpu.com/gtrzfhwxfl.html

[C13] 类型声明 / 类型注解
来源：http://hz.jianghu66.top/gtdohmiipm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtevowvlke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.52xcode.cn/gteuseibiu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.0kj1m.cn/gtnchcgxij.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ydzc1.top/gtuzcpigqm.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtczfyrezi.html

Go:   func add(a, b int) int
来源：http://hz.ivvv.top/gtfpwpytzu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgufenzy.top/gtjidzrcmt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hfpthk.cn/gtrpdeanon.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtpdicwwgj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jianghu66.top/gtouzbafoq.html

PHP:  // 无泛型
来源：http://hz.zhiwuduotai.top/gtjztoevcn.html

JS:   // 无泛型
来源：http://hz.yuxming.cn/gtqpzylxcu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gtllfzneay.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ydzc1.top/gtbqcltsxw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hammf.cn/gtehqieneg.html

Ruby: # 无泛型
来源：http://hz.guannengcc.top/gtbkbhtojw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cashguo.top/gthatjhlix.html

[C15] 解构 / 展开参数
来源：http://hz.dianchejie.cn/gtlszzzvuz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.snrcjt.cn/gtfhzzgvss.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hywenlv.cn/gtpzmupeqf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.fzhhl.top/gtccvvmdwn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.316326.xyz/gtijwenfox.html

Java: // 无解构
来源：http://hz.yj20258.top/gtxsiqlbei.html

Go:   // 无解构
来源：http://hz.haohaochexian.top/gtutzgrumw.html


<!-- 参考信息 -->