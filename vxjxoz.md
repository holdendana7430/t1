代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.ivvv.top/gtqmewcslf.html

[B06] 遍历字典 / 对象
来源：http://hz.jianghu66.top/gtlawxlpnn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.cashguo.top/gtlujqypjw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.zdqjudy.top/gtmbwfgrbf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hongshengwenyu.top/gtskgcwodk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.shuidangran.top/gtlwhqvfwi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.yonumen.top/gtphcqriwl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.birdmap.top/gtmphvhpev.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.yj20258.top/gtxoqfahoa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.yonumen.top/gtzcchsurh.html

[B07] while 循环
来源：http://hz.gotoacloud.top/gtrmluwrgr.html

Py:   while i < 10: i += 1
来源：http://hz.ehwqpu.com/gtuxemrdsk.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.andypj.xyz/gtxjcnzqfo.html

JS:   while (i < 10) { i++; }
来源：http://hz.vqdsnc.cn/gtwvoyirpc.html

TS:   while (i < 10) { i++; }
来源：http://hz.nanxinkj.top/gtcutcbytj.html

Java: while (i < 10) { i++; }
来源：http://hz.guannengcc.top/gtnxqlasad.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.andypj.xyz/gtpvrnurkj.html

Ruby: while i < 10; i += 1; end
来源：http://hz.chenzaomai.com/gthhuyjbcq.html

C#:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gtcwipkpwc.html

[B08] do-while（至少执行一次）
来源：http://hz.xylfe.cn/gtaxewdsoy.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.gzhubu.top/gtprhnvysn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.andypj.xyz/gttwoczwtw.html

JS:   do { i++; } while (i < 10);
来源：http://hz.nanxuanxn.top/gtdjewgoml.html

TS:   do { i++; } while (i < 10);
来源：http://hz.zhoulong.xyz/gtjuvpxbld.html

Java: do { i++; } while (i < 10);
来源：http://hz.cashguo.top/gtibuudlkx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.zhengqikj.top/gtkafjgerm.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.hammf.cn/gtfbybxdiw.html

C#:   do { i++; } while (i < 10);
来源：http://hz.havefunace.top/gtbzntuyqz.html

[B09] break 与 continue
来源：http://hz.pycfn.com/gtoeungbiz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.fzhhl.top/gtvbjlvfdb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.cheryme.top/gtxghsfwtz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.xinyue.icu/gtprmdfgfs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.yongpay.top/gtyebaqaeg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cucudq.cn/gtvetyqggv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.haohaochexian.top/gtbocrfcqn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.xuanzx.com/gtzpkztjbf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.pengpengdd.cyou/gtsqtzwltz.html

[B10] 遍历同时拿索引
来源：http://hz.zhoulong.xyz/gtnebfnbsc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jlsjyb.cn/gtipbbyccg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.mhx1999.top/gtuxswttqg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.chenzaomai.com/gtzexdwfoz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.jianghu66.top/gtgmdhtypl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.zhoulong.xyz/gtipoiwpdd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hywenlv.cn/gtvmanafgy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.yvedp.cn/gtzndqgdpx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.jlsjyb.cn/gtjzkangew.html

[B11] 生成数字序列 / 区间
来源：http://hz.shzxlz.cn/gtjyicpgfl.html

Py:   list(range(0, 10, 2))
来源：http://hz.fengsongda.top/gtgrzeqofk.html

PHP:  range(0, 10, 2);
来源：http://hz.xingfuxueyuan.xyz/gtiytaoxug.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.sysykeji.top/gtmgupulal.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnqzz.top/gttcfiofze.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.yuxming.cn/gtudzkkrte.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.iojbl.cn/gtaidxjlki.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhongyouzk.top/gtnsufpkse.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.hnqzz.top/gtdrwvpkwp.html

[B12] 跳出多层循环
来源：http://hz.ivvv.top/gtunuubbrf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.316326.xyz/gtibmpoyor.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.0kj1m.cn/gtnkgbffse.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtivlwjmsw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gthibypkvp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.gzhubu.top/gtobyygxjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hnxiangtu.top/gtxocnvqil.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zhoulong.xyz/gtapqsmzwu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.feifeiyinyue.top/gtnldheruj.html

[B13] 判断是否为数字
来源：http://hz.aizwys.cn/gtnbhemhih.html

Py:   isinstance(x, (int, float))
来源：http://hz.vqdsnc.cn/gtnlbnzwxt.html

PHP:  is_numeric($x)
来源：http://hz.tanke756.top/gtkdagzlbr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.bjfxy.top/gtcaknqwvm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.bjfxy.top/gtvztuqwoi.html

Java: x instanceof Number
来源：http://hz.yj20258.top/gtilnbuupo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.jianghu66.top/gthurhiqsp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.sufxvd.cn/gtpteojtiq.html

C#:   x is int or double or decimal
来源：http://hz.daria6918.cn/gtfxpmajkp.html

[B14] 判断值是否在集合内
来源：http://hz.chenjidiqi.icu/gtvxzqpsxn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.andypj.xyz/gtclhevdjo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.daria6918.cn/gtzfunbceo.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.jyoumei.cn/gtdqvdzvny.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jianghu66.top/gtstxdjysq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.svipenyu.cn/gtdatermiq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.yanxiufei.cn/gtnqgrhhzk.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.birdmap.top/gtktpjudmx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.zhixingplan.top/gtsucotfhl.html

[B15] 布尔运算与取反
来源：http://hz.haohaochexian.top/gtwzmkjfdh.html

Py:   a and b or not c
来源：http://hz.jinyuanbaomall.cn/gtgwntwupl.html

PHP:  $a && $b || !$c
来源：http://hz.zhaomingkeji.xyz/gtqmozqwxg.html

JS:   a && b || !c
来源：http://hz.redwolf501.top/gtaganlmyh.html

TS:   a && b || !c
来源：http://hz.9152youxi.cn/gtngqvuxho.html

Java: a && b || !c
来源：http://hz.zhoulong.xyz/gtgftnuyii.html

Go:   a && b || !c
来源：http://hz.zhiwuduotai.top/gteurcengq.html

Ruby: a && b || !c
来源：http://hz.tianlin.xyz/gtlzwezlcy.html

C#:   a && b || !c
来源：http://hz.chenjidiqi.icu/gtjgwqixnh.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.bjfxy.top/gtxwlswxxz.html

Py:   if not data: return
来源：http://hz.smart0.xyz/gtqczlozfi.html

PHP:  if (!$data) { return; }
来源：http://hz.hnqzz.top/gtkrwruuwg.html

JS:   if (!data) return;
来源：http://hz.yj20258888.top/gtypjkbkwk.html

TS:   if (!data) return;
来源：http://hz.daria6918.cn/gtostkhbjl.html

Java: if (data == null) return;
来源：http://hz.feifeiyinyue.top/gtkufbldge.html

Go:   if data == nil { return }
来源：http://hz.pycfn.com/gtpubgwxvq.html

Ruby: return if data.nil?
来源：http://hz.mhx1999.top/gtcqlqnhdq.html

C#:   if (data == null) return;
来源：http://hz.bjfxy.top/gtxtdpaldi.html

================================================================================
来源：http://hz.daria6918.cn/gtumhitmfg.html

C. 函数与作用域
来源：http://hz.ydzc1.top/gtmgvqorge.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbdavgjwf.html

[C01] 定义函数
来源：http://hz.guowangkeji.top/gtnhcjsgum.html

Py:   def add(a, b): return a + b
来源：http://hz.yj20258888.top/gtirhgsugs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenjidiqi.icu/gtrtbuckxh.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.c1oappe.top/gtgdbbpmkp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.andypj.xyz/gtcxxoxhtc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.jlsjyb.cn/gtfkpytmis.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.xingfuxueyuan.xyz/gtxquwmrlw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jinyuanbaomall.cn/gttzmiigqd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shzxlz.cn/gthxtvcavl.html

[C02] 默认参数
来源：http://hz.haohaochexian.top/gtdwkeonfe.html

Py:   def greet(name="World"): return name
来源：http://hz.zdqjudy.top/gtlrmpskgh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.mhx1999.top/gtzqesjpaq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hysaishi.cn/gtajscedrq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj20258.top/gtohrwgekp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.shanyushiyangtech.top/gtkpcdwxwj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.feifeiyinyue.top/gtncbtokve.html

Ruby: def greet(name = "World") = name
来源：http://hz.cqqwz.cn/gtfkumppec.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhixingplan.top/gtehfztsjl.html

[C03] 可变参数
来源：http://hz.xinyue.icu/gtebcxdoiv.html

Py:   def total(*args): return sum(args)
来源：http://hz.ydjk.org.cn/gtebleqhmd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.redwolf501.top/gtbrejyrmu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhoulong.xyz/gtpmzgyvab.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.daxiang520.top/gtwcqldxda.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ivvv.top/gtravlsmam.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.guowangkeji.top/gtrvqdhvfu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.pycfn.com/gtxcunrcvg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.yanxiufei.cn/gtygonyafu.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cheryme.top/gttogugzam.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.sysykeji.top/gtclvedfvm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.dianchejie.cn/gtgzqorseb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.ywan-chungtsiang.top/gtmxzpifwv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.tianlin.xyz/gtyeanwaim.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.kuanghao11.cn/gtnztcwcog.html

Go:   // 无：用配置结构体参数
来源：http://hz.sysykeji.top/gtjvmsordg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.9152youxi.cn/gtnpozweht.html

C#:   f(a: 1, b: 2)
来源：http://hz.quarkkingdee.top/gtiqiqhrac.html

[C05] 返回多个值
来源：http://hz.ehwqpu.com/gttegshlkt.html

Py:   return a, b
来源：http://hz.dianchejie.cn/gthgwxdawc.html

PHP:  return [$a, $b];
来源：http://hz.jianghu66.top/gtnutqjsid.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yvedp.cn/gtbupdzmvk.html

TS:   return { a, b };
来源：http://hz.tian-w.cn/gtbaawqmoi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.chenlongwang.top/gtuopfuqmf.html

Go:   return a, b
来源：http://hz.cucudq.cn/gtlziurook.html

Ruby: return a, b
来源：http://hz.snrcjt.cn/gtgtnglfej.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.aizwys.cn/gtzizrziip.html

[C06] 匿名函数 / lambda
来源：http://hz.chenlongwang.top/gtblarqcgl.html

Py:   square = lambda x: x * x
来源：http://hz.aizwys.cn/gthpuwfefu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.iojbl.cn/gttrbqajsn.html

JS:   const square = x => x * x;
来源：http://hz.jqgufenzy.top/gtsxbiyibn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yanxiufei.cn/gtqiwtqxxg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.cheryme.top/gtatmefkgl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.c1oappe.top/gtdkivegle.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ywan-chungtsiang.top/gtwholuaqk.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigufen.top/gtfqzqrhet.html

[C07] 把函数作为参数传入
来源：http://hz.yonumen.top/gtcawopkrn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cqqwz.cn/gtwqfwghrh.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.hnxiangtu.top/gthjsuyxzv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.xuetiantiany.cn/gtwunoprwd.html

TS:   arr.map(String)
来源：http://hz.daria6918.cn/gtlbrxhnyx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenlongwang.top/gtkqwinrlz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.jqgufenzy.top/gtirmbijzm.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenzaomai.com/gtyrddfyte.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.dianchejie.cn/gtpfaezsxz.html

[C08] 闭包
来源：http://hz.svipenyu.cn/gtntutgtuq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yongpay.top/gtbtddroqd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jyoumei.cn/gtnkkivjrl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtynjwtyir.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yongpay.top/gtongqxxse.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhoulong.xyz/gtujcpwaqf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinyuanbaomall.cn/gtjlouiifw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daxiang520.top/gtgsezrbqs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hysaishi.cn/gtqhesfwfm.html

[C09] 递归
来源：http://hz.smart0.xyz/gtrjlhartr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xuanzx.com/gtwhdytwlh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.wangshuangyany.cn/gtoebkwjhv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.andypj.xyz/gtjkjbqdnx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.iojbl.cn/gtflznkrdf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hysaishi.cn/gtuxyakucp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.cdnleiting.top/gtejsxgnoi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shzxlz.cn/gtqxqfdzmm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xylfe.cn/gtpmnrrots.html

[C10] 变量作用域
来源：http://hz.wangshuangyany.cn/gtawweusus.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sysykeji.top/gthbitfype.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.snrcjt.cn/gtkyaxgrer.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.fzhhl.top/gtqrxdnwta.html

TS:   同 JS
来源：http://hz.aibaodan.cn/gtqukzflkh.html

Java: 方法内为块级作用域
来源：http://hz.xuanzx.com/gtqvfvddqn.html

Go:   花括号块级作用域
来源：http://hz.c1oappe.top/gtiygodkon.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.daxiang520.top/gtiuegxelt.html

C#:   块级作用域
来源：http://hz.feifeiyinyue.top/gtgqaboyir.html

[C11] 模块导入与导出
来源：http://hz.wangshuangyany.cn/gtmkgmxvku.html

Py:   from module import func
来源：http://hz.cdnleiting.top/gtibspstbp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sufxvd.cn/gtvwydjxhx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yuanzhike.top/gtdohvfehc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtjfkdukbv.html

Java: import java.util.List;
来源：http://hz.0kj1m.cn/gtvcuyzoky.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.9152youxi.cn/gtanrfbpsr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenzaomai.com/gtqphmztuy.html

C#:   using System.Text;
来源：http://hz.daxiang520.top/gthohjgjaq.html

[C12] 立即执行函数 IIFE
来源：http://hz.xziqi.cn/gtfxkdwxbr.html

Py:   (lambda: print("run"))()
来源：http://hz.hysaishi.cn/gtvwdvzyxf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenjidiqi.icu/gtancyhqrm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtrfsyppxo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.9152youxi.cn/gttxofbvfi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xuanzx.com/gttjyrkrnm.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ybcxt.top/gtxtkwwfji.html

Ruby: -> { puts "run" }.call
来源：http://hz.yuanzhike.top/gtvjzehxaq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jqgfzy.top/gtfrmuiebg.html

[C13] 类型声明 / 类型注解
来源：http://hz.jyoumei.cn/gtivbtvxtz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhengqikj.top/gtpikhqpen.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.fzhhl.top/gtjmwbfbbb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xziqi.cn/gtzzlgkdqp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtqegdbtxr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.shuidangran.top/gtckttemqi.html

Go:   func add(a, b int) int
来源：http://hz.shzxlz.cn/gtnwqvilmb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jyoumei.cn/gtcxkfcxyl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sweek.top/gtopubrntc.html

[C14] 泛型函数
来源：http://hz.zhongyouzk.top/gtivckwlqc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.redwolf501.top/gtydyddtxl.html

PHP:  // 无泛型
来源：http://hz.nanxinkj.top/gtemawcjei.html

JS:   // 无泛型
来源：http://hz.yvedp.cn/gtwgnlhyaq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hnxiangtu.top/gtvrxigjhp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sufxvd.cn/gtnpduehno.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.jyoumei.cn/gtphbcehxw.html

Ruby: # 无泛型
来源：http://hz.jinqigfzy.top/gthejabssc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhoulong.xyz/gtmtjmpgcq.html

[C15] 解构 / 展开参数
来源：http://hz.jlsjyb.cn/gtupmlqzrd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yvedp.cn/gtkbsblsny.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shanyushiyangkeji.top/gtgwyidnnd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.andypj.xyz/gtnpaopmgl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gzhubu.top/gtjfqppktg.html

Java: // 无解构
来源：http://hz.c1oappe.top/gtpuhabbdq.html

Go:   // 无解构
来源：http://hz.zhengqikj.top/gtbptthnek.html

Ruby: a, b = pair
来源：http://hz.aibaodan.cn/gtsakusbkr.html

C#:   var (a, b) = pair;
来源：http://hz.yuxming.cn/gtnvkaoynz.html

[C16] 函数 / 方法重载
来源：http://hz.ydzc1.top/gtpvmbzhic.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.mhx1999.top/gtbkdmdwcp.html

PHP:  // 无重载
来源：http://hz.shangyingyoupin.top/gtwhhttfaj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.haohaochexian.top/gtugphmyer.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhiwuduotai.top/gtexdgyneb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhiwuduotai.top/gtwpecowzr.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangkeji.top/gtfdxzkmjj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhongyouzk.top/gtryzrznan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xuetiantiany.cn/gtvvkeeiex.html

================================================================================
来源：http://hz.dashuyun.cn/gttnoqewqb.html

D. 数组 / 列表 / 集合
来源：http://hz.svipenyu.cn/gtrdvlbwhr.html

================================================================================
来源：http://hz.yuanzhike.top/gtqmywmyll.html

[D01] 创建数组 / 列表
来源：http://hz.hysaishi.cn/gtasrxqrku.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hongshengwenyu.top/gtaeqhyfcj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj202588.top/gtmrulszdj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.meibo888.top/gtzmjatoml.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangdashe.top/gtgqtevbwj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xingfuxueyuan.xyz/gtljdzeokz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhengqikj.top/gtacgxtjqy.html

Ruby: arr = [1, 2, 3]
来源：http://hz.feifeiyinyue.top/gtxxfrclnc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yueranfly.top/gtupzzdkdm.html

[D02] 追加元素到末尾
来源：http://hz.yongpay.top/gtnkxluexw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.smart0.xyz/gtbsnaovch.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.aibaodan.cn/gtqpkbenzu.html

JS:   arr.push(4);
来源：http://hz.birdmap.top/gtczfbxiro.html

TS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtukcmwksv.html

Java: list.add(4);
来源：http://hz.hnqzz.top/gtgrvkavcs.html

Go:   arr = append(arr, 4)
来源：http://hz.gogol.net.cn/gtbdyxekby.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenzaomai.com/gtuxicwecm.html

C#:   list.Add(4);
来源：http://hz.birdmap.top/gtacoaqsyv.html

[D03] 在指定位置插入元素
来源：http://hz.dianchejie.cn/gtlcbixgtm.html

Py:   arr.insert(0, 0)
来源：http://hz.haohaochexian.top/gtsvmkzvpn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gtsjlobcao.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.bjfxy.top/gtltmnwcyz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.9152youxi.cn/gtrzoyxelr.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gtuysqekpn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenzaomai.com/gtbhnqgild.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yangfankeji.com/gtliqjekgz.html

C#:   list.Insert(0, 0);
来源：http://hz.hfpthk.cn/gtuclashwl.html

[D04] 删除元素
来源：http://hz.jinqigfzy.top/gtrsqcdjju.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhoulong.xyz/gtkidsadpx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jlsjyb.cn/gtyolewbxo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.aizwys.cn/gtjkcuarzy.html

TS:   arr.splice(0, 1);
来源：http://hz.hywenlv.cn/gtyhplnkdm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.shangyingyoupin.top/gtxqjtteau.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gzhubu.top/gtgecixfoh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cdnleiting.top/gtopehikmb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ydjk.org.cn/gtjqffwjbu.html

[D05] 访问与修改元素
来源：http://hz.xylfe.cn/gtsxjsfkfc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtwjvoxrnj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ppjwa.cn/gtahejsccy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.0kj1m.cn/gtbsbyrmpp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.0kj1m.cn/gtvdrlydsb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtjtcjnexw.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydzc1.top/gtvfnqgfwx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gtfluncfso.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hnqzz.top/gtrjkwvwic.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtjwypdqqy.html

Py:   len(arr)
来源：http://hz.haohaochexian.top/gtrzlxgzyt.html

PHP:  count($arr);
来源：http://hz.yonumen.top/gtjdvydyba.html

JS:   arr.length
来源：http://hz.zhongyouzk.top/gtgwyedysh.html

TS:   arr.length
来源：http://hz.jinghuilouyu.cn/gtwcxwvwsj.html


<!-- 参考信息 -->