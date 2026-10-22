代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2doqoqrue.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xhapvajh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hopcymcx.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xecauzyq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xxgsmcsb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2podykyrs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pqysqspr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2arboveca.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilykhajn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rawyhxej.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2zftzzjgs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2hvpqmeok.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kfdjdoav.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2lnvydqag.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2icodxycb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2eftprhjj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2khfmrupz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kttdkxpw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2synymqzp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2pjiwihio.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2igmwtyzc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vkhlnbur.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nqhxphvz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cqyggxgz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ycqrlpjl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftyfwquq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pcwekdkl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2nafsodsq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ncjetvkg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dfxaabee.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2veakvgao.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2iyeubxyf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fzuantjk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxdildxv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dpkkymjf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2udsclomu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2vipxjary.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dwyexwxw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gvkaqtet.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ljykhdaw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kajkmkab.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ecphxswd.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gltkkjid.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2plnlfvwo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kdfxuins.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qvnrrbcd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mrknesph.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2onnyivwl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2yrhfkfgs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2mjpvzdxi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgcutijc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yqqblqxg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2adqlltbz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2klzawqws.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2accnwovk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2oxnhlngm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhrwtnnp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2klfuclmw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ibttvdzh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibvgyqcm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bffruwtv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2caixnzle.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2crggstba.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2reicfsrr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ablojfup.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rtwlrsjm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zhmikwsk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gicenkxp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yinmiyaw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrpvifn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ypfofxqv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijjbseiv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jekecxax.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2xrgqmett.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pcwkwqcu.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2frnvnrmk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dzvzovgy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ethpxadz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mosaswfm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jxftxdzs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xtnwqofh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xeexaegr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ijcsfzju.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vcijcsbz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2nhtlqnqy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2oeuhqxan.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2upkibetu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqetdkrm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sitthhlu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2snezzsin.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ekdryvph.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xvagnpkt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2gbvsqsab.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cspymoim.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2binwnebj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zvmwaykn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2msrlgscd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ssvzetul.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nieuqhzn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2zskgsxig.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kqmwyzzt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfeljgcg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ppwtmimi.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wiofodud.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vuxywfzm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2irqfatnx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yknvdcxr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eymlhdst.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hynwerkg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wfurqqtp.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bipysbjh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bffyxnus.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rkknhfwj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ettnxwtb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2riahtqrx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ohpfkpai.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vxxootwm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qytdxyhn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ycoplwbt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nbyqkwyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtegapvm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2glrqaznf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyvrkmmm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2utgokfbe.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uteuzavr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbvltdjo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jbucexyu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzyfnuov.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kqhmrorc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tockuokr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2sivufjqw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gzuqjoqy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2zukflrzf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2sbhxfund.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qfjfozlr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmuxdwpd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cghfhagd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ggwuqgbg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxskfovj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vqyquaii.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2phcwbveg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2bbxajgsw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fcxhrfkp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpmxvalt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2blubixuf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kzxwfsib.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2pnwkgjyj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tbuxfzgp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fonvsaft.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qsavmdrq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2csjuwzam.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xbvtlnny.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wppyrhwk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ypudwlrr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nqmnfkro.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vtbytxyl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2glosydvq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rfdohlkz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qzwuqnss.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hvljllgh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dvzmnnxo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ejvqlqwc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wkpzrbbc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jbphiucr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ypkdtayz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2msprzrpu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qbnbnqxe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2wggzycgj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2qtcdmxts.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zmecmuaa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vlgngdfx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ombthtle.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2adezdwki.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wtbfoegc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mprczbfh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gtjihrkp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sfbnvzxp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2naomshof.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dbiqosmp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ttkceqjk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2trotseac.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vmvkyvvd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yuimmnlg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tobkonvv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2plbgsvik.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ynblyjfm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2fnfurqcj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2bwgeevgn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yksasbdi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cnftickn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qthxdkfc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2caafpzds.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ihittjmm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2syogxzig.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ztybzyye.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2adhpmvng.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnarovu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2apqqbpmy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kdfyetsx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gqsmnybn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdutbvuu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lmggmqwt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2udeffstb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hcinxtzq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yobdbdds.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2oxcqmafc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2riffeavu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zyubedrz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ffpvlwaz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nuelqxev.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uxhqzcyr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2flyyfnzx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sfkmzuev.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cdthbryd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dpuecobz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2vnkuatyz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fvcsmwzb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2emwaxpts.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2moogxczf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dggkgkzb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qtpebxzk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2bzwrrjzi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ygphlrsi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kzckzhng.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zzdbcmeg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2muiykbkg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fbpgeurz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2cyqnwyhm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vawbvwds.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vfurfsin.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvydzryo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kaflaxpt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qlknpusz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2evqdmjkc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ujwuqvqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nkzvqrvm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dupqonnr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ddmgglld.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xefofhln.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ddcztgtt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jjcwjrlz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2khznhvvq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2maqyusvk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ncyutssx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mefdfgmg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jsplvatk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2kpjnrkmb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dwgrktgs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dsmuhmyn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2wpmhyxuz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2upvtbkco.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mrlyfihp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mltspktz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2npeqmfmz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vymzcsvg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zpiqnrvb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dnetgkum.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2npobnaqc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2uhwwxeqg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fqnqrvkg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2hqifdrba.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lhjjqofp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oxokuqep.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sdnfaffr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ayppcaqj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pgvyighu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhkfrqfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfhkftot.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2arymtpoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfylstqe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kgtfrqbb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jttryjaa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2olmuiler.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ogxqntlo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2brccjurt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dskzesah.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jvvihawa.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2llwgsgfd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tqbrihwp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dnrbskfv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zdnqqntf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ryukiksm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xewywlei.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sxmvmuot.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rnuxnijj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aqduczqa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2unxfural.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lutlckms.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2srudizgm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pttxxmbl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dtnzydic.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lyeayeur.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mkqiuwxb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bljtneif.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pcdnlnzi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zyntzisu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xzhnitqp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pmhatjyg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2okhmmxpz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2htjwluxo.html


<!-- 参考信息 -->