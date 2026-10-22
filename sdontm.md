代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hllxoecz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rqmnujhf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmyblbea.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyjmaosy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeacldyd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2btgcogsb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zcjmuego.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mytxrfrk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2krpdykyc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pxonqqpk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ppakwtee.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2hosqjzpv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nzzitrym.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nzquktkb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqgosohd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2jibbxnoz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ctyfqefd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2roktppnc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2znwycjsh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ltpgffyn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhkwtomp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2puwuwojk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhszntaa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiyqumfg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zjfkpkis.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjiwjanj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyfyliow.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rftscjxg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2bbjieimc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yswlmdjt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bcycukph.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zigeyawe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tigrluxx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fkxriggh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2azdnbuii.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2irlpghde.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cuwxwgnz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tznpgneb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnsscdri.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxaocxye.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgjutvsn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvmsryrj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwazfrmz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2pdmxpsau.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2boksdyjg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bidelfdi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2txmwveir.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iezhvawk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ivmduufr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2avhxwgym.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2moavhohb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2abpqdxbu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ohzusoxf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cqflsodh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ndreoihq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2jntukmsw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2disxhraw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pssyedra.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vluwmjbr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2rqlekboc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nkhzodob.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tbzbokhi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wsmamnxw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ymqjidbh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ssrlwfec.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2lorldgms.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rhvygich.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lefjtlta.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2raujcipz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zvtfzazy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2khiqndbg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2rkmhgsfx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2aomizmxa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2apxbxbvp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zxmiwtex.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2frtfsezp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uglvjure.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2gzojtvoa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rrehgkul.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pwjyhfda.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ncabcphm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wqfooubj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fwkkrtjc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tukryvps.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hswspllc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ejhhfnka.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qgtoxlqc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfoxhdji.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vrlutbgl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2siwmllsk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xyjvvpzw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ngomflsj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qoztopsd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yjqebfdw.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dgnqrdxv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ajkqluah.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yxylrweu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ouoeroyg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eujtmgrx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ozyeqqhd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qfdcepyy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pnmvtzkq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vqkhzfug.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uyqmnwjj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cmdfwvpy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dlhfymif.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mpccqxcc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zjrzxtmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kguripbj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2olavnmbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iftclaft.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uklagktg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2oblcxcqp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2artdhlkn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bznbiwab.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrhhglim.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlacuglz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pdgnejds.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uinhglrq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ursxqakb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ugqeeaex.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hpaexjrx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxqvdjii.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzqidxhf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fkrrsvva.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2moygpcor.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqccpeuj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qjgqvwtg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dvwnpuzc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2egrixolc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nykwught.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ymmyboml.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2aeumwcux.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sehekskt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2smcflzno.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2giqemjxp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2evzbgydy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pihxtitv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2mujurtrk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2tmqiykty.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2blwdvedl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxkghxko.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mwpqmyso.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kaweegjf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qmoqmgbx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vqjfoxzc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jegkzlvf.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2eetjmugd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fxenmrnv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2duxbjher.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rnfnggry.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jvsowmge.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kmhpgtim.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gfkhhttv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zvdhrtbb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ptfbiuio.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2aaaiqdnq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2onvigkhx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yxaltkak.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yycwrqnq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zwkjtsvg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2liblmlyl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xyfcpyys.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2idpplrqb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qlphjmqd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dlvabzzw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2tdzhuhcj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2houhjexq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnjqcax.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ehapmhmn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvzmvniq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jdwcjbgw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2quqwoicx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2iivbevgw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gpfagdgq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hakkinsu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2iwaoltar.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gewqvpqi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxecriq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vocfgvrc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yxewujtq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhinkxcs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnepktgg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2evvcohlp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfyqasjg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2htlildbd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lbmhkdxi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dbxwdwxp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ioqzwlrg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zctmxywg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eeobekxk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vhnwltgy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bgnadgsw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2uzedtxgp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2odlixtsm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kaeljnqv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ymmgpnfu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2irbydglw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2agjewqrr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ogkpqajg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wrozfsqp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nsqttlck.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fglrvjec.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lljwhbjd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gdmqmrvx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kywkwqdw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mzewmemf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cytvsbde.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2umiulhew.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2atjcpaws.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fzfjwbiz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ggctunil.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pberdlyi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sqnklczr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nqurgkyy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2duxrgjgt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2usqkzyiw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iejylfsr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtlsmudz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2vhrvadqp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vrseisli.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzvyrplt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gyxofzgv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnmcgefv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrapengs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qefnfwgo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ftfkvinq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lyaheggl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ukdrmdwj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jdoboguw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2njgxcdfh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ecwqqfbu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2tlrfyljc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvvfwfmo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2lpxnmmez.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ahxhsglv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2uopyqask.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xonrpfwu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kknzdire.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2maeykxhw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gxuejpxh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fihwlqeb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lrnjgfkx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sywtxlnj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2iivikixd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2njbleeak.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lmyduznu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2iabblpvr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kfvfdsze.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hjrelzxw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ownsjeld.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rqlpaevw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2djxulygc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2cytlrdlh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gkjtokxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aihmygku.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xmqmcibs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tudsnzxf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tkrtoyvl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qauxadcd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2anwyhycl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yrlcmegm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zyfplfpl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bqehgotn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sfxgebke.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bidhgfsn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tmrftrsy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2gxevdjbk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2eqriygvz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2aeslhhbg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2auulqzbr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2frhnfnzw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bmtotfmp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nauvykyn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zlvyxvyg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oiiwuhmt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2hoiwrhfl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tgicqefk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2chfmbsfd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rjiriizi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jlharkjb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dcjvnypc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xidsjkmc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tjawhjlb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2apwuzktv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwvehq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgbbdutd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygfryhip.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ryuwubbf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uvncbhvs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fkeklpjp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrrlsni.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gjvxnfld.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2padhjsli.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nlssofql.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2urhgirel.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ukcjcqbb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2aqqbmjuw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2icrrkqog.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ekctskeg.html


<!-- 参考信息 -->