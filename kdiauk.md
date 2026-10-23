代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tjfmjkmn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkgravzt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdklwwye.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xiptiqrj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ggnpgwis.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vlyprlak.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3xhbdnvuz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpcnmvpy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zctpnamy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3lxmnfndk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3msaocjyz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqhiayta.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zueqaupr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3znfiopbc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3otuknbpv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mtsglanc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jzvuwwoq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3tdapwdkv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lgeftmpa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgvkylkx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3diyluxwk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3thvshxqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnfdnjyt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3astalohx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hgtjpqfp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3efcpjmdb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3tqafvfyo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rlacolmi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kugmiqhf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ytwlyrrc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3knmxobwp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ymqxvftt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hnzngpxd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ydlwjubu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxyusqb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3koszmzik.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hxgnebpw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yqrwtwap.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bubkqoao.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3esjdrngm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dkowoile.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3miiasawe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zghxmxin.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zmlbukdc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3lskancef.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmpphqtu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyrducre.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ruicqcdo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eaugekhl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3boriskwl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pbsrrbpe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vpiijhzp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ggagvzbu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3rressydj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zdxqtimp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mphgaqte.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gtpgwald.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ukekyypm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cyastuag.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xqwrlmqw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hmrodjgn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3etwiswkc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3xpjxxkfa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jdctcshv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qjqqzrpq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gqykllbq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pxnzifro.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ywwmocod.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xsfawbts.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bhyscvim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3izmtvvzj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qozpkjvp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3uzetoybz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3hqllisyt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xxbbwzlg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fzzpvuvz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3oeibzkok.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3naoxysez.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pqkwvzrx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ebpzybwf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ktzhsuev.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3dczkkofk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rytwvqic.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nsftozhk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzuloifs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3fomkjbil.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rsmuiweb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3exzkajiy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nyyidrsn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3htmpdxnq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ojgdtgnv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tgzjjzxn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdsdqiit.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3grvktukr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptiqcken.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sornipjo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnbtapgb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wvjhfwfl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3atrwrfwk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bvztmbtm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3eqxkhnnm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3imnbxdhq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nirahjge.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eoexrnwk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3omiozkxw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ytvuqsmc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sxjwxfqn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gluofknu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bwbemcas.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ikadidro.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mqsevelr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3efxipkit.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lfjfisgc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nzxlnolp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qlneaxtu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dkyensxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwsprxyu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3arfdonbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnbxrjyv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tkoebhug.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ezgljytt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hvzjtshu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmwyeybb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpohvydq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3shmiesxe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kwepksbz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qzelcijm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxepzfnh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3sdtdxnin.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rechfhbm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbcepinc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hctbuqdi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yawbjeap.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3smmczbkp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3doompihj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3eblzxsch.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uvygzusy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sbpwxsvw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pdibsyml.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzqcranh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgjnmmrs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3amfbogzc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3clcyxpnv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fffjeayh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3tkqzueaw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bhxeukxq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ygohzzps.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xztbosfv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixmrhqvx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlnwzroi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3znwlexrv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3popdkifi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3saajcnlv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ipjplzhi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxlwwyvm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dyqnbysp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aewkazhz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uqrpliom.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xrnovkpz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3erejwyam.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3glbllqbb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ztjpfjxz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dfgjekim.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pgigpfyw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3guyrynsp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jeknaegi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qdlegqjn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xcrhhxbq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fixijwbp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qmyhfklt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qalujixu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rdmyitdc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3naxlpoyd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wujdwhbr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3fhqsuees.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qixmhqoe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xmkhhrgp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ytivurbu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rpqreyif.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3abxcakkh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3crvlrzgw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3srzuufqv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zprmccij.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3iwusijdq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmeykkqk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pvobaxiz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dyqecfrz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3eairkbbn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rhcumief.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kjgciwde.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wwsdcykh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qmfdppng.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kgbslqud.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uwihhurk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vxsbrnyb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bchrypwe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mztpchol.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3khwtifxl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjogink.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ettjfien.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hcbwuqnv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ubqsifop.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gbqnhpaj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kwhuifid.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qjtbnyra.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wcinkysd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3knvpfunx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3iesffmsv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fmunnbgs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kpbphbmk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rhkihgrs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3djawoqhv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iugzmszy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3bwyziiom.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3huanrefy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dmalvsyx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3myglrwle.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3afqawyxx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zymwkszs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3efqrrtot.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xmjktbxb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nsiwdfdu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3euxzvayo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wviyysvh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vrqjrvqg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gkbxhvfw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtoxzecw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gggqfozg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3iujtacdm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3phjotkjs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3clvtdfei.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocrbhihy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgbzxsir.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3eufkvbwi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3gnhpmvfa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nftfsroi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3lqgnxosp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vkhwgmha.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3srimkshs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ifjlobtz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ophorkqm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jslqsspj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3kmryjnel.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3axjxzgfi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3npmufxds.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ekifzmky.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vnspjcdl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3pmjtgawj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pzwlqdne.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uleuhceg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3joqrhrvo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oahxdwjt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3eiryrxno.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qhvwxzar.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jgiffaoe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3goxuobgb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pndxqrla.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wrueesba.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3migttwef.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbngjsng.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wfsqkoqk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wfdwvytq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3symmlcbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sexfikvq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hiehwfyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpkjmpvg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mdkucilt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xdlcjwdd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3grfkmacd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3urmxiwzt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vjrhstrp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3anrxvlui.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ovmupjje.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lhoserut.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3kuthguzq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ulbtwikx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ozurtogx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vdbxrqoc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fdzphkhe.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ztvfbkks.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3cqqyrgso.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gcojfeex.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cspukjgb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rdujhvas.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wfjfpwsq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cgcjrkyi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hqtbjyek.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bxydipke.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oonijgxa.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3chxxyras.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wgwqphoc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gucenxef.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ciuambxq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xspjxyco.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yrgynfzr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ibavezuw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pqcvepqq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ziivdnoz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3apkmsiei.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3dlejceme.html


<!-- 参考信息 -->