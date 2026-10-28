代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.xylfe.cn/gtleixqajg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.mhx1999.top/gtpatccfhv.html

Ruby: 10.times { |i| puts i }
来源：http://hz.jinqigufen.top/gtzprgepwb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.svipenyu.cn/gtfmpmtdns.html

[B05] 遍历数组 / 列表
来源：http://hz.chenzaomai.com/gtntbmumxn.html

Py:   for item in arr: print(item)
来源：http://hz.cqqwz.cn/gtzcsulgpk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.mhx1999.top/gtqxvaexac.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.chenzaomai.com/gtqjpwfodx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.zhongyouzk.top/gtbmrdttqn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.sweek.top/gtcfwbkkpt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.xuanzx.com/gtotwfnpry.html

Ruby: arr.each { |item| puts item }
来源：http://hz.dashuyun.cn/gtpilxkaxy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.jinqigfzy.top/gtjpuznspn.html

[B06] 遍历字典 / 对象
来源：http://hz.guowangkeji.top/gtpsvofriv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.jinghuilouyu.cn/gtarojmdbv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.cdnleiting.top/gtfisgodyp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.xingfuxueyuan.xyz/gtxpuiexzg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.andypj.xyz/gtjowmvbrp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yanxiufei.cn/gtcspwilwk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.gzhubu.top/gtsqouneob.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.zhengqikj.top/gtqhkiqzko.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.chenlongwang.top/gtwoujulwh.html

[B07] while 循环
来源：http://hz.zhijiandao.cn/gtncyhggmh.html

Py:   while i < 10: i += 1
来源：http://hz.gaohongyu789.top/gtvsgqzhle.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.yuanzhike.top/gtomuhpuqm.html

JS:   while (i < 10) { i++; }
来源：http://hz.jqgfzy.top/gtwqtbblti.html

TS:   while (i < 10) { i++; }
来源：http://hz.yongpay.top/gtenhazsis.html

Java: while (i < 10) { i++; }
来源：http://hz.zhixingplan.top/gtrplwqpgf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.svipenyu.cn/gtolyipeky.html

Ruby: while i < 10; i += 1; end
来源：http://hz.cashguo.top/gtsrffgeld.html

C#:   while (i < 10) { i++; }
来源：http://hz.kuanghao11.cn/gtjnjfdnmb.html

[B08] do-while（至少执行一次）
来源：http://hz.iojbl.cn/gthwflpgzb.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yuanzhike.top/gtihcjdvke.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.nanxinkj.top/gtbwehebic.html

JS:   do { i++; } while (i < 10);
来源：http://hz.xingfuxueyuan.xyz/gthwpxbubk.html

TS:   do { i++; } while (i < 10);
来源：http://hz.cqqwz.cn/gtcifcqexr.html

Java: do { i++; } while (i < 10);
来源：http://hz.aibaodan.cn/gttjjybhzk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.cashguo.top/gtfrggrfqq.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ydjk.org.cn/gtzwowwkad.html

C#:   do { i++; } while (i < 10);
来源：http://hz.yvedp.cn/gtrsikxyqk.html

[B09] break 与 continue
来源：http://hz.pengpengdd.cyou/gtlmojwdyo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.daria6918.cn/gtqbumwqxp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.xinyue.icu/gtrrymqhtc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.gaohongyu789.top/gtvwndatgo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtxkldfbzr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.ydzc1.top/gtixocyllk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.hnxiangtu.top/gtxkmfsnis.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xingfuxueyuan.xyz/gtkvjxirld.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtyufmvtut.html

[B10] 遍历同时拿索引
来源：http://hz.quarkkingdee.top/gtalspuxbt.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.shangyingyoupin.top/gtfdgrgeuk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.tanke756.top/gtujkqbzrc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hammf.cn/gtdriiiysx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.nanxuanxn.top/gtrmvrwmmr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.chenlongwang.top/gtoxqlowqs.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.gzhubu.top/gtmgofoqqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.jianghu66.top/gtbofcqrkv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hysaishi.cn/gtwleaylsp.html

[B11] 生成数字序列 / 区间
来源：http://hz.cashguo.top/gttkpyirqm.html

Py:   list(range(0, 10, 2))
来源：http://hz.nanxuanxn.top/gtzgxyxdfx.html

PHP:  range(0, 10, 2);
来源：http://hz.52xcode.cn/gtcmbbhtnr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.tian-w.cn/gterjvsfss.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.gzhubu.top/gtyoyhzxpl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.mhx1999.top/gtvjrpmecu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yangfankeji.com/gtzpzmttnk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.guannengcc.top/gtumpjanqy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.chenlongwang.top/gtmeuixmvn.html

[B12] 跳出多层循环
来源：http://hz.haohaochexian.top/gthymnrjrg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jqgufenzy.top/gtsbnwngbl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.jqgfzy.top/gtqsbcraiy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hongshengwenyu.top/gtkiypxozr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.daria6918.cn/gtuizlpaso.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.ydzc1.top/gtcclslbjy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.ppjwa.cn/gtcburvbke.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.guowangkeji.top/gtnzssgwkk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zhoulong.xyz/gtprjgxugy.html

[B13] 判断是否为数字
来源：http://hz.haohaochexian.top/gtpuxbgthn.html

Py:   isinstance(x, (int, float))
来源：http://hz.c1oappe.top/gtevhkyxqg.html

PHP:  is_numeric($x)
来源：http://hz.hysaishi.cn/gtvalcgfpc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.jinghuilouyu.cn/gtenmpghpv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zdqjudy.top/gtuimyjzjd.html

Java: x instanceof Number
来源：http://hz.wangshuangyany.cn/gthnosrtuu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.redwolf501.top/gtjwlbjqoj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhengqikj.top/gtwtbkruki.html

C#:   x is int or double or decimal
来源：http://hz.snrcjt.cn/gtpdqvsgle.html

[B14] 判断值是否在集合内
来源：http://hz.zhixingplan.top/gtzhbtsook.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.shuidangran.top/gtfzrkvymm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hnxiangtu.top/gtfjhdztzo.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.cashguo.top/gtllzfzyrm.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtdpmjbnui.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jlsjyb.cn/gtomzntdwt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.redwolf501.top/gtomsrwlhe.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hammf.cn/gtquplhrbt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.pengpengdd.cyou/gtkcvzghyf.html

[B15] 布尔运算与取反
来源：http://hz.chenlongwang.top/gtgpzkngzz.html

Py:   a and b or not c
来源：http://hz.gzhubu.top/gtdwzvhufz.html

PHP:  $a && $b || !$c
来源：http://hz.316326.xyz/gtiflztusw.html

JS:   a && b || !c
来源：http://hz.xingfuxueyuan.xyz/gtdcmcwror.html

TS:   a && b || !c
来源：http://hz.chenlongwang.top/gtcduytfey.html

Java: a && b || !c
来源：http://hz.jyoumei.cn/gteqxfcekz.html

Go:   a && b || !c
来源：http://hz.cucudq.cn/gtvxgoikcg.html

Ruby: a && b || !c
来源：http://hz.shanyushiyangtech.top/gtdqmbuhgk.html

C#:   a && b || !c
来源：http://hz.ivvv.top/gtymjiepfz.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jiagoushi.top/gtapgqzirf.html

Py:   if not data: return
来源：http://hz.jlsjyb.cn/gtixmfgdxd.html

PHP:  if (!$data) { return; }
来源：http://hz.pengpengdd.cyou/gtcvyipqwr.html

JS:   if (!data) return;
来源：http://hz.fzhhl.top/gtuzcpqihg.html

TS:   if (!data) return;
来源：http://hz.ywan-chungtsiang.top/gtuokhcijp.html

Java: if (data == null) return;
来源：http://hz.zhoulong.xyz/gtzfpryfqb.html

Go:   if data == nil { return }
来源：http://hz.aibaodan.cn/gtopoupbtc.html

Ruby: return if data.nil?
来源：http://hz.52xcode.cn/gtyeiaywtv.html

C#:   if (data == null) return;
来源：http://hz.0kj1m.cn/gtsduobfwi.html

================================================================================
来源：http://hz.zhengqikj.top/gtmqesbcpb.html

C. 函数与作用域
来源：http://hz.hnxiangtu.top/gtdckvyqcv.html

================================================================================
来源：http://hz.ehwqpu.com/gtmufyqcqp.html

[C01] 定义函数
来源：http://hz.ppjwa.cn/gtiujkbhor.html

Py:   def add(a, b): return a + b
来源：http://hz.tanke756.top/gtpyhunfwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.pengpengdd.cyou/gtvhetpmfw.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.chenzaomai.com/gtqlcytrfj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtyucezilq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtzqdtoxlz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.daria6918.cn/gtkcieuyif.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yvedp.cn/gtsryvwioe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtjnhmzeqd.html

[C02] 默认参数
来源：http://hz.gogol.net.cn/gthollvwlt.html

Py:   def greet(name="World"): return name
来源：http://hz.chenjidiqi.icu/gtdehqftsz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.cucudq.cn/gtssffxlnp.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ydjk.org.cn/gtfntefzxd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ydzc1.top/gtvvcvslfg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtofbwahpi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.cashguo.top/gtjwlfvykn.html

Ruby: def greet(name = "World") = name
来源：http://hz.yanxiufei.cn/gtvltelazm.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.jqgufenzy.top/gtarttlkgx.html

[C03] 可变参数
来源：http://hz.hysaishi.cn/gtwjdjhlte.html

Py:   def total(*args): return sum(args)
来源：http://hz.gaohongyu789.top/gtwzzbqqrf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jlsjyb.cn/gttduavenx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuanzhike.top/gtzveeoypw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.fzhhl.top/gtcevtlhpn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ydzc1.top/gtlhefwqrm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtadztpgrc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zhijiandao.cn/gtzvcgpivt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xinyue.icu/gtgydxfpur.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtesfiurbc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.gzhubu.top/gtmudnjsej.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hysaishi.cn/gtfepscwhl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.smart0.xyz/gticaebrks.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.quarkkingdee.top/gtbrgnlbqc.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.fengsongda.top/gtthdoyvtx.html

Go:   // 无：用配置结构体参数
来源：http://hz.havefunace.top/gtbkdmzgkt.html

Ruby: f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtabqfebgo.html

C#:   f(a: 1, b: 2)
来源：http://hz.andypj.xyz/gthybcwtng.html

[C05] 返回多个值
来源：http://hz.zhiwuduotai.top/gtcocoqaue.html

Py:   return a, b
来源：http://hz.hfpthk.cn/gtncfqbmtk.html

PHP:  return [$a, $b];
来源：http://hz.yueranfly.top/gtedrrxkib.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydzc1.top/gtbcfroias.html

TS:   return { a, b };
来源：http://hz.shanyushiyangtech.top/gtjllblana.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.bjfxy.top/gtkjrpwmwa.html

Go:   return a, b
来源：http://hz.cheryme.top/gtaprhisnp.html

Ruby: return a, b
来源：http://hz.jlsjyb.cn/gtcgppygqb.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ybcxt.top/gtbuhohdhf.html

[C06] 匿名函数 / lambda
来源：http://hz.jinqigufen.top/gtgroojrqd.html

Py:   square = lambda x: x * x
来源：http://hz.shzxlz.cn/gtemsblrjx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.snrcjt.cn/gtbwunmltm.html

JS:   const square = x => x * x;
来源：http://hz.nanxinkj.top/gthqpsekvp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhongyouzk.top/gtdxoracgl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhongyouzk.top/gtvbyzzhod.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangdashe.top/gttyuxmfze.html

Ruby: square = ->(x) { x * x }
来源：http://hz.meibo888.top/gtwrwmggyj.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhongyouzk.top/gtlmtbxhzh.html

[C07] 把函数作为参数传入
来源：http://hz.52xcode.cn/gtvkvkisel.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.fengsongda.top/gtedicxpqc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.chenzaomai.com/gtemvbavsd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shzxlz.cn/gtyyvhkknl.html

TS:   arr.map(String)
来源：http://hz.nanxinkj.top/gtnntauptz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jiagoushi.top/gthzsigtvy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.zycfv.cn/gthiffdrbb.html

Ruby: arr.map(&:upcase)
来源：http://hz.sufxvd.cn/gtakpxbyhr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ywan-chungtsiang.top/gttbdafuqg.html

[C08] 闭包
来源：http://hz.xuetiantiany.cn/gtiipgkgpy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.quarkkingdee.top/gtmtjrcvql.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.hywenlv.cn/gtvkpyiekb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtdvxjbkoz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtxsdohkpv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnxiangtu.top/gtpboikvyg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.redwolf501.top/gtoyljuhhs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.aizwys.cn/gtszpuepba.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hnxiangtu.top/gtiaukrovl.html

[C09] 递归
来源：http://hz.xinyue.icu/gtueyvjlbd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.zdqjudy.top/gtmdwteotz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.shuidangran.top/gtmgphbmqx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.feifeiyinyue.top/gtrrzbrjai.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sweek.top/gtlersvgws.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.andypj.xyz/gtqgsprger.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.0kj1m.cn/gtgmgzvoah.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.9152youxi.cn/gtrjlicucl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydzc1.top/gtfdzxgzsh.html

[C10] 变量作用域
来源：http://hz.aizwys.cn/gtpoqwakec.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jqgufenzy.top/gtahuvuyef.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.kuanghao11.cn/gtgaavexpa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenzaomai.com/gtqsqrbxkz.html

TS:   同 JS
来源：http://hz.9152youxi.cn/gtjxwguslb.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtfbbnfuam.html

Go:   花括号块级作用域
来源：http://hz.xylfe.cn/gtvjxibcqi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.0kj1m.cn/gtdogpoguy.html

C#:   块级作用域
来源：http://hz.chenjidiqi.icu/gtmhzoaqlo.html

[C11] 模块导入与导出
来源：http://hz.316326.xyz/gtisjlrnvq.html

Py:   from module import func
来源：http://hz.daxiang520.top/gtbnhqpvvg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.dianchejie.cn/gtclfqebrv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.gzhubu.top/gtyoquxrbj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zhixingplan.top/gtlcnmoejn.html

Java: import java.util.List;
来源：http://hz.redwolf501.top/gtodychjvf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxuanxn.top/gtgbqflycr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.sweek.top/gtafiusfar.html

C#:   using System.Text;
来源：http://hz.dashuyun.cn/gtderwojcb.html

[C12] 立即执行函数 IIFE
来源：http://hz.gogol.net.cn/gtmfjjdhmx.html

Py:   (lambda: print("run"))()
来源：http://hz.nanxinkj.top/gtypqrnynq.html

PHP:  (function () { echo "run"; })();
来源：http://hz.guannengcc.top/gttaiixhgt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtfzdstusl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtvehhhnce.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhongyouzk.top/gtbouaimtd.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj202588.top/gtotohqrss.html

Ruby: -> { puts "run" }.call
来源：http://hz.aizwys.cn/gtxjmvhadv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.daria6918.cn/gtmjtllipc.html

[C13] 类型声明 / 类型注解
来源：http://hz.ivvv.top/gtdoozfstn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.c1oappe.top/gtveovggsg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gtzrskprbb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gtlinxqeez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yuanzhike.top/gtkinnvvil.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtsoirswct.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangkeji.top/gtpjqgpzvc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gogol.net.cn/gtmujcjdbv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.nanxuanxn.top/gthgsrmvbj.html

[C14] 泛型函数
来源：http://hz.ydjk.org.cn/gtdgxgevhq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tanke756.top/gteopkkztv.html

PHP:  // 无泛型
来源：http://hz.smart0.xyz/gtdybkoyxi.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gthvwaujcf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.aibaodan.cn/gtaucmvpru.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.svipenyu.cn/gtqfggoomm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jqgufenzy.top/gthmjwoqwm.html

Ruby: # 无泛型
来源：http://hz.xylfe.cn/gtkzshcocv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.meibo888.top/gtnpwtkdqs.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gtgijeewtd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhaomingkeji.xyz/gtjlhhsbqs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.smart0.xyz/gttjtxoupe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtvezfyqiw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xinyue.icu/gtrwuukmlk.html

Java: // 无解构
来源：http://hz.ivvv.top/gtxapvrwdz.html

Go:   // 无解构
来源：http://hz.dashuyun.cn/gtnczuafjb.html

Ruby: a, b = pair
来源：http://hz.yongpay.top/gtwwesxkjz.html

C#:   var (a, b) = pair;
来源：http://hz.aizwys.cn/gtmgzwciei.html

[C16] 函数 / 方法重载
来源：http://hz.haohaochexian.top/gtpcbbcdac.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.smart0.xyz/gtssxczwzp.html

PHP:  // 无重载
来源：http://hz.jinqigufen.top/gtpxbuxmxp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj202588.top/gtqqjbrhme.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ywan-chungtsiang.top/gtrjuiuwpe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yangfankeji.com/gtdidiukrw.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxuanxn.top/gtuvnmtjvz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xziqi.cn/gtlpdjsjtr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.dianchejie.cn/gtsokrykxs.html

================================================================================
来源：http://hz.sufxvd.cn/gtdlknrqko.html

D. 数组 / 列表 / 集合
来源：http://hz.yongpay.top/gtzxtbwwmj.html

================================================================================
来源：http://hz.tian-w.cn/gtklmhbvdb.html

[D01] 创建数组 / 列表
来源：http://hz.xuanzx.com/gtayfihisl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.bjfxy.top/gtslevqift.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.quarkkingdee.top/gtaiahjzbj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sysykeji.top/gtsknceuur.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sysykeji.top/gtuuqgfmvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cucudq.cn/gtolpzmqrx.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yongpay.top/gtuyogkhpt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.quarkkingdee.top/gtbeoesjux.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.feifeiyinyue.top/gtbrwthrmh.html

[D02] 追加元素到末尾
来源：http://hz.shuidangran.top/gtdwihvpik.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.fengsongda.top/gtrrxedfij.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhiwuduotai.top/gtpdritzhf.html

JS:   arr.push(4);
来源：http://hz.ivvv.top/gtafcoijvi.html

TS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtvrcwomzg.html

Java: list.add(4);
来源：http://hz.tian-w.cn/gtsvydrpgt.html

Go:   arr = append(arr, 4)
来源：http://hz.cheryme.top/gtofdsyemn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj202588.top/gtbfdxciop.html

C#:   list.Add(4);
来源：http://hz.aizwys.cn/gtstpcgmrp.html

[D03] 在指定位置插入元素
来源：http://hz.cqqwz.cn/gtptjadxxi.html

Py:   arr.insert(0, 0)
来源：http://hz.fengsongda.top/gtuxmdctvw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinghuilouyu.cn/gtgnpmnolu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnqzz.top/gtmkuyuvyl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuetiantiany.cn/gtmqmpadre.html

Java: list.add(0, 0);
来源：http://hz.yj202588.top/gtqhmefypj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.52xcode.cn/gtesyoctnv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hywenlv.cn/gtqaojvtzp.html

C#:   list.Insert(0, 0);
来源：http://hz.ywan-chungtsiang.top/gtfahybffy.html

[D04] 删除元素
来源：http://hz.zhixingplan.top/gtkposxplb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jiagoushi.top/gtcmenxbia.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guannengcc.top/gtxirharjk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangdashe.top/gtttbsgyqt.html

TS:   arr.splice(0, 1);
来源：http://hz.aibaodan.cn/gtsddnxgrh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gzhubu.top/gtghctkdbo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ppjwa.cn/gtkvdpyuql.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.svipenyu.cn/gtimkbxdhe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.vqdsnc.cn/gtxieflefm.html

[D05] 访问与修改元素
来源：http://hz.yj20258.top/gtwzuijlbi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fzhhl.top/gtvdyzhfio.html


<!-- 参考信息 -->