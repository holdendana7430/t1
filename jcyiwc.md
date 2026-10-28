代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.shuidangran.top/gthrkvuymi.html

[B06] 遍历字典 / 对象
来源：http://hz.guowangkeji.top/gtwgzacfxl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.hnxiangtu.top/gtddutotek.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.dianchejie.cn/gthuxzwkax.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.wangdashe.top/gtslrlmlax.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.yanxiufei.cn/gttivufkoy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.zhaomingkeji.xyz/gthdrtscld.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.hnqzz.top/gtfatcuaav.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.cqqwz.cn/gtjsusidhg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.aizwys.cn/gtbczlhypk.html

[B07] while 循环
来源：http://hz.chenjidiqi.icu/gtkbfcglbo.html

Py:   while i < 10: i += 1
来源：http://hz.fengsongda.top/gtavdjbbxp.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.jqgfzy.top/gtzvgmaxzx.html

JS:   while (i < 10) { i++; }
来源：http://hz.shanyushiyangtech.top/gthsssjfik.html

TS:   while (i < 10) { i++; }
来源：http://hz.feifeiyinyue.top/gtethmzpfd.html

Java: while (i < 10) { i++; }
来源：http://hz.dianchejie.cn/gtrkethpsv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.52xcode.cn/gttsvpsays.html

Ruby: while i < 10; i += 1; end
来源：http://hz.hnqzz.top/gtvlqljvxa.html

C#:   while (i < 10) { i++; }
来源：http://hz.sweek.top/gtdaxxglmj.html

[B08] do-while（至少执行一次）
来源：http://hz.gaohongyu789.top/gtyfhtlzyt.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.xingfuxueyuan.xyz/gtcmpozpuh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.hysaishi.cn/gtpkwsikhh.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xziqi.cn/gtyhjgdjvg.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhoulong.xyz/gtlvdpdmek.html

Java: do { i++; } while (i < 10);
来源：http://hz.zhixingplan.top/gtbphbligv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.jinqigufen.top/gtmdtcnfqz.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.zhoulong.xyz/gttencscfw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yueranfly.top/gtrgdniadc.html

[B09] break 与 continue
来源：http://hz.yonumen.top/gtuucwwutc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.aizwys.cn/gtyftoprui.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.feifeiyinyue.top/gtvyjsxkrw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.shangyingyoupin.top/gtkutmunfv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.wangdashe.top/gtrsejghhu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.haohaochexian.top/gtsrdsonnt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.xylfe.cn/gttvlunjbn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.9152youxi.cn/gtvdzmfpaj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtcyprsmny.html

[B10] 遍历同时拿索引
来源：http://hz.cheryme.top/gtzfjxuezm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.zdqjudy.top/gtqyxruity.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.ehwqpu.com/gtrfmusaxp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.shzxlz.cn/gtpxiwibnm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.daxiang520.top/gtstuxelac.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.sxryk.cn/gtrgawzdom.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.redwolf501.top/gtvjartclz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.fzhhl.top/gtdezibwvi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.vqdsnc.cn/gtfxyrfebg.html

[B11] 生成数字序列 / 区间
来源：http://hz.chenzaomai.com/gtctbqkjpw.html

Py:   list(range(0, 10, 2))
来源：http://hz.tian-w.cn/gtesyunltl.html

PHP:  range(0, 10, 2);
来源：http://hz.shangyingyoupin.top/gthxqkuiwx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhiwuduotai.top/gtoqgcdzjt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtkofykiod.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.mhx1999.top/gtpapuhjwp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yuxming.cn/gtuebwcsbv.html

Ruby: (0...10).step(2).to_a
来源：http://hz.sxryk.cn/gtwwwlamoi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.bjfxy.top/gttajaeryj.html

[B12] 跳出多层循环
来源：http://hz.guannengcc.top/gtqidpmyxv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.aibaodan.cn/gtvjpzxwvy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.hfpthk.cn/gtfdpeahpb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.jianghu66.top/gtwyoztlkn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258.top/gtsxzbkmot.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cucudq.cn/gtinkrxjsm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xingfuxueyuan.xyz/gtguktrdeq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.cdnleiting.top/gtxvayciua.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.cucudq.cn/gtztxfvnyx.html

[B13] 判断是否为数字
来源：http://hz.aizwys.cn/gtdzwdbfkx.html

Py:   isinstance(x, (int, float))
来源：http://hz.zdqjudy.top/gtpolsawzz.html

PHP:  is_numeric($x)
来源：http://hz.hywenlv.cn/gtmzhtumhx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.c1oappe.top/gtsmpxvdca.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.fengsongda.top/gtfyxbsxkp.html

Java: x instanceof Number
来源：http://hz.ydzc1.top/gthswnitnr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtfhuqgmmq.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuetiantiany.cn/gtcaromife.html

C#:   x is int or double or decimal
来源：http://hz.kuanghao11.cn/gtvdfnyzfa.html

[B14] 判断值是否在集合内
来源：http://hz.dashuyun.cn/gtykilmauw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shanyushiyangkeji.top/gtgkjlgpdn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.wangshuangyany.cn/gtzljvluzz.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jinqigfzy.top/gtiuugaznl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.c1oappe.top/gtgkejvmrc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.iojbl.cn/gtizifxauc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.daria6918.cn/gttytkisyc.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.fzhhl.top/gtzmvwdrbw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.cqqwz.cn/gtwcxqdkib.html

[B15] 布尔运算与取反
来源：http://hz.ivvv.top/gtystonkmt.html

Py:   a and b or not c
来源：http://hz.zhijiandao.cn/gtvimdcwav.html

PHP:  $a && $b || !$c
来源：http://hz.snrcjt.cn/gtefyhucmy.html

JS:   a && b || !c
来源：http://hz.yj20258.top/gtalcygmog.html

TS:   a && b || !c
来源：http://hz.guannengcc.top/gtynfmymsi.html

Java: a && b || !c
来源：http://hz.zhongyouzk.top/gtgzvwantz.html

Go:   a && b || !c
来源：http://hz.yongpay.top/gtzhhfiwcr.html

Ruby: a && b || !c
来源：http://hz.ehwqpu.com/gtxhajgdkw.html

C#:   a && b || !c
来源：http://hz.chenlongwang.top/gtidggdhui.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jiagoushi.top/gtmlkuakca.html

Py:   if not data: return
来源：http://hz.316326.xyz/gtorzqicuc.html

PHP:  if (!$data) { return; }
来源：http://hz.quarkkingdee.top/gtfzatvlgu.html

JS:   if (!data) return;
来源：http://hz.sweek.top/gtvhbotedl.html

TS:   if (!data) return;
来源：http://hz.bjfxy.top/gtiobveleu.html

Java: if (data == null) return;
来源：http://hz.svipenyu.cn/gtqhkphzcp.html

Go:   if data == nil { return }
来源：http://hz.yuanzhike.top/gtywmqqqxb.html

Ruby: return if data.nil?
来源：http://hz.gogol.net.cn/gtggminvtb.html

C#:   if (data == null) return;
来源：http://hz.yuxming.cn/gtjsieinii.html

================================================================================
来源：http://hz.mhx1999.top/gtlnccfbea.html

C. 函数与作用域
来源：http://hz.iojbl.cn/gtdldnbugl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqmahhwqa.html

[C01] 定义函数
来源：http://hz.snrcjt.cn/gtfiigfpcn.html

Py:   def add(a, b): return a + b
来源：http://hz.xinyue.icu/gtomfahtaq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.havefunace.top/gtuozbtvxm.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtsfgsaaky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.birdmap.top/gtmwgfexrp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.ydjk.org.cn/gtdyxfvkno.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.chenlongwang.top/gtrvqdmpfo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yanxiufei.cn/gtotqoohrk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.52xcode.cn/gtjueslrdp.html

[C02] 默认参数
来源：http://hz.pycfn.com/gtdsmahjgm.html

Py:   def greet(name="World"): return name
来源：http://hz.0kj1m.cn/gtishtkfiq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ywan-chungtsiang.top/gtpipbvyel.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jlsjyb.cn/gtpgwkfpia.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gtciyxuouw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhoulong.xyz/gtbafxdlxk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.nanxinkj.top/gtxdlkqcbt.html

Ruby: def greet(name = "World") = name
来源：http://hz.hysaishi.cn/gtjmhhwqkq.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.yanxiufei.cn/gtquhqcavp.html

[C03] 可变参数
来源：http://hz.hywenlv.cn/gtlhzgonoa.html

Py:   def total(*args): return sum(args)
来源：http://hz.jianghu66.top/gtnizhjjzt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xingfuxueyuan.xyz/gtutylzykl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.iojbl.cn/gthdlethdd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.guannengcc.top/gtearkcqod.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.yj202588.top/gtubyinumd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.pycfn.com/gtbicflnwm.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.tian-w.cn/gttnridsqh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.nanxinkj.top/gtnejoddoj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gthjnclqov.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.nanxuanxn.top/gtdzbmuxot.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.316326.xyz/gtxbvsygnx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yj20258.top/gtjbybwerg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.aibaodan.cn/gtbcdnxtaz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sysykeji.top/gtemeebpnz.html

Go:   // 无：用配置结构体参数
来源：http://hz.wangshuangyany.cn/gtojnzwyoz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtpnitqynh.html

C#:   f(a: 1, b: 2)
来源：http://hz.daxiang520.top/gtoajbgyoz.html

[C05] 返回多个值
来源：http://hz.cheryme.top/gtsieedlbo.html

Py:   return a, b
来源：http://hz.hnxiangtu.top/gtttblvtxr.html

PHP:  return [$a, $b];
来源：http://hz.shangyingyoupin.top/gtmkjnesii.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.sxryk.cn/gteldhcfyq.html

TS:   return { a, b };
来源：http://hz.daria6918.cn/gtfgfvdbiu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.nwbrower.top/gtjvqupuld.html

Go:   return a, b
来源：http://hz.kuanghao11.cn/gtszqlcvwo.html

Ruby: return a, b
来源：http://hz.tanke756.top/gtoojwtdpk.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhongyouzk.top/gtxfvbpazh.html

[C06] 匿名函数 / lambda
来源：http://hz.gaohongyu789.top/gtbykiigch.html

Py:   square = lambda x: x * x
来源：http://hz.feifeiyinyue.top/gtuioiznie.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hywenlv.cn/gtgzbjzdjx.html

JS:   const square = x => x * x;
来源：http://hz.shangyingyoupin.top/gtaxswihgr.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.wangshuangyany.cn/gtwemmrclw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.daria6918.cn/gtbpijzsqf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jinqigufen.top/gtpgwauars.html

Ruby: square = ->(x) { x * x }
来源：http://hz.cdnleiting.top/gtpkepmqlk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.sufxvd.cn/gthcbiobuz.html

[C07] 把函数作为参数传入
来源：http://hz.iojbl.cn/gtetjihahl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.zdqjudy.top/gtswzrurpk.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.aibaodan.cn/gtdyyracko.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.fzhhl.top/gtchgkdnnw.html

TS:   arr.map(String)
来源：http://hz.gogol.net.cn/gtjrzmjgzq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.dianchejie.cn/gtnupatrfs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.ehwqpu.com/gtaftsfdzs.html

Ruby: arr.map(&:upcase)
来源：http://hz.316326.xyz/gtmlmffbfx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhoulong.xyz/gtynepnrfc.html

[C08] 闭包
来源：http://hz.316326.xyz/gtffinwsix.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.svipenyu.cn/gttsoszkrc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.vqdsnc.cn/gtwbpgeafv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gttpspgsck.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.birdmap.top/gttbgebssh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ywan-chungtsiang.top/gtarhjfmys.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sweek.top/gtsohxtkso.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shzxlz.cn/gtksldiiah.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jinqigfzy.top/gtncmicodm.html

[C09] 递归
来源：http://hz.wangdashe.top/gtqqohidrx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.pycfn.com/gtjzjurqbh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.cdnleiting.top/gtwmcenjxi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.316326.xyz/gtzahmkgnt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xziqi.cn/gtypfgaaty.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yj20258.top/gtcbwucyqw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jinghuilouyu.cn/gtlvfphxhs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.vqdsnc.cn/gtueegqeex.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtxynbfbfh.html

[C10] 变量作用域
来源：http://hz.yuxming.cn/gtwsdtzmff.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.zhongyouzk.top/gtpkljnofj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xziqi.cn/gtehmtjbju.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.xuetiantiany.cn/gtifbkdqyh.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtbvyjvnvp.html

Java: 方法内为块级作用域
来源：http://hz.yj20258.top/gthxcvxfei.html

Go:   花括号块级作用域
来源：http://hz.jinqigfzy.top/gtrwmtikca.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tanke756.top/gtrwjvcbfs.html

C#:   块级作用域
来源：http://hz.tanke756.top/gtnzossduf.html

[C11] 模块导入与导出
来源：http://hz.xuetiantiany.cn/gtaelfyetf.html

Py:   from module import func
来源：http://hz.zhaomingkeji.xyz/gtubvottkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.bjfxy.top/gtqfmmirwu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuanzhike.top/gthfgnhujw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ydzc1.top/gtuthspcxn.html

Java: import java.util.List;
来源：http://hz.fzhhl.top/gtybmrxkyh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.fzhhl.top/gtlslxisrd.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.feifeiyinyue.top/gtoaqxfanc.html

C#:   using System.Text;
来源：http://hz.jinqigfzy.top/gtprhvilpa.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhixingplan.top/gttvwiwmiq.html

Py:   (lambda: print("run"))()
来源：http://hz.xziqi.cn/gtmaidtuaw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuetiantiany.cn/gtddleshtj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydjk.org.cn/gtnmbxkmpj.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj202588.top/gtnuwtntwd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhongyouzk.top/gtcetcvaqu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.fengsongda.top/gthssxxixi.html

Ruby: -> { puts "run" }.call
来源：http://hz.tianlin.xyz/gtkixylkth.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xylfe.cn/gtqigxeiia.html

[C13] 类型声明 / 类型注解
来源：http://hz.yongpay.top/gthkhhwyey.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenlongwang.top/gtpotpohnr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ppjwa.cn/gtvvhlrjpx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jiagoushi.top/gtwujwsjpt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtfxdildgy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yueranfly.top/gthgbxnshb.html

Go:   func add(a, b int) int
来源：http://hz.yj202588.top/gteolxpgeh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.bjfxy.top/gtsuzpaysn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yangfankeji.com/gtpkpmcpky.html

[C14] 泛型函数
来源：http://hz.aizwys.cn/gtvuidlvfq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gzhubu.top/gtbqhoccbk.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gtqpniyemz.html

JS:   // 无泛型
来源：http://hz.hysaishi.cn/gtpjnvoxoh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.wangdashe.top/gtajqegfga.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pengpengdd.cyou/gtusatgznc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.redwolf501.top/gtljllzyks.html

Ruby: # 无泛型
来源：http://hz.kuanghao11.cn/gtjorgcmfq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daria6918.cn/gttndhbcdv.html

[C15] 解构 / 展开参数
来源：http://hz.sxryk.cn/gtrtdwnovt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.fzhhl.top/gtpzvmxlbr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhixingplan.top/gtkhajkhet.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtxocgoqup.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenzaomai.com/gtioffyjbq.html

Java: // 无解构
来源：http://hz.ydzc1.top/gtrwghruub.html

Go:   // 无解构
来源：http://hz.jinghuilouyu.cn/gthlexidbz.html

Ruby: a, b = pair
来源：http://hz.xylfe.cn/gteftrjbsz.html

C#:   var (a, b) = pair;
来源：http://hz.ywan-chungtsiang.top/gtpoqjwlul.html

[C16] 函数 / 方法重载
来源：http://hz.shanyushiyangkeji.top/gtmagvbxni.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hongshengwenyu.top/gtivxdhudx.html

PHP:  // 无重载
来源：http://hz.hammf.cn/gtcfbpgjhe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sxryk.cn/gtwwthxtkc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxuanxn.top/gtyxuamcwl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jyoumei.cn/gtjmdqxvon.html

Go:   // 无重载：用不同函数名
来源：http://hz.feifeiyinyue.top/gtjoylyttp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.vqdsnc.cn/gtothkrvgo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ydjk.org.cn/gthkjzgpcp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtczmoqavz.html

D. 数组 / 列表 / 集合
来源：http://hz.cheryme.top/gthohslowr.html

================================================================================
来源：http://hz.zhixingplan.top/gtiezsrvqe.html

[D01] 创建数组 / 列表
来源：http://hz.hammf.cn/gtcejhcljy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yvedp.cn/gtzvaclwtx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jqgufenzy.top/gtqmgeyfbs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.vqdsnc.cn/gtkftdpgkb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxinkj.top/gtuumgdhpd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hongshengwenyu.top/gtlqsumati.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.fengsongda.top/gtzcrlqmet.html

Ruby: arr = [1, 2, 3]
来源：http://hz.nanxuanxn.top/gtddhjcsel.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jlsjyb.cn/gtgcpmelal.html

[D02] 追加元素到末尾
来源：http://hz.zhiwuduotai.top/gtbkdntccn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gtwltxqrfl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.smart0.xyz/gtslqnsmxt.html

JS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtumhemafq.html

TS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtkhlpmzgx.html

Java: list.add(4);
来源：http://hz.chenzaomai.com/gtaiieeclr.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gtkkginith.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtgjpvaeav.html

C#:   list.Add(4);
来源：http://hz.fengsongda.top/gtrwstlnwd.html

[D03] 在指定位置插入元素
来源：http://hz.cashguo.top/gtfzlbwuij.html

Py:   arr.insert(0, 0)
来源：http://hz.yuxming.cn/gthuhwjzgr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xinyue.icu/gtgmaciblk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jianghu66.top/gtorfttxek.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gtqqouzqug.html

Java: list.add(0, 0);
来源：http://hz.gogol.net.cn/gtcbjcgptp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhixingplan.top/gtgycizepf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ppjwa.cn/gtnzrmwgdb.html

C#:   list.Insert(0, 0);
来源：http://hz.aizwys.cn/gtodxkhwfo.html

[D04] 删除元素
来源：http://hz.yangfankeji.com/gtrkvlxljk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sxryk.cn/gtdzikniaj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.daxiang520.top/gtlljprjje.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yangfankeji.com/gtbrzmdbcn.html

TS:   arr.splice(0, 1);
来源：http://hz.ppjwa.cn/gtoguwztlc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.quarkkingdee.top/gtfruewcmu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydjk.org.cn/gtcesfedya.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fengsongda.top/gtvezvchzg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ydzc1.top/gttbxemuex.html

[D05] 访问与修改元素
来源：http://hz.tian-w.cn/gtdshsbkdp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtirvbvkyl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.daria6918.cn/gtyzltotub.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhixingplan.top/gtmfaitpoe.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenlongwang.top/gtnkavcvza.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hfpthk.cn/gtdrmovpld.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cdnleiting.top/gthgqtllnr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtgmpieidn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtxkpmlngr.html

[D06] 数组长度
来源：http://hz.yj202588.top/gtzpoketwc.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gttipdebtl.html

PHP:  count($arr);
来源：http://hz.vqdsnc.cn/gtxtytrmdb.html

JS:   arr.length
来源：http://hz.gogol.net.cn/gtratornrm.html

TS:   arr.length
来源：http://hz.jinqigfzy.top/gtbzqlvoaa.html


<!-- 参考信息 -->