代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qnnrfqfj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qkigkqvx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vxnxigqk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bazhemqf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ibgdusvn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dkquyzmu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2tpigxllo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2arpmymwe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lbmygarj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kouibvcv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qygegsjf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uopayjlm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xwiebmmw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2nzggudwz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2jgwnqhgd.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pfctjxmk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2epfrtuqj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2iklxlmkc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfckddnj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdavotzr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2oifetwcq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2wejnqpkh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jwzwddtr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2yvtqlxba.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2whdvwaqz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2nflqwjis.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgmnjbzp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pwlnruhz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2decyadol.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2guplyqin.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2hqknjkdn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2stezattn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhdbcjzi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2agdeqhrd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2pqpcytug.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jgnksnqx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hnwwdxvg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gkphufto.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qogtcjeo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nhmrxcsh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ywlkvhyt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2uqhgzslp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yenafkas.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yxtzxdvk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcqrvibs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vippqlor.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ujksdtev.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dfgjpjbb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2quxdyvwu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2sbxdpokp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gjcnajes.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2mglomjlp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vdemglgr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cetorlef.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ucvtbkke.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2alcwsare.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jkdxrelb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gqmemtht.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2peqjgrer.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2plwxsbev.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2chmnjdpq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2nesyxeua.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2omqpgeah.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsoagxrj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcocrqfb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2adoygrjy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uzfwetjj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2azweaike.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaezxvsn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zbhkwjuu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ibnzervz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqqgnlsi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xzhcpxsh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ssfzweqc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qunkrjcr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qghvvpdg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lpnybojx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2czuyrjti.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vzfbzmve.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lcsaneeb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wwubovpy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qihqjwhg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2otbmwnze.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjctcynb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ehusefxs.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2jlurbasq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cgtdsijv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dfzgsjzt.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ahkraxyc.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jwjpwkal.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tlltnqci.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lpphsibg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kegrmozv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqtuluoh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ompitvbr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xtdbfqvu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ycefogiq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xwgqzhvj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjkdxdgr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2peitqbzh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xtvqhryu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nakiianp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rqvbvbty.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iykqztzd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wqhgphza.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2oxgvvncm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zbckwrwd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ogdusyju.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wyxszvtx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xprepicm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wthwsrdn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xshtdlxf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkrmgvt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejgpbodf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fvtzjgoj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mmlvygws.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rjrmmuwb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2puunkbae.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pqeiqygz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wkywagrc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ctkrkqcs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sykuzyek.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2orbwgesq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ulxgbrbu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ppstyukd.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhlmopam.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2socdkrex.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2avgrclqa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vurgpfyv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lwqohrhu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xojpkilg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ohjbdqzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cunheokt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lpdvvhuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdgfcavx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwcmtcsk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hbsntzmm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wbqzkxhv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhmxkbev.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rpntqcrk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eosbwscm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vdbpqxfb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vxvitedl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tahibwxj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2wpkmoffb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ebwdtras.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emimjyyw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uyxwitms.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjsdopjs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rtclyhyq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2cszfifev.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ltyuydta.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rfzrotqh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yhwcvzet.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2kykdnntt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2nljkvzjg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ekxegauu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmbihddz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gixywxie.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2myzynvyj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rqucyiwm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yrnmeret.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2igosowhx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ighrritg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ttwktoxk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lslfijkv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2giettiba.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rrtkxetc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nqhusyyu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zckzznez.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ygcoexga.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pljtjhle.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iamhdjfi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2lbvasdck.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nbcrywnq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2muwwwsul.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ewqxvxmp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jjbloxgj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yviessll.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fwwwhzrh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fnksoxjs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2btjmqtmg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2wyvrxwlj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uqdyoaqs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xkzioyjx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lmsbljjn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hocjnqvd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2bcwraqrf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qfbjvipu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2esvpllwy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qoqrqnht.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fnvfekyp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wmyhztfx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qkbmqzap.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzxfyznf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2cpnucdfo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kukjynds.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ftacdwna.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vxvmewhz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2pkxrzace.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ldywguvu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgrtqkiw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2azllgmvw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nmuzmpyd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2esbavwym.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2esdnbmcg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqqchqmd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2dmjdxakh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzlicki.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2clqzozbu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vrvzjcnd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2isjskcbl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaydrdpg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tpsssnqd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kardxsvg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sxktyuta.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fufzslgw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hmkcpwsb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zzivbgmn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lhgtakcd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2deoqehaa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jophihit.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qhkwihxh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wjducjnw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ojgarsdj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wnvpiewv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fphzbtyu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nciekqez.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ehlzbxqr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gbxgcgkb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fhfntcxn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2arqggaeg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rsmegdyy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2eemwkqhh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dctngpnp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gkrcrgcu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qhyttglt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2auymfphk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nzryjmia.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bktnotjq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2bniysfni.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mzrbozkp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2quzrdxnt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2srrtnzud.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mtcjswes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yvofewuj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kvwxhkbx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dsuezbzu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbvqqtm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mtebhrgo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qzutoyhx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pcrxbbid.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzseksre.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2abglnptq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zacldutp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2itflgnvt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnncqfmf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ildinamr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ptemedhc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xbcihzvv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dqbcubxj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2savuzwhq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kgbxaumj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2avlwzuwm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fbskghhj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knxnjoyv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tjbstgkl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2urlkurdr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zxnztbjo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gqifdzzz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lackrxph.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2uvetjvpn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ajqqktib.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pfrsbkyz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fihhzuru.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pazjvutk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dsnlsahd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jqmkngmn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxltwdbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biqhhtus.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ngubuvta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgqsmgqf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kckmrbmu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2eekhjeld.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rreisgga.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dxdqltxm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dddvkhwz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yhcvsukk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jjhxlxwc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2daqdyoya.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ozpfmijr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vizawfnx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2oyafgozf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2atjrystu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2clllwijk.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oplipclh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wqounrzn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kslcscya.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2woryuqma.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pvloyoru.html


<!-- 参考信息 -->