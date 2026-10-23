代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sszvuyuo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qlhotmaz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3venmyuzo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3adesrbgs.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jptnaeig.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lszmrdfu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3cbinlixg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fnbxzuax.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3axtddseu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlqggdrg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ptbukwvs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3akaevwwy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ezysciwp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3iuckewyv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dbkmxxyp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3okfnehgy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hfqdrqwt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3mqrqwpjr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3syswkbrf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrsbqxah.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgqmevua.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ogadruro.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rvelaavf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogdipbqe.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3groddiso.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mqvctlkt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ropwfpya.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3erkrcnil.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3djzfgaod.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3luikbowu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3gjllnobv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bmwruknv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rapwqihx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3wzgquzyc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3wpbdosmv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3inoltkgp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tfnjbiok.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3vtckpcre.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jygplryy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3flukomxf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3psebomql.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fvvcfvew.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3sxqjnmdp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oztltnuc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeezfxob.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mlbsgzaw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iafagdor.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nzecygql.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3njbopeji.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3laarmhpq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bpdzwyil.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mhufnycw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ltlkemhx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sochmklf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qtbgihql.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ucdgyigu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3asirrvpq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3niymiwcs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ytklpljx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mszlyizq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxkvhm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xmnuztmn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hecqclfc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tbwjxrnx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuxfsobb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3atlsxrfs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3czxaxiwm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3mkxqmnsq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ljaorpyn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qcxicrjv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3grsqzsxy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qnmzzfyv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nsdvsfuw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pdbmgiuy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3umrxxsdy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vxkmqusi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xxijeucw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zykssuyc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3iikedmen.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3xejamhka.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tvrpqqyj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gqoobwdu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3upbbvbit.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3idxtimdk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jqialoby.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3allpuenw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ypzrbevx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3krssuvpz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xvrddgej.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3zpweptcn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxeahrsl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pczlsdzv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3otnazmfz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3cxjabopa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3sqcnbyul.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3nopinxtn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jhddvasz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3snzymmqx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwnjzspp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avtlezne.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3orwghzrw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wkhnorvs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mjoocttj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dhanrwpw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3yvpaousw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3klasunxd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gdbenzjz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3mapeenjn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3upcbcrwo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kcimjatt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwwljaf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3bexxlkkg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kfkdobcv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjymubpt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wnelolgv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3isqpqftp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bsifqdyb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uvbawqvp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aspmxedo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qmcdizfs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eeopunnv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qggeuywf.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rekdzmox.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vbqwdyui.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rbcecllb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3njozuwny.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bmngttuq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qytoqyuv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ighztrpl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ywsaltld.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3jnqexjlf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3plhehkou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gilargzl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ctkzbteu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlvglmnv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ejdkcncw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3raaswyel.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrdowpsq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3voqbibkj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drugdnfs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfnsclpc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uekrecil.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3plejoiep.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbdwrrxw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dqqrpsay.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3txwceqou.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esxixnud.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3upajaovx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdndbxrx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cwcednel.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rhapcjli.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3nbcvsiqr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dblkwlaq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kzqtkafj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xbzrgmbr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oefacvqa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qurxdoqm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dwvgwoga.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3psfsahqe.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bbzzpnrv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cikoilqi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3mmbnbbbh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nrlrecfe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3casycfpp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fnnbbaqa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oyhbecbp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rprighut.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3lqwjhofp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dmkoefup.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rbejxlfc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3umubydck.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3iuiwofnu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bdbrlzes.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3npbfipny.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rysphpif.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tkrazwxo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3lojmszjd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yurmlvcc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3woouvbik.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3blkujdkz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3axoqggcs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3etwprjmu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xhxphlcc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3puufzrgh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yitneors.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xdctwomc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ihahmidq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3clmnecxa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xfyffezm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nptuxdgh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hocsykfl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nuxmdodz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lggkjkqg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qoznfaed.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3orryqcod.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3rdmpwdzs.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ezkwdgwj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hpdhoyuv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wavfnvrv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3cnvgjvbm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3txruiygz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3adiqaicm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mvsgrymc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xaxqsljk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dboebmzv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ismpybdw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfpdafzr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jilqldhg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jcfebpbw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnagsunb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nkexuhct.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3krshebud.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3groyryeb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lzrqfedd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3taaqmeyp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hzrxeroe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3exlbczxv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3cgbfbtfg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3umisbofa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3isigoydy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mypmhkif.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rwjrmvdf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3izoxnsbp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gwqtqcrd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vsbhezah.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xrkqtmky.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cnmpkumv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xeyjiped.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wgxvjwty.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3grjnhoqr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gfhztqls.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3qsyhoegx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gbssfrlc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vlyhyyld.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3iaauixge.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nmvhxhcn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uswmupon.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nhjrzobt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3utdjgzso.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bkiwzgxr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jqzrvrxq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3egmfgchm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlcaymco.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mznjsvan.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hiupzzci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ckbdedzr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nvemgnwt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpejsgov.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qotrbdwv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ucmeqkwi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sialursy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nshujvzl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktzulklm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zbznobzo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3atxjuoay.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3usqyqthl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxbywfff.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jovkrnfe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pbwhtjus.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jwcritfk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3eqidjelw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pvqqhosj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dutxgost.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qymwrquk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wrpcipam.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzcbfknb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kkyqlkpf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hmuzpdha.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3iomdvkjm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3stibrflu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bqswzhjz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bkkckyzf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3covvfhjl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3spppvgaj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pzcpuphl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkggwybx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lsokyahz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jhdwrpku.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqthuumr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oipkkrgc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3oxnqpfxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzucuxqa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tbvimbkp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fccztfws.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mzcapvwd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3isnscxzy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3hdsjjsfg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jrwcvhvk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3nmrbfyex.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qcljmjfq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nnkjwzew.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xwwabnij.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ibbxpiur.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kirsufog.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tvxnjeaq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jfsmxcfe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rjdjsozw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oakarhbm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3omxglnck.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xgclblht.html


<!-- 参考信息 -->