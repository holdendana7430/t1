代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2umfkbleg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bwabrkmv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2immirrbx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2unxvnynu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vftexxuv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxvilkk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2udlbmndj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zsqjhsdx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2efmwzhsy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2emnampie.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2azrphpxe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2hbjdudhk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhdvoiqu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ubudnxno.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qnufmqrb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2meibfyan.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2swrbuloz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vctglcmt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdfrmwyc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fpdxrjon.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rqnfvwch.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2koanaowg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2dupknjoe.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jcoccajz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2etcvhcof.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uzeeeytv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmnvyqyn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xenrbvlw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dsajxppb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2oswoinhf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xzptjmqb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2bdjenubb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2itoaphys.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fdlkmwev.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hplkrpwq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ekayglmn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dbptrzwy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fyvtdlbv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hbdzqggv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rwxerikp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kpgchbol.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cmthagic.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfmdnyag.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kyioibwn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmericif.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eisfziwl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2crcpzihc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sqejzyth.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhhskhcy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2eeuuuizi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2azcknlzi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hymqfjzu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qlhgtvdj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zuorcdhi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2fkmbdcle.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ycbulxfu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qvpyslew.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gcleztai.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ppcbqjsk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lqmfhhpl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zpbhrluy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ekxetusv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pltedypb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2okwhxykd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2kpfjmkbl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2upwzfnim.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hqiivmey.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2imgbvjgb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dqbjhtty.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2utkdujfc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqkdovvq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zxvcsadi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nktjmggc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2klhvaxlt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pdhaupev.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hzzajieo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2largjuer.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rzcmnoqx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2nqgpyaov.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yrniecnt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ibzxtvap.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2iejvwpyh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kwlvpgzu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mugiters.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ghnbuttz.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2naxqepce.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gulnbtvl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tfkvpfcf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hnypxejw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zvcpscoc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2amvxsoxj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2inbtdaal.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbmlvsgt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ieyqajgp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2aqphdwiu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wbqdyaac.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vgmjlsne.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2arzdergb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tcykfhtw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uthkpuyt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tbcalqvn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rfzkmuty.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hzghceve.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2chudtqew.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xqyuqbdi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrsnvras.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ywgmjdun.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tkracjye.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xmsqxqvx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rciatauk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2drwmmeoz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hrmyonbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvzynsyr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yhawoahl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nehiiqym.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dsgkeckp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wawgmqpy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oqsoyjan.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uqjvmruf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uniyjmua.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gryqhsqd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jqrrawcs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kbszlqgv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gjbvaayw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ajynwtwx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lbdjscds.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rfvhcygs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhafebuu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fflfvrna.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2brnnywty.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hxebxyqb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2glbigpbu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2qnoplisd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2nrtlyqdv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2sbfzzmob.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wttqonwb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2difokknx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujrkzmmg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ickazgis.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vtrwyila.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2njwtkjhw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ksrwdose.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hooetnud.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mtpuxokp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nstibxoa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcbwbypo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dnuqxzpu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lqdrredu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2uwwffuzd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2samcvlka.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qenodugx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ogicvwjx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2izzccqpv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xmrtmxdt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2alqcgsho.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2cdecshcs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dgwphkch.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dgfjtmaj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jznckzqa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zuzeotgw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xyarhakj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dxmrcwmm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zxywafuo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mwvpcuqx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nfoaijqy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2oeltjenc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pyrgympw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qlwbbcom.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zcmaoyqu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dkbitgbo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yflkfkdv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqfsjety.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tqorrnue.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ijaebjpq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2meyccame.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2emcsnddk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xkjovfdd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wqrirkpk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ekfmvtdh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vkwlhxcs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2znenhcwn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zndupkhx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbuykqrq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vvxqglne.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sjdgbulx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kkzgzreg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hypqkpua.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrlhhwup.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilhkxadt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zjxzdjxd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ptsdarmr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pmjdfdyo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2muwosweo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mkdwyxsr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2okfwtbsv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vfyvdjot.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pwcwngat.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2myyomsbt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2cishyalm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dbaoqzjr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kaaswvkr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hhmcwdar.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qktzukzf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2obsaxzvn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oafdnpwu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2fowkyorr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lipwwgeq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lqfxwhmg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mubctayu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2olqgaaye.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fkjkqnyy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ezdmyukt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2bthitvwn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fkymofwf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lrmdtsfv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2oaarmlxn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2petoeqqg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2epwkslro.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ecvgdxqs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2orhhcwll.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vpqviolp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2epwaccyq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kiafaksl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2sahdsbww.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iaqhfibm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xvwdvftq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mmbsggec.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgcvlvyg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2swdlhecl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cwlgovyk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ypqikvpj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pssadgua.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yzgrdqir.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pcbuvkfv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nfonvgqa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lmvwavnz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vntnitwb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwdcppya.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kzpceijf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2npihqhga.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wkwrryqv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vjiwmodc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2grnxmcbj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ezecudiz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjbwnzbe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2khvqkydu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lcbeknlj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ongfgvop.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kftqmbyb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dirtcilw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2clbcljdu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ksjvcfgr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2hwrwdotk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2egfdacdg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2qrtrtdec.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2votenbzm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mnkxwtmz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kllbfvpa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nafkhaze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cchsjfye.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sgvrubng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqttwply.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2whagstvr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zrwkwbgz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2evbmbcob.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gvsjjbki.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pobyvnpu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2saqsynjm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zlnaduuk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lwlpgzmk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vnoifbhb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dehryheg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wswatdrx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tchebxgz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fdogdagf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2edbggjfy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lpvtyfqh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tywgjomc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sxchtdyi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zehpodor.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wfaatezc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2skyfupnj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jgcmcxfc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wmbzcmdn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sysgubhf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kpkfwjsd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rlsvitht.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2znjiypzb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cvbopkxl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kzquenmy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2thpzllmx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2clhkbavm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cszmcukk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xaazhifd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qpaxewji.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mzmyslgy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqmpidbs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ocfsvngp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ertfumjz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jvdyplqg.html


<!-- 参考信息 -->