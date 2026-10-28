代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://hz.bjfxy.top/gtdeytggej.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.52xcode.cn/gtajjgijoa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.kuanghao11.cn/gtljayfped.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.yongpay.top/gtluvffgkn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.quarkkingdee.top/gtisilqxvv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.ivvv.top/gtowqxjxht.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.hnxiangtu.top/gtwzgxhpak.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.mhx1999.top/gtnzxmnxmd.html

[A26] 类型转换总览
来源：http://hz.daxiang520.top/gthfbzdavs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.zdqjudy.top/gtxnnedszk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.zhoulong.xyz/gtfmpnsnaf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.yj20258.top/gtowdevisv.html

TS:   Number() String() Boolean() x as number
来源：http://hz.aizwys.cn/gtdvmgjlas.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.wangdashe.top/gtiyzrvlwd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.andypj.xyz/gthjjsgmej.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.redwolf501.top/gtxztbrcnh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.xuetiantiany.cn/gtadkzpdcj.html

================================================================================
来源：http://hz.chenlongwang.top/gtoifdwimg.html

B. 流程控制
来源：http://hz.dianchejie.cn/gtpxrhutpr.html

================================================================================
来源：http://hz.smart0.xyz/gtmelrioqk.html

[B01] 条件判断 if / else
来源：http://hz.fengsongda.top/gttafrykkb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.hnxiangtu.top/gtogsczyjd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.nwbrower.top/gtswrjkepj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.wangdashe.top/gtebyaqczl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jianghu66.top/gtotuawcbn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.wangdashe.top/gtjeytbwzj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.svipenyu.cn/gtdmlodmuc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.quarkkingdee.top/gtgmozevoq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.jinqigufen.top/gtuxhdtbvb.html

[B02] 多分支 else if / elif
来源：http://hz.xylfe.cn/gtergcovlz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.yanxiufei.cn/gtbgdduksq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.nanxuanxn.top/gtjblrrrpw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.dashuyun.cn/gtktfzgrxo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.jlsjyb.cn/gtuyoumwjz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shzxlz.cn/gtkjulqpqd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.gaohongyu789.top/gtfjepmytl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.jinghuilouyu.cn/gtdqvwkubl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.cashguo.top/gtbczqsroc.html

[B03] switch / match / case
来源：http://hz.quarkkingdee.top/gtcinzrewb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.fzhhl.top/gtfftpxwaj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.haohaochexian.top/gtjcmykmgw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.9152youxi.cn/gtuuppdhcz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.gotoacloud.top/gttdyszgfo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.jqgfzy.top/gtxywlpkzk.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.cdnleiting.top/gtcrbpiczy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.ydjk.org.cn/gtvlfalcpe.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.nwbrower.top/gtenblwvdy.html

[B04] for 计数循环
来源：http://hz.cucudq.cn/gtbcewjymz.html

Py:   for i in range(10): print(i)
来源：http://hz.shanyushiyangkeji.top/gtextxmmoc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.yj20258888.top/gtizuopmrv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.kuanghao11.cn/gtriwrxtpr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.jinqigufen.top/gtujzibcgh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.ppjwa.cn/gtxtbrzwwf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.jlsjyb.cn/gtklbofwkw.html

Ruby: 10.times { |i| puts i }
来源：http://hz.shuidangran.top/gtuvqntnga.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.52xcode.cn/gtmhyissih.html

[B05] 遍历数组 / 列表
来源：http://hz.jinqigufen.top/gtcvejknlc.html

Py:   for item in arr: print(item)
来源：http://hz.jlsjyb.cn/gtqwjmdcao.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.316326.xyz/gtzhxnqwnn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.smart0.xyz/gtuhovllev.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.sxryk.cn/gtatslqpwn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.shzxlz.cn/gtnfkqtcho.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.aizwys.cn/gtlsqegmvu.html

Ruby: arr.each { |item| puts item }
来源：http://hz.wangshuangyany.cn/gtpdhxyruf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.snrcjt.cn/gtnycfgwwu.html

[B06] 遍历字典 / 对象
来源：http://hz.zhiwuduotai.top/gtexqozlni.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.gaohongyu789.top/gtnlcpesbx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.haohaochexian.top/gtjzdihnqs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.smart0.xyz/gthiknqjro.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.haohaochexian.top/gtxrzwfogh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cashguo.top/gtkehuyuia.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.wangdashe.top/gtgaagcxlk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.redwolf501.top/gtgpxtfvxt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.snrcjt.cn/gtctwgjvol.html

[B07] while 循环
来源：http://hz.nanxuanxn.top/gtvgzzyfgi.html

Py:   while i < 10: i += 1
来源：http://hz.pycfn.com/gtehfrexbz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jinqigfzy.top/gtapqucxrf.html

JS:   while (i < 10) { i++; }
来源：http://hz.snrcjt.cn/gteiduzukp.html

TS:   while (i < 10) { i++; }
来源：http://hz.shuidangran.top/gtazrvaetw.html

Java: while (i < 10) { i++; }
来源：http://hz.shzxlz.cn/gtmaunlngf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.tianlin.xyz/gtiyilqjhq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.yuxming.cn/gtcdfshivp.html

C#:   while (i < 10) { i++; }
来源：http://hz.hnqzz.top/gthbtbgjfv.html

[B08] do-while（至少执行一次）
来源：http://hz.aizwys.cn/gtpkaqcagz.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.zhaomingkeji.xyz/gthrwjhqnw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.andypj.xyz/gtletlbsph.html

JS:   do { i++; } while (i < 10);
来源：http://hz.0kj1m.cn/gtgveunbih.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj202588.top/gthcqasbwx.html

Java: do { i++; } while (i < 10);
来源：http://hz.52xcode.cn/gtwlgjmdda.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.yj202588.top/gtiskaenqc.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.svipenyu.cn/gtedsyiklk.html

C#:   do { i++; } while (i < 10);
来源：http://hz.aizwys.cn/gttyvoqcgb.html

[B09] break 与 continue
来源：http://hz.hywenlv.cn/gthehbryne.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.pycfn.com/gttivvbiys.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.tianlin.xyz/gtbnbcygnu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gogol.net.cn/gtqtcssbbh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.hywenlv.cn/gttcxukgaq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pycfn.com/gtcyunicve.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.vqdsnc.cn/gtblbifmsp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.wangshuangyany.cn/gtqmnqswhr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinqigufen.top/gtouhgqabv.html

[B10] 遍历同时拿索引
来源：http://hz.pengpengdd.cyou/gttdbpxrzb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.xuetiantiany.cn/gtbfsaekpe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.guowangkeji.top/gtefbetkgo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shuidangran.top/gthxaushiz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxinkj.top/gtvwfwapfr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.feifeiyinyue.top/gtgldzuouc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.shanyushiyangtech.top/gtcioztldq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.smart0.xyz/gtkceyjvti.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.xingfuxueyuan.xyz/gtljtynifv.html

[B11] 生成数字序列 / 区间
来源：http://hz.tianlin.xyz/gtlzitwwdp.html

Py:   list(range(0, 10, 2))
来源：http://hz.sweek.top/gtlkcjiyyb.html

PHP:  range(0, 10, 2);
来源：http://hz.redwolf501.top/gtlewolqkv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.wangdashe.top/gtapcgjyfa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.jinqigufen.top/gtylokdsbt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.smart0.xyz/gtbgrbzntl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.hywenlv.cn/gtgddpneae.html

Ruby: (0...10).step(2).to_a
来源：http://hz.316326.xyz/gtkigyksfm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.cheryme.top/gtotpahzgy.html

[B12] 跳出多层循环
来源：http://hz.zhijiandao.cn/gtxhoqdlfo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.yj20258.top/gtpwzddxhn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.bjfxy.top/gteuppdkdn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jqgfzy.top/gttmkuqvim.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.bjfxy.top/gtsshqyrpl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.xuetiantiany.cn/gtsmbcliaq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.mhx1999.top/gtqifpmdeg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.chenzaomai.com/gtoqtoacif.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.ppjwa.cn/gtekvtnstb.html

[B13] 判断是否为数字
来源：http://hz.quarkkingdee.top/gtgkamodog.html

Py:   isinstance(x, (int, float))
来源：http://hz.shzxlz.cn/gtwekokpfi.html

PHP:  is_numeric($x)
来源：http://hz.ydzc1.top/gteeajpnnl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.cheryme.top/gtynhlkves.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fzhhl.top/gtjoumyzps.html

Java: x instanceof Number
来源：http://hz.hnqzz.top/gtvcgajxkv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jyoumei.cn/gtxcjiwbdq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.havefunace.top/gtmmanrqmo.html

C#:   x is int or double or decimal
来源：http://hz.sweek.top/gtxktlyafa.html

[B14] 判断值是否在集合内
来源：http://hz.52xcode.cn/gtinutysji.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xinyue.icu/gtmazrjajv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.guowangkeji.top/gtclggxmkt.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.redwolf501.top/gtyzrsbeoy.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gtaujyblzh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gthnrcuuby.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zdqjudy.top/gtqjylhahi.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.smart0.xyz/gtdurivboj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.0kj1m.cn/gtfrldzuos.html

[B15] 布尔运算与取反
来源：http://hz.cucudq.cn/gtuwhswclt.html

Py:   a and b or not c
来源：http://hz.meibo888.top/gtgpuriaib.html

PHP:  $a && $b || !$c
来源：http://hz.aibaodan.cn/gtgbupnmcr.html

JS:   a && b || !c
来源：http://hz.cqqwz.cn/gtkicsehec.html

TS:   a && b || !c
来源：http://hz.yongpay.top/gtmngqihns.html

Java: a && b || !c
来源：http://hz.sxryk.cn/gtbdyvyagi.html

Go:   a && b || !c
来源：http://hz.tian-w.cn/gttulzpyyq.html

Ruby: a && b || !c
来源：http://hz.smart0.xyz/gtedxexecr.html

C#:   a && b || !c
来源：http://hz.fengsongda.top/gtwitzlhtl.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.xziqi.cn/gtsnssgdey.html

Py:   if not data: return
来源：http://hz.shzxlz.cn/gttefapizg.html

PHP:  if (!$data) { return; }
来源：http://hz.smart0.xyz/gtyiswynlb.html

JS:   if (!data) return;
来源：http://hz.gaohongyu789.top/gtpmnpldmd.html

TS:   if (!data) return;
来源：http://hz.pycfn.com/gtxizbvpot.html

Java: if (data == null) return;
来源：http://hz.fzhhl.top/gtcdbysrgw.html

Go:   if data == nil { return }
来源：http://hz.hfpthk.cn/gtoiwuluid.html

Ruby: return if data.nil?
来源：http://hz.shzxlz.cn/gtznoahazh.html

C#:   if (data == null) return;
来源：http://hz.guannengcc.top/gtywyyvqad.html

================================================================================
来源：http://hz.xinyue.icu/gtzxokjerd.html

C. 函数与作用域
来源：http://hz.yvedp.cn/gtxzymsqub.html

================================================================================
来源：http://hz.yongpay.top/gtlplhkpxj.html

[C01] 定义函数
来源：http://hz.shzxlz.cn/gtguklkpyo.html

Py:   def add(a, b): return a + b
来源：http://hz.xinyue.icu/gtcytmwdjk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.mhx1999.top/gtdnesetak.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.fengsongda.top/gtswqjnshy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.wangdashe.top/gteavhevjf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jinqigfzy.top/gtmtoilnxj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xuanzx.com/gtcyvqrfqj.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shanyushiyangkeji.top/gtkslcasxj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yj202588.top/gtttqdmars.html

[C02] 默认参数
来源：http://hz.xziqi.cn/gtjkzholrj.html

Py:   def greet(name="World"): return name
来源：http://hz.dashuyun.cn/gtmeqsmbya.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cqqwz.cn/gtkrqnlbpq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.vqdsnc.cn/gtpvnsdscx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtmhctemeg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangdashe.top/gtxcocmxdl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gzhubu.top/gtjegzfiqc.html

Ruby: def greet(name = "World") = name
来源：http://hz.hfpthk.cn/gtymjvudju.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhengqikj.top/gtxvjddpyi.html

[C03] 可变参数
来源：http://hz.jyoumei.cn/gtshtulcii.html

Py:   def total(*args): return sum(args)
来源：http://hz.zycfv.cn/gtezfnrvsr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cashguo.top/gtpcraprvo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ivvv.top/gteyyzjanv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.0kj1m.cn/gttrfftxiw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.tianlin.xyz/gtilpwdxzs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.wangshuangyany.cn/gthbqexhug.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.fengsongda.top/gtpcqvoahu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shanyushiyangtech.top/gtsgejzycv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yj20258.top/gteebaljbx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fzhhl.top/gteufmsjqa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.pengpengdd.cyou/gtxzjzupoo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ydzc1.top/gtzplitkog.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shanyushiyangtech.top/gtfgrcqyqj.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.nwbrower.top/gtynfifniv.html

Go:   // 无：用配置结构体参数
来源：http://hz.feifeiyinyue.top/gtxkbyzsab.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xuetiantiany.cn/gtcbzkyyiw.html

C#:   f(a: 1, b: 2)
来源：http://hz.cqqwz.cn/gtamtbpunu.html

[C05] 返回多个值
来源：http://hz.xinyue.icu/gtppyobjkp.html

Py:   return a, b
来源：http://hz.mhx1999.top/gtljwlrfcd.html

PHP:  return [$a, $b];
来源：http://hz.cheryme.top/gtmudfeeeu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zycfv.cn/gtplfarebi.html

TS:   return { a, b };
来源：http://hz.hnqzz.top/gtdcqwwjex.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ivvv.top/gtbtwbsyhi.html

Go:   return a, b
来源：http://hz.xinyue.icu/gtqirfvdxi.html

Ruby: return a, b
来源：http://hz.shanyushiyangkeji.top/gtzdwqpkyy.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jiagoushi.top/gtuwvguwoz.html

[C06] 匿名函数 / lambda
来源：http://hz.nanxinkj.top/gtvqtzafzl.html

Py:   square = lambda x: x * x
来源：http://hz.xylfe.cn/gtgcdxpxrg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangkeji.top/gtayczyoxy.html

JS:   const square = x => x * x;
来源：http://hz.nanxinkj.top/gtxumuqgut.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ybcxt.top/gtrximrgts.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xylfe.cn/gttijuctmx.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hysaishi.cn/gtaipvfljv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yonumen.top/gtovtwmmfx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ybcxt.top/gtxwjkeqex.html

[C07] 把函数作为参数传入
来源：http://hz.shanyushiyangkeji.top/gtmwozalmk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.wangshuangyany.cn/gtplachbwd.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.vqdsnc.cn/gtpzbrvski.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.dashuyun.cn/gtjskuastd.html

TS:   arr.map(String)
来源：http://hz.ppjwa.cn/gtvmhgdwot.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yonumen.top/gtcoatbkdh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hnxiangtu.top/gtyaaiowak.html

Ruby: arr.map(&:upcase)
来源：http://hz.andypj.xyz/gtawrpgjwb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daxiang520.top/gtropwcmva.html

[C08] 闭包
来源：http://hz.hywenlv.cn/gtcbfojqxr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gtwkrwhefi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.sysykeji.top/gtucgbulot.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgfzy.top/gtmrrdmidg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtegkuoxdr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gogol.net.cn/gtrzaqojop.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jiagoushi.top/gtfscsgkdq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.0kj1m.cn/gtonazuffr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj202588.top/gtknygjwvb.html

[C09] 递归
来源：http://hz.aizwys.cn/gteoygtpgc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zhaomingkeji.xyz/gtprddcdly.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xingfuxueyuan.xyz/gttfjaxltv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yuanzhike.top/gtekikwywm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shuidangran.top/gtukkvauzy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yvedp.cn/gtfgjqjyci.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.vqdsnc.cn/gtqttsnyci.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.zhixingplan.top/gtuvqfixua.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigufen.top/gtcfyjzcci.html

[C10] 变量作用域
来源：http://hz.gotoacloud.top/gthzvfabga.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.dashuyun.cn/gtxozusocf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jqgfzy.top/gtjmmbfxvh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.smart0.xyz/gtyedlludm.html

TS:   同 JS
来源：http://hz.gaohongyu789.top/gthwmcxpwq.html

Java: 方法内为块级作用域
来源：http://hz.zdqjudy.top/gtytrdeyhw.html

Go:   花括号块级作用域
来源：http://hz.xuanzx.com/gtumemyocf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.snrcjt.cn/gttgeqqpjv.html

C#:   块级作用域
来源：http://hz.yj20258.top/gtobjwxalk.html

[C11] 模块导入与导出
来源：http://hz.daxiang520.top/gtgmqsueom.html

Py:   from module import func
来源：http://hz.nanxinkj.top/gtyspinaoa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.kuanghao11.cn/gtccgvawta.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.snrcjt.cn/gtfrknnlaf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.52xcode.cn/gtwuccztnk.html

Java: import java.util.List;
来源：http://hz.hnxiangtu.top/gtzpnmethv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shanyushiyangtech.top/gtzbhrtvpm.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yongpay.top/gtmncilhin.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtftmqhdmm.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnqzz.top/gtnrdtkunk.html

Py:   (lambda: print("run"))()
来源：http://hz.pycfn.com/gtwheapidx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jqgfzy.top/gtcbvilphm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangdashe.top/gtfncwvmal.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yanxiufei.cn/gtyoxmeevj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hnxiangtu.top/gtfhrooalv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hfpthk.cn/gtbvzmtfqj.html

Ruby: -> { puts "run" }.call
来源：http://hz.gzhubu.top/gtwhrvfbcm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xingfuxueyuan.xyz/gtxjupehmj.html

[C13] 类型声明 / 类型注解
来源：http://hz.dashuyun.cn/gtfqxbcckg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.iojbl.cn/gtghmllntc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gthwiiblvf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenlongwang.top/gtlbfxlakg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhengqikj.top/gtnlypzknb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yuanzhike.top/gtxvutoxhk.html

Go:   func add(a, b int) int
来源：http://hz.sxryk.cn/gtpkwhaxgo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sweek.top/gtnimeqzlc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hnqzz.top/gtgdbuqxth.html

[C14] 泛型函数
来源：http://hz.ivvv.top/gtijoqsyvc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.pengpengdd.cyou/gtgnpiivij.html

PHP:  // 无泛型
来源：http://hz.pengpengdd.cyou/gtxycwgrmz.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtwhpfoxbk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenzaomai.com/gtaihodlxm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yangfankeji.com/gtmzvtouke.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aizwys.cn/gtlhslwaku.html

Ruby: # 无泛型
来源：http://hz.gzhubu.top/gtnjcspztp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jinyuanbaomall.cn/gtsgfeqjrk.html

[C15] 解构 / 展开参数
来源：http://hz.daxiang520.top/gtilgtqetp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yongpay.top/gtdiyetdrj.html

PHP:  [$a, $b] = $pair;
来源：http://hz.fengsongda.top/gtdapprivu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.dianchejie.cn/gtprcqaaui.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.wangdashe.top/gtzzdoiwbo.html

Java: // 无解构
来源：http://hz.andypj.xyz/gthiacnppw.html

Go:   // 无解构
来源：http://hz.hywenlv.cn/gtclkcduxm.html


<!-- 参考信息 -->