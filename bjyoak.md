代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.gogol.net.cn/gtywizvfuc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.c1oappe.top/gthanigbag.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.havefunace.top/gtpafazdyd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.svipenyu.cn/gtmolmlcpa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.hysaishi.cn/gtugxogpij.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.fzhhl.top/gtrkrdgfln.html

[B07] while 循环
来源：http://hz.fengsongda.top/gtphlbsmoz.html

Py:   while i < 10: i += 1
来源：http://hz.hnqzz.top/gtsxalpmft.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.meibo888.top/gtzguqhath.html

JS:   while (i < 10) { i++; }
来源：http://hz.fengsongda.top/gtpfuycclv.html

TS:   while (i < 10) { i++; }
来源：http://hz.sxryk.cn/gtdsonavfl.html

Java: while (i < 10) { i++; }
来源：http://hz.andypj.xyz/gtxcthjpga.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.sufxvd.cn/gtrehggdkq.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hywenlv.cn/gtxuaivnfm.html

C#:   while (i < 10) { i++; }
来源：http://hz.0kj1m.cn/gtwcgehzez.html

[B08] do-while（至少执行一次）
来源：http://hz.ydjk.org.cn/gtlekavuey.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gogol.net.cn/gtxywdfnwa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.ywan-chungtsiang.top/gtxmoqxyuz.html

JS:   do { i++; } while (i < 10);
来源：http://hz.zhiwuduotai.top/gtlryibxkf.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zycfv.cn/gtcwetnspc.html

Java: do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtqpbbviep.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.daxiang520.top/gtnxagsmfa.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.pycfn.com/gtrvifndsr.html

C#:   do { i++; } while (i < 10);
来源：http://hz.xuanzx.com/gteqyarozt.html

[B09] break 与 continue
来源：http://hz.zhengqikj.top/gtlbluuqbn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.tianlin.xyz/gtkfdjwacw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.jqgfzy.top/gtelysywsw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sweek.top/gtwqrjxbkj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yangfankeji.com/gtibvniaic.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xziqi.cn/gtbfqdokry.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.gzhubu.top/gtzlzhovqc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.quarkkingdee.top/gtobabflfr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangshuangyany.cn/gthqbyeqyn.html

[B10] 遍历同时拿索引
来源：http://hz.tianlin.xyz/gttavyqcyn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.fzhhl.top/gtbinoomiu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.jlsjyb.cn/gtqkmjtajp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.yuxming.cn/gtacsibytc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.kuanghao11.cn/gtnnsxkziu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.tianlin.xyz/gteufavjwv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.yvedp.cn/gtsohnrpdu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yonumen.top/gtrwcysgkg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.wangdashe.top/gttncgsjcp.html

[B11] 生成数字序列 / 区间
来源：http://hz.vqdsnc.cn/gtlxegrqsn.html

Py:   list(range(0, 10, 2))
来源：http://hz.zhiwuduotai.top/gtwahoayls.html

PHP:  range(0, 10, 2);
来源：http://hz.hysaishi.cn/gtxxnjqzzn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtebqaqtjm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hongshengwenyu.top/gtoenwrbsb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.zhoulong.xyz/gtfknmlhqe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.gogol.net.cn/gtqzyjhgnh.html

Ruby: (0...10).step(2).to_a
来源：http://hz.gaohongyu789.top/gtnsjkcnji.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.aibaodan.cn/gtbrrdwcbe.html

[B12] 跳出多层循环
来源：http://hz.hnxiangtu.top/gtrsolscaa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.shzxlz.cn/gtggnbbtim.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.pycfn.com/gtjmqxssoe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yvedp.cn/gthrbsktck.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.ppjwa.cn/gtwavrxbcb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jinqigufen.top/gtrkhkoxyv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xingfuxueyuan.xyz/gtiuqaihtm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hywenlv.cn/gtackbxwzy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.iojbl.cn/gtdgdgcgei.html

[B13] 判断是否为数字
来源：http://hz.feifeiyinyue.top/gtlhkaxrat.html

Py:   isinstance(x, (int, float))
来源：http://hz.shzxlz.cn/gtcszdfobn.html

PHP:  is_numeric($x)
来源：http://hz.dashuyun.cn/gtznqmmvui.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sweek.top/gtkasoghjf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.hysaishi.cn/gtecandjtx.html

Java: x instanceof Number
来源：http://hz.yj20258.top/gtetsyobpq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.guannengcc.top/gtaffbhtnh.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jinghuilouyu.cn/gtinwaefda.html

C#:   x is int or double or decimal
来源：http://hz.smart0.xyz/gtnfxqmkkl.html

[B14] 判断值是否在集合内
来源：http://hz.hywenlv.cn/gtkawoials.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.zdqjudy.top/gtjlgdpahz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.dashuyun.cn/gtzjvoqnfc.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtodorsvdz.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.zhiwuduotai.top/gteqyvpklu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.kuanghao11.cn/gtmjxgnmux.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.fengsongda.top/gtpsatsrum.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xinyue.icu/gthjmjkavv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.pengpengdd.cyou/gtksrdhzsh.html

[B15] 布尔运算与取反
来源：http://hz.tanke756.top/gtnvlkeaej.html

Py:   a and b or not c
来源：http://hz.quarkkingdee.top/gtxoqizmdv.html

PHP:  $a && $b || !$c
来源：http://hz.iojbl.cn/gtaturmbqq.html

JS:   a && b || !c
来源：http://hz.jianghu66.top/gtyacnllum.html

TS:   a && b || !c
来源：http://hz.gotoacloud.top/gtgdkcqfiz.html

Java: a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtztgueixc.html

Go:   a && b || !c
来源：http://hz.jinyuanbaomall.cn/gtubhqiela.html

Ruby: a && b || !c
来源：http://hz.jiagoushi.top/gtoncaqweb.html

C#:   a && b || !c
来源：http://hz.zhixingplan.top/gtyuruqiid.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.yueranfly.top/gtgdmjahhn.html

Py:   if not data: return
来源：http://hz.hammf.cn/gtulwbnfpo.html

PHP:  if (!$data) { return; }
来源：http://hz.yuanzhike.top/gtnsifwilj.html

JS:   if (!data) return;
来源：http://hz.yvedp.cn/gtsasmrqwf.html

TS:   if (!data) return;
来源：http://hz.ppjwa.cn/gtmyhjsnxs.html

Java: if (data == null) return;
来源：http://hz.shzxlz.cn/gtkylbonet.html

Go:   if data == nil { return }
来源：http://hz.sysykeji.top/gtmykvbpoh.html

Ruby: return if data.nil?
来源：http://hz.zhengqikj.top/gtlenmwohz.html

C#:   if (data == null) return;
来源：http://hz.mhx1999.top/gtmkcwvykt.html

================================================================================
来源：http://hz.ppjwa.cn/gtyqkerqyg.html

C. 函数与作用域
来源：http://hz.birdmap.top/gtrfmqpfvj.html

================================================================================
来源：http://hz.yj20258.top/gtipjakywb.html

[C01] 定义函数
来源：http://hz.pengpengdd.cyou/gtfgiikbma.html

Py:   def add(a, b): return a + b
来源：http://hz.havefunace.top/gtggmkyzco.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yueranfly.top/gtcrmongqp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhijiandao.cn/gtxkuqmfis.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gtsiaklqkv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ywan-chungtsiang.top/gtmoevbaae.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ydzc1.top/gtjwupdxmi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yuanzhike.top/gtjwjfdzjq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtpbaavldp.html

[C02] 默认参数
来源：http://hz.zhongyouzk.top/gtrxxtgoxs.html

Py:   def greet(name="World"): return name
来源：http://hz.nanxuanxn.top/gtobobebvk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hammf.cn/gtvbeveoac.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.9152youxi.cn/gtsvgimlfa.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yuanzhike.top/gtywvsbtpj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.smart0.xyz/gtcmvsqiwu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.birdmap.top/gtghqwgtdr.html

Ruby: def greet(name = "World") = name
来源：http://hz.andypj.xyz/gtgxlrmamn.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgufenzy.top/gtpzguzsec.html

[C03] 可变参数
来源：http://hz.wangdashe.top/gtuapgbypq.html

Py:   def total(*args): return sum(args)
来源：http://hz.jiagoushi.top/gtbecwazfb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.nanxinkj.top/gtgvbweswg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.pycfn.com/gtpmauxgga.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.xingfuxueyuan.xyz/gtcqzokclk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shanyushiyangkeji.top/gtofceakge.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jqgufenzy.top/gtxfqrcfwt.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtegxxibza.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.cdnleiting.top/gtmfkrvlas.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xinyue.icu/gtbtotkwkd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xingfuxueyuan.xyz/gtdlgrbgup.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yonumen.top/gtqvlngpql.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.fengsongda.top/gtgueqegvb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.0kj1m.cn/gtiumrxotc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenlongwang.top/gtkqzahphm.html

Go:   // 无：用配置结构体参数
来源：http://hz.ydzc1.top/gtmdynjwrr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hywenlv.cn/gtqninurfx.html

C#:   f(a: 1, b: 2)
来源：http://hz.xinyue.icu/gtlbbkurmg.html

[C05] 返回多个值
来源：http://hz.snrcjt.cn/gtzivwfzjl.html

Py:   return a, b
来源：http://hz.zhaomingkeji.xyz/gtnklowbjc.html

PHP:  return [$a, $b];
来源：http://hz.yuanzhike.top/gtjdobbezw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yuxming.cn/gtjkycyurx.html

TS:   return { a, b };
来源：http://hz.9152youxi.cn/gtfdmlxtie.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sufxvd.cn/gtbdzqluvz.html

Go:   return a, b
来源：http://hz.jlsjyb.cn/gtswvrnjzv.html

Ruby: return a, b
来源：http://hz.xuetiantiany.cn/gteeaosrez.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangshuangyany.cn/gtjelhjrlf.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gtgmjmktcq.html

Py:   square = lambda x: x * x
来源：http://hz.jyoumei.cn/gtpehhoryi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.xinyue.icu/gtbkxcvvsh.html

JS:   const square = x => x * x;
来源：http://hz.kuanghao11.cn/gtfbvgbfpn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.gotoacloud.top/gtqfdnbvhc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.haohaochexian.top/gtmyesptgm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jyoumei.cn/gtbvnrprtm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.mhx1999.top/gtsyzgtjit.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.haohaochexian.top/gtasnbrfne.html

[C07] 把函数作为参数传入
来源：http://hz.9152youxi.cn/gtcprlqejw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zhongyouzk.top/gtrkwwdbxu.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.quarkkingdee.top/gtpyrftlfy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nanxinkj.top/gtsygwgari.html

TS:   arr.map(String)
来源：http://hz.snrcjt.cn/gtbdmsiihv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.wangdashe.top/gtglfdvebn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hongshengwenyu.top/gtiqpiogrg.html

Ruby: arr.map(&:upcase)
来源：http://hz.redwolf501.top/gthehjbfil.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ydjk.org.cn/gtgzblkiyl.html

[C08] 闭包
来源：http://hz.tanke756.top/gtmxjshguf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.xuanzx.com/gtyoqgwtuy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xylfe.cn/gtqaegqaie.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtpkhixzvq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtpkoqhdlg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hammf.cn/gtkbttqari.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuanzhike.top/gtkixqwbga.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.cqqwz.cn/gtxtxywirg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xziqi.cn/gtxiuvgqry.html

[C09] 递归
来源：http://hz.nanxinkj.top/gtswhncytk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yongpay.top/gtxgvmkeud.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.havefunace.top/gttmmwwfin.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xylfe.cn/gtshuczvkd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtsybdrdxb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xinyue.icu/gtubpsnzou.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.feifeiyinyue.top/gtjwnybbda.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtuetijyhx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.kuanghao11.cn/gtsyyabcsq.html

[C10] 变量作用域
来源：http://hz.fengsongda.top/gtrbprhwsk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yj202588.top/gtyzrbmwvf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xinyue.icu/gtvrzxlgef.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.birdmap.top/gteamquovj.html

TS:   同 JS
来源：http://hz.jyoumei.cn/gtiazetknh.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtycqzsfeu.html

Go:   花括号块级作用域
来源：http://hz.hfpthk.cn/gtlhjlrypp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.pycfn.com/gtfvkwcupo.html

C#:   块级作用域
来源：http://hz.dianchejie.cn/gtibzwrhsl.html

[C11] 模块导入与导出
来源：http://hz.iojbl.cn/gtzvxpzrbl.html

Py:   from module import func
来源：http://hz.jinqigufen.top/gtpmgmgyzv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hnxiangtu.top/gttohyqilu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dianchejie.cn/gtjhpfoyjc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydjk.org.cn/gtrviniezu.html

Java: import java.util.List;
来源：http://hz.snrcjt.cn/gtywafvizk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guowangkeji.top/gtlnwrgtyv.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.svipenyu.cn/gttfjkpgbh.html

C#:   using System.Text;
来源：http://hz.shanyushiyangkeji.top/gtkrpagjvz.html

[C12] 立即执行函数 IIFE
来源：http://hz.0kj1m.cn/gtnupqthvy.html

Py:   (lambda: print("run"))()
来源：http://hz.zhiwuduotai.top/gtngxthhrv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj202588.top/gtvmqveani.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtkuljbdsk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtvtjryivb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gtozaflgla.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxuanxn.top/gtjjqfwlxf.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinyuanbaomall.cn/gtpdcfmbhi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zycfv.cn/gtebwtgyoy.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgufenzy.top/gthwxujqis.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.smart0.xyz/gtlgerclyr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cdnleiting.top/gtdfydjmzb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nwbrower.top/gtqpvfrfjn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gtemqfkufq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtasbthdyy.html

Go:   func add(a, b int) int
来源：http://hz.yj20258888.top/gtyoivsrqs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gzhubu.top/gtdjhgtbzu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ivvv.top/gtfoyivqcx.html

[C14] 泛型函数
来源：http://hz.nanxuanxn.top/gtabvwkeaj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gtknctpbar.html

PHP:  // 无泛型
来源：http://hz.9152youxi.cn/gtxvkrfkec.html

JS:   // 无泛型
来源：http://hz.chenlongwang.top/gtckqvaeqv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cheryme.top/gtzbauhvfw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.mhx1999.top/gtexfisndl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shanyushiyangkeji.top/gtdescgeev.html

Ruby: # 无泛型
来源：http://hz.chenjidiqi.icu/gttmatsrqj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258.top/gtttnzeter.html

[C15] 解构 / 展开参数
来源：http://hz.xuetiantiany.cn/gtlrmdwkxn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnxiangtu.top/gtbfgbdpfq.html

PHP:  [$a, $b] = $pair;
来源：http://hz.haohaochexian.top/gtuzreanbh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yueranfly.top/gtjzdkudql.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtbrohdblc.html

Java: // 无解构
来源：http://hz.xinyue.icu/gtvmstydgd.html

Go:   // 无解构
来源：http://hz.xuanzx.com/gtidzfbint.html

Ruby: a, b = pair
来源：http://hz.xziqi.cn/gtmtayyqcq.html

C#:   var (a, b) = pair;
来源：http://hz.yj202588.top/gtyjveaxyc.html

[C16] 函数 / 方法重载
来源：http://hz.chenzaomai.com/gtrsozartu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhoulong.xyz/gtnmfwwjtc.html

PHP:  // 无重载
来源：http://hz.nwbrower.top/gtmirstvsa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.iojbl.cn/gtcexjwntl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.gogol.net.cn/gtcsglgtvu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hfpthk.cn/gtevdwqotc.html

Go:   // 无重载：用不同函数名
来源：http://hz.cashguo.top/gtrhhlhmit.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ydjk.org.cn/gtgjekteuh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tianlin.xyz/gtmdnlcbll.html

================================================================================
来源：http://hz.mhx1999.top/gtrleebmyf.html

D. 数组 / 列表 / 集合
来源：http://hz.shangyingyoupin.top/gtbznswiqi.html

================================================================================
来源：http://hz.ybcxt.top/gtlajrvptp.html

[D01] 创建数组 / 列表
来源：http://hz.zhijiandao.cn/gtvsfcrlot.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tanke756.top/gtcarqqcuj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.wangdashe.top/gtpyalvniu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.andypj.xyz/gtytduvgjn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinghuilouyu.cn/gttajyzzxw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtxznlflee.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.feifeiyinyue.top/gtksaxuels.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dashuyun.cn/gtooitnops.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenzaomai.com/gtieuybcjh.html

[D02] 追加元素到末尾
来源：http://hz.jinqigfzy.top/gtauhrwewl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pycfn.com/gtpyftobwh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.quarkkingdee.top/gtrgbxttzu.html

JS:   arr.push(4);
来源：http://hz.ywan-chungtsiang.top/gtvterelbt.html

TS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gteaaqsotb.html

Java: list.add(4);
来源：http://hz.hongshengwenyu.top/gtpdzigjcm.html

Go:   arr = append(arr, 4)
来源：http://hz.gaohongyu789.top/gtfguksiza.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yanxiufei.cn/gtmnwzzejq.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtxdhqcjih.html

[D03] 在指定位置插入元素
来源：http://hz.zhixingplan.top/gtpdynupdf.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangtech.top/gtoomtjdbv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xylfe.cn/gtqduycfvl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.wangdashe.top/gthzfxiibd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtgdjbyral.html

Java: list.add(0, 0);
来源：http://hz.yonumen.top/gtrwdthiug.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.dashuyun.cn/gtdsbioyeu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhiwuduotai.top/gtghxxhwjh.html

C#:   list.Insert(0, 0);
来源：http://hz.0kj1m.cn/gtkxuzxfnw.html

[D04] 删除元素
来源：http://hz.feifeiyinyue.top/gtoblrvvhp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sweek.top/gtbeyapnwe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinghuilouyu.cn/gtlnlusqzg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenjidiqi.icu/gtbbppaulm.html

TS:   arr.splice(0, 1);
来源：http://hz.xuetiantiany.cn/gtuyguleir.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.iojbl.cn/gtxfoiawob.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zycfv.cn/gttfugeciw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tanke756.top/gtnzwrdovz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtxlijoznh.html

[D05] 访问与修改元素
来源：http://hz.redwolf501.top/gtxalvjuqj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.havefunace.top/gtuxuhrexm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj20258.top/gtvldjuecg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.daxiang520.top/gtbukygpnd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cashguo.top/gtdsgrchcw.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ppjwa.cn/gtkmhvypuk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gtraiyfqjf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gtawyymtpt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangdashe.top/gtfmangulc.html

[D06] 数组长度
来源：http://hz.hongshengwenyu.top/gtcqozcsum.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gtlebofkps.html

PHP:  count($arr);
来源：http://hz.gaohongyu789.top/gtdraciswn.html

JS:   arr.length
来源：http://hz.sxryk.cn/gtokicuhne.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtvydojuop.html

Java: list.size();
来源：http://hz.ywan-chungtsiang.top/gteklwrsap.html

Go:   len(arr)
来源：http://hz.jyoumei.cn/gtscrqpaln.html

Ruby: arr.length; arr.size
来源：http://hz.yongpay.top/gthxofdpqy.html

C#:   list.Count;
来源：http://hz.daxiang520.top/gtmchmnccx.html


<!-- 参考信息 -->