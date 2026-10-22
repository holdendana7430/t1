代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2sthnumjn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tsxnctvg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2axgfvkbk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhgynfe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwtdzocc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fglnaxcy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2algnrsgv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhszjtdz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rsfeaynd.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2pmybabbv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiuffvfr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zfxogzut.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qvahidek.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqcmqikw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qlfywvet.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bzvefofz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2cjaezfaq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nrdyxqgv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvduzea.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2jmiqgmrn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zxuqfbrk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnqthszq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxlkanvx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jzmjnwhp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2yxetxvyk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dcfnrvkp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2bdqvttbt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ufzqpkfm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ysdzzrwm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cqhkczqr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjkzwtnh.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mohmlxcl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2cyachcqo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgflxsqm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpnnjejk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ycaibtvw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ccywekty.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2griprwof.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nkhzdvin.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qaaosnsh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gvdqfjxg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jedwcpck.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2aqnbhquk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2flsmrhny.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ttmjlroc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgdcrwsv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hizeeuac.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeuvabrz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uwxcqkqm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxowiyt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2koaaridi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ninyclwm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwwtxnks.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2njkuwxkx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tiwqvucw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pydkixfc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qwhdkrwb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pafrheyp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2iruvgrdb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vyleffbx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2vhesgmnz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2zcgnxowl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xvjwsgut.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bhzrqtqr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yhznkpef.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pcosvpwo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iooothrt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2zuvrvcxl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vxcijqcd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bbrzmjbc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ijkrbtep.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2apjmrvjg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2umvmtuyd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nrirldce.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ubbdyikq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zlwrjgui.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gfntcfrf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvosrxnr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gcktixar.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2onzbjzwv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2vyhnyfow.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2scxqusty.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2emfegmoa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ofggyvfo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uauibmmc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bgyamruo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hauxoeqk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fevykjub.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ferpypqr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lhhfyalm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rtbcflpm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tvlrqspz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vzuzhgsr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rezbvojw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lrsmpidc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mvynzwtj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2awjduagl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cleknmjg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2lifyfyox.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2cmlawhzf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ybggkskc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dmigumuy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yuhkuyph.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wgfcilvh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kzkoxmuq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wkfmlrnx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jnybsbll.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gvnrensn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jyzwzqvg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnumuqxd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zdqdxjhl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cvftbosi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qjvcmrrl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2whqpyeee.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2iyemysme.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nctqbqfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drnoqfyp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zdolporz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brkxfoaf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oxnocuhf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pmaaqknz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xfcfsfpz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2psrtaatc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkjjbqpa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvtvdxnc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gpqwtfke.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ubtwutxf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gnvvkjeb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hwhygfls.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ggparceu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wvxllkpy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cjuifdiv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2khikvpvs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nsaaajjp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mnsrgatv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fmftuxmh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2naomkfkp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhnxbpcd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2dklxtiop.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2oytnmrxt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcipkibx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jalsoupz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2urtmzxlk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zkjnhxxd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mwngtjmk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2arlbxoja.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tglznqow.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gcxbcnun.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lfofmjjf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fygalqqw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vdioklpx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bcopatvn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgfzgxeh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdepeox.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxtzmda.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zqhfhrva.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zwabmokp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kniaxpwl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tkhwkhbr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hqsnfhqs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lndtpben.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iqqgtayl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2luwjgnga.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2swnqqufl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fcwkalnm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bmluxbtr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ciyiaqoj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vmegswrc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oiuwrndn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2obbmvgxq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vwqqqxok.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2voalsrso.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vrsvesuy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ozomxavk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ymxlmctl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vpjxkgcn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2sxoktaqk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ppxargvc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dxeugsjs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ovmzkros.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ewnmhlrp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2luinorzh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oxiimfrg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ooarbqee.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oeigliiu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohceyxqm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecixmyrl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ujnxzyrg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2llgfotsr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2muoocpab.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pghmusje.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkwyzjul.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xexpzfyc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yczcblhg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jukszpsi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kmyatqoa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2moxnpyfb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lkowcfxd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzzdstqv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qkbebgjw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2grltfiej.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2svcjahix.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2oeayckyc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lsuodech.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2lvzauvfp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aqexdwnc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ldguegqq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ajimidok.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qzichcca.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2iiugqcbx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dstnvhah.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2vbemxmty.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ypchqsvh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2femgvxyt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ajmytaeq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wlzkllsg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2gqqxbntv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vdarcmhc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2etmhpjmq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2sbntuxfr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gurckvnb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2idzuaxjn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ijrreauq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gsajeckt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hqgnrjul.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gskistgk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vfvvtjht.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cuznwbxi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ebeehjnv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qagensey.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xlwvcbnc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyranaet.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ctxyyprq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bbywiltw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2loirjzhd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tuogheam.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2txzyunyg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2riqupysi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nmtmbkij.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mkmtuheh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uqjedyqi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojgsbhvd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fsrcyezc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ibanjhlb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2urbdztue.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xlxxqphb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2douioafr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bkhbwmvw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qloienof.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ghtwhysv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cmfcyoog.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gtdfgogt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2tftyootg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pfmoncph.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nwabtpup.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nuhdwiel.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xfnmxuti.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rntpozkh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2edenkmfx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2caxolykt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2chftmiba.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpklkxyg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wenbggiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtkhkeae.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xcsnxgaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhstbatq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hvakhllc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pfsijwnx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bucvguqw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tyomkjuy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xwwbqyiq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2onpevlyt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2muvilozk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ilwqouzf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2iokbwsjl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pkrqimrk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pkobuymx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xrhtprww.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hnjtctcy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vddzmvjt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cueurcti.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2egatdrag.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ztawjose.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tqppmkvw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wupfghjv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kzwhnvph.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hkloyhbi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2viuzisan.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jfpcqfoa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2biamojbc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lwhzexwc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wbuwllti.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yvnpjpod.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2awijrsqj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xpynpucq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmkfvavn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2csacdcag.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wrundkuu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hpgutgss.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tidsqhgj.html


<!-- 参考信息 -->